# Comparing `tmp/xia_scw_instance-0.0.9-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_instance-0.1.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,13 @@
-Zip file size: 114821 bytes, number of entries: 12
--rw-r--r--  2.0 unx      133 b- defN 23-Apr-22 16:35 xia_scw_instance/__init__.py
--rw-r--r--  2.0 unx   266752 b- defN 23-Apr-22 16:44 xia_scw_instance/instance.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx       69 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/backend.tf
--rw-rw-rw-  2.0 unx     3026 b- defN 23-Apr-22 12:29 xia_scw_instance/templates/ScwInstance/main.tf
--rw-rw-rw-  2.0 unx      766 b- defN 23-Apr-22 16:35 xia_scw_instance/templates/ScwInstance/output.tf
+Zip file size: 141323 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      133 b- defN 23-May-03 21:18 xia_scw_instance/__init__.py
+-rw-r--r--  2.0 unx   334848 b- defN 23-May-03 21:27 xia_scw_instance/instance.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 unx     3518 b- defN 23-May-03 09:32 xia_scw_instance/templates/ScwInstance/main.tf
+-rw-rw-rw-  2.0 unx      882 b- defN 23-May-03 05:16 xia_scw_instance/templates/ScwInstance/output.tf
 -rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 11:31 xia_scw_instance/templates/ScwInstance/provider.tf
--rw-rw-rw-  2.0 unx     4173 b- defN 23-Apr-22 10:42 xia_scw_instance/templates/ScwInstance/variables.tf
--rw-rw-rw-  2.0 unx      152 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      699 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1145 b- defN 23-Apr-22 16:44 xia_scw_instance-0.0.9.dist-info/RECORD
-12 files, 277374 bytes uncompressed, 112839 bytes compressed:  59.3%
+-rw-rw-rw-  2.0 unx     4919 b- defN 23-May-03 09:32 xia_scw_instance/templates/ScwInstance/variables.tf
+-rw-rw-rw-  2.0 unx      150 b- defN 23-May-03 21:27 xia_scw_instance-0.1.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      693 b- defN 23-May-03 21:27 xia_scw_instance-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       99 b- defN 23-May-03 21:27 xia_scw_instance-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-03 21:27 xia_scw_instance-0.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1041 b- defN 23-May-03 21:27 xia_scw_instance-0.1.0.dist-info/RECORD
+11 files, 346643 bytes uncompressed, 139515 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,37 +1,34 @@
 Filename: xia_scw_instance/__init__.py
 Comment: 
 
 Filename: xia_scw_instance/instance.cp39-win_amd64.pyd
 Comment: 
 
-Filename: xia_scw_instance/templates/ScwInstance/backend.tf
-Comment: 
-
 Filename: xia_scw_instance/templates/ScwInstance/main.tf
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/output.tf
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/provider.tf
 Comment: 
 
 Filename: xia_scw_instance/templates/ScwInstance/variables.tf
 Comment: 
 
-Filename: xia_scw_instance-0.0.9.dist-info/LICENSE.txt
+Filename: xia_scw_instance-0.1.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.9.dist-info/METADATA
+Filename: xia_scw_instance-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_instance-0.0.9.dist-info/WHEEL
+Filename: xia_scw_instance-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_instance-0.0.9.dist-info/top_level.txt
+Filename: xia_scw_instance-0.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_instance-0.0.9.dist-info/RECORD
+Filename: xia_scw_instance-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_instance/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_instance.instance import ScwInstance, ScwForward
 
 
 __all__ = [
     "ScwInstance", "ScwForward"
 ]
 
-__version__ = "0.0.9"
+__version__ = "0.1.0"
```

## xia_scw_instance/templates/ScwInstance/main.tf

```diff
@@ -1,76 +1,81 @@
+locals {
+  wan_ip = try(var.vpc_details.wan_ip, null)
+  ssh_hosts = try(concat([var.vpc_details.lan_address], var.ssh_hosts), [])
+  bastion_port = try(var.vpc_details.bastion_port, null)
+  private_network_id = try(var.vpc_details.private_network_id, null)
+  gateway_network_id = try(var.vpc_details.gateway_network_id, null)
+}
+
 data "scaleway_instance_image" "my_image" {
-  name  = var.image
+  name = var.image
+  zone = var.zone
 }
 
 resource "scaleway_instance_server" "instance" {
-  name = var.name
-  type = var.type
+  name  = var.name
+  zone  = var.zone
+  type  = var.type
   image = data.scaleway_instance_image.my_image.id
-  tags = var.tags
-  state = var.state
+  tags  = var.tags
+  state = var.state == "maintenance" ? "started" : var.state
 }
 
 
 data "scaleway_vpc_public_gateway" "main" {
+  zone = var.zone
   name = var.vpc_name
 }
 
