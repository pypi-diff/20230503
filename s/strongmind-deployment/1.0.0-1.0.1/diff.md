# Comparing `tmp/strongmind_deployment-1.0.0-py3-none-any.whl.zip` & `tmp/strongmind_deployment-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4893 bytes, number of entries: 7
+Zip file size: 5699 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 strongmind_deployment/__init__.py
--rw-r--r--  2.0 unx     4277 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
--rw-r--r--  2.0 unx     4454 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
-?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.0.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.0.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.0.dist-info/RECORD
-7 files, 11169 bytes uncompressed, 3771 bytes compressed:  66.2%
+-rw-r--r--  2.0 unx     7511 b- defN 20-Feb-02 00:00 strongmind_deployment/container.py
+-rw-r--r--  2.0 unx     4969 b- defN 20-Feb-02 00:00 strongmind_deployment/rails.py
+?rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.1.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1053 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.1.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      623 b- defN 20-Feb-02 00:00 strongmind_deployment-1.0.1.dist-info/RECORD
+7 files, 14918 bytes uncompressed, 4577 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -3,20 +3,20 @@
 
 Filename: strongmind_deployment/container.py
 Comment: 
 
 Filename: strongmind_deployment/rails.py
 Comment: 
 
-Filename: strongmind_deployment-1.0.0.dist-info/METADATA
+Filename: strongmind_deployment-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: strongmind_deployment-1.0.0.dist-info/WHEEL
+Filename: strongmind_deployment-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: strongmind_deployment-1.0.0.dist-info/licenses/LICENSE
+Filename: strongmind_deployment-1.0.1.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: strongmind_deployment-1.0.0.dist-info/RECORD
+Filename: strongmind_deployment-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## strongmind_deployment/container.py

```diff
@@ -1,97 +1,191 @@
 import json
 import os
+import re
 
 import pulumi
 import pulumi_aws as aws
 import pulumi_awsx as awsx
 from pulumi import Config, export, Output
+from pulumi_cloudflare import get_zone, Record
 
 
 class ContainerComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:container', name, None, opts)
 
+        self.cert_validation_cert = None
+        self.cert_validation_record = None
+        self.cert = None
         self._security_group_name = None
+        self.cname_record = None
         self.container_image = kwargs.get('container_image')
         self.app_path = kwargs.get('app_path') or './'
         self.container_port = kwargs.get('container_port') or 3000
         self.cpu = kwargs.get('cpu') or 256
         self.memory = kwargs.get("memory") or 512
         self.env_vars = kwargs.get('env_vars', {})
+        self.kwargs = kwargs
+        self.env_name = os.environ.get('ENVIRONMENT_NAME', 'stage')
 
         stack = pulumi.get_stack()
         project = pulumi.get_project()
+        project_stack = f"{project}-{stack}"
+
         self.tags = {
             "product": project,
             "repository": project,
             "service": project,
-            "environment": self.env_vars.get("ENVIRONMENT_NAME", "stage"),
+            "environment": self.env_name,
         }
 
         self.ecs_cluster = aws.ecs.Cluster("cluster",
-                                           name=stack,
+                                           name=project_stack,
                                            tags=self.tags,
                                            opts=pulumi.ResourceOptions(parent=self),
                                            )
         self.load_balancer = awsx.lb.ApplicationLoadBalancer(
             "loadbalancer",
-            name=stack,
+            name=project_stack,
             default_target_group_port=self.container_port,
             tags=self.tags,
             opts=pulumi.ResourceOptions(parent=self),
         )
 
+        self.dns(project)
+
         load_balancer_arn = kwargs.get('load_balancer_arn', self.load_balancer.load_balancer.arn)
         target_group_arn = kwargs.get('target_group_arn', self.load_balancer.default_target_group.arn)
-        self.load_balancer_listener = aws.lb.Listener("listener80",
-                                                      port=80,
-                                                      protocol="HTTP",
-                                                      load_balancer_arn=load_balancer_arn,
-                                                      # port=443,
-                                                      # protocol="HTTPS",
-                                                      default_actions=[
-                                                          aws.lb.ListenerDefaultActionArgs(
-                                                              type="forward",
-                                                              target_group_arn=target_group_arn
-                                                          )],
-                                                      )
-        # aws.lb.ListenerArgs(
-        #     port=80,
-        #     protocol="HTTP",
-        #     default_action=awsx.lb.ApplicationListenerDefaultActionArgs(
-        #         type="redirect",
-        #         redirect=awsx.lb.ApplicationListenerDefaultActionRedirectArgs(
-        #             port="443",
-        #             protocol="HTTPS",
-        #             status_code="HTTP_301",
-        #         ),
-        #     )
-        # ),
+        self.load_balancer_listener = aws.lb.Listener(
+            "listener443",
+            load_balancer_arn=load_balancer_arn,
+            certificate_arn=self.cert.arn,
+            port=443,
+            protocol="HTTPS",
+            default_actions=[
+                aws.lb.ListenerDefaultActionArgs(
+                    type="forward",
+                    target_group_arn=target_group_arn
+                )],
+            tags=self.tags,
+            opts=pulumi.ResourceOptions(parent=self,
+                                        depends_on=[
+                                            self.cert,
+                                            self.cert_validation_record,
+                                            self.cert_validation_cert,
+                                        ]),
+        )
+        self.load_balancer_listener_redirect_http_to_https = aws.lb.Listener(
+            "listener80",
+            load_balancer_arn=load_balancer_arn,
+            port=80,
+            protocol="HTTP",
+            default_actions=[aws.lb.ListenerDefaultActionArgs(
+                type="redirect",
+                redirect=aws.lb.ListenerDefaultActionRedirectArgs(
+                    port="443",
+                    protocol="HTTPS",
+                    status_code="HTTP_301",
+                ),
+            )],
+            tags=self.tags,
+            opts=pulumi.ResourceOptions(parent=self),
+        )
+
+        logs = aws.cloudwatch.LogGroup(
+            f'log',
+            retention_in_days=14,
+            name=f'/aws/ecs/{project_stack}',
+            tags=self.tags
+        )
         task_definition_args = awsx.ecs.FargateServiceTaskDefinitionArgs(
             skip_destroy=True,
+            family=project_stack,
             container=awsx.ecs.TaskDefinitionContainerDefinitionArgs(
+                name=project_stack,
+                log_configuration=awsx.ecs.TaskDefinitionLogConfigurationArgs(
+                    log_driver="awslogs",
+                    options={
+                        "awslogs-group": logs.name,
+                        "awslogs-region": "us-west-2",
+                        "awslogs-stream-prefix": "container",
+                    },
+                ),
                 image=self.container_image,
                 cpu=self.cpu,
                 memory=self.memory,
                 essential=True,
                 port_mappings=[awsx.ecs.TaskDefinitionPortMappingArgs(
                     container_port=self.container_port,
                     host_port=self.container_port,
                     target_group=self.load_balancer.default_target_group,
                 )],
                 environment=[{"name": k, "value": v} for k, v in self.env_vars.items()]
             )
         )
         self.fargate_service = awsx.ecs.FargateService(
             "service",
-            name=stack,
+            name=project_stack,
             cluster=self.ecs_cluster.arn,
             continue_before_steady_state=True,
             assign_public_ip=True,
             task_definition_args=task_definition_args,
             tags=self.tags,
             opts=pulumi.ResourceOptions(parent=self),
         )
 
-        export("url", Output.concat("http://", self.load_balancer.load_balancer.dns_name))
         self.register_outputs({})
+
+    def dns(self, name):
+        if self.env_name != "prod":
+            name = f"{self.env_name}-{name}"
+        domain = 'strongmind.com'
+        full_name = f"{name}.{domain}"
+        zone_id = self.kwargs.get('zone_id', 'b4b7fec0d0aacbd55c5a259d1e64fff5')
+        lb_dns_name = self.kwargs.get('load_balancer_dns_name',
+                                      self.load_balancer.load_balancer.dns_name)  # pragma: no cover
+        self.cname_record = Record(
+            'cname_record',
+            name=name,
+            type='CNAME',
+            zone_id=zone_id,
+            value=lb_dns_name,
+            ttl=1,
+            opts=pulumi.ResourceOptions(parent=self),
+        )
+        pulumi.export("url", Output.concat("https://", full_name))
+
+        self.cert = aws.acm.Certificate(
+            "cert",
+            domain_name=full_name,
+            validation_method="DNS",
+            tags=self.tags,
+            opts=pulumi.ResourceOptions(parent=self),
+        )
+        domain_validation_options = self.kwargs.get('domain_validation_options',
+                                                    self.cert.domain_validation_options)  # pragma: no cover
+
+        resource_record_value = domain_validation_options[0].resource_record_value
+
+        def remove_trailing_period(value):
+            return re.sub("\\.$", "", value)
+
+        if type(resource_record_value) != str:
+            resource_record_value = resource_record_value.apply(remove_trailing_period)
+
+        self.cert_validation_record = Record(
+            'cert_validation_record',
+            name=domain_validation_options[0].resource_record_name,
+            type=domain_validation_options[0].resource_record_type,
+            zone_id=zone_id,
+            value=resource_record_value,
+            ttl=1,
+            opts=pulumi.ResourceOptions(parent=self, depends_on=[self.cert,
+                                                                 self.cname_record]),
+        )
+
+        self.cert_validation_cert = aws.acm.CertificateValidation(
+            "cert_validation",
+            certificate_arn=self.cert.arn,
+            validation_record_fqdns=[self.cert_validation_record.hostname],
+            opts=pulumi.ResourceOptions(parent=self, depends_on=[self.cert_validation_record]),
+        )
```