-data scaleway_vpc_private_network "service" {
-  name = var.lan_name
-}
-
-data scaleway_vpc_gateway_network "service_net" {
-    gateway_id = data.scaleway_vpc_public_gateway.main.id
-    private_network_id = data.scaleway_vpc_private_network.service.id
-}
-
 resource "scaleway_instance_private_nic" "service_nic" {
-  count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
-  server_id = scaleway_instance_server.instance.id
-  private_network_id = data.scaleway_vpc_private_network.service.id
+  count              = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
+  zone               = var.zone
+  server_id          = scaleway_instance_server.instance.id
+  private_network_id = local.private_network_id
 }
 
 resource "time_sleep" "wait_5_seconds_after_service_nic" {
-  count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
-  depends_on = [scaleway_instance_private_nic.service_nic]
+  count           = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
+  depends_on      = [scaleway_instance_private_nic.service_nic]
   create_duration = "5s"
 }
 
 resource scaleway_vpc_public_gateway_dhcp_reservation main {
-    count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
+  count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
 
-    gateway_network_id = data.scaleway_vpc_gateway_network.service_net.id
-    mac_address = scaleway_instance_private_nic.service_nic[0].mac_address
-    ip_address = var.lan_ip
-    depends_on = [time_sleep.wait_5_seconds_after_service_nic]
+  zone               = var.zone
+  gateway_network_id = local.gateway_network_id
+  mac_address        = scaleway_instance_private_nic.service_nic[0].mac_address
+  ip_address         = var.lan_ip
+  depends_on         = [time_sleep.wait_5_seconds_after_service_nic]
 }
 
 locals {
-  ufw_ssh = length(var.ssh_hosts) > 0 ? [
-    for ip in var.ssh_hosts : "ufw allow from ${ip} to any port 22 proto tcp"
+  ufw_ssh = length(local.ssh_hosts) > 0 && var.state != "maintenance" ? [
+  for ip in local.ssh_hosts : "ufw allow from ${ip} to any port 22 proto tcp"
   ] : [
     "ufw allow ssh"
   ]
   ufw_commands = flatten([
-    for rule in var.forwards : [
-      for ip in rule.allowed_ips : "ufw allow from ${ip} to any port ${rule.lan_port} proto ${rule.protocol}"
-    ]
+  for rule in var.forwards : [
+  for ip in rule.allowed_ips : "ufw allow from ${ip} to any port ${rule.lan_port} proto ${rule.protocol}"
+  ]
   ])
 }
 
 resource scaleway_vpc_public_gateway_pat_rule service_pat {
-    for_each = { for i, item in var.forwards : i => item }
+  for_each = { for i, item in var.forwards : i => item if contains(keys(item), "wan_port") && item.wan_port != null }
 
-    gateway_id = data.scaleway_vpc_public_gateway.main.id
-    private_ip = var.lan_ip
-    private_port = each.value["lan_port"]
-    public_port = each.value["wan_port"]
-    protocol = each.value["protocol"]
-    depends_on = [scaleway_vpc_public_gateway_dhcp_reservation.main]
+  zone         = var.zone
+  gateway_id   = data.scaleway_vpc_public_gateway.main.id
+  private_ip   = var.lan_ip != "" && var.lan_ip != null ? var.lan_ip : "192.0.0.1"
+  private_port = each.value["lan_port"]
+  public_port  = contains(keys(each.value), "wan_port") && each.value["wan_port"] != null ? each.value["wan_port"] : 59999
+  protocol     = each.value["protocol"]
+  depends_on   = [scaleway_vpc_public_gateway_dhcp_reservation.main]
 }
 
 resource "null_resource" "ufw_status" {
   count = (var.state != "stopped" && length(var.lan_ip) > 0) ? 1 : 0
 
   triggers = {
     ssh_status = jsonencode(local.ufw_ssh)
@@ -87,19 +92,19 @@
 
     connection {
       type        = "ssh"
       user        = "root"
       private_key = file(var.ssh_private_key)
       host        = var.lan_ip
 
-      bastion_host        = var.wan_ip
-      bastion_port        = 59999
+      bastion_host        = local.wan_ip
+      bastion_port        = local.bastion_port
       bastion_user        = "bastion"
       bastion_private_key = file(var.ssh_private_key)
 
-      timeout              = "5m"   # Maximum time to wait for the connection to become available
+      timeout = "5m"   # Maximum time to wait for the connection to become available
     }
   }
 
   depends_on = [scaleway_vpc_public_gateway_dhcp_reservation.main]
 }
```

## xia_scw_instance/templates/ScwInstance/output.tf

```diff
@@ -2,14 +2,18 @@
   value = var.project_id
 }
 
 output "name" {
   value = scaleway_instance_server.instance.name
 }
 