## strongmind_deployment/rails.py

```diff
@@ -1,40 +1,46 @@
 import json
+import os
 
 import pulumi
 import pulumi_random as random
 import pulumi_aws as aws
 from pulumi import export, Output
 
 from strongmind_deployment.container import ContainerComponent
 
 
 class RailsComponent(pulumi.ComponentResource):
     def __init__(self, name, opts=None, **kwargs):
         super().__init__('strongmind:global_build:commons:rails', name, None, opts)
+        self.cname_record = None
         self.firewall_rule = None
         self.db_password = None
         self.container = None
         self.rds_serverless_cluster_instance = None
         self.rds_serverless_cluster = None
         self.kwargs = kwargs
         self.env_vars = self.kwargs.get('env_vars', {})
 
+        self.env_name = os.environ.get('ENVIRONMENT_NAME', 'stage')
+
         project = pulumi.get_project()
         stack = pulumi.get_stack()
+        project_stack = f"{project}-{stack}"
+
         self.tags = {
             "product": project,
             "repository": project,
             "service": project,
-            "environment": self.env_vars.get("ENVIRONMENT_NAME", "stage"),
+            "environment": self.env_name,
         }
 
-        self.rds(stack)
+        self.rds(project_stack)
 
-        self.ecs(stack)
+        self.ecs()
 
         self.security()
 
         self.register_outputs({})
 
     def security(self):
         container_security_group_id = self.kwargs.get(
@@ -50,60 +56,67 @@
             security_group_id=self.rds_serverless_cluster.vpc_security_group_ids[0],
             source_security_group_id=container_security_group_id,
             opts=pulumi.ResourceOptions(parent=self,
                                         depends_on=[self.rds_serverless_cluster_instance,
                                                     self.container])
         )
 
-    def ecs(self, name):
+    def ecs(self):
+        container_image = os.environ['CONTAINER_IMAGE']
+        master_key = os.environ['RAILS_MASTER_KEY']
         additional_env_vars = {
+            'RAILS_MASTER_KEY': master_key,
             'DATABASE_HOST': self.rds_serverless_cluster.endpoint,
             'DB_USERNAME': self.rds_serverless_cluster.master_username,
             'DB_PASSWORD': self.rds_serverless_cluster.master_password,
             'DATABASE_URL': self.get_database_url(),
             'RAILS_ENV': 'production'
         }
 
         self.env_vars.update(additional_env_vars)
         self.kwargs['env_vars'] = self.env_vars
+        self.kwargs['container_image'] = container_image
 
         self.container = ContainerComponent("container",
                                             pulumi.ResourceOptions(parent=self),
                                             **self.kwargs
                                             )
 
-    def rds(self, name):
+    def rds(self, project_stack):
         self.db_password = random.RandomPassword("password",
                                                  length=30,
                                                  special=False)
         self.rds_serverless_cluster = aws.rds.Cluster(
             'rds_serverless_cluster',
-            cluster_identifier=name,
+            cluster_identifier=project_stack,
             engine='aurora-postgresql',
             engine_mode='provisioned',
             engine_version='15.2',
             database_name="app",
-            master_username=name.replace('-', '_'),
+            master_username=project_stack.replace('-', '_'),
             master_password=self.db_password.result,
             serverlessv2_scaling_configuration=aws.rds.ClusterServerlessv2ScalingConfigurationArgs(
                 min_capacity=0.5,
                 max_capacity=16,
             ),
             tags=self.tags,
-            opts=pulumi.ResourceOptions(parent=self),
+            opts=pulumi.ResourceOptions(parent=self,
+                                        protect=True),
         )
         self.rds_serverless_cluster_instance = aws.rds.ClusterInstance(
             'rds_serverless_cluster_instance',
-            identifier=name,
+            identifier=project_stack,
             cluster_identifier=self.rds_serverless_cluster.cluster_identifier,
             instance_class='db.serverless',
             engine=self.rds_serverless_cluster.engine,
             engine_version=self.rds_serverless_cluster.engine_version,
             publicly_accessible=True,
-            opts=pulumi.ResourceOptions(parent=self, depends_on=[self.rds_serverless_cluster]),
+            opts=pulumi.ResourceOptions(parent=self,
+                                        depends_on=[self.rds_serverless_cluster],
+                                        protect=True),
         )
 
         export("db_endpoint", Output.concat(self.rds_serverless_cluster.endpoint))
 
     def get_database_url(self):
         return Output.concat('postgres://',
                              self.rds_serverless_cluster.master_username,
```

## Comparing `strongmind_deployment-1.0.0.dist-info/METADATA` & `strongmind_deployment-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strongmind_deployment
-Version: 1.0.0
+Version: 1.0.1
 Summary: Deployment tools for Strongmind
 Project-URL: Homepage, https://github.com/strongmind/public-reusable-workflows/tree/main/deployment
 Author-email: Belding <teambelding@strongmind.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

## Comparing `strongmind_deployment-1.0.0.dist-info/licenses/LICENSE` & `strongmind_deployment-1.0.1.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `strongmind_deployment-1.0.0.dist-info/RECORD` & `strongmind_deployment-1.0.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 strongmind_deployment/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-strongmind_deployment/container.py,sha256=0SUoH0F1J64VW6Fwo5iUXzgPVJztV6ALNVTb8ws1y9w,4277
-strongmind_deployment/rails.py,sha256=JSQ0VbsxFANA3fdxnFdIZ-6zR8ItIlUj_RQ0NS48sds,4454
-strongmind_deployment-1.0.0.dist-info/METADATA,sha256=suIrQQszEpw0opbtOdQX3dHz3FClQ1PZa7JsMaxTkxg,675
-strongmind_deployment-1.0.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-strongmind_deployment-1.0.0.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
-strongmind_deployment-1.0.0.dist-info/RECORD,,
+strongmind_deployment/container.py,sha256=HIUuyJ6rSwnwPmY6bvLiyaAJXu0VX9rEo5ERl6aB7VU,7511
+strongmind_deployment/rails.py,sha256=hX2_z5Lb6wyphcrWCLfFWr1cqXNylXCI3nNdQJfhePA,4969
+strongmind_deployment-1.0.1.dist-info/METADATA,sha256=xR-nXsqRfT5CoYKfyMKBZl0dM7Hhw6Oxv5rkPrZDcc0,675
+strongmind_deployment-1.0.1.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+strongmind_deployment-1.0.1.dist-info/licenses/LICENSE,sha256=2zBZXFllrbHYl8Zg63B1X0QWHK1ed93SzZQVh9gd77c,1053
+strongmind_deployment-1.0.1.dist-info/RECORD,,
```