+output "zone" {
+  value = scaleway_instance_server.instance.zone
+}
+
 output "type" {
   value = scaleway_instance_server.instance.type
 }
 
 output "image" {
   value = data.scaleway_instance_image.my_image.name
 }
@@ -18,20 +22,24 @@
   value = scaleway_instance_server.instance.state
 }
 
 output "tags" {
   value = scaleway_instance_server.instance.tags
 }
 
+output "tf_state" {
+  value = var.tf_state
+}
+
 output "vpc_name" {
   value = var.vpc_name
 }
 
 output "wan_ip" {
-  value = var.wan_ip
+  value = local.wan_ip
 }
 
 output "lan_ip" {
   value = var.lan_ip
 }
 
 output "lan_name" {
```

## xia_scw_instance/templates/ScwInstance/variables.tf

```diff
@@ -15,14 +15,21 @@
 variable "name" {
   type = string
   default = null  #xia#
   #xia# default = {% if name is defined and name is not none %}"{{ name }}"{% else %}null{% endif %}
 
 }
 
+variable "zone" {
+  type = string
+  default = null  #xia#
+  #xia# default = {% if zone is defined and zone is not none %}"{{ zone }}"{% else %}null{% endif %}
+
+}
+
 variable "type" {
   type = string
   default = null  #xia#
   #xia# default = {% if type is defined and type is not none %}"{{ type }}"{% else %}null{% endif %}
 
 }
 
@@ -35,28 +42,47 @@
 
 variable "tags" {
     type = list(string)
     default = null  #xia#
     #xia# default = [{% for v in tags %}{% if loop.index > 1 %}, {% endif %}{% if v is not none %}"{{ v }}"{% else %}null{% endif %}{% endfor %}]
 }
 
-variable "vpc_name" {
+variable "tf_state" {
   type = string
   default = null  #xia#
-  #xia# default = {% if vpc_name is defined and vpc_name is not none %}"{{ vpc_name }}"{% else %}null{% endif %}
+  #xia# default = {% if tf_state is defined and tf_state is not none %}"{{ tf_state }}"{% else %}null{% endif %}
 
 }
 
-variable "wan_ip" {
+variable "vpc_name" {
   type = string
   default = null  #xia#
-  #xia# default = {% if wan_ip is defined and wan_ip is not none %}"{{ wan_ip }}"{% else %}null{% endif %}
+  #xia# default = {% if vpc_name is defined and vpc_name is not none %}"{{ vpc_name }}"{% else %}null{% endif %}
 
 }
 
+variable "vpc_details" {
+  type = any
+  default = null  #xia#
+#xia#   default = {
+#xia#     {% for k, v in vpc_details.items() if not k.startswith('_') %}
+#xia#       {% if v is boolean %}
+#xia#       {{ k }} = {% if v is none %}null{% elif v %}true{% else %}false{% endif %}
+
+#xia#       {% elif v is string %}
+#xia#       {{ k }} = {% if v is not none %}"{{ v }}"{% else %}null{% endif %}
+
+#xia#       {% elif v is number %}
+#xia#       {{ k }} = {% if v is not none %}{{ v }}{% else %}null{% endif %}
+
+#xia#       {% endif %}
+#xia#     {% endfor %}
+#xia#   }
+}
+
 variable "lan_ip" {
   type = string
   default = null  #xia#
   #xia# default = {% if lan_ip is defined and lan_ip is not none %}"{{ lan_ip }}"{% else %}null{% endif %}
 
 }
 
@@ -84,15 +110,15 @@
     error_message = "Each element of the allowed_ip variable must be a valid IPv4 address or an IPv4 address with a subnet mask."
   }
 }
 
 variable "forwards" {
     type = list(object({
       protocol = string
-      wan_port = number
+      wan_port = optional(number)
       lan_port = number
       allowed_ips = list(string)
     }))
     default = null  #xia#
 #xia#     default = [{% for v in forwards %}
 #xia#             {% if loop.index > 1 %},{% endif %}{
 #xia#             {% for w, x in v.items() %}
```

## Comparing `xia_scw_instance-0.0.9.dist-info/METADATA` & `xia_scw_instance-0.1.0.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: xia-scw-instance
-Version: 0.0.9
+Version: 0.1.0
 Summary: X-I-A
-Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.0.9/index.html
+Home-page: https://develop.x-i-a.com/docs/xia-scw-instance/0.1.0/index.html
 Author: X-I-A
 Author-email: admin@x-i-a.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: xia-engine-terraform
+Requires-Dist: xia-fields-scw
 Requires-Dist: xia-scw-vpc
 
 .. image:: https://img.shields.io/pypi/v/xia-scw-instance.svg?color=blue
    :alt: PyPI-Server
    :target: https://pypi.org/project/xia-scw-instance/
 
 ====================================
```

