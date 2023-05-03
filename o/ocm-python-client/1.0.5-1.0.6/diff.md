# Comparing `tmp/ocm_python_client-1.0.5.tar.gz` & `tmp/ocm_python_client-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocm_python_client-1.0.5.tar", last modified: Mon Aug  8 09:55:35 2022, max compression
+gzip compressed data, was "ocm_python_client-1.0.6.tar", last modified: Wed Mar  8 14:24:24 2023, max compression
```

## Comparing `ocm_python_client-1.0.5.tar` & `ocm_python_client-1.0.6.tar`

### file list

```diff
@@ -1,189 +1,215 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 09:55:35.727470 ocm_python_client-1.0.5/
--rw-r--r--   0 root         (0) root         (0)    11357 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)    58124 2022-08-08 09:55:35.727470 ocm_python_client-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    57407 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 09:55:35.696467 ocm_python_client-1.0.5/ocm_python_client/
--rw-r--r--   0 root         (0) root         (0)      830 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 09:55:35.697467 ocm_python_client-1.0.5/ocm_python_client/api/
--rw-r--r--   0 root         (0) root         (0)      221 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   787442 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/api/default_api.py
--rw-r--r--   0 root         (0) root         (0)    39265 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 09:55:35.698467 ocm_python_client-1.0.5/ocm_python_client/apis/
--rw-r--r--   0 root         (0) root         (0)      487 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/apis/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16702 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5138 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 09:55:35.727470 ocm_python_client-1.0.5/ocm_python_client/model/
--rw-r--r--   0 root         (0) root         (0)      351 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19366 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on.py
--rw-r--r--   0 root         (0) root         (0)    12848 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_config.py
--rw-r--r--   0 root         (0) root         (0)    12719 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_environment_variable.py
--rw-r--r--   0 root         (0) root         (0)    12283 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_install_mode.py
--rw-r--r--   0 root         (0) root         (0)    15618 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_installation.py
--rw-r--r--   0 root         (0) root         (0)    12503 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_installation_parameter.py
--rw-r--r--   0 root         (0) root         (0)    12491 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_installation_state.py
--rw-r--r--   0 root         (0) root         (0)    15765 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_parameter.py
--rw-r--r--   0 root         (0) root         (0)    12399 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_parameter_option.py
--rw-r--r--   0 root         (0) root         (0)    13071 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_requirement.py
--rw-r--r--   0 root         (0) root         (0)    11960 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_requirement_status.py
--rw-r--r--   0 root         (0) root         (0)    12227 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_sub_operator.py
--rw-r--r--   0 root         (0) root         (0)    15340 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/add_on_version.py
--rw-r--r--   0 root         (0) root         (0)    11814 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/admin_credentials.py
--rw-r--r--   0 root         (0) root         (0)    11993 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/alert_info.py
--rw-r--r--   0 root         (0) root         (0)    12282 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/alert_severity.py
--rw-r--r--   0 root         (0) root         (0)    11662 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/alerts_info.py
--rw-r--r--   0 root         (0) root         (0)    12916 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_addons_addon_id_versions_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12805 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_addons_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    13023 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_infrastructure_access_roles_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12916 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_machine_types_post200_response.py
--rw-r--r--   0 root         (0) root         (0)    13541 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_regions_post200_response.py
--rw-r--r--   0 root         (0) root         (0)    13000 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_credential_requests_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12907 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_policies_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    13503 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_vpcs_post200_response.py
--rw-r--r--   0 root         (0) root         (0)    13631 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post200_response.py
--rw-r--r--   0 root         (0) root         (0)    13585 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12901 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12967 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addons_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    13189 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12740 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12764 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12840 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12677 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12704 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12812 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12874 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12891 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post200_response.py
--rw-r--r--   0 root         (0) root         (0)    12610 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request.py
--rw-r--r--   0 root         (0) root         (0)    12706 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12833 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12663 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_logs_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12752 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12955 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12777 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12826 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12826 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_flavours_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    13592 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_encryption_keys_post200_response.py
--rw-r--r--   0 root         (0) root         (0)    13528 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_key_rings_post200_response.py
--rw-r--r--   0 root         (0) root         (0)    12863 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_limited_support_reason_templates_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12881 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_machine_types_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12826 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_products_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12783 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_provision_shards_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12927 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_version_gates_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    12876 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_versions_get200_response.py
--rw-r--r--   0 root         (0) root         (0)    13739 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws.py
--rw-r--r--   0 root         (0) root         (0)    13404 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws_flavour.py
--rw-r--r--   0 root         (0) root         (0)    13419 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws_infrastructure_access_role.py
--rw-r--r--   0 root         (0) root         (0)    14273 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws_infrastructure_access_role_grant.py
--rw-r--r--   0 root         (0) root         (0)    12502 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws_infrastructure_access_role_grant_state.py
--rw-r--r--   0 root         (0) root         (0)    12307 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws_infrastructure_access_role_state.py
--rw-r--r--   0 root         (0) root         (0)    12700 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws_machine_pool.py
--rw-r--r--   0 root         (0) root         (0)    12599 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws_spot_market_options.py
--rw-r--r--   0 root         (0) root         (0)    11733 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/aws_volume.py
--rw-r--r--   0 root         (0) root         (0)    11961 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/awssts_policy.py
--rw-r--r--   0 root         (0) root         (0)    12183 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/billing_model.py
--rw-r--r--   0 root         (0) root         (0)    12890 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/ccs.py
--rw-r--r--   0 root         (0) root         (0)    12911 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cloud_provider.py
--rw-r--r--   0 root         (0) root         (0)    12686 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cloud_provider_data.py
--rw-r--r--   0 root         (0) root         (0)    14512 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cloud_region.py
--rw-r--r--   0 root         (0) root         (0)    12568 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cloud_vpc.py
--rw-r--r--   0 root         (0) root         (0)    30250 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster.py
--rw-r--r--   0 root         (0) root         (0)    11972 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_api.py
--rw-r--r--   0 root         (0) root         (0)    12167 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_configuration_mode.py
--rw-r--r--   0 root         (0) root         (0)    11551 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_console.py
--rw-r--r--   0 root         (0) root         (0)    13262 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_credentials.py
--rw-r--r--   0 root         (0) root         (0)    12668 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_deployment.py
--rw-r--r--   0 root         (0) root         (0)    12329 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_health_state.py
--rw-r--r--   0 root         (0) root         (0)    14800 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_nodes.py
--rw-r--r--   0 root         (0) root         (0)    13020 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_operator_info.py
--rw-r--r--   0 root         (0) root         (0)    12363 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_operator_state.py
--rw-r--r--   0 root         (0) root         (0)    11778 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_operators_info.py
--rw-r--r--   0 root         (0) root         (0)    12996 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_registration.py
--rw-r--r--   0 root         (0) root         (0)    13164 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_resources.py
--rw-r--r--   0 root         (0) root         (0)    12927 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_state.py
--rw-r--r--   0 root         (0) root         (0)    14878 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cluster_status.py
--rw-r--r--   0 root         (0) root         (0)    12492 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cpu_total_node_role_os_metric_node.py
--rw-r--r--   0 root         (0) root         (0)    11877 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/cpu_totals_node_role_os_metric_node.py
--rw-r--r--   0 root         (0) root         (0)    12643 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/credential_request.py
--rw-r--r--   0 root         (0) root         (0)    11980 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/detection_type.py
--rw-r--r--   0 root         (0) root         (0)    14444 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/dns.py
--rw-r--r--   0 root         (0) root         (0)    12415 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/encryption_key.py
--rw-r--r--   0 root         (0) root         (0)    12363 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/environment.py
--rw-r--r--   0 root         (0) root         (0)    13472 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/error.py
--rw-r--r--   0 root         (0) root         (0)    12186 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/event.py
--rw-r--r--   0 root         (0) root         (0)    12213 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/external_configuration.py
--rw-r--r--   0 root         (0) root         (0)    13903 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/flavour.py
--rw-r--r--   0 root         (0) root         (0)    11560 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/flavour_nodes.py
--rw-r--r--   0 root         (0) root         (0)    14027 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/gcp.py
--rw-r--r--   0 root         (0) root         (0)    12522 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/gcp_flavour.py
--rw-r--r--   0 root         (0) root         (0)    12192 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/gcp_network.py
--rw-r--r--   0 root         (0) root         (0)    13824 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/github_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)    12527 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/gitlab_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)    12261 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/google_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)    12516 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/group.py
--rw-r--r--   0 root         (0) root         (0)    12407 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/ht_passwd_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)    12204 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/ht_passwd_user.py
--rw-r--r--   0 root         (0) root         (0)    11968 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/hyper_shift.py
--rw-r--r--   0 root         (0) root         (0)    16717 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/identity_provider.py
--rw-r--r--   0 root         (0) root         (0)    12512 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/identity_provider_mapping_method.py
--rw-r--r--   0 root         (0) root         (0)    12989 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/identity_provider_type.py
--rw-r--r--   0 root         (0) root         (0)    14233 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/inflight_check.py
--rw-r--r--   0 root         (0) root         (0)    12279 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/inflight_check_state.py
--rw-r--r--   0 root         (0) root         (0)    13725 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/ingress.py
--rw-r--r--   0 root         (0) root         (0)    12010 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/instance_iam_roles.py
--rw-r--r--   0 root         (0) root         (0)    12361 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/key_ring.py
--rw-r--r--   0 root         (0) root         (0)    12585 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/label.py
--rw-r--r--   0 root         (0) root         (0)    12539 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/ldap_attributes.py
--rw-r--r--   0 root         (0) root         (0)    13633 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/ldap_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)    14000 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/limited_support_reason.py
--rw-r--r--   0 root         (0) root         (0)    12834 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/limited_support_reason_template.py
--rw-r--r--   0 root         (0) root         (0)    12174 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/listening_method.py
--rw-r--r--   0 root         (0) root         (0)    12344 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/log.py
--rw-r--r--   0 root         (0) root         (0)    15671 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/machine_pool.py
--rw-r--r--   0 root         (0) root         (0)    12894 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/machine_pool_autoscaling.py
--rw-r--r--   0 root         (0) root         (0)    11707 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/machine_pool_security_group_filter.py
--rw-r--r--   0 root         (0) root         (0)    15218 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/machine_type.py
--rw-r--r--   0 root         (0) root         (0)    12520 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/machine_type_category.py
--rw-r--r--   0 root         (0) root         (0)    12138 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/machine_type_size.py
--rw-r--r--   0 root         (0) root         (0)    11894 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/managed_service.py
--rw-r--r--   0 root         (0) root         (0)    11556 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/metadata.py
--rw-r--r--   0 root         (0) root         (0)    13120 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/network.py
--rw-r--r--   0 root         (0) root         (0)    11903 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/node_info.py
--rw-r--r--   0 root         (0) root         (0)    12201 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/node_type.py
--rw-r--r--   0 root         (0) root         (0)    11647 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/nodes_info.py
--rw-r--r--   0 root         (0) root         (0)    12525 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/open_id_claims.py
--rw-r--r--   0 root         (0) root         (0)    13872 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/open_id_identity_provider.py
--rw-r--r--   0 root         (0) root         (0)    12823 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/operator_iam_role.py
--rw-r--r--   0 root         (0) root         (0)    12359 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/product.py
--rw-r--r--   0 root         (0) root         (0)    15075 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/provision_shard.py
--rw-r--r--   0 root         (0) root         (0)    12302 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/proxy.py
--rw-r--r--   0 root         (0) root         (0)    12406 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/server_config.py
--rw-r--r--   0 root         (0) root         (0)    12522 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/socket_total_node_role_os_metric_node.py
--rw-r--r--   0 root         (0) root         (0)    11922 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/socket_totals_node_role_os_metric_node.py
--rw-r--r--   0 root         (0) root         (0)    11849 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/ssh_credentials.py
--rw-r--r--   0 root         (0) root         (0)    14959 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/sts.py
--rw-r--r--   0 root         (0) root         (0)    11930 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/sts_credential_request.py
--rw-r--r--   0 root         (0) root         (0)    12570 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/sts_operator.py
--rw-r--r--   0 root         (0) root         (0)    12234 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/subnetwork.py
--rw-r--r--   0 root         (0) root         (0)    12172 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/subscription.py
--rw-r--r--   0 root         (0) root         (0)    12646 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/syncset.py
--rw-r--r--   0 root         (0) root         (0)    12119 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/taint.py
--rw-r--r--   0 root         (0) root         (0)    14668 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/upgrade_policy.py
--rw-r--r--   0 root         (0) root         (0)    12946 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/upgrade_policy_state.py
--rw-r--r--   0 root         (0) root         (0)    12630 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/upgrade_policy_state_value.py
--rw-r--r--   0 root         (0) root         (0)    12116 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/user.py
--rw-r--r--   0 root         (0) root         (0)    11760 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/value.py
--rw-r--r--   0 root         (0) root         (0)    15536 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/version.py
--rw-r--r--   0 root         (0) root         (0)    15119 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/version_gate.py
--rw-r--r--   0 root         (0) root         (0)    12987 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model/version_gate_agreement.py
--rw-r--r--   0 root         (0) root         (0)    82559 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/model_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 09:55:35.727470 ocm_python_client-1.0.5/ocm_python_client/models/
--rw-r--r--   0 root         (0) root         (0)    15134 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14345 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/ocm_python_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-08 09:55:35.697467 ocm_python_client-1.0.5/ocm_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    58124 2022-08-08 09:55:35.000000 ocm_python_client-1.0.5/ocm_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9714 2022-08-08 09:55:35.000000 ocm_python_client-1.0.5/ocm_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-08 09:55:35.000000 ocm_python_client-1.0.5/ocm_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2022-08-08 09:55:35.000000 ocm_python_client-1.0.5/ocm_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-08-08 09:55:35.000000 ocm_python_client-1.0.5/ocm_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      724 2022-08-08 09:55:35.728470 ocm_python_client-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      366 2022-08-08 09:55:24.000000 ocm_python_client-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 14:24:24.334824 ocm_python_client-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-03-08 14:24:09.000000 ocm_python_client-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    58124 2023-03-08 14:24:24.334824 ocm_python_client-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    57407 2023-03-08 14:24:09.000000 ocm_python_client-1.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 14:24:24.283823 ocm_python_client-1.0.6/ocm_python_client/
+-rw-r--r--   0 root         (0) root         (0)      830 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 14:24:24.285823 ocm_python_client-1.0.6/ocm_python_client/api/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1011822 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/api/default_api.py
+-rw-r--r--   0 root         (0) root         (0)    39265 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 14:24:24.287823 ocm_python_client-1.0.6/ocm_python_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/apis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16702 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5138 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 14:24:24.333824 ocm_python_client-1.0.6/ocm_python_client/model/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20643 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on.py
+-rw-r--r--   0 root         (0) root         (0)    13404 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_config.py
+-rw-r--r--   0 root         (0) root         (0)    12719 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_environment_variable.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_install_mode.py
+-rw-r--r--   0 root         (0) root         (0)    16036 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_installation.py
+-rw-r--r--   0 root         (0) root         (0)    13049 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_installation_billing.py
+-rw-r--r--   0 root         (0) root         (0)    12503 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_installation_parameter.py
+-rw-r--r--   0 root         (0) root         (0)    12491 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_installation_state.py
+-rw-r--r--   0 root         (0) root         (0)    13047 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_namespace.py
+-rw-r--r--   0 root         (0) root         (0)    16731 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_parameter.py
+-rw-r--r--   0 root         (0) root         (0)    12743 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_parameter_option.py
+-rw-r--r--   0 root         (0) root         (0)    13071 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    11960 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_requirement_status.py
+-rw-r--r--   0 root         (0) root         (0)    12551 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_secret_propagation.py
+-rw-r--r--   0 root         (0) root         (0)    12227 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_sub_operator.py
+-rw-r--r--   0 root         (0) root         (0)    16317 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/add_on_version.py
+-rw-r--r--   0 root         (0) root         (0)    12426 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/additional_catalog_source.py
+-rw-r--r--   0 root         (0) root         (0)    14457 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/addon_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)    12981 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/addon_upgrade_policy_state.py
+-rw-r--r--   0 root         (0) root         (0)    11814 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/admin_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    11993 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/alert_info.py
+-rw-r--r--   0 root         (0) root         (0)    12282 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)    11662 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/alerts_info.py
+-rw-r--r--   0 root         (0) root         (0)    12916 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_addons_addon_id_versions_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12805 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_addons_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13023 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_infrastructure_access_roles_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12916 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_machine_types_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13541 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_regions_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13000 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_credential_requests_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12907 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_policies_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13503 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_vpcs_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13631 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13585 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12901 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12840 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12967 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addons_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13189 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12899 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12740 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12776 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12764 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12840 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12704 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12812 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12874 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12891 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12610 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request.py
+-rw-r--r--   0 root         (0) root         (0)    12706 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12833 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12663 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_logs_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12752 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12716 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12955 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12777 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_flavours_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13592 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_encryption_keys_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13528 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_key_rings_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12863 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_limited_support_reason_templates_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12881 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_machine_types_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_products_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_provision_shards_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12927 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_version_gates_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12876 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_versions_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    14709 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws.py
+-rw-r--r--   0 root         (0) root         (0)    11622 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_etcd_encryption.py
+-rw-r--r--   0 root         (0) root         (0)    13404 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_flavour.py
+-rw-r--r--   0 root         (0) root         (0)    13419 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_infrastructure_access_role.py
+-rw-r--r--   0 root         (0) root         (0)    14273 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_infrastructure_access_role_grant.py
+-rw-r--r--   0 root         (0) root         (0)    12502 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_infrastructure_access_role_grant_state.py
+-rw-r--r--   0 root         (0) root         (0)    12307 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_infrastructure_access_role_state.py
+-rw-r--r--   0 root         (0) root         (0)    12700 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_machine_pool.py
+-rw-r--r--   0 root         (0) root         (0)    13400 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_node_pool.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_spot_market_options.py
+-rw-r--r--   0 root         (0) root         (0)    11733 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/aws_volume.py
+-rw-r--r--   0 root         (0) root         (0)    12196 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/awssts_policy.py
+-rw-r--r--   0 root         (0) root         (0)    12573 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/billing_model.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/byo_oidc.py
+-rw-r--r--   0 root         (0) root         (0)    12890 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/ccs.py
+-rw-r--r--   0 root         (0) root         (0)    12911 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cloud_provider.py
+-rw-r--r--   0 root         (0) root         (0)    13274 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cloud_provider_data.py
+-rw-r--r--   0 root         (0) root         (0)    14932 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cloud_region.py
+-rw-r--r--   0 root         (0) root         (0)    12568 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cloud_vpc.py
+-rw-r--r--   0 root         (0) root         (0)    31402 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster.py
+-rw-r--r--   0 root         (0) root         (0)    11972 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_api.py
+-rw-r--r--   0 root         (0) root         (0)    12167 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_configuration_mode.py
+-rw-r--r--   0 root         (0) root         (0)    11551 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_console.py
+-rw-r--r--   0 root         (0) root         (0)    13262 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    12668 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_deployment.py
+-rw-r--r--   0 root         (0) root         (0)    12329 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_health_state.py
+-rw-r--r--   0 root         (0) root         (0)    15343 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_nodes.py
+-rw-r--r--   0 root         (0) root         (0)    13020 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_operator_info.py
+-rw-r--r--   0 root         (0) root         (0)    12363 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_operator_state.py
+-rw-r--r--   0 root         (0) root         (0)    11778 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_operators_info.py
+-rw-r--r--   0 root         (0) root         (0)    12687 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_registration.py
+-rw-r--r--   0 root         (0) root         (0)    13164 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_resources.py
+-rw-r--r--   0 root         (0) root         (0)    12927 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_state.py
+-rw-r--r--   0 root         (0) root         (0)    15209 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cluster_status.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/control_plane_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)    12492 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cpu_total_node_role_os_metric_node.py
+-rw-r--r--   0 root         (0) root         (0)    11877 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/cpu_totals_node_role_os_metric_node.py
+-rw-r--r--   0 root         (0) root         (0)    12643 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/credential_request.py
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/detection_type.py
+-rw-r--r--   0 root         (0) root         (0)    14444 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/dns.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/encryption_key.py
+-rw-r--r--   0 root         (0) root         (0)    12363 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/environment.py
+-rw-r--r--   0 root         (0) root         (0)    13472 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/error.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/event.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/external_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    13903 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/flavour.py
+-rw-r--r--   0 root         (0) root         (0)    11560 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/flavour_nodes.py
+-rw-r--r--   0 root         (0) root         (0)    14027 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    12519 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/gcp_encryption_key.py
+-rw-r--r--   0 root         (0) root         (0)    13404 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/gcp_flavour.py
+-rw-r--r--   0 root         (0) root         (0)    12192 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/gcp_network.py
+-rw-r--r--   0 root         (0) root         (0)    11503 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/gcp_volume.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/github_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12527 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/gitlab_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12261 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/google_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12516 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/group.py
+-rw-r--r--   0 root         (0) root         (0)    12407 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/ht_passwd_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12204 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/ht_passwd_user.py
+-rw-r--r--   0 root         (0) root         (0)    11968 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/hypershift.py
+-rw-r--r--   0 root         (0) root         (0)    12468 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/hypershift_config.py
+-rw-r--r--   0 root         (0) root         (0)    16717 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12512 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/identity_provider_mapping_method.py
+-rw-r--r--   0 root         (0) root         (0)    12989 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/identity_provider_type.py
+-rw-r--r--   0 root         (0) root         (0)    14233 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/inflight_check.py
+-rw-r--r--   0 root         (0) root         (0)    12279 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/inflight_check_state.py
+-rw-r--r--   0 root         (0) root         (0)    13725 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/ingress.py
+-rw-r--r--   0 root         (0) root         (0)    12010 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/instance_iam_roles.py
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)    12585 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/label.py
+-rw-r--r--   0 root         (0) root         (0)    12539 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/ldap_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    13633 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/ldap_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    14000 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/limited_support_reason.py
+-rw-r--r--   0 root         (0) root         (0)    12796 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/limited_support_reason_template.py
+-rw-r--r--   0 root         (0) root         (0)    12174 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/listening_method.py
+-rw-r--r--   0 root         (0) root         (0)    12344 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/log.py
+-rw-r--r--   0 root         (0) root         (0)    15964 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/machine_pool.py
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/machine_pool_autoscaling.py
+-rw-r--r--   0 root         (0) root         (0)    11707 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/machine_pool_security_group_filter.py
+-rw-r--r--   0 root         (0) root         (0)    15218 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)    12520 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/machine_type_category.py
+-rw-r--r--   0 root         (0) root         (0)    12138 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/machine_type_size.py
+-rw-r--r--   0 root         (0) root         (0)    11894 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/managed_service.py
+-rw-r--r--   0 root         (0) root         (0)    12655 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    13120 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/network.py
+-rw-r--r--   0 root         (0) root         (0)    11903 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/node_info.py
+-rw-r--r--   0 root         (0) root         (0)    15956 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/node_pool.py
+-rw-r--r--   0 root         (0) root         (0)    12851 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/node_pool_autoscaling.py
+-rw-r--r--   0 root         (0) root         (0)    12939 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/node_pool_status.py
+-rw-r--r--   0 root         (0) root         (0)    12201 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/node_type.py
+-rw-r--r--   0 root         (0) root         (0)    11647 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/nodes_info.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/open_id_claims.py
+-rw-r--r--   0 root         (0) root         (0)    13872 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/open_id_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12823 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/operator_iam_role.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/private_link_cluster_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    11803 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/private_link_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    12551 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/private_link_principal.py
+-rw-r--r--   0 root         (0) root         (0)    12813 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/private_link_principals.py
+-rw-r--r--   0 root         (0) root         (0)    12359 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/product.py
+-rw-r--r--   0 root         (0) root         (0)    16784 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/provision_shard.py
+-rw-r--r--   0 root         (0) root         (0)    12302 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/proxy.py
+-rw-r--r--   0 root         (0) root         (0)    12674 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/server_config.py
+-rw-r--r--   0 root         (0) root         (0)    12522 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/socket_total_node_role_os_metric_node.py
+-rw-r--r--   0 root         (0) root         (0)    11922 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/socket_totals_node_role_os_metric_node.py
+-rw-r--r--   0 root         (0) root         (0)    11849 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/ssh_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    16007 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/sts.py
+-rw-r--r--   0 root         (0) root         (0)    11930 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/sts_credential_request.py
+-rw-r--r--   0 root         (0) root         (0)    12570 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/sts_operator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)    12172 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    12646 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/syncset.py
+-rw-r--r--   0 root         (0) root         (0)    12119 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/taint.py
+-rw-r--r--   0 root         (0) root         (0)    14668 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)    12946 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/upgrade_policy_state.py
+-rw-r--r--   0 root         (0) root         (0)    12630 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/upgrade_policy_state_value.py
+-rw-r--r--   0 root         (0) root         (0)    12116 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/user.py
+-rw-r--r--   0 root         (0) root         (0)    11760 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/value.py
+-rw-r--r--   0 root         (0) root         (0)    15973 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/version.py
+-rw-r--r--   0 root         (0) root         (0)    15119 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/version_gate.py
+-rw-r--r--   0 root         (0) root         (0)    12987 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model/version_gate_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    82559 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/model_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 14:24:24.334824 ocm_python_client-1.0.6/ocm_python_client/models/
+-rw-r--r--   0 root         (0) root         (0)    17685 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14345 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/ocm_python_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-08 14:24:24.284823 ocm_python_client-1.0.6/ocm_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    58124 2023-03-08 14:24:24.000000 ocm_python_client-1.0.6/ocm_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11272 2023-03-08 14:24:24.000000 ocm_python_client-1.0.6/ocm_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-08 14:24:24.000000 ocm_python_client-1.0.6/ocm_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-03-08 14:24:24.000000 ocm_python_client-1.0.6/ocm_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-03-08 14:24:24.000000 ocm_python_client-1.0.6/ocm_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      724 2023-03-08 14:24:24.334824 ocm_python_client-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      366 2023-03-08 14:24:14.000000 ocm_python_client-1.0.6/setup.py
```

### Comparing `ocm_python_client-1.0.5/LICENSE` & `ocm_python_client-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/PKG-INFO` & `ocm_python_client-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ocm_python_client
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python client for https://api.openshift.com/api/ APIs
 Home-page: https://github.com/RedHatQE/openshift-cluster-management-python-client
-Download-URL: https://github.com/RedHatQE/openshift-cluster-management-python-client/archive/refs/tags/v1.0.5.tar.gz
+Download-URL: https://github.com/RedHatQE/openshift-cluster-management-python-client/archive/refs/tags/v1.0.6.tar.gz
 Author: Ruth Netser
 Author-email: rnetser@redhat.com
 License: apache-2.0
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-cluster-management-python-client/tree/main/docs
 Keywords: Openshift,ocm
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ocm_python_client-1.0.5/README.md` & `ocm_python_client-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/__init__.py` & `ocm_python_client-1.0.6/ocm_python_client/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     The version of the OpenAPI document: v1
     Contact: ocm-feedback@redhat.com
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 # import ApiClient
 from ocm_python_client.api_client import ApiClient
 
 # import Configuration
 from ocm_python_client.configuration import Configuration
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/api/default_api.py` & `ocm_python_client-1.0.6/ocm_python_client/api/default_api.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,41 +24,48 @@
 )
 from ocm_python_client.model.aws import AWS
 from ocm_python_client.model.aws_infrastructure_access_role import AWSInfrastructureAccessRole
 from ocm_python_client.model.aws_infrastructure_access_role_grant import AWSInfrastructureAccessRoleGrant
 from ocm_python_client.model.add_on import AddOn
 from ocm_python_client.model.add_on_installation import AddOnInstallation
 from ocm_python_client.model.add_on_version import AddOnVersion
+from ocm_python_client.model.addon_upgrade_policy import AddonUpgradePolicy
+from ocm_python_client.model.addon_upgrade_policy_state import AddonUpgradePolicyState
 from ocm_python_client.model.alerts_info import AlertsInfo
 from ocm_python_client.model.api_clusters_mgmt_v1_addons_addon_id_versions_get200_response import ApiClustersMgmtV1AddonsAddonIdVersionsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_addons_get200_response import ApiClustersMgmtV1AddonsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_infrastructure_access_roles_get200_response import ApiClustersMgmtV1AwsInfrastructureAccessRolesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_machine_types_post200_response import ApiClustersMgmtV1AwsInquiriesMachineTypesPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_regions_post200_response import ApiClustersMgmtV1AwsInquiriesRegionsPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_sts_credential_requests_get200_response import ApiClustersMgmtV1AwsInquiriesStsCredentialRequestsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_sts_policies_get200_response import ApiClustersMgmtV1AwsInquiriesStsPoliciesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_vpcs_post200_response import ApiClustersMgmtV1AwsInquiriesVpcsPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post200_response import ApiClustersMgmtV1CloudProvidersCloudProviderIdAvailableRegionsPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get200_response import ApiClustersMgmtV1CloudProvidersCloudProviderIdRegionsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_cloud_providers_get200_response import ApiClustersMgmtV1CloudProvidersGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get200_response import ApiClustersMgmtV1ClustersClusterIdAddonUpgradePoliciesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_addons_get200_response import ApiClustersMgmtV1ClustersClusterIdAddonsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get200_response import ApiClustersMgmtV1ClustersClusterIdAwsInfrastructureAccessRoleGrantsGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get200_response import ApiClustersMgmtV1ClustersClusterIdAwsPrivateLinkConfigurationPrincipalsGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get200_response import ApiClustersMgmtV1ClustersClusterIdControlPlaneUpgradePoliciesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get200_response import ApiClustersMgmtV1ClustersClusterIdExternalConfigurationLabelsGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get200_response import ApiClustersMgmtV1ClustersClusterIdExternalConfigurationManifestsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get200_response import ApiClustersMgmtV1ClustersClusterIdExternalConfigurationSyncsetsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get200_response import ApiClustersMgmtV1ClustersClusterIdGateAgreementsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_groups_get200_response import ApiClustersMgmtV1ClustersClusterIdGroupsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get200_response import ApiClustersMgmtV1ClustersClusterIdGroupsGroupIdUsersGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get200_response import ApiClustersMgmtV1ClustersClusterIdIdentityProvidersGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get200_response import ApiClustersMgmtV1ClustersClusterIdIdentityProvidersIdentityProviderIdHtpasswdUsersGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post200_response import ApiClustersMgmtV1ClustersClusterIdIdentityProvidersIdentityProviderIdHtpasswdUsersImportPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request import ApiClustersMgmtV1ClustersClusterIdIdentityProvidersIdentityProviderIdHtpasswdUsersImportPostRequest
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get200_response import ApiClustersMgmtV1ClustersClusterIdIngressesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get200_response import ApiClustersMgmtV1ClustersClusterIdLimitedSupportReasonsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_logs_get200_response import ApiClustersMgmtV1ClustersClusterIdLogsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get200_response import ApiClustersMgmtV1ClustersClusterIdMachinePoolsGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get200_response import ApiClustersMgmtV1ClustersClusterIdNodePoolsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get200_response import ApiClustersMgmtV1ClustersClusterIdStsOperatorRolesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get200_response import ApiClustersMgmtV1ClustersClusterIdUpgradePoliciesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_get200_response import ApiClustersMgmtV1ClustersGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_flavours_get200_response import ApiClustersMgmtV1FlavoursGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_gcp_inquiries_encryption_keys_post200_response import ApiClustersMgmtV1GcpInquiriesEncryptionKeysPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_gcp_inquiries_key_rings_post200_response import ApiClustersMgmtV1GcpInquiriesKeyRingsPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_limited_support_reason_templates_get200_response import ApiClustersMgmtV1LimitedSupportReasonTemplatesGet200Response
@@ -72,31 +79,38 @@
 from ocm_python_client.model.cloud_provider_data import CloudProviderData
 from ocm_python_client.model.cloud_region import CloudRegion
 from ocm_python_client.model.cluster import Cluster
 from ocm_python_client.model.cluster_credentials import ClusterCredentials
 from ocm_python_client.model.cluster_operators_info import ClusterOperatorsInfo
 from ocm_python_client.model.cluster_resources import ClusterResources
 from ocm_python_client.model.cluster_status import ClusterStatus
+from ocm_python_client.model.control_plane_upgrade_policy import ControlPlaneUpgradePolicy
 from ocm_python_client.model.environment import Environment
 from ocm_python_client.model.error import Error
 from ocm_python_client.model.event import Event
 from ocm_python_client.model.external_configuration import ExternalConfiguration
 from ocm_python_client.model.flavour import Flavour
 from ocm_python_client.model.group import Group
 from ocm_python_client.model.ht_passwd_user import HTPasswdUser
+from ocm_python_client.model.hypershift_config import HypershiftConfig
 from ocm_python_client.model.identity_provider import IdentityProvider
 from ocm_python_client.model.ingress import Ingress
 from ocm_python_client.model.label import Label
 from ocm_python_client.model.limited_support_reason import LimitedSupportReason
 from ocm_python_client.model.limited_support_reason_template import LimitedSupportReasonTemplate
 from ocm_python_client.model.log import Log
 from ocm_python_client.model.machine_pool import MachinePool
+from ocm_python_client.model.machine_type import MachineType
+from ocm_python_client.model.manifest import Manifest
 from ocm_python_client.model.metadata import Metadata
+from ocm_python_client.model.node_pool import NodePool
 from ocm_python_client.model.nodes_info import NodesInfo
 from ocm_python_client.model.operator_iam_role import OperatorIAMRole
+from ocm_python_client.model.private_link_configuration import PrivateLinkConfiguration
+from ocm_python_client.model.private_link_principal import PrivateLinkPrincipal
 from ocm_python_client.model.product import Product
 from ocm_python_client.model.provision_shard import ProvisionShard
 from ocm_python_client.model.socket_totals_node_role_os_metric_node import SocketTotalsNodeRoleOSMetricNode
 from ocm_python_client.model.syncset import Syncset
 from ocm_python_client.model.upgrade_policy import UpgradePolicy
 from ocm_python_client.model.upgrade_policy_state import UpgradePolicyState
 from ocm_python_client.model.user import User
@@ -127,15 +141,17 @@
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'addon_id',
                 ],
-                'required': [],
+                'required': [
+                    'addon_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -176,15 +192,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'addon_id',
                 ],
-                'required': [],
+                'required': [
+                    'addon_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -226,15 +244,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'addon_id',
                     'add_on',
                 ],
-                'required': [],
+                'required': [
+                    'addon_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -284,15 +304,17 @@
                 'all': [
                     'addon_id',
                     'order',
                     'page',
                     'search',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'addon_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -350,15 +372,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'addon_id',
                     'add_on_version',
                 ],
-                'required': [],
+                'required': [
+                    'addon_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -405,15 +429,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'addon_id',
                     'version_id',
                 ],
-                'required': [],
+                'required': [
+                    'addon_id',
+                    'version_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -459,15 +486,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'addon_id',
                     'version_id',
                 ],
-                'required': [],
+                'required': [
+                    'addon_id',
+                    'version_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -514,15 +544,18 @@
             },
             params_map={
                 'all': [
                     'addon_id',
                     'version_id',
                     'add_on_version',
                 ],
-                'required': [],
+                'required': [
+                    'addon_id',
+                    'version_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -686,15 +719,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'aws_infrastructure_access_role_id',
                 ],
-                'required': [],
+                'required': [
+                    'aws_infrastructure_access_role_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1100,15 +1135,17 @@
             params_map={
                 'all': [
                     'cloud_provider_id',
                     'page',
                     'size',
                     'aws',
                 ],
-                'required': [],
+                'required': [
+                    'cloud_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1162,15 +1199,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cloud_provider_id',
                 ],
-                'required': [],
+                'required': [
+                    'cloud_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1213,15 +1252,17 @@
             },
             params_map={
                 'all': [
                     'cloud_provider_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cloud_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1271,15 +1312,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cloud_provider_id',
                     'region_id',
                 ],
-                'required': [],
+                'required': [
+                    'cloud_provider_id',
+                    'region_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1389,15 +1433,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'addon_inquiry_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'addon_inquiry_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1446,15 +1493,17 @@
                 'all': [
                     'cluster_id',
                     'order',
                     'page',
                     'search',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1496,14 +1545,429 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/addon_upgrade_policies/{addon_upgrade_policy_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'addon_upgrade_policy_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'addon_upgrade_policy_id': 'addon_upgrade_policy_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'addon_upgrade_policy_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (AddonUpgradePolicy,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/addon_upgrade_policies/{addon_upgrade_policy_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'addon_upgrade_policy_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'addon_upgrade_policy_id': 'addon_upgrade_policy_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'addon_upgrade_policy_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (AddonUpgradePolicy,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/addon_upgrade_policies/{addon_upgrade_policy_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                    'addon_upgrade_policy',
+                ],
+                'required': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'addon_upgrade_policy_id':
+                        (str,),
+                    'addon_upgrade_policy':
+                        (AddonUpgradePolicy,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'addon_upgrade_policy_id': 'addon_upgrade_policy_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'addon_upgrade_policy_id': 'path',
+                    'addon_upgrade_policy': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (AddonUpgradePolicyState,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/addon_upgrade_policies/{addon_upgrade_policy_id}/state',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'addon_upgrade_policy_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'addon_upgrade_policy_id': 'addon_upgrade_policy_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'addon_upgrade_policy_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (AddonUpgradePolicyState,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/addon_upgrade_policies/{addon_upgrade_policy_id}/state',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                    'addon_upgrade_policy_state',
+                ],
+                'required': [
+                    'cluster_id',
+                    'addon_upgrade_policy_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'addon_upgrade_policy_id':
+                        (str,),
+                    'addon_upgrade_policy_state':
+                        (AddonUpgradePolicyState,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'addon_upgrade_policy_id': 'addon_upgrade_policy_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'addon_upgrade_policy_id': 'path',
+                    'addon_upgrade_policy_state': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (ApiClustersMgmtV1ClustersClusterIdAddonUpgradePoliciesGet200Response,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/addon_upgrade_policies',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'page',
+                    'size',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'page': 'page',
+                    'size': 'size',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (AddonUpgradePolicy,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/addon_upgrade_policies',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'addon_upgrade_policy',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'addon_upgrade_policy':
+                        (AddonUpgradePolicy,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'addon_upgrade_policy': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/addons/{addoninstallation_id}',
@@ -1512,15 +1976,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'addoninstallation_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'addoninstallation_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1566,15 +2033,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'addoninstallation_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'addoninstallation_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1621,15 +2091,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'addoninstallation_id',
                     'add_on_installation',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'addoninstallation_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1683,15 +2156,17 @@
                 'all': [
                     'cluster_id',
                     'order',
                     'page',
                     'search',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1749,15 +2224,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'add_on_installation',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1804,15 +2281,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'aws_infrastructure_access_role_grant_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'aws_infrastructure_access_role_grant_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1858,15 +2338,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'aws_infrastructure_access_role_grant_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'aws_infrastructure_access_role_grant_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1915,15 +2398,17 @@
                 'all': [
                     'cluster_id',
                     'order',
                     'page',
                     'search',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -1981,15 +2466,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'aws_infrastructure_access_role_grant',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2020,14 +2507,302 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (PrivateLinkConfiguration,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/aws/private_link_configuration',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (ApiClustersMgmtV1ClustersClusterIdAwsPrivateLinkConfigurationPrincipalsGet200Response,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/aws/private_link_configuration/principals',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'page',
+                    'search',
+                    'size',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'page':
+                        (int,),
+                    'search':
+                        (str,),
+                    'size':
+                        (int,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'page': 'page',
+                    'search': 'search',
+                    'size': 'size',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'page': 'query',
+                    'search': 'query',
+                    'size': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (PrivateLinkPrincipal,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/aws/private_link_configuration/principals',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'private_link_principal',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'private_link_principal':
+                        (PrivateLinkPrincipal,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'private_link_principal': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/aws/private_link_configuration/principals/{principal_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'principal_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'principal_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'principal_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'principal_id': 'principal_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'principal_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (PrivateLinkPrincipal,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/aws/private_link_configuration/principals/{principal_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'principal_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'principal_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'principal_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'principal_id': 'principal_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'principal_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_clusters_cluster_id_clusterdeployment_delete_endpoint = _Endpoint(
             settings={
                 'response_type': None,
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/clusterdeployment',
@@ -2035,15 +2810,17 @@
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2069,14 +2846,309 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/control_plane/upgrade_policies/{control_plane_upgrade_policy_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'control_plane_upgrade_policy_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'control_plane_upgrade_policy_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'control_plane_upgrade_policy_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'control_plane_upgrade_policy_id': 'control_plane_upgrade_policy_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'control_plane_upgrade_policy_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (ControlPlaneUpgradePolicy,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/control_plane/upgrade_policies/{control_plane_upgrade_policy_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'control_plane_upgrade_policy_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'control_plane_upgrade_policy_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'control_plane_upgrade_policy_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'control_plane_upgrade_policy_id': 'control_plane_upgrade_policy_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'control_plane_upgrade_policy_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (ControlPlaneUpgradePolicy,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/control_plane/upgrade_policies/{control_plane_upgrade_policy_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'control_plane_upgrade_policy_id',
+                    'control_plane_upgrade_policy',
+                ],
+                'required': [
+                    'cluster_id',
+                    'control_plane_upgrade_policy_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'control_plane_upgrade_policy_id':
+                        (str,),
+                    'control_plane_upgrade_policy':
+                        (ControlPlaneUpgradePolicy,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'control_plane_upgrade_policy_id': 'control_plane_upgrade_policy_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'control_plane_upgrade_policy_id': 'path',
+                    'control_plane_upgrade_policy': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (ApiClustersMgmtV1ClustersClusterIdControlPlaneUpgradePoliciesGet200Response,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/control_plane/upgrade_policies',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'page',
+                    'size',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'page': 'page',
+                    'size': 'size',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (ControlPlaneUpgradePolicy,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/control_plane/upgrade_policies',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'control_plane_upgrade_policy',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'control_plane_upgrade_policy':
+                        (ControlPlaneUpgradePolicy,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'control_plane_upgrade_policy': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_clusters_cluster_id_credentials_get_endpoint = _Endpoint(
             settings={
                 'response_type': (ClusterCredentials,),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/credentials',
@@ -2084,15 +3156,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2135,15 +3209,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'deprovision',
                     'dry_run',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2192,15 +3268,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2243,15 +3321,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2301,15 +3381,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'label_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'label_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2355,15 +3438,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'label_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'label_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2410,15 +3496,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'label_id',
                     'label',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'label_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2469,15 +3558,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'label',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2508,14 +3599,309 @@
                 ],
                 'content_type': [
                     'application/json'
                 ]
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (ApiClustersMgmtV1ClustersClusterIdExternalConfigurationManifestsGet200Response,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/external_configuration/manifests',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'page',
+                    'size',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'page': 'page',
+                    'size': 'size',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/external_configuration/manifests/{manifest_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'manifest_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'manifest_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'manifest_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'manifest_id': 'manifest_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'manifest_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (Manifest,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/external_configuration/manifests/{manifest_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'manifest_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'manifest_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'manifest_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'manifest_id': 'manifest_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'manifest_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (Manifest,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/external_configuration/manifests/{manifest_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'manifest_id',
+                    'manifest',
+                ],
+                'required': [
+                    'cluster_id',
+                    'manifest_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'manifest_id':
+                        (str,),
+                    'manifest':
+                        (Manifest,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'manifest_id': 'manifest_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'manifest_id': 'path',
+                    'manifest': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (Manifest,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/external_configuration/manifests',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'manifest',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'manifest':
+                        (Manifest,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'manifest': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get_endpoint = _Endpoint(
             settings={
                 'response_type': (ApiClustersMgmtV1ClustersClusterIdExternalConfigurationSyncsetsGet200Response,),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/external_configuration/syncsets',
@@ -2525,15 +3911,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2583,15 +3971,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'syncset',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2638,15 +4028,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'syncset_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'syncset_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2692,15 +4085,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'syncset_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'syncset_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2747,15 +4143,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'syncset_id',
                     'syncset',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'syncset_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2807,15 +4206,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2865,15 +4266,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'version_gate_agreement',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2920,15 +4323,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'version_gate_agreement_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'version_gate_agreement_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -2974,15 +4380,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'version_gate_agreement_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'version_gate_agreement_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3027,15 +4436,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3078,15 +4489,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3136,15 +4549,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'group_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'group_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3192,15 +4608,18 @@
             params_map={
                 'all': [
                     'cluster_id',
                     'group_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'group_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3255,15 +4674,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'group_id',
                     'user',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'group_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3315,15 +4737,19 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'group_id',
                     'user_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'group_id',
+                    'user_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3374,15 +4800,19 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'group_id',
                     'user_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'group_id',
+                    'user_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3431,15 +4861,68 @@
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_hypershift_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (HypershiftConfig,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/hypershift',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_hypershift_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3482,15 +4965,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3540,15 +5025,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3594,15 +5082,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3650,15 +5141,18 @@
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3713,15 +5207,19 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                     'htpasswd_user_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                    'htpasswd_user_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3772,15 +5270,19 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                     'htpasswd_user_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                    'htpasswd_user_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3832,15 +5334,19 @@
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                     'htpasswd_user_id',
                     'ht_passwd_user',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                    'htpasswd_user_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3896,15 +5402,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                     'api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -3956,15 +5465,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                     'ht_passwd_user',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4016,15 +5528,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider_id',
                     'identity_provider',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'identity_provider_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4075,15 +5590,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'identity_provider',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4131,15 +5648,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4189,15 +5708,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'ingress_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'ingress_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4243,15 +5765,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'ingress_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'ingress_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4298,15 +5823,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'ingress_id',
                     'ingress',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'ingress_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4357,15 +5885,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'ingress',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4412,15 +5942,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'ingress',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4468,15 +6000,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4526,15 +6060,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'limited_support_reason_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'limited_support_reason_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4580,15 +6117,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'limited_support_reason_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'limited_support_reason_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4634,15 +6174,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'limited_support_reason',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4690,15 +6232,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4749,15 +6293,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'offset',
                     'tail',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4808,15 +6354,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'offset',
                     'tail',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4867,15 +6415,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4925,15 +6475,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'machine_pool_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'machine_pool_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -4979,15 +6532,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'machine_pool_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'machine_pool_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5034,15 +6590,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'machine_pool_id',
                     'machine_pool',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'machine_pool_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5093,15 +6652,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'machine_pool',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5147,15 +6708,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5196,15 +6759,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5245,15 +6810,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5294,15 +6861,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5343,15 +6912,188 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (ApiClustersMgmtV1ClustersClusterIdNodePoolsGet200Response,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/node_pools',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'page',
+                    'size',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'page':
+                        (int,),
+                    'size':
+                        (int,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'page': 'page',
+                    'size': 'size',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'page': 'query',
+                    'size': 'query',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/node_pools/{node_pool_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'node_pool_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'node_pool_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'node_pool_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'node_pool_id': 'node_pool_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'node_pool_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (NodePool,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/node_pools/{node_pool_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'node_pool_id',
+                ],
+                'required': [
+                    'cluster_id',
+                    'node_pool_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5359,32 +7101,156 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'cluster_id':
                         (str,),
+                    'node_pool_id':
+                        (str,),
                 },
                 'attribute_map': {
                     'cluster_id': 'cluster_id',
+                    'node_pool_id': 'node_pool_id',
                 },
                 'location_map': {
                     'cluster_id': 'path',
+                    'node_pool_id': 'path',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (NodePool,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/node_pools/{node_pool_id}',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'node_pool_id',
+                    'node_pool',
+                ],
+                'required': [
+                    'cluster_id',
+                    'node_pool_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'node_pool_id':
+                        (str,),
+                    'node_pool':
+                        (NodePool,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                    'node_pool_id': 'node_pool_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'node_pool_id': 'path',
+                    'node_pool': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (NodePool,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/node_pools',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_node_pools_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'node_pool',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'node_pool':
+                        (NodePool,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'node_pool': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_clusters_cluster_id_patch_endpoint = _Endpoint(
             settings={
                 'response_type': (Cluster,),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}',
@@ -5393,15 +7259,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'cluster',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5447,15 +7315,68 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/provision_shard',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5496,15 +7417,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5530,14 +7453,71 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (ProvisionShard,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/provision_shard',
+                'operation_id': 'api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'cluster_id',
+                    'provision_shard',
+                ],
+                'required': [
+                    'cluster_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'cluster_id':
+                        (str,),
+                    'provision_shard':
+                        (ProvisionShard,),
+                },
+                'attribute_map': {
+                    'cluster_id': 'cluster_id',
+                },
+                'location_map': {
+                    'cluster_id': 'path',
+                    'provision_shard': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_clusters_cluster_id_resources_get_endpoint = _Endpoint(
             settings={
                 'response_type': (ClusterResources,),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/clusters/{cluster_id}/resources',
@@ -5545,15 +7525,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5594,15 +7576,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5643,15 +7627,17 @@
                 'http_method': 'POST',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5692,15 +7678,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5743,15 +7731,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5801,15 +7791,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'operator_iam_role_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'operator_iam_role_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5855,15 +7848,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'operator_iam_role',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5911,15 +7906,17 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'page',
                     'size',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -5969,15 +7966,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'upgrade_policy',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -6024,15 +8023,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'upgrade_policy_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'upgrade_policy_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -6078,15 +8080,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'upgrade_policy_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'upgrade_policy_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -6133,15 +8138,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'upgrade_policy_id',
                     'upgrade_policy',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'upgrade_policy_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -6192,15 +8200,18 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'upgrade_policy_id',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'upgrade_policy_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -6247,15 +8258,18 @@
             },
             params_map={
                 'all': [
                     'cluster_id',
                     'upgrade_policy_id',
                     'upgrade_policy_state',
                 ],
-                'required': [],
+                'required': [
+                    'cluster_id',
+                    'upgrade_policy_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -6563,15 +8577,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'flavour_id',
                 ],
-                'required': [],
+                'required': [
+                    'flavour_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -6613,15 +8629,17 @@
                 'servers': None,
             },
             params_map={
                 'all': [
                     'flavour_id',
                     'flavour',
                 ],
-                'required': [],
+                'required': [
+                    'flavour_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -7119,15 +9137,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'limited_support_reason_template_id',
                 ],
-                'required': [],
+                'required': [
+                    'limited_support_reason_template_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -7217,14 +9237,65 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_machine_types_machine_type_id_get_endpoint = _Endpoint(
+            settings={
+                'response_type': (MachineType,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/machine_types/{machine_type_id}',
+                'operation_id': 'api_clusters_mgmt_v1_machine_types_machine_type_id_get',
+                'http_method': 'GET',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'machine_type_id',
+                ],
+                'required': [
+                    'machine_type_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'machine_type_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'machine_type_id': 'machine_type_id',
+                },
+                'location_map': {
+                    'machine_type_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_products_get_endpoint = _Endpoint(
             settings={
                 'response_type': (ApiClustersMgmtV1ProductsGet200Response,),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/products',
@@ -7296,15 +9367,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'product_id',
                 ],
-                'required': [],
+                'required': [
+                    'product_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -7344,14 +9417,15 @@
                 'operation_id': 'api_clusters_mgmt_v1_provision_shards_get',
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'page',
+                    'search',
                     'size',
                 ],
                 'required': [],
                 'nullable': [
                 ],
                 'enum': [
                 ],
@@ -7362,36 +9436,141 @@
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'page':
                         (int,),
+                    'search':
+                        (str,),
                     'size':
                         (int,),
                 },
                 'attribute_map': {
                     'page': 'page',
+                    'search': 'search',
                     'size': 'size',
                 },
                 'location_map': {
                     'page': 'query',
+                    'search': 'query',
                     'size': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_provision_shards_post_endpoint = _Endpoint(
+            settings={
+                'response_type': (ProvisionShard,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/provision_shards',
+                'operation_id': 'api_clusters_mgmt_v1_provision_shards_post',
+                'http_method': 'POST',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'provision_shard',
+                ],
+                'required': [],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'provision_shard':
+                        (ProvisionShard,),
+                },
+                'attribute_map': {
+                },
+                'location_map': {
+                    'provision_shard': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
+        self.api_clusters_mgmt_v1_provision_shards_provision_shard_id_delete_endpoint = _Endpoint(
+            settings={
+                'response_type': None,
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/provision_shards/{provision_shard_id}',
+                'operation_id': 'api_clusters_mgmt_v1_provision_shards_provision_shard_id_delete',
+                'http_method': 'DELETE',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'provision_shard_id',
+                ],
+                'required': [
+                    'provision_shard_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'provision_shard_id':
+                        (str,),
+                },
+                'attribute_map': {
+                    'provision_shard_id': 'provision_shard_id',
+                },
+                'location_map': {
+                    'provision_shard_id': 'path',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [],
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_provision_shards_provision_shard_id_get_endpoint = _Endpoint(
             settings={
                 'response_type': (ProvisionShard,),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/provision_shards/{provision_shard_id}',
@@ -7399,15 +9578,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'provision_shard_id',
                 ],
-                'required': [],
+                'required': [
+                    'provision_shard_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -7433,14 +9614,71 @@
                 'accept': [
                     'application/json'
                 ],
                 'content_type': [],
             },
             api_client=api_client
         )
+        self.api_clusters_mgmt_v1_provision_shards_provision_shard_id_patch_endpoint = _Endpoint(
+            settings={
+                'response_type': (ProvisionShard,),
+                'auth': [
+                    'bearer'
+                ],
+                'endpoint_path': '/api/clusters_mgmt/v1/provision_shards/{provision_shard_id}',
+                'operation_id': 'api_clusters_mgmt_v1_provision_shards_provision_shard_id_patch',
+                'http_method': 'PATCH',
+                'servers': None,
+            },
+            params_map={
+                'all': [
+                    'provision_shard_id',
+                    'provision_shard',
+                ],
+                'required': [
+                    'provision_shard_id',
+                ],
+                'nullable': [
+                ],
+                'enum': [
+                ],
+                'validation': [
+                ]
+            },
+            root_map={
+                'validations': {
+                },
+                'allowed_values': {
+                },
+                'openapi_types': {
+                    'provision_shard_id':
+                        (str,),
+                    'provision_shard':
+                        (ProvisionShard,),
+                },
+                'attribute_map': {
+                    'provision_shard_id': 'provision_shard_id',
+                },
+                'location_map': {
+                    'provision_shard_id': 'path',
+                    'provision_shard': 'body',
+                },
+                'collection_format_map': {
+                }
+            },
+            headers_map={
+                'accept': [
+                    'application/json'
+                ],
+                'content_type': [
+                    'application/json'
+                ]
+            },
+            api_client=api_client
+        )
         self.api_clusters_mgmt_v1_version_gates_get_endpoint = _Endpoint(
             settings={
                 'response_type': (ApiClustersMgmtV1VersionGatesGet200Response,),
                 'auth': [
                     'bearer'
                 ],
                 'endpoint_path': '/api/clusters_mgmt/v1/version_gates',
@@ -7562,15 +9800,17 @@
                 'http_method': 'DELETE',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'version_gate_id',
                 ],
-                'required': [],
+                'required': [
+                    'version_gate_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -7611,15 +9851,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'version_gate_id',
                 ],
-                'required': [],
+                'required': [
+                    'version_gate_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -7724,15 +9966,17 @@
                 'http_method': 'GET',
                 'servers': None,
             },
             params_map={
                 'all': [
                     'version_id',
                 ],
-                'required': [],
+                'required': [
+                    'version_id',
+                ],
                 'nullable': [
                 ],
                 'enum': [
                 ],
                 'validation': [
                 ]
             },
@@ -7761,28 +10005,30 @@
                 'content_type': [],
             },
             api_client=api_client
         )
 
     def api_clusters_mgmt_v1_addons_addon_id_delete(
         self,
+        addon_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_addon_id_delete  # noqa: E501
 
         Deletes the add-on.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_delete(addon_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            addon_id (str):
 
         Keyword Args:
-            addon_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -7836,32 +10082,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['addon_id'] = \
+            addon_id
         return self.api_clusters_mgmt_v1_addons_addon_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_addons_addon_id_get(
         self,
+        addon_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_addon_id_get  # noqa: E501
 
         Retrieves the details of the add-on.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_get(addon_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            addon_id (str):
 
         Keyword Args:
-            addon_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -7915,32 +10165,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['addon_id'] = \
+            addon_id
         return self.api_clusters_mgmt_v1_addons_addon_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_addons_addon_id_patch(
         self,
+        addon_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_addon_id_patch  # noqa: E501
 
         Updates the add-on.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_patch(addon_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            addon_id (str):
 
         Keyword Args:
-            addon_id (str): [optional]
             add_on (AddOn): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -7995,32 +10249,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['addon_id'] = \
+            addon_id
         return self.api_clusters_mgmt_v1_addons_addon_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_addons_addon_id_versions_get(
         self,
+        addon_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_addon_id_versions_get  # noqa: E501
 
         Retrieves the list of add-on versions.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_get(addon_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            addon_id (str):
 
         Keyword Args:
-            addon_id (str): [optional]
             order (str): Order criteria.  The syntax of this parameter is similar to the syntax of the _order by_ clause of a SQL statement, but using the names of the attributes of the add-on instead of the names of the columns of a table. For example, in order to sort the add-on versions descending by id the value should be:  ```sql id desc ```  If the parameter isn't provided, or if the value is empty, then the order of the results is undefined.. [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             search (str): Search criteria.  The syntax of this parameter is similar to the syntax of the _where_ clause of an SQL statement, but using the names of the attributes of the add-on version instead of the names of the columns of a table. For example, in order to retrieve all the add-on versions with an id starting with `0.1` the value should be:  ```sql id like '0.1.%' ```  If the parameter isn't provided, or if the value is empty, then all the add-on versions that the user has permission to see will be returned.. [optional]
             size (int): Maximum number of items that will be contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -8078,32 +10336,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['addon_id'] = \
+            addon_id
         return self.api_clusters_mgmt_v1_addons_addon_id_versions_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_addons_addon_id_versions_post(
         self,
+        addon_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_addon_id_versions_post  # noqa: E501
 
         Create a new add-on version and add it to the collection of add-ons.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_post(addon_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            addon_id (str):
 
         Keyword Args:
-            addon_id (str): [optional]
             add_on_version (AddOnVersion): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -8158,33 +10420,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['addon_id'] = \
+            addon_id
         return self.api_clusters_mgmt_v1_addons_addon_id_versions_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_addons_addon_id_versions_version_id_delete(
         self,
+        addon_id,
+        version_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_addon_id_versions_version_id_delete  # noqa: E501
 
         Deletes the add-on version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_delete(addon_id, version_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            addon_id (str):
+            version_id (str):
 
         Keyword Args:
-            addon_id (str): [optional]
-            version_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -8238,33 +10505,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['addon_id'] = \
+            addon_id
+        kwargs['version_id'] = \
+            version_id
         return self.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_addons_addon_id_versions_version_id_get(
         self,
+        addon_id,
+        version_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_addon_id_versions_version_id_get  # noqa: E501
 
         Retrieves the details of the add-on version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_get(addon_id, version_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            addon_id (str):
+            version_id (str):
 
         Keyword Args:
-            addon_id (str): [optional]
-            version_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -8318,33 +10592,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['addon_id'] = \
+            addon_id
+        kwargs['version_id'] = \
+            version_id
         return self.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_addons_addon_id_versions_version_id_patch(
         self,
+        addon_id,
+        version_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_addon_id_versions_version_id_patch  # noqa: E501
 
         Updates the add-on version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_patch(addon_id, version_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            addon_id (str):
+            version_id (str):
 
         Keyword Args:
-            addon_id (str): [optional]
-            version_id (str): [optional]
             add_on_version (AddOnVersion): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -8399,14 +10680,18 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['addon_id'] = \
+            addon_id
+        kwargs['version_id'] = \
+            version_id
         return self.api_clusters_mgmt_v1_addons_addon_id_versions_version_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_addons_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_addons_get  # noqa: E501
@@ -8564,28 +10849,30 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_addons_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_aws_infrastructure_access_roles_aws_infrastructure_access_role_id_get(
         self,
+        aws_infrastructure_access_role_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_aws_infrastructure_access_roles_aws_infrastructure_access_role_id_get  # noqa: E501
 
         Retrieves the details of the aws infrastructure access role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_aws_infrastructure_access_roles_aws_infrastructure_access_role_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_aws_infrastructure_access_roles_aws_infrastructure_access_role_id_get(aws_infrastructure_access_role_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            aws_infrastructure_access_role_id (str):
 
         Keyword Args:
-            aws_infrastructure_access_role_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -8639,14 +10926,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['aws_infrastructure_access_role_id'] = \
+            aws_infrastructure_access_role_id
         return self.api_clusters_mgmt_v1_aws_infrastructure_access_roles_aws_infrastructure_access_role_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_aws_infrastructure_access_roles_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_aws_infrastructure_access_roles_get  # noqa: E501
@@ -9129,28 +11418,30 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_aws_inquiries_vpcs_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post(
         self,
+        cloud_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post  # noqa: E501
 
         Retrieves the list of available regions of the cloud provider.  IMPORTANT: This collection doesn't currently support paging or searching, so the returned `page` will always be 1 and `size` and `total` will always be the total number of available regions of the provider.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post(cloud_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cloud_provider_id (str):
 
         Keyword Args:
-            cloud_provider_id (str): [optional]
             page (int): Index of the returned page, where one corresponds to the first page. As this collection doesn't support paging the result will always be `1`.. [optional]
             size (int): Number of items that will be contained in the returned page. As this collection doesn't support paging or searching the result will always be the total number of regions of the provider.. [optional]
             aws (AWS): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
@@ -9207,32 +11498,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cloud_provider_id'] = \
+            cloud_provider_id
         return self.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_get(
         self,
+        cloud_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_get  # noqa: E501
 
         Retrieves the details of the cloud provider.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_get(cloud_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cloud_provider_id (str):
 
         Keyword Args:
-            cloud_provider_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -9286,32 +11581,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cloud_provider_id'] = \
+            cloud_provider_id
         return self.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get(
         self,
+        cloud_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get  # noqa: E501
 
         Retrieves the list of regions of the cloud provider.  IMPORTANT: This collection doesn't currently support paging or searching, so the returned `page` will always be 1 and `size` and `total` will always be the total number of regions of the provider.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get(cloud_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cloud_provider_id (str):
 
         Keyword Args:
-            cloud_provider_id (str): [optional]
             page (int): Index of the returned page, where one corresponds to the first page. As this collection doesn't support paging the result will always be `1`.. [optional]
             size (int): Number of items that will be contained in the returned page. As this collection doesn't support paging or searching the result will always be the total number of regions of the provider.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -9367,33 +11666,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cloud_provider_id'] = \
+            cloud_provider_id
         return self.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_region_id_get(
         self,
+        cloud_provider_id,
+        region_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_region_id_get  # noqa: E501
 
         Retrieves the details of the region.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_region_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_region_id_get(cloud_provider_id, region_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cloud_provider_id (str):
+            region_id (str):
 
         Keyword Args:
-            cloud_provider_id (str): [optional]
-            region_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -9447,14 +11751,18 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cloud_provider_id'] = \
+            cloud_provider_id
+        kwargs['region_id'] = \
+            region_id
         return self.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_region_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_cloud_providers_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_cloud_providers_get  # noqa: E501
@@ -9533,28 +11841,31 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_cloud_providers_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_addon_inquiry_id_get(
         self,
+        cluster_id,
+        addon_inquiry_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_addon_inquiry_id_get  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_addon_inquiry_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_addon_inquiry_id_get(cluster_id, addon_inquiry_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            addon_inquiry_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            addon_inquiry_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -9608,31 +11919,37 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addon_inquiry_id'] = \
+            addon_inquiry_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_addon_inquiry_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_get  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             order (str): Order criteria.  The syntax of this parameter is similar to the syntax of the _order by_ clause of a SQL statement, but using the names of the attributes of the add-on instead of the names of the columns of a table. For example, in order to sort the add-ons descending by name the value should be:  ```sql name desc ```  If the parameter isn't provided, or if the value is empty, then the order of the results is undefined.. [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             search (str): Search criteria.  The syntax of this parameter is similar to the syntax of the _where_ clause of an SQL statement, but using the names of the attributes of the add-on instead of the names of the columns of a table. For example, in order to retrieve all the add-ons with a name starting with `my` the value should be:  ```sql name like 'my%' ```  If the parameter isn't provided, or if the value is empty, then all the add-ons that the user has permission to see will be returned.. [optional]
             size (int): Maximum number of items that will be contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -9690,33 +12007,644 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_inquiries_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_delete(
+        self,
+        cluster_id,
+        addon_upgrade_policy_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_delete  # noqa: E501
+
+        Deletes the addon upgrade policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_delete(cluster_id, addon_upgrade_policy_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            addon_upgrade_policy_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addon_upgrade_policy_id'] = \
+            addon_upgrade_policy_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_delete_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_get(
+        self,
+        cluster_id,
+        addon_upgrade_policy_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_get  # noqa: E501
+
+        Retrieves the details of the addon upgrade policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_get(cluster_id, addon_upgrade_policy_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            addon_upgrade_policy_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            AddonUpgradePolicy
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addon_upgrade_policy_id'] = \
+            addon_upgrade_policy_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_patch(
+        self,
+        cluster_id,
+        addon_upgrade_policy_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_patch  # noqa: E501
+
+        Update the addon upgrade policy.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_patch(cluster_id, addon_upgrade_policy_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            addon_upgrade_policy_id (str):
+
+        Keyword Args:
+            addon_upgrade_policy (AddonUpgradePolicy): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            AddonUpgradePolicy
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addon_upgrade_policy_id'] = \
+            addon_upgrade_policy_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_patch_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_get(
+        self,
+        cluster_id,
+        addon_upgrade_policy_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_get  # noqa: E501
+
+        Retrieves the details of the upgrade policy state.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_get(cluster_id, addon_upgrade_policy_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            addon_upgrade_policy_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            AddonUpgradePolicyState
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addon_upgrade_policy_id'] = \
+            addon_upgrade_policy_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_patch(
+        self,
+        cluster_id,
+        addon_upgrade_policy_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_patch  # noqa: E501
+
+        Update the upgrade policy state.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_patch(cluster_id, addon_upgrade_policy_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            addon_upgrade_policy_id (str):
+
+        Keyword Args:
+            addon_upgrade_policy_state (AddonUpgradePolicyState): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            AddonUpgradePolicyState
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addon_upgrade_policy_id'] = \
+            addon_upgrade_policy_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_addon_upgrade_policy_id_state_patch_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get  # noqa: E501
+
+        Retrieves the list of addon upgrade policies.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            page (int): Index of the requested page, where one corresponds to the first page.. [optional]
+            size (int): Number of items contained in the returned page.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ApiClustersMgmtV1ClustersClusterIdAddonUpgradePoliciesGet200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_post(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_post  # noqa: E501
+
+        Adds a new addon upgrade policy to the cluster.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_post(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            addon_upgrade_policy (AddonUpgradePolicy): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            AddonUpgradePolicy
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_post_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_delete(
         self,
+        cluster_id,
+        addoninstallation_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_delete  # noqa: E501
 
         Delete an add-on installation and remove it from the collection of add-on installations on the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_delete(cluster_id, addoninstallation_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            addoninstallation_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            addoninstallation_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -9770,33 +12698,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addoninstallation_id'] = \
+            addoninstallation_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_get(
         self,
+        cluster_id,
+        addoninstallation_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_get  # noqa: E501
 
         Retrieves the details of the add-on installation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_get(cluster_id, addoninstallation_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            addoninstallation_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            addoninstallation_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -9850,33 +12785,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addoninstallation_id'] = \
+            addoninstallation_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_patch(
         self,
+        cluster_id,
+        addoninstallation_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_patch  # noqa: E501
 
         Updates the add-on installation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_patch(cluster_id, addoninstallation_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            addoninstallation_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            addoninstallation_id (str): [optional]
             add_on_installation (AddOnInstallation): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -9931,32 +12873,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['addoninstallation_id'] = \
+            addoninstallation_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_addons_addoninstallation_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_addons_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_addons_get  # noqa: E501
 
         Retrieves the list of add-on installations.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             order (str): Order criteria.  The syntax of this parameter is similar to the syntax of the _order by_ clause of a SQL statement, but using the names of the attributes of the add-on installation instead of the names of the columns of a table. For example, in order to sort the add-on installations descending by name the value should be:  ```sql name desc ```  If the parameter isn't provided, or if the value is empty, then the order of the results is undefined.. [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             search (str): Search criteria.  The syntax of this parameter is similar to the syntax of the _where_ clause of an SQL statement, but using the names of the attributes of the add-on installation instead of the names of the columns of a table. For example, in order to retrieve all the add-on installations with a name starting with `my` the value should be:  ```sql name like 'my%' ```  If the parameter isn't provided, or if the value is empty, then all the add-on installations that the user has permission to see will be returned.. [optional]
             size (int): Maximum number of items that will be contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -10014,32 +12962,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_addons_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_addons_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_addons_post  # noqa: E501
 
         Create a new add-on installation and add it to the collection of add-on installations on the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_addons_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             add_on_installation (AddOnInstallation): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -10094,33 +13046,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_addons_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_delete(
         self,
+        cluster_id,
+        aws_infrastructure_access_role_grant_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_delete  # noqa: E501
 
         Deletes the AWS infrastructure access role grant.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_delete(cluster_id, aws_infrastructure_access_role_grant_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            aws_infrastructure_access_role_grant_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            aws_infrastructure_access_role_grant_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -10174,33 +13131,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['aws_infrastructure_access_role_grant_id'] = \
+            aws_infrastructure_access_role_grant_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_get(
         self,
+        cluster_id,
+        aws_infrastructure_access_role_grant_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_get  # noqa: E501
 
         Retrieves the details of the AWS infrastructure access role grant.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_get(cluster_id, aws_infrastructure_access_role_grant_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            aws_infrastructure_access_role_grant_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            aws_infrastructure_access_role_grant_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -10254,32 +13218,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['aws_infrastructure_access_role_grant_id'] = \
+            aws_infrastructure_access_role_grant_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_aws_infrastructure_access_role_grant_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get  # noqa: E501
 
         Retrieves the list of AWS infrastructure access role grants.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             order (str): Order criteria.  The syntax of this parameter is similar to the syntax of the _order by_ clause of a SQL statement, but using the names of the attributes of the AWS infrastructure access role grant instead of the names of the columns of a table. For example, in order to sort the AWS infrastructure access role grants descending by user ARN the value should be:  ```sql user_arn desc ```  If the parameter isn't provided, or if the value is empty, then the order of the results is undefined.. [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             search (str): Search criteria.  The syntax of this parameter is similar to the syntax of the _where_ clause of an SQL statement, but using the names of the attributes of the AWS infrastructure access role grant instead of the names of the columns of a table. For example, in order to retrieve all the AWS infrastructure access role grants with a user ARN starting with `user` the value should be:  ```sql user_arn like '%user' ```  If the parameter isn't provided, or if the value is empty, then all the AWS infrastructure access role grants that the user has permission to see will be returned.. [optional]
             size (int): Maximum number of items that will be contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
@@ -10337,32 +13307,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_post  # noqa: E501
 
         Create a new AWS infrastructure access role grant and add it to the collection of AWS infrastructure access role grants on the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             aws_infrastructure_access_role_grant (AWSInfrastructureAccessRoleGrant): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -10417,32 +13391,463 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_post_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_get(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_get  # noqa: E501
+
+        Retrieves the details of the configuration for the Private Link.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_get(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            PrivateLinkConfiguration
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get  # noqa: E501
+
+        Retrieves the list of principals.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            page (int): Index of the requested page, where one corresponds to the first page.. [optional]
+            search (str): Search criteria.  The syntax of this parameter is similar to the syntax of the _where_ clause of an SQL statement, but using the names of the attributes of the role binding instead of the names of the columns of a table. For example, in order to retrieve role bindings with role_id AuthenticatedUser:  ```sql role_id = 'AuthenticatedUser' ```  If the parameter isn't provided, or if the value is empty, then all the items that the user has permission to see will be returned.. [optional]
+            size (int): Number of items contained in the returned page.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ApiClustersMgmtV1ClustersClusterIdAwsPrivateLinkConfigurationPrincipalsGet200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_post(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_post  # noqa: E501
+
+        Adds a new principal for the Private Link.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_post(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            private_link_principal (PrivateLinkPrincipal): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            PrivateLinkPrincipal
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_post_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_delete(
+        self,
+        cluster_id,
+        principal_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_delete  # noqa: E501
+
+        Deletes the principal.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_delete(cluster_id, principal_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            principal_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['principal_id'] = \
+            principal_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_delete_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_get(
+        self,
+        cluster_id,
+        principal_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_get  # noqa: E501
+
+        Retrieves the details of the principal.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_get(cluster_id, principal_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            principal_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            PrivateLinkPrincipal
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['principal_id'] = \
+            principal_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_principal_id_get_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_clusters_cluster_id_clusterdeployment_delete(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_clusterdeployment_delete  # noqa: E501
 
         Deletes the clusterdeployment.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_clusterdeployment_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_clusterdeployment_delete(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -10496,32 +13901,467 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_clusterdeployment_delete_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_delete(
+        self,
+        cluster_id,
+        control_plane_upgrade_policy_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_delete  # noqa: E501
+
+        Deletes the upgrade policy for the control plane.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_delete(cluster_id, control_plane_upgrade_policy_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            control_plane_upgrade_policy_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['control_plane_upgrade_policy_id'] = \
+            control_plane_upgrade_policy_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_delete_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_get(
+        self,
+        cluster_id,
+        control_plane_upgrade_policy_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_get  # noqa: E501
+
+        Retrieves the details of the upgrade policy for the control plane.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_get(cluster_id, control_plane_upgrade_policy_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            control_plane_upgrade_policy_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ControlPlaneUpgradePolicy
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['control_plane_upgrade_policy_id'] = \
+            control_plane_upgrade_policy_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_patch(
+        self,
+        cluster_id,
+        control_plane_upgrade_policy_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_patch  # noqa: E501
+
+        Update the upgrade policy for the control plane.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_patch(cluster_id, control_plane_upgrade_policy_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            control_plane_upgrade_policy_id (str):
+
+        Keyword Args:
+            control_plane_upgrade_policy (ControlPlaneUpgradePolicy): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ControlPlaneUpgradePolicy
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['control_plane_upgrade_policy_id'] = \
+            control_plane_upgrade_policy_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_control_plane_upgrade_policy_id_patch_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get  # noqa: E501
+
+        Retrieves the list of upgrade policies for the control plane.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            page (int): Index of the requested page, where one corresponds to the first page.. [optional]
+            size (int): Number of items contained in the returned page.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ApiClustersMgmtV1ClustersClusterIdControlPlaneUpgradePoliciesGet200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_post(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_post  # noqa: E501
+
+        Adds a new upgrade policy to the control plane of the cluster.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_post(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            control_plane_upgrade_policy (ControlPlaneUpgradePolicy): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ControlPlaneUpgradePolicy
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_post_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_clusters_cluster_id_credentials_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_credentials_get  # noqa: E501
 
         Retrieves the details of the credentials of a cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_credentials_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_credentials_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -10575,32 +14415,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_credentials_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_delete(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_delete  # noqa: E501
 
         Deletes the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_delete(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             deprovision (bool): If false it will only delete from OCM but not the actual cluster resources. false is only allowed for OCP clusters. true by default.. [optional]
             dry_run (bool): Dry run flag is used to check if the operation can be completed, but won't delete.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -10656,32 +14500,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_get  # noqa: E501
 
         Retrieves the details of the external configuration.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -10735,32 +14583,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get  # noqa: E501
 
         Retrieves the list of labels.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -10816,33 +14668,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_delete(
         self,
+        cluster_id,
+        label_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_delete  # noqa: E501
 
         Deletes the label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_delete(cluster_id, label_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            label_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            label_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -10896,33 +14753,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['label_id'] = \
+            label_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_get(
         self,
+        cluster_id,
+        label_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_get  # noqa: E501
 
         Retrieves the details of the label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_get(cluster_id, label_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            label_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            label_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -10976,33 +14840,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['label_id'] = \
+            label_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_patch(
         self,
+        cluster_id,
+        label_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_patch  # noqa: E501
 
         Update the label.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_patch(cluster_id, label_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            label_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            label_id (str): [optional]
             label (Label): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -11057,32 +14928,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['label_id'] = \
+            label_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_label_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_post  # noqa: E501
 
         Adds a new label to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             label (Label): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -11137,32 +15014,467 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_post_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get  # noqa: E501
+
+        Retrieves the list of manifests.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            page (int): Index of the requested page, where one corresponds to the first page.. [optional]
+            size (int): Number of items contained in the returned page.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ApiClustersMgmtV1ClustersClusterIdExternalConfigurationManifestsGet200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_delete(
+        self,
+        cluster_id,
+        manifest_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_delete  # noqa: E501
+
+        Deletes the manifest.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_delete(cluster_id, manifest_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            manifest_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['manifest_id'] = \
+            manifest_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_delete_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_get(
+        self,
+        cluster_id,
+        manifest_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_get  # noqa: E501
+
+        Retrieves the details of the manifest.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_get(cluster_id, manifest_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            manifest_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Manifest
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['manifest_id'] = \
+            manifest_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_patch(
+        self,
+        cluster_id,
+        manifest_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_patch  # noqa: E501
+
+        Update the manifest.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_patch(cluster_id, manifest_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            manifest_id (str):
+
+        Keyword Args:
+            manifest (Manifest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Manifest
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['manifest_id'] = \
+            manifest_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_manifest_id_patch_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_post(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_post  # noqa: E501
+
+        Adds a new manifest to a cluster.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_post(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            manifest (Manifest): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            Manifest
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_post_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get  # noqa: E501
 
         Retrieves the list of syncsets.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -11218,32 +15530,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_post  # noqa: E501
 
         Adds a new syncset to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             syncset (Syncset): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -11298,33 +15614,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_delete(
         self,
+        cluster_id,
+        syncset_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_delete  # noqa: E501
 
         Deletes the syncset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_delete(cluster_id, syncset_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            syncset_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            syncset_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -11378,33 +15699,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['syncset_id'] = \
+            syncset_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_get(
         self,
+        cluster_id,
+        syncset_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_get  # noqa: E501
 
         Retrieves the details of the syncset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_get(cluster_id, syncset_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            syncset_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            syncset_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -11458,33 +15786,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['syncset_id'] = \
+            syncset_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_patch(
         self,
+        cluster_id,
+        syncset_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_patch  # noqa: E501
 
         Update the syncset.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_patch(cluster_id, syncset_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            syncset_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            syncset_id (str): [optional]
             syncset (Syncset): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -11539,32 +15874,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['syncset_id'] = \
+            syncset_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_syncset_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get  # noqa: E501
 
         Retrieves the list of reasons.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -11620,32 +15961,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_post  # noqa: E501
 
         Adds a new agreed version gate to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             version_gate_agreement (VersionGateAgreement): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -11700,33 +16045,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_delete(
         self,
+        cluster_id,
+        version_gate_agreement_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_delete  # noqa: E501
 
         Deletes the version gate agreement.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_delete(cluster_id, version_gate_agreement_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            version_gate_agreement_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            version_gate_agreement_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -11780,33 +16130,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['version_gate_agreement_id'] = \
+            version_gate_agreement_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_get(
         self,
+        cluster_id,
+        version_gate_agreement_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_get  # noqa: E501
 
         Retrieves the details of the version gate agreement.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_get(cluster_id, version_gate_agreement_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            version_gate_agreement_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            version_gate_agreement_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -11860,32 +16217,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['version_gate_agreement_id'] = \
+            version_gate_agreement_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_version_gate_agreement_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_get  # noqa: E501
 
         Retrieves the details of the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -11939,32 +16302,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_groups_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_groups_get  # noqa: E501
 
         Retrieves the list of groups.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -12020,33 +16387,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_groups_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_get(
         self,
+        cluster_id,
+        group_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_get  # noqa: E501
 
         Retrieves the details of the group.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_get(cluster_id, group_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            group_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            group_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -12100,33 +16472,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['group_id'] = \
+            group_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get(
         self,
+        cluster_id,
+        group_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get  # noqa: E501
 
         Retrieves the list of users.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get(cluster_id, group_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            group_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            group_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -12182,33 +16561,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['group_id'] = \
+            group_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_post(
         self,
+        cluster_id,
+        group_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_post  # noqa: E501
 
         Adds a new user to the group.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_post(cluster_id, group_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            group_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            group_id (str): [optional]
             user (User): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -12263,34 +16649,42 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['group_id'] = \
+            group_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_delete(
         self,
+        cluster_id,
+        group_id,
+        user_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_delete  # noqa: E501
 
         Deletes the user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_delete(cluster_id, group_id, user_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            group_id (str):
+            user_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            group_id (str): [optional]
-            user_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -12344,34 +16738,44 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['group_id'] = \
+            group_id
+        kwargs['user_id'] = \
+            user_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_get(
         self,
+        cluster_id,
+        group_id,
+        user_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_get  # noqa: E501
 
         Retrieves the details of the user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_get(cluster_id, group_id, user_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            group_id (str):
+            user_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            group_id (str): [optional]
-            user_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -12425,32 +16829,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['group_id'] = \
+            group_id
+        kwargs['user_id'] = \
+            user_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_user_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_hibernate_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_hibernate_post  # noqa: E501
 
         Initiates cluster hibernation. While hibernating a cluster will not consume any cloud provider infrastructure but will be counted for quota.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_hibernate_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_hibernate_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -12504,32 +16916,119 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_hibernate_post_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_clusters_cluster_id_hypershift_get(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_hypershift_get  # noqa: E501
+
+        Retrieves the Hypershift details for a single cluster.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_hypershift_get(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            HypershiftConfig
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_hypershift_get_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get  # noqa: E501
 
         Retrieves the list of identity providers.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -12585,33 +17084,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_delete(
         self,
+        cluster_id,
+        identity_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_delete  # noqa: E501
 
         Deletes the identity provider.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_delete(cluster_id, identity_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -12665,33 +17169,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_get(
         self,
+        cluster_id,
+        identity_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_get  # noqa: E501
 
         Retrieves the details of the identity provider.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_get(cluster_id, identity_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -12745,33 +17256,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get(
         self,
+        cluster_id,
+        identity_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get  # noqa: E501
 
         Retrieves the list of _HTPasswd_ IDP users.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get(cluster_id, identity_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -12827,34 +17345,42 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_delete(
         self,
+        cluster_id,
+        identity_provider_id,
+        htpasswd_user_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_delete  # noqa: E501
 
         Deletes the user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_delete(cluster_id, identity_provider_id, htpasswd_user_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
+            htpasswd_user_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
-            htpasswd_user_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -12908,34 +17434,44 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
+        kwargs['htpasswd_user_id'] = \
+            htpasswd_user_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_get(
         self,
+        cluster_id,
+        identity_provider_id,
+        htpasswd_user_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_get  # noqa: E501
 
         Retrieves the details of the user.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_get(cluster_id, identity_provider_id, htpasswd_user_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
+            htpasswd_user_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
-            htpasswd_user_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -12989,34 +17525,44 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
+        kwargs['htpasswd_user_id'] = \
+            htpasswd_user_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_patch(
         self,
+        cluster_id,
+        identity_provider_id,
+        htpasswd_user_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_patch  # noqa: E501
 
         Updates the user's password. The username is not editable  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_patch(cluster_id, identity_provider_id, htpasswd_user_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
+            htpasswd_user_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
-            htpasswd_user_id (str): [optional]
             ht_passwd_user (HTPasswdUser): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -13071,33 +17617,42 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
+        kwargs['htpasswd_user_id'] = \
+            htpasswd_user_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_htpasswd_user_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post(
         self,
+        cluster_id,
+        identity_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post  # noqa: E501
 
         Adds multiple new users to the _HTPasswd_ file.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post(cluster_id, identity_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
             api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request (ApiClustersMgmtV1ClustersClusterIdIdentityProvidersIdentityProviderIdHtpasswdUsersImportPostRequest): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -13152,33 +17707,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_post(
         self,
+        cluster_id,
+        identity_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_post  # noqa: E501
 
         Adds a new user to the _HTPasswd_ file.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_post(cluster_id, identity_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
             ht_passwd_user (HTPasswdUser): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -13233,33 +17795,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_patch(
         self,
+        cluster_id,
+        identity_provider_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_patch  # noqa: E501
 
         Update identity provider in the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_patch(cluster_id, identity_provider_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            identity_provider_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            identity_provider_id (str): [optional]
             identity_provider (IdentityProvider): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -13314,32 +17883,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['identity_provider_id'] = \
+            identity_provider_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_post  # noqa: E501
 
         Adds a new identity provider to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             identity_provider (IdentityProvider): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -13394,32 +17969,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get  # noqa: E501
 
         Retrieves the list of ingresses.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -13475,33 +18054,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_delete(
         self,
+        cluster_id,
+        ingress_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_delete  # noqa: E501
 
         Deletes the ingress.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_delete(cluster_id, ingress_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            ingress_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            ingress_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -13555,33 +18139,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['ingress_id'] = \
+            ingress_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_get(
         self,
+        cluster_id,
+        ingress_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_get  # noqa: E501
 
         Retrieves the details of the ingress.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_get(cluster_id, ingress_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            ingress_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            ingress_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -13635,33 +18226,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['ingress_id'] = \
+            ingress_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_patch(
         self,
+        cluster_id,
+        ingress_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_patch  # noqa: E501
 
         Updates the ingress.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_patch(cluster_id, ingress_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            ingress_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            ingress_id (str): [optional]
             ingress (Ingress): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -13716,32 +18314,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['ingress_id'] = \
+            ingress_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_ingress_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_ingresses_patch(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_ingresses_patch  # noqa: E501
 
         Updates all ingresses  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_patch(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             ingress ([Ingress]): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -13796,32 +18400,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_ingresses_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_ingresses_post  # noqa: E501
 
         Adds a new ingress to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             ingress (Ingress): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -13876,32 +18484,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get  # noqa: E501
 
         Retrieves the list of reasons.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -13957,33 +18569,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_delete(
         self,
+        cluster_id,
+        limited_support_reason_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_delete  # noqa: E501
 
         Deletes the reason.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_delete(cluster_id, limited_support_reason_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            limited_support_reason_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            limited_support_reason_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -14037,33 +18654,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['limited_support_reason_id'] = \
+            limited_support_reason_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_get(
         self,
+        cluster_id,
+        limited_support_reason_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_get  # noqa: E501
 
         Retrieves the details of the reason.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_get(cluster_id, limited_support_reason_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            limited_support_reason_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            limited_support_reason_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -14117,32 +18741,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['limited_support_reason_id'] = \
+            limited_support_reason_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_limited_support_reason_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_post  # noqa: E501
 
         Adds a new reason to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             limited_support_reason (LimitedSupportReason): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -14197,32 +18827,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_logs_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_logs_get  # noqa: E501
 
         Retrieves the list of log links.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_logs_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_logs_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -14278,32 +18912,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_logs_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_logs_install_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_logs_install_get  # noqa: E501
 
         Retrieves the details of the log.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_logs_install_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_logs_install_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             offset (int): Line offset to start logs from. if 0 retreive entire log. If offset > #lines return an empty log.. [optional]
             tail (int): Returns the number of tail lines from the end of the log. If there are no line breaks or the number of lines < tail return the entire log. Either 'tail' or 'offset' can be set. Not both. . [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -14359,32 +18997,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_logs_install_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_logs_uninstall_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_logs_uninstall_get  # noqa: E501
 
         Retrieves the details of the log.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_logs_uninstall_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_logs_uninstall_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             offset (int): Line offset to start logs from. if 0 retreive entire log. If offset > #lines return an empty log.. [optional]
             tail (int): Returns the number of tail lines from the end of the log. If there are no line breaks or the number of lines < tail return the entire log. Either 'tail' or 'offset' can be set. Not both. . [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -14440,32 +19082,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_logs_uninstall_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get  # noqa: E501
 
         Retrieves the list of machine pools.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -14521,33 +19167,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_delete(
         self,
+        cluster_id,
+        machine_pool_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_delete  # noqa: E501
 
         Deletes the machine pool.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_delete(cluster_id, machine_pool_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            machine_pool_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            machine_pool_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -14601,33 +19252,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['machine_pool_id'] = \
+            machine_pool_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_get(
         self,
+        cluster_id,
+        machine_pool_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_get  # noqa: E501
 
         Retrieves the details of the machine pool.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_get(cluster_id, machine_pool_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            machine_pool_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            machine_pool_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -14681,33 +19339,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['machine_pool_id'] = \
+            machine_pool_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_patch(
         self,
+        cluster_id,
+        machine_pool_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_patch  # noqa: E501
 
         Updates the machine pool.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_patch(cluster_id, machine_pool_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            machine_pool_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            machine_pool_id (str): [optional]
             machine_pool (MachinePool): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -14762,32 +19427,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['machine_pool_id'] = \
+            machine_pool_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_machine_pool_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_post  # noqa: E501
 
         Adds a new machine pool to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             machine_pool (MachinePool): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -14842,31 +19513,35 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_alerts_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_alerts_get  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_alerts_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_alerts_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -14920,31 +19595,35 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_alerts_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cluster_operators_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cluster_operators_get  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cluster_operators_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cluster_operators_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -14998,32 +19677,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cluster_operators_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cpu_total_by_node_roles_os_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cpu_total_by_node_roles_os_get  # noqa: E501
 
         Retrieves the metrics.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cpu_total_by_node_roles_os_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cpu_total_by_node_roles_os_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15077,31 +19760,35 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_cpu_total_by_node_roles_os_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_nodes_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_nodes_get  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_nodes_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_nodes_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15155,32 +19842,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_nodes_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_socket_total_by_node_roles_os_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_socket_total_by_node_roles_os_get  # noqa: E501
 
         Retrieves the metrics.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_socket_total_by_node_roles_os_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_socket_total_by_node_roles_os_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15234,32 +19925,467 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_metric_queries_socket_total_by_node_roles_os_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get  # noqa: E501
+
+        Retrieves the list of node pools.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            page (int): Index of the requested page, where one corresponds to the first page.. [optional]
+            size (int): Number of items contained in the returned page.. [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ApiClustersMgmtV1ClustersClusterIdNodePoolsGet200Response
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_delete(
+        self,
+        cluster_id,
+        node_pool_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_delete  # noqa: E501
+
+        Deletes the node pool.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_delete(cluster_id, node_pool_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            node_pool_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['node_pool_id'] = \
+            node_pool_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_delete_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_get(
+        self,
+        cluster_id,
+        node_pool_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_get  # noqa: E501
+
+        Retrieves the details of the node pool.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_get(cluster_id, node_pool_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            node_pool_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            NodePool
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['node_pool_id'] = \
+            node_pool_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_get_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_patch(
+        self,
+        cluster_id,
+        node_pool_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_patch  # noqa: E501
+
+        Updates the node pool.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_patch(cluster_id, node_pool_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+            node_pool_id (str):
+
+        Keyword Args:
+            node_pool (NodePool): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            NodePool
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['node_pool_id'] = \
+            node_pool_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_node_pool_id_patch_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_clusters_cluster_id_node_pools_post(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_node_pools_post  # noqa: E501
+
+        Adds a new node pool to the cluster.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_post(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            node_pool (NodePool): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            NodePool
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_post_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_clusters_cluster_id_patch(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_patch  # noqa: E501
 
         Updates the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_patch(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             cluster (Cluster): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -15314,32 +20440,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_product_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_product_get  # noqa: E501
 
         Retrieves the details of the product.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_product_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_product_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15393,32 +20523,119 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_product_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_delete(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_delete  # noqa: E501
+
+        Delete the provision shard.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_delete(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_delete_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_get  # noqa: E501
 
         Retrieves the details of the provision shard.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15472,32 +20689,120 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_patch(
+        self,
+        cluster_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_patch  # noqa: E501
+
+        Updates the details of the provision shard.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_patch(cluster_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            cluster_id (str):
+
+        Keyword Args:
+            provision_shard (ProvisionShard): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ProvisionShard
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        return self.api_clusters_mgmt_v1_clusters_cluster_id_provision_shard_patch_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_clusters_cluster_id_resources_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_resources_get  # noqa: E501
 
         Retrieves a list of resources for a cluster in error state  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_resources_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_resources_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15551,32 +20856,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_resources_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_resources_live_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_resources_live_get  # noqa: E501
 
         Retrieves currently available cluster resources  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_resources_live_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_resources_live_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15630,32 +20939,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_resources_live_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_resume_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_resume_post  # noqa: E501
 
         Resumes from Hibernation.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_resume_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_resume_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15709,31 +21022,35 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_resume_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_status_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_status_get  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_status_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_status_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15787,32 +21104,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_status_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get  # noqa: E501
 
         Retrieves the list of operator roles.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items that will be contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -15868,33 +21189,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_operator_iam_role_id_delete(
         self,
+        cluster_id,
+        operator_iam_role_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_operator_iam_role_id_delete  # noqa: E501
 
         Deletes the operator role.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_operator_iam_role_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_operator_iam_role_id_delete(cluster_id, operator_iam_role_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            operator_iam_role_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            operator_iam_role_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -15948,32 +21274,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['operator_iam_role_id'] = \
+            operator_iam_role_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_operator_iam_role_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_post  # noqa: E501
 
         Adds a new operator role to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             operator_iam_role (OperatorIAMRole): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -16028,32 +21360,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get  # noqa: E501
 
         Retrieves the list of upgrade policies.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
             size (int): Number of items contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
@@ -16109,32 +21445,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_post(
         self,
+        cluster_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_post  # noqa: E501
 
         Adds a new upgrade policy to the cluster.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_post(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_post(cluster_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
             upgrade_policy (UpgradePolicy): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -16189,33 +21529,38 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_delete(
         self,
+        cluster_id,
+        upgrade_policy_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_delete  # noqa: E501
 
         Deletes the upgrade policy.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_delete(cluster_id, upgrade_policy_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            upgrade_policy_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            upgrade_policy_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -16269,33 +21614,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['upgrade_policy_id'] = \
+            upgrade_policy_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_get(
         self,
+        cluster_id,
+        upgrade_policy_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_get  # noqa: E501
 
         Retrieves the details of the upgrade policy.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_get(cluster_id, upgrade_policy_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            upgrade_policy_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            upgrade_policy_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -16349,33 +21701,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['upgrade_policy_id'] = \
+            upgrade_policy_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_patch(
         self,
+        cluster_id,
+        upgrade_policy_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_patch  # noqa: E501
 
         Update the upgrade policy.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_patch(cluster_id, upgrade_policy_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            upgrade_policy_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            upgrade_policy_id (str): [optional]
             upgrade_policy (UpgradePolicy): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -16430,33 +21789,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['upgrade_policy_id'] = \
+            upgrade_policy_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_get(
         self,
+        cluster_id,
+        upgrade_policy_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_get  # noqa: E501
 
         Retrieves the details of the upgrade policy state.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_get(cluster_id, upgrade_policy_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            upgrade_policy_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            upgrade_policy_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -16510,33 +21876,40 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['upgrade_policy_id'] = \
+            upgrade_policy_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_patch(
         self,
+        cluster_id,
+        upgrade_policy_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_patch  # noqa: E501
 
         Update the upgrade policy state.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_patch(cluster_id, upgrade_policy_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            cluster_id (str):
+            upgrade_policy_id (str):
 
         Keyword Args:
-            cluster_id (str): [optional]
-            upgrade_policy_id (str): [optional]
             upgrade_policy_state (UpgradePolicyState): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -16591,14 +21964,18 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['cluster_id'] = \
+            cluster_id
+        kwargs['upgrade_policy_id'] = \
+            upgrade_policy_id
         return self.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_upgrade_policy_id_state_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_clusters_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_clusters_get  # noqa: E501
@@ -16992,28 +22369,30 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_events_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_flavours_flavour_id_get(
         self,
+        flavour_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_flavours_flavour_id_get  # noqa: E501
 
         Retrieves the details of the cluster flavour.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_flavours_flavour_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_flavours_flavour_id_get(flavour_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            flavour_id (str):
 
         Keyword Args:
-            flavour_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -17067,32 +22446,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['flavour_id'] = \
+            flavour_id
         return self.api_clusters_mgmt_v1_flavours_flavour_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_flavours_flavour_id_patch(
         self,
+        flavour_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_flavours_flavour_id_patch  # noqa: E501
 
         Updates the flavour.  Attributes that can be updated are:  - `aws.infra_volume` - `aws.infra_instance_type` - `gcp.infra_instance_type`  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_flavours_flavour_id_patch(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_flavours_flavour_id_patch(flavour_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            flavour_id (str):
 
         Keyword Args:
-            flavour_id (str): [optional]
             flavour (Flavour): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -17147,14 +22530,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['flavour_id'] = \
+            flavour_id
         return self.api_clusters_mgmt_v1_flavours_flavour_id_patch_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_flavours_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_flavours_get  # noqa: E501
@@ -17793,28 +23178,30 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_limited_support_reason_templates_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_limited_support_reason_templates_limited_support_reason_template_id_get(
         self,
+        limited_support_reason_template_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_limited_support_reason_templates_limited_support_reason_template_id_get  # noqa: E501
 
         Retrieves the details of the template.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_limited_support_reason_templates_limited_support_reason_template_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_limited_support_reason_templates_limited_support_reason_template_id_get(limited_support_reason_template_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            limited_support_reason_template_id (str):
 
         Keyword Args:
-            limited_support_reason_template_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -17868,14 +23255,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['limited_support_reason_template_id'] = \
+            limited_support_reason_template_id
         return self.api_clusters_mgmt_v1_limited_support_reason_templates_limited_support_reason_template_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_machine_types_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_machine_types_get  # noqa: E501
@@ -17952,14 +23341,97 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_machine_types_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_machine_types_machine_type_id_get(
+        self,
+        machine_type_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_machine_types_machine_type_id_get  # noqa: E501
+
+        Retrieves the details of the machine type.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_machine_types_machine_type_id_get(machine_type_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            machine_type_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            MachineType
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['machine_type_id'] = \
+            machine_type_id
+        return self.api_clusters_mgmt_v1_machine_types_machine_type_id_get_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_products_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_products_get  # noqa: E501
 
         Retrieves the list of products.  # noqa: E501
@@ -18036,28 +23508,30 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_products_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_products_product_id_get(
         self,
+        product_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_products_product_id_get  # noqa: E501
 
         Retrieves the details of the product.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_products_product_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_products_product_id_get(product_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            product_id (str):
 
         Keyword Args:
-            product_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -18111,14 +23585,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['product_id'] = \
+            product_id
         return self.api_clusters_mgmt_v1_products_product_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_provision_shards_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_provision_shards_get  # noqa: E501
@@ -18128,14 +23604,15 @@
 
         >>> thread = api.api_clusters_mgmt_v1_provision_shards_get(async_req=True)
         >>> result = thread.get()
 
 
         Keyword Args:
             page (int): Index of the requested page, where one corresponds to the first page.. [optional]
+            search (str): Search criteria.  The syntax of this parameter is similar to the syntax of the _where_ clause of a SQL statement, but using the names of the attributes of the cluster instead of the names of the columns of a table. For example, in order to retrieve all the clusters with a name starting with `my` in the `us-east-1` region the value should be:  ```sql name like 'my%' and region.id = 'us-east-1' ```  If the parameter isn't provided, or if the value is empty, then all the provision shards that the user has permission to see will be returned.. [optional]
             size (int): Maximum number of items that will be contained in the returned page.. [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
@@ -18192,30 +23669,194 @@
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_provision_shards_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_provision_shards_post(
+        self,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_provision_shards_post  # noqa: E501
+
+        Adds a provision shard.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_provision_shards_post(async_req=True)
+        >>> result = thread.get()
+
+
+        Keyword Args:
+            provision_shard (ProvisionShard): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ProvisionShard
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        return self.api_clusters_mgmt_v1_provision_shards_post_endpoint.call_with_http_info(**kwargs)
+
+    def api_clusters_mgmt_v1_provision_shards_provision_shard_id_delete(
+        self,
+        provision_shard_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_provision_shards_provision_shard_id_delete  # noqa: E501
+
+        Delete the provision shard.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_provision_shards_provision_shard_id_delete(provision_shard_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            provision_shard_id (str):
+
+        Keyword Args:
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            None
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['provision_shard_id'] = \
+            provision_shard_id
+        return self.api_clusters_mgmt_v1_provision_shards_provision_shard_id_delete_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_provision_shards_provision_shard_id_get(
         self,
+        provision_shard_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_provision_shards_provision_shard_id_get  # noqa: E501
 
         Retrieves the details of the provision shard.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_provision_shards_provision_shard_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_provision_shards_provision_shard_id_get(provision_shard_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            provision_shard_id (str):
 
         Keyword Args:
-            provision_shard_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -18269,16 +23910,102 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['provision_shard_id'] = \
+            provision_shard_id
         return self.api_clusters_mgmt_v1_provision_shards_provision_shard_id_get_endpoint.call_with_http_info(**kwargs)
 
+    def api_clusters_mgmt_v1_provision_shards_provision_shard_id_patch(
+        self,
+        provision_shard_id,
+        **kwargs
+    ):
+        """api_clusters_mgmt_v1_provision_shards_provision_shard_id_patch  # noqa: E501
+
+        Updates the details of the provision shard.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.api_clusters_mgmt_v1_provision_shards_provision_shard_id_patch(provision_shard_id, async_req=True)
+        >>> result = thread.get()
+
+        Args:
+            provision_shard_id (str):
+
+        Keyword Args:
+            provision_shard (ProvisionShard): [optional]
+            _return_http_data_only (bool): response data without head status
+                code and headers. Default is True.
+            _preload_content (bool): if False, the urllib3.HTTPResponse object
+                will be returned without reading/decoding response data.
+                Default is True.
+            _request_timeout (int/float/tuple): timeout setting for this request. If
+                one number provided, it will be total request timeout. It can also
+                be a pair (tuple) of (connection, read) timeouts.
+                Default is None.
+            _check_input_type (bool): specifies if type checking
+                should be done one the data sent to the server.
+                Default is True.
+            _check_return_type (bool): specifies if type checking
+                should be done one the data received from the server.
+                Default is True.
+            _spec_property_naming (bool): True if the variable names in the input data
+                are serialized names, as specified in the OpenAPI document.
+                False if the variable names in the input data
+                are pythonic names, e.g. snake case (default)
+            _content_type (str/None): force body content-type.
+                Default is None and content-type will be predicted by allowed
+                content-types and body.
+            _host_index (int/None): specifies the index of the server
+                that we want to use.
+                Default is read from the configuration.
+            _request_auths (list): set to override the auth_settings for an a single
+                request; this effectively ignores the authentication
+                in the spec for a single request.
+                Default is None
+            async_req (bool): execute request asynchronously
+
+        Returns:
+            ProvisionShard
+                If the method is called asynchronously, returns the request
+                thread.
+        """
+        kwargs['async_req'] = kwargs.get(
+            'async_req', False
+        )
+        kwargs['_return_http_data_only'] = kwargs.get(
+            '_return_http_data_only', True
+        )
+        kwargs['_preload_content'] = kwargs.get(
+            '_preload_content', True
+        )
+        kwargs['_request_timeout'] = kwargs.get(
+            '_request_timeout', None
+        )
+        kwargs['_check_input_type'] = kwargs.get(
+            '_check_input_type', True
+        )
+        kwargs['_check_return_type'] = kwargs.get(
+            '_check_return_type', True
+        )
+        kwargs['_spec_property_naming'] = kwargs.get(
+            '_spec_property_naming', False
+        )
+        kwargs['_content_type'] = kwargs.get(
+            '_content_type')
+        kwargs['_host_index'] = kwargs.get('_host_index')
+        kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['provision_shard_id'] = \
+            provision_shard_id
+        return self.api_clusters_mgmt_v1_provision_shards_provision_shard_id_patch_endpoint.call_with_http_info(**kwargs)
+
     def api_clusters_mgmt_v1_version_gates_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_version_gates_get  # noqa: E501
 
         Retrieves a list of version gates.  # noqa: E501
@@ -18434,28 +24161,30 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_version_gates_post_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_version_gates_version_gate_id_delete(
         self,
+        version_gate_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_version_gates_version_gate_id_delete  # noqa: E501
 
         Deletes the version gate.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_version_gates_version_gate_id_delete(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_version_gates_version_gate_id_delete(version_gate_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            version_gate_id (str):
 
         Keyword Args:
-            version_gate_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -18509,32 +24238,36 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['version_gate_id'] = \
+            version_gate_id
         return self.api_clusters_mgmt_v1_version_gates_version_gate_id_delete_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_version_gates_version_gate_id_get(
         self,
+        version_gate_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_version_gates_version_gate_id_get  # noqa: E501
 
         Retrieves the details of the version gate.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_version_gates_version_gate_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_version_gates_version_gate_id_get(version_gate_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            version_gate_id (str):
 
         Keyword Args:
-            version_gate_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -18588,14 +24321,16 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['version_gate_id'] = \
+            version_gate_id
         return self.api_clusters_mgmt_v1_version_gates_version_gate_id_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_versions_get(
         self,
         **kwargs
     ):
         """api_clusters_mgmt_v1_versions_get  # noqa: E501
@@ -18674,28 +24409,30 @@
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
         return self.api_clusters_mgmt_v1_versions_get_endpoint.call_with_http_info(**kwargs)
 
     def api_clusters_mgmt_v1_versions_version_id_get(
         self,
+        version_id,
         **kwargs
     ):
         """api_clusters_mgmt_v1_versions_version_id_get  # noqa: E501
 
         Retrieves the details of the version.  # noqa: E501
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.api_clusters_mgmt_v1_versions_version_id_get(async_req=True)
+        >>> thread = api.api_clusters_mgmt_v1_versions_version_id_get(version_id, async_req=True)
         >>> result = thread.get()
 
+        Args:
+            version_id (str):
 
         Keyword Args:
-            version_id (str): [optional]
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
@@ -18749,9 +24486,11 @@
         kwargs['_spec_property_naming'] = kwargs.get(
             '_spec_property_naming', False
         )
         kwargs['_content_type'] = kwargs.get(
             '_content_type')
         kwargs['_host_index'] = kwargs.get('_host_index')
         kwargs['_request_auths'] = kwargs.get('_request_auths', None)
+        kwargs['version_id'] = \
+            version_id
         return self.api_clusters_mgmt_v1_versions_version_id_get_endpoint.call_with_http_info(**kwargs)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/api_client.py` & `ocm_python_client-1.0.6/ocm_python_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/1.0.1/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/configuration.py` & `ocm_python_client-1.0.6/ocm_python_client/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 1.0.0".\
+               "SDK Package Version: 1.0.1".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/exceptions.py` & `ocm_python_client-1.0.6/ocm_python_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,21 +29,23 @@
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ocm_python_client.model.add_on_config import AddOnConfig
     from ocm_python_client.model.add_on_install_mode import AddOnInstallMode
+    from ocm_python_client.model.add_on_namespace import AddOnNamespace
     from ocm_python_client.model.add_on_parameter import AddOnParameter
     from ocm_python_client.model.add_on_requirement import AddOnRequirement
     from ocm_python_client.model.add_on_sub_operator import AddOnSubOperator
     from ocm_python_client.model.add_on_version import AddOnVersion
     from ocm_python_client.model.credential_request import CredentialRequest
     globals()['AddOnConfig'] = AddOnConfig
     globals()['AddOnInstallMode'] = AddOnInstallMode
+    globals()['AddOnNamespace'] = AddOnNamespace
     globals()['AddOnParameter'] = AddOnParameter
     globals()['AddOnRequirement'] = AddOnRequirement
     globals()['AddOnSubOperator'] = AddOnSubOperator
     globals()['AddOnVersion'] = AddOnVersion
     globals()['CredentialRequest'] = CredentialRequest
 
 
@@ -99,26 +101,29 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
+            'common_annotations': ({str: (str,)},),  # noqa: E501
+            'common_labels': ({str: (str,)},),  # noqa: E501
             'config': (AddOnConfig,),  # noqa: E501
             'credentials_requests': ([CredentialRequest],),  # noqa: E501
             'description': (str,),  # noqa: E501
             'docs_link': (str,),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
             'has_external_resources': (bool,),  # noqa: E501
             'hidden': (bool,),  # noqa: E501
             'icon': (str,),  # noqa: E501
             'install_mode': (AddOnInstallMode,),  # noqa: E501
             'label': (str,),  # noqa: E501
             'managed_service': (bool,),  # noqa: E501
             'name': (str,),  # noqa: E501
+            'namespaces': ([AddOnNamespace],),  # noqa: E501
             'operator_name': (str,),  # noqa: E501
             'parameters': ([AddOnParameter],),  # noqa: E501
             'requirements': ([AddOnRequirement],),  # noqa: E501
             'resource_cost': (float,),  # noqa: E501
             'resource_name': (str,),  # noqa: E501
             'sub_operators': ([AddOnSubOperator],),  # noqa: E501
             'target_namespace': (str,),  # noqa: E501
@@ -130,26 +135,29 @@
         return None
 
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
+        'common_annotations': 'common_annotations',  # noqa: E501
+        'common_labels': 'common_labels',  # noqa: E501
         'config': 'config',  # noqa: E501
         'credentials_requests': 'credentials_requests',  # noqa: E501
         'description': 'description',  # noqa: E501
         'docs_link': 'docs_link',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
         'has_external_resources': 'has_external_resources',  # noqa: E501
         'hidden': 'hidden',  # noqa: E501
         'icon': 'icon',  # noqa: E501
         'install_mode': 'install_mode',  # noqa: E501
         'label': 'label',  # noqa: E501
         'managed_service': 'managed_service',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'namespaces': 'namespaces',  # noqa: E501
         'operator_name': 'operator_name',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'requirements': 'requirements',  # noqa: E501
         'resource_cost': 'resource_cost',  # noqa: E501
         'resource_name': 'resource_name',  # noqa: E501
         'sub_operators': 'sub_operators',  # noqa: E501
         'target_namespace': 'target_namespace',  # noqa: E501
@@ -196,26 +204,29 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOn' if this is a complete object or 'AddOnLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
+            common_annotations ({str: (str,)}): Common annotations to be applied to all resources created by this addon.. [optional]  # noqa: E501
+            common_labels ({str: (str,)}): Common labels to be applied to all resources created by this addon.. [optional]  # noqa: E501
             config (AddOnConfig): [optional]  # noqa: E501
             credentials_requests ([CredentialRequest]): List of credentials requests to authenticate operators to access cloud resources.. [optional]  # noqa: E501
             description (str): Description of the add-on.. [optional]  # noqa: E501
             docs_link (str): Link to documentation about the add-on.. [optional]  # noqa: E501
             enabled (bool): Indicates if this add-on can be added to clusters.. [optional]  # noqa: E501
             has_external_resources (bool): Indicates if this add-on has external resources associated with it. [optional]  # noqa: E501
             hidden (bool): Indicates if this add-on is hidden.. [optional]  # noqa: E501
             icon (str): Base64-encoded icon representing an add-on. The icon should be in PNG format.. [optional]  # noqa: E501
             install_mode (AddOnInstallMode): [optional]  # noqa: E501
             label (str): Label used to attach to a cluster deployment when add-on is installed.. [optional]  # noqa: E501
             managed_service (bool): Indicates if add-on is part of a managed service. [optional]  # noqa: E501
             name (str): Name of the add-on.. [optional]  # noqa: E501
+            namespaces ([AddOnNamespace]): Namespaces which are required by this addon.. [optional]  # noqa: E501
             operator_name (str): The name of the operator installed by this add-on.. [optional]  # noqa: E501
             parameters ([AddOnParameter]): List of parameters for this add-on.. [optional]  # noqa: E501
             requirements ([AddOnRequirement]): List of requirements for this add-on.. [optional]  # noqa: E501
             resource_cost (float): Used to determine how many units of quota an add-on consumes per resource name.. [optional]  # noqa: E501
             resource_name (str): Used to determine from where to reserve quota for this add-on.. [optional]  # noqa: E501
             sub_operators ([AddOnSubOperator]): List of sub operators for this add-on.. [optional]  # noqa: E501
             target_namespace (str): The namespace in which the addon CRD exists.. [optional]  # noqa: E501
@@ -304,26 +315,29 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOn' if this is a complete object or 'AddOnLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
+            common_annotations ({str: (str,)}): Common annotations to be applied to all resources created by this addon.. [optional]  # noqa: E501
+            common_labels ({str: (str,)}): Common labels to be applied to all resources created by this addon.. [optional]  # noqa: E501
             config (AddOnConfig): [optional]  # noqa: E501
             credentials_requests ([CredentialRequest]): List of credentials requests to authenticate operators to access cloud resources.. [optional]  # noqa: E501
             description (str): Description of the add-on.. [optional]  # noqa: E501
             docs_link (str): Link to documentation about the add-on.. [optional]  # noqa: E501
             enabled (bool): Indicates if this add-on can be added to clusters.. [optional]  # noqa: E501
             has_external_resources (bool): Indicates if this add-on has external resources associated with it. [optional]  # noqa: E501
             hidden (bool): Indicates if this add-on is hidden.. [optional]  # noqa: E501
             icon (str): Base64-encoded icon representing an add-on. The icon should be in PNG format.. [optional]  # noqa: E501
             install_mode (AddOnInstallMode): [optional]  # noqa: E501
             label (str): Label used to attach to a cluster deployment when add-on is installed.. [optional]  # noqa: E501
             managed_service (bool): Indicates if add-on is part of a managed service. [optional]  # noqa: E501
             name (str): Name of the add-on.. [optional]  # noqa: E501
+            namespaces ([AddOnNamespace]): Namespaces which are required by this addon.. [optional]  # noqa: E501
             operator_name (str): The name of the operator installed by this add-on.. [optional]  # noqa: E501
             parameters ([AddOnParameter]): List of parameters for this add-on.. [optional]  # noqa: E501
             requirements ([AddOnRequirement]): List of requirements for this add-on.. [optional]  # noqa: E501
             resource_cost (float): Used to determine how many units of quota an add-on consumes per resource name.. [optional]  # noqa: E501
             resource_name (str): Used to determine from where to reserve quota for this add-on.. [optional]  # noqa: E501
             sub_operators ([AddOnSubOperator]): List of sub operators for this add-on.. [optional]  # noqa: E501
             target_namespace (str): The namespace in which the addon CRD exists.. [optional]  # noqa: E501
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_config.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ocm_python_client.model.add_on_environment_variable import AddOnEnvironmentVariable
+    from ocm_python_client.model.add_on_secret_propagation import AddOnSecretPropagation
     globals()['AddOnEnvironmentVariable'] = AddOnEnvironmentVariable
+    globals()['AddOnSecretPropagation'] = AddOnSecretPropagation
 
 
 class AddOnConfig(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -88,26 +90,28 @@
         """
         lazy_import()
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
             'add_on_environment_variables': ([AddOnEnvironmentVariable],),  # noqa: E501
+            'secret_propagations': ([AddOnSecretPropagation],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
         'add_on_environment_variables': 'add_on_environment_variables',  # noqa: E501
+        'secret_propagations': 'secret_propagations',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -147,14 +151,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOnConfig' if this is a complete object or 'AddOnConfigLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             add_on_environment_variables ([AddOnEnvironmentVariable]): List of environment variables for the addon. [optional]  # noqa: E501
+            secret_propagations ([AddOnSecretPropagation]): List of secret propagations for the addon. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -236,14 +241,15 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOnConfig' if this is a complete object or 'AddOnConfigLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             add_on_environment_variables ([AddOnEnvironmentVariable]): List of environment variables for the addon. [optional]  # noqa: E501
+            secret_propagations ([AddOnSecretPropagation]): List of secret propagations for the addon. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_environment_variable.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_environment_variable.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_install_mode.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_install_mode.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_installation.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_installation.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,19 +28,21 @@
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ocm_python_client.model.add_on import AddOn
+    from ocm_python_client.model.add_on_installation_billing import AddOnInstallationBilling
     from ocm_python_client.model.add_on_installation_parameter import AddOnInstallationParameter
     from ocm_python_client.model.add_on_installation_state import AddOnInstallationState
     from ocm_python_client.model.add_on_version import AddOnVersion
     from ocm_python_client.model.cluster import Cluster
     globals()['AddOn'] = AddOn
+    globals()['AddOnInstallationBilling'] = AddOnInstallationBilling
     globals()['AddOnInstallationParameter'] = AddOnInstallationParameter
     globals()['AddOnInstallationState'] = AddOnInstallationState
     globals()['AddOnVersion'] = AddOnVersion
     globals()['Cluster'] = Cluster
 
 
 class AddOnInstallation(ModelNormal):
@@ -97,14 +99,15 @@
         lazy_import()
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
             'addon': (AddOn,),  # noqa: E501
             'addon_version': (AddOnVersion,),  # noqa: E501
+            'billing': (AddOnInstallationBilling,),  # noqa: E501
             'cluster': (Cluster,),  # noqa: E501
             'creation_timestamp': (datetime,),  # noqa: E501
             'operator_version': (str,),  # noqa: E501
             'parameters': ([AddOnInstallationParameter],),  # noqa: E501
             'state': (AddOnInstallationState,),  # noqa: E501
             'state_description': (str,),  # noqa: E501
             'updated_timestamp': (datetime,),  # noqa: E501
@@ -117,14 +120,15 @@
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
         'addon': 'addon',  # noqa: E501
         'addon_version': 'addon_version',  # noqa: E501
+        'billing': 'billing',  # noqa: E501
         'cluster': 'cluster',  # noqa: E501
         'creation_timestamp': 'creation_timestamp',  # noqa: E501
         'operator_version': 'operator_version',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
         'state': 'state',  # noqa: E501
         'state_description': 'state_description',  # noqa: E501
         'updated_timestamp': 'updated_timestamp',  # noqa: E501
@@ -172,14 +176,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOnInstallation' if this is a complete object or 'AddOnInstallationLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             addon (AddOn): [optional]  # noqa: E501
             addon_version (AddOnVersion): [optional]  # noqa: E501
+            billing (AddOnInstallationBilling): [optional]  # noqa: E501
             cluster (Cluster): [optional]  # noqa: E501
             creation_timestamp (datetime): Date and time when the add-on was initially installed in the cluster.. [optional]  # noqa: E501
             operator_version (str): Version of the operator installed by the add-on.. [optional]  # noqa: E501
             parameters ([AddOnInstallationParameter]): List of add-on parameters for this add-on installation.. [optional]  # noqa: E501
             state (AddOnInstallationState): [optional]  # noqa: E501
             state_description (str): Reason for the current State.. [optional]  # noqa: E501
             updated_timestamp (datetime): Date and time when the add-on installation information was last updated.. [optional]  # noqa: E501
@@ -269,14 +274,15 @@
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOnInstallation' if this is a complete object or 'AddOnInstallationLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             addon (AddOn): [optional]  # noqa: E501
             addon_version (AddOnVersion): [optional]  # noqa: E501
+            billing (AddOnInstallationBilling): [optional]  # noqa: E501
             cluster (Cluster): [optional]  # noqa: E501
             creation_timestamp (datetime): Date and time when the add-on was initially installed in the cluster.. [optional]  # noqa: E501
             operator_version (str): Version of the operator installed by the add-on.. [optional]  # noqa: E501
             parameters ([AddOnInstallationParameter]): List of add-on parameters for this add-on installation.. [optional]  # noqa: E501
             state (AddOnInstallationState): [optional]  # noqa: E501
             state_description (str): Reason for the current State.. [optional]  # noqa: E501
             updated_timestamp (datetime): Date and time when the add-on installation information was last updated.. [optional]  # noqa: E501
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_installation_parameter.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_installation_parameter.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_installation_state.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_installation_state.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_parameter.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ocm_python_client.model.add_on import AddOn
     from ocm_python_client.model.add_on_parameter_option import AddOnParameterOption
+    from ocm_python_client.model.add_on_requirement import AddOnRequirement
     globals()['AddOn'] = AddOn
     globals()['AddOnParameterOption'] = AddOnParameterOption
+    globals()['AddOnRequirement'] = AddOnRequirement
 
 
 class AddOnParameter(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -90,17 +92,19 @@
         """
         lazy_import()
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
             'addon': (AddOn,),  # noqa: E501
+            'conditions': ([AddOnRequirement],),  # noqa: E501
             'default_value': (str,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'editable': (bool,),  # noqa: E501
+            'editable_direction': (str,),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'options': ([AddOnParameterOption],),  # noqa: E501
             'required': (bool,),  # noqa: E501
             'validation': (str,),  # noqa: E501
             'validation_err_msg': (str,),  # noqa: E501
             'value_type': (str,),  # noqa: E501
@@ -112,17 +116,19 @@
 
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
         'addon': 'addon',  # noqa: E501
+        'conditions': 'conditions',  # noqa: E501
         'default_value': 'default_value',  # noqa: E501
         'description': 'description',  # noqa: E501
         'editable': 'editable',  # noqa: E501
+        'editable_direction': 'editable_direction',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
         'name': 'name',  # noqa: E501
         'options': 'options',  # noqa: E501
         'required': 'required',  # noqa: E501
         'validation': 'validation',  # noqa: E501
         'validation_err_msg': 'validation_err_msg',  # noqa: E501
         'value_type': 'value_type',  # noqa: E501
@@ -169,17 +175,19 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOnParameter' if this is a complete object or 'AddOnParameterLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             addon (AddOn): [optional]  # noqa: E501
+            conditions ([AddOnRequirement]): Conditions in which this parameter is valid for. [optional]  # noqa: E501
             default_value (str): Indicates the value default for the add-on parameter.. [optional]  # noqa: E501
             description (str): Description of the add-on parameter.. [optional]  # noqa: E501
             editable (bool): Indicates if this parameter can be edited after creation.. [optional]  # noqa: E501
+            editable_direction (str): Restricts if the parameter can be upscaled/downscaled Expected values are \"up\", \"down\", or \"\" (no restriction).. [optional]  # noqa: E501
             enabled (bool): Indicates if this parameter is enabled for the add-on.. [optional]  # noqa: E501
             name (str): Name of the add-on parameter.. [optional]  # noqa: E501
             options ([AddOnParameterOption]): List of options for the add-on parameter value.. [optional]  # noqa: E501
             required (bool): Indicates if this parameter is required by the add-on.. [optional]  # noqa: E501
             validation (str): Validation rule for the add-on parameter.. [optional]  # noqa: E501
             validation_err_msg (str): Error message to return should the parameter be invalid.. [optional]  # noqa: E501
             value_type (str): Type of value of the add-on parameter.. [optional]  # noqa: E501
@@ -268,17 +276,19 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOnParameter' if this is a complete object or 'AddOnParameterLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             addon (AddOn): [optional]  # noqa: E501
+            conditions ([AddOnRequirement]): Conditions in which this parameter is valid for. [optional]  # noqa: E501
             default_value (str): Indicates the value default for the add-on parameter.. [optional]  # noqa: E501
             description (str): Description of the add-on parameter.. [optional]  # noqa: E501
             editable (bool): Indicates if this parameter can be edited after creation.. [optional]  # noqa: E501
+            editable_direction (str): Restricts if the parameter can be upscaled/downscaled Expected values are \"up\", \"down\", or \"\" (no restriction).. [optional]  # noqa: E501
             enabled (bool): Indicates if this parameter is enabled for the add-on.. [optional]  # noqa: E501
             name (str): Name of the add-on parameter.. [optional]  # noqa: E501
             options ([AddOnParameterOption]): List of options for the add-on parameter value.. [optional]  # noqa: E501
             required (bool): Indicates if this parameter is required by the add-on.. [optional]  # noqa: E501
             validation (str): Validation rule for the add-on parameter.. [optional]  # noqa: E501
             validation_err_msg (str): Error message to return should the parameter be invalid.. [optional]  # noqa: E501
             value_type (str): Type of value of the add-on parameter.. [optional]  # noqa: E501
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_parameter_option.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_parameter_option.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,25 +85,27 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'name': (str,),  # noqa: E501
+            'rank': (int,),  # noqa: E501
             'requirements': ([AddOnRequirement],),  # noqa: E501
             'value': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'name': 'name',  # noqa: E501
+        'rank': 'rank',  # noqa: E501
         'requirements': 'requirements',  # noqa: E501
         'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
@@ -142,14 +144,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): Name of the add-on parameter option.. [optional]  # noqa: E501
+            rank (int): Rank of option to be used in cases where editable direction should be restricted.. [optional]  # noqa: E501
             requirements ([AddOnRequirement]): List of add-on requirements for this parameter option.. [optional]  # noqa: E501
             value (str): Value of the add-on parameter option.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -230,14 +233,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             name (str): Name of the add-on parameter option.. [optional]  # noqa: E501
+            rank (int): Rank of option to be used in cases where editable direction should be restricted.. [optional]  # noqa: E501
             requirements ([AddOnRequirement]): List of add-on requirements for this parameter option.. [optional]  # noqa: E501
             value (str): Value of the add-on parameter option.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_requirement.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_requirement.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_requirement_status.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_requirement_status.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_sub_operator.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_sub_operator.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/add_on_version.py` & `ocm_python_client-1.0.6/ocm_python_client/model/add_on_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,18 +31,20 @@
 
 
 def lazy_import():
     from ocm_python_client.model.add_on_config import AddOnConfig
     from ocm_python_client.model.add_on_parameter import AddOnParameter
     from ocm_python_client.model.add_on_requirement import AddOnRequirement
     from ocm_python_client.model.add_on_sub_operator import AddOnSubOperator
+    from ocm_python_client.model.additional_catalog_source import AdditionalCatalogSource
     globals()['AddOnConfig'] = AddOnConfig
     globals()['AddOnParameter'] = AddOnParameter
     globals()['AddOnRequirement'] = AddOnRequirement
     globals()['AddOnSubOperator'] = AddOnSubOperator
+    globals()['AdditionalCatalogSource'] = AdditionalCatalogSource
 
 
 class AddOnVersion(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -93,38 +95,42 @@
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
+            'additional_catalog_sources': ([AdditionalCatalogSource],),  # noqa: E501
             'available_upgrades': ([str],),  # noqa: E501
             'channel': (str,),  # noqa: E501
             'config': (AddOnConfig,),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
             'parameters': ([AddOnParameter],),  # noqa: E501
+            'pull_secret_name': (str,),  # noqa: E501
             'requirements': ([AddOnRequirement],),  # noqa: E501
             'source_image': (str,),  # noqa: E501
             'sub_operators': ([AddOnSubOperator],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
+        'additional_catalog_sources': 'additional_catalog_sources',  # noqa: E501
         'available_upgrades': 'available_upgrades',  # noqa: E501
         'channel': 'channel',  # noqa: E501
         'config': 'config',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
         'parameters': 'parameters',  # noqa: E501
+        'pull_secret_name': 'pull_secret_name',  # noqa: E501
         'requirements': 'requirements',  # noqa: E501
         'source_image': 'source_image',  # noqa: E501
         'sub_operators': 'sub_operators',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -166,19 +172,21 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOnVersion' if this is a complete object or 'AddOnVersionLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
+            additional_catalog_sources ([AdditionalCatalogSource]): Additional catalog sources associated with this addon version. [optional]  # noqa: E501
             available_upgrades ([str]): AvailableUpgrades is the list of versions this version can be upgraded to.. [optional]  # noqa: E501
             channel (str): The specific addon catalog source channel of packages. [optional]  # noqa: E501
             config (AddOnConfig): [optional]  # noqa: E501
             enabled (bool): Indicates if this add-on version can be added to clusters.. [optional]  # noqa: E501
             parameters ([AddOnParameter]): List of parameters for this add-on version.. [optional]  # noqa: E501
+            pull_secret_name (str): The pull secret name used for this addon version.. [optional]  # noqa: E501
             requirements ([AddOnRequirement]): List of requirements for this add-on version.. [optional]  # noqa: E501
             source_image (str): The catalog source image for this add-on version.. [optional]  # noqa: E501
             sub_operators ([AddOnSubOperator]): List of sub operators for this add-on version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -262,19 +270,21 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'AddOnVersion' if this is a complete object or 'AddOnVersionLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
+            additional_catalog_sources ([AdditionalCatalogSource]): Additional catalog sources associated with this addon version. [optional]  # noqa: E501
             available_upgrades ([str]): AvailableUpgrades is the list of versions this version can be upgraded to.. [optional]  # noqa: E501
             channel (str): The specific addon catalog source channel of packages. [optional]  # noqa: E501
             config (AddOnConfig): [optional]  # noqa: E501
             enabled (bool): Indicates if this add-on version can be added to clusters.. [optional]  # noqa: E501
             parameters ([AddOnParameter]): List of parameters for this add-on version.. [optional]  # noqa: E501
+            pull_secret_name (str): The pull secret name used for this addon version.. [optional]  # noqa: E501
             requirements ([AddOnRequirement]): List of requirements for this add-on version.. [optional]  # noqa: E501
             source_image (str): The catalog source image for this add-on version.. [optional]  # noqa: E501
             sub_operators ([AddOnSubOperator]): List of sub operators for this add-on version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/admin_credentials.py` & `ocm_python_client-1.0.6/ocm_python_client/model/admin_credentials.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/alert_info.py` & `ocm_python_client-1.0.6/ocm_python_client/model/alert_info.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/alert_severity.py` & `ocm_python_client-1.0.6/ocm_python_client/model/alert_severity.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/alerts_info.py` & `ocm_python_client-1.0.6/ocm_python_client/model/alerts_info.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_addons_addon_id_versions_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_addons_addon_id_versions_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_addons_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_addons_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_infrastructure_access_roles_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_infrastructure_access_roles_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_machine_types_post200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_machine_types_post200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_regions_post200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_regions_post200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_credential_requests_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_credential_requests_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_policies_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_policies_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_vpcs_post200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_vpcs_post200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addons_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addons_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_logs_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_logs_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_clusters_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_clusters_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_flavours_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_flavours_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_encryption_keys_post200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_encryption_keys_post200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_key_rings_post200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_key_rings_post200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_limited_support_reason_templates_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_limited_support_reason_templates_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_machine_types_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_machine_types_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_products_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_products_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_provision_shards_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_provision_shards_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_version_gates_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_version_gates_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/api_clusters_mgmt_v1_versions_get200_response.py` & `ocm_python_client-1.0.6/ocm_python_client/model/api_clusters_mgmt_v1_versions_get200_response.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,19 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
+    from ocm_python_client.model.aws_etcd_encryption import AwsEtcdEncryption
+    from ocm_python_client.model.private_link_cluster_configuration import PrivateLinkClusterConfiguration
     from ocm_python_client.model.sts import STS
+    globals()['AwsEtcdEncryption'] = AwsEtcdEncryption
+    globals()['PrivateLinkClusterConfiguration'] = PrivateLinkClusterConfiguration
     globals()['STS'] = STS
 
 
 class AWS(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -88,15 +92,17 @@
         """
         lazy_import()
         return {
             'kms_key_arn': (str,),  # noqa: E501
             'sts': (STS,),  # noqa: E501
             'access_key_id': (str,),  # noqa: E501
             'account_id': (str,),  # noqa: E501
+            'etcd_encryption': (AwsEtcdEncryption,),  # noqa: E501
             'private_link': (bool,),  # noqa: E501
+            'private_link_configuration': (PrivateLinkClusterConfiguration,),  # noqa: E501
             'secret_access_key': (str,),  # noqa: E501
             'subnet_ids': ([str],),  # noqa: E501
             'tags': ({str: (str,)},),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
@@ -104,15 +110,17 @@
 
 
     attribute_map = {
         'kms_key_arn': 'kms_key_arn',  # noqa: E501
         'sts': 'sts',  # noqa: E501
         'access_key_id': 'access_key_id',  # noqa: E501
         'account_id': 'account_id',  # noqa: E501
+        'etcd_encryption': 'etcd_encryption',  # noqa: E501
         'private_link': 'private_link',  # noqa: E501
+        'private_link_configuration': 'private_link_configuration',  # noqa: E501
         'secret_access_key': 'secret_access_key',  # noqa: E501
         'subnet_ids': 'subnet_ids',  # noqa: E501
         'tags': 'tags',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -155,15 +163,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kms_key_arn (str): Customer Managed Key to encrypt EBS Volume. [optional]  # noqa: E501
             sts (STS): [optional]  # noqa: E501
             access_key_id (str): AWS access key identifier.. [optional]  # noqa: E501
             account_id (str): AWS account identifier.. [optional]  # noqa: E501
+            etcd_encryption (AwsEtcdEncryption): [optional]  # noqa: E501
             private_link (bool): Sets cluster to be inaccessible externally.. [optional]  # noqa: E501
+            private_link_configuration (PrivateLinkClusterConfiguration): [optional]  # noqa: E501
             secret_access_key (str): AWS secret access key.. [optional]  # noqa: E501
             subnet_ids ([str]): The subnet ids to be used when installing the cluster.. [optional]  # noqa: E501
             tags ({str: (str,)}): Optional keys and values that the installer will add as tags to all AWS resources it creates. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
@@ -248,15 +258,17 @@
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kms_key_arn (str): Customer Managed Key to encrypt EBS Volume. [optional]  # noqa: E501
             sts (STS): [optional]  # noqa: E501
             access_key_id (str): AWS access key identifier.. [optional]  # noqa: E501
             account_id (str): AWS account identifier.. [optional]  # noqa: E501
+            etcd_encryption (AwsEtcdEncryption): [optional]  # noqa: E501
             private_link (bool): Sets cluster to be inaccessible externally.. [optional]  # noqa: E501
+            private_link_configuration (PrivateLinkClusterConfiguration): [optional]  # noqa: E501
             secret_access_key (str): AWS secret access key.. [optional]  # noqa: E501
             subnet_ids ([str]): The subnet ids to be used when installing the cluster.. [optional]  # noqa: E501
             tags ({str: (str,)}): Optional keys and values that the installer will add as tags to all AWS resources it creates. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws_flavour.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws_flavour.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws_infrastructure_access_role.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws_infrastructure_access_role.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws_infrastructure_access_role_grant.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws_infrastructure_access_role_grant.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws_infrastructure_access_role_grant_state.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws_infrastructure_access_role_grant_state.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws_infrastructure_access_role_state.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws_infrastructure_access_role_state.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws_machine_pool.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws_machine_pool.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws_spot_market_options.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws_spot_market_options.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/aws_volume.py` & `ocm_python_client-1.0.6/ocm_python_client/model/aws_volume.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/awssts_policy.py` & `ocm_python_client-1.0.6/ocm_python_client/model/subscription.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class AWSSTSPolicy(ModelNormal):
+class Subscription(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,39 +78,39 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'details': (str,),  # noqa: E501
-            'type': (str,),  # noqa: E501
+            'href': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'details': 'details',  # noqa: E501
-        'type': 'type',  # noqa: E501
+        'href': 'href',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """AWSSTSPolicy - a model defined in OpenAPI
+        """Subscription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +135,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Policy ID. [optional]  # noqa: E501
-            details (str): Policy Details. [optional]  # noqa: E501
-            type (str): Type of policy operator/account role. [optional]  # noqa: E501
+            kind (str): Indicates the type of this object. Will be 'Subscription' if this is a complete object or 'SubscriptionLink' if it is just a link.. [optional]  # noqa: E501
+            id (str): Unique identifier of the object.. [optional]  # noqa: E501
+            href (str): Self link.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +190,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """AWSSTSPolicy - a model defined in OpenAPI
+        """Subscription - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,17 +223,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            id (str): Policy ID. [optional]  # noqa: E501
-            details (str): Policy Details. [optional]  # noqa: E501
-            type (str): Type of policy operator/account role. [optional]  # noqa: E501
+            kind (str): Indicates the type of this object. Will be 'Subscription' if this is a complete object or 'SubscriptionLink' if it is just a link.. [optional]  # noqa: E501
+            id (str): Unique identifier of the object.. [optional]  # noqa: E501
+            href (str): Self link.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/billing_model.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_configuration_mode.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class BillingModel(ModelSimple):
+class ClusterConfigurationMode(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,16 +49,16 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'MARKETPLACE': "marketplace",
-            'STANDARD': "standard",
+            'FULL': "full",
+            'READ_ONLY': "read_only",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -97,23 +97,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """BillingModel - a model defined in OpenAPI
+        """ClusterConfigurationMode - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Billing model for cluster resources.., must be one of ["marketplace", "standard", ]  # noqa: E501
+            args[0] (str): Configuration mode of a cluster.., must be one of ["full", "read_only", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Billing model for cluster resources.., must be one of ["marketplace", "standard", ]  # noqa: E501
+            value (str): Configuration mode of a cluster.., must be one of ["full", "read_only", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -191,23 +191,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """BillingModel - a model defined in OpenAPI
+        """ClusterConfigurationMode - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Billing model for cluster resources.., must be one of ["marketplace", "standard", ]  # noqa: E501
+            args[0] (str): Configuration mode of a cluster.., must be one of ["full", "read_only", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Billing model for cluster resources.., must be one of ["marketplace", "standard", ]  # noqa: E501
+            value (str): Configuration mode of a cluster.., must be one of ["full", "read_only", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/ccs.py` & `ocm_python_client-1.0.6/ocm_python_client/model/ccs.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cloud_provider.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cloud_provider.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cloud_provider_data.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cloud_provider_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,17 +30,19 @@
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ocm_python_client.model.aws import AWS
     from ocm_python_client.model.cloud_region import CloudRegion
     from ocm_python_client.model.gcp import GCP
+    from ocm_python_client.model.version import Version
     globals()['AWS'] = AWS
     globals()['CloudRegion'] = CloudRegion
     globals()['GCP'] = GCP
+    globals()['Version'] = Version
 
 
 class CloudProviderData(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -90,30 +92,34 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'aws': (AWS,),  # noqa: E501
             'gcp': (GCP,),  # noqa: E501
+            'availability_zones': ([str],),  # noqa: E501
             'key_location': (str,),  # noqa: E501
             'key_ring_name': (str,),  # noqa: E501
             'region': (CloudRegion,),  # noqa: E501
+            'version': (Version,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'aws': 'aws',  # noqa: E501
         'gcp': 'gcp',  # noqa: E501
+        'availability_zones': 'availability_zones',  # noqa: E501
         'key_location': 'key_location',  # noqa: E501
         'key_ring_name': 'key_ring_name',  # noqa: E501
         'region': 'region',  # noqa: E501
+        'version': 'version',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
@@ -151,17 +157,19 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             aws (AWS): [optional]  # noqa: E501
             gcp (GCP): [optional]  # noqa: E501
+            availability_zones ([str]): Availability zone. [optional]  # noqa: E501
             key_location (str): Key location. [optional]  # noqa: E501
             key_ring_name (str): Key ring name. [optional]  # noqa: E501
             region (CloudRegion): [optional]  # noqa: E501
+            version (Version): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -241,17 +249,19 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             aws (AWS): [optional]  # noqa: E501
             gcp (GCP): [optional]  # noqa: E501
+            availability_zones ([str]): Availability zone. [optional]  # noqa: E501
             key_location (str): Key location. [optional]  # noqa: E501
             key_ring_name (str): Key ring name. [optional]  # noqa: E501
             region (CloudRegion): [optional]  # noqa: E501
+            version (Version): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cloud_region.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cloud_region.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,14 +92,15 @@
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
             'ccs_only': (bool,),  # noqa: E501
             'cloud_provider': (CloudProvider,),  # noqa: E501
             'display_name': (str,),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
             'name': (str,),  # noqa: E501
+            'supports_hypershift': (bool,),  # noqa: E501
             'supports_multi_az': (bool,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -109,14 +110,15 @@
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
         'ccs_only': 'ccs_only',  # noqa: E501
         'cloud_provider': 'cloud_provider',  # noqa: E501
         'display_name': 'display_name',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'supports_hypershift': 'supports_hypershift',  # noqa: E501
         'supports_multi_az': 'supports_multi_az',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -161,14 +163,15 @@
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             ccs_only (bool): 'true' if the region is supported only for CCS clusters, 'false' otherwise.. [optional]  # noqa: E501
             cloud_provider (CloudProvider): [optional]  # noqa: E501
             display_name (str): Name of the region for display purposes, for example `N. Virginia`.. [optional]  # noqa: E501
             enabled (bool): Whether the region is enabled for deploying an OSD cluster.. [optional]  # noqa: E501
             name (str): Human friendly identifier of the region, for example `us-east-1`.  NOTE: Currently for all cloud providers and all regions `id` and `name` have exactly the same values.. [optional]  # noqa: E501
+            supports_hypershift (bool): 'true' if the region is supported for Hypershift deployments, 'false' otherwise.. [optional]  # noqa: E501
             supports_multi_az (bool): Whether the region supports multiple availability zones.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -255,14 +258,15 @@
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             ccs_only (bool): 'true' if the region is supported only for CCS clusters, 'false' otherwise.. [optional]  # noqa: E501
             cloud_provider (CloudProvider): [optional]  # noqa: E501
             display_name (str): Name of the region for display purposes, for example `N. Virginia`.. [optional]  # noqa: E501
             enabled (bool): Whether the region is enabled for deploying an OSD cluster.. [optional]  # noqa: E501
             name (str): Human friendly identifier of the region, for example `us-east-1`.  NOTE: Currently for all cloud providers and all regions `id` and `name` have exactly the same values.. [optional]  # noqa: E501
+            supports_hypershift (bool): 'true' if the region is supported for Hypershift deployments, 'false' otherwise.. [optional]  # noqa: E501
             supports_multi_az (bool): Whether the region supports multiple availability zones.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cloud_vpc.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cloud_vpc.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,68 +31,74 @@
 
 
 def lazy_import():
     from ocm_python_client.model.add_on_installation import AddOnInstallation
     from ocm_python_client.model.aws import AWS
     from ocm_python_client.model.aws_infrastructure_access_role_grant import AWSInfrastructureAccessRoleGrant
     from ocm_python_client.model.billing_model import BillingModel
+    from ocm_python_client.model.byo_oidc import ByoOidc
     from ocm_python_client.model.ccs import CCS
     from ocm_python_client.model.cloud_provider import CloudProvider
     from ocm_python_client.model.cloud_region import CloudRegion
     from ocm_python_client.model.cluster_api import ClusterAPI
     from ocm_python_client.model.cluster_console import ClusterConsole
     from ocm_python_client.model.cluster_health_state import ClusterHealthState
     from ocm_python_client.model.cluster_nodes import ClusterNodes
     from ocm_python_client.model.cluster_state import ClusterState
     from ocm_python_client.model.cluster_status import ClusterStatus
     from ocm_python_client.model.dns import DNS
     from ocm_python_client.model.external_configuration import ExternalConfiguration
     from ocm_python_client.model.flavour import Flavour
     from ocm_python_client.model.gcp import GCP
+    from ocm_python_client.model.gcp_encryption_key import GCPEncryptionKey
     from ocm_python_client.model.gcp_network import GCPNetwork
     from ocm_python_client.model.group import Group
-    from ocm_python_client.model.hyper_shift import HyperShift
+    from ocm_python_client.model.hypershift import Hypershift
     from ocm_python_client.model.identity_provider import IdentityProvider
     from ocm_python_client.model.inflight_check import InflightCheck
     from ocm_python_client.model.ingress import Ingress
     from ocm_python_client.model.machine_pool import MachinePool
     from ocm_python_client.model.managed_service import ManagedService
     from ocm_python_client.model.network import Network
+    from ocm_python_client.model.node_pool import NodePool
     from ocm_python_client.model.product import Product
     from ocm_python_client.model.provision_shard import ProvisionShard
     from ocm_python_client.model.proxy import Proxy
     from ocm_python_client.model.subscription import Subscription
     from ocm_python_client.model.value import Value
     from ocm_python_client.model.version import Version
     globals()['AWS'] = AWS
     globals()['AWSInfrastructureAccessRoleGrant'] = AWSInfrastructureAccessRoleGrant
     globals()['AddOnInstallation'] = AddOnInstallation
     globals()['BillingModel'] = BillingModel
+    globals()['ByoOidc'] = ByoOidc
     globals()['CCS'] = CCS
     globals()['CloudProvider'] = CloudProvider
     globals()['CloudRegion'] = CloudRegion
     globals()['ClusterAPI'] = ClusterAPI
     globals()['ClusterConsole'] = ClusterConsole
     globals()['ClusterHealthState'] = ClusterHealthState
     globals()['ClusterNodes'] = ClusterNodes
     globals()['ClusterState'] = ClusterState
     globals()['ClusterStatus'] = ClusterStatus
     globals()['DNS'] = DNS
     globals()['ExternalConfiguration'] = ExternalConfiguration
     globals()['Flavour'] = Flavour
     globals()['GCP'] = GCP
+    globals()['GCPEncryptionKey'] = GCPEncryptionKey
     globals()['GCPNetwork'] = GCPNetwork
     globals()['Group'] = Group
-    globals()['HyperShift'] = HyperShift
+    globals()['Hypershift'] = Hypershift
     globals()['IdentityProvider'] = IdentityProvider
     globals()['InflightCheck'] = InflightCheck
     globals()['Ingress'] = Ingress
     globals()['MachinePool'] = MachinePool
     globals()['ManagedService'] = ManagedService
     globals()['Network'] = Network
+    globals()['NodePool'] = NodePool
     globals()['Product'] = Product
     globals()['ProvisionShard'] = ProvisionShard
     globals()['Proxy'] = Proxy
     globals()['Subscription'] = Subscription
     globals()['Value'] = Value
     globals()['Version'] = Version
 
@@ -156,42 +162,45 @@
             'api': (ClusterAPI,),  # noqa: E501
             'aws': (AWS,),  # noqa: E501
             'aws_infrastructure_access_role_grants': ([AWSInfrastructureAccessRoleGrant],),  # noqa: E501
             'ccs': (CCS,),  # noqa: E501
             'dns': (DNS,),  # noqa: E501
             'fips': (bool,),  # noqa: E501
             'gcp': (GCP,),  # noqa: E501
+            'gcp_encryption_key': (GCPEncryptionKey,),  # noqa: E501
             'gcp_network': (GCPNetwork,),  # noqa: E501
             'additional_trust_bundle': (str,),  # noqa: E501
             'addons': ([AddOnInstallation],),  # noqa: E501
             'billing_model': (BillingModel,),  # noqa: E501
+            'byo_oidc': (ByoOidc,),  # noqa: E501
             'cloud_provider': (CloudProvider,),  # noqa: E501
             'console': (ClusterConsole,),  # noqa: E501
             'creation_timestamp': (datetime,),  # noqa: E501
             'disable_user_workload_monitoring': (bool,),  # noqa: E501
-            'display_name': (str,),  # noqa: E501
             'etcd_encryption': (bool,),  # noqa: E501
             'expiration_timestamp': (datetime,),  # noqa: E501
             'external_id': (str,),  # noqa: E501
             'external_configuration': (ExternalConfiguration,),  # noqa: E501
             'flavour': (Flavour,),  # noqa: E501
             'groups': ([Group],),  # noqa: E501
             'health_state': (ClusterHealthState,),  # noqa: E501
-            'hypershift': (HyperShift,),  # noqa: E501
+            'hypershift': (Hypershift,),  # noqa: E501
             'identity_providers': ([IdentityProvider],),  # noqa: E501
             'inflight_checks': ([InflightCheck],),  # noqa: E501
+            'infra_id': (str,),  # noqa: E501
             'ingresses': ([Ingress],),  # noqa: E501
             'load_balancer_quota': (int,),  # noqa: E501
             'machine_pools': ([MachinePool],),  # noqa: E501
             'managed': (bool,),  # noqa: E501
             'managed_service': (ManagedService,),  # noqa: E501
             'multi_az': (bool,),  # noqa: E501
             'name': (str,),  # noqa: E501
             'network': (Network,),  # noqa: E501
             'node_drain_grace_period': (Value,),  # noqa: E501
+            'node_pools': ([NodePool],),  # noqa: E501
             'nodes': (ClusterNodes,),  # noqa: E501
             'openshift_version': (str,),  # noqa: E501
             'product': (Product,),  # noqa: E501
             'properties': ({str: (str,)},),  # noqa: E501
             'provision_shard': (ProvisionShard,),  # noqa: E501
             'proxy': (Proxy,),  # noqa: E501
             'region': (CloudRegion,),  # noqa: E501
@@ -214,42 +223,45 @@
         'api': 'api',  # noqa: E501
         'aws': 'aws',  # noqa: E501
         'aws_infrastructure_access_role_grants': 'aws_infrastructure_access_role_grants',  # noqa: E501
         'ccs': 'ccs',  # noqa: E501
         'dns': 'dns',  # noqa: E501
         'fips': 'fips',  # noqa: E501
         'gcp': 'gcp',  # noqa: E501
+        'gcp_encryption_key': 'gcp_encryption_key',  # noqa: E501
         'gcp_network': 'gcp_network',  # noqa: E501
         'additional_trust_bundle': 'additional_trust_bundle',  # noqa: E501
         'addons': 'addons',  # noqa: E501
         'billing_model': 'billing_model',  # noqa: E501
+        'byo_oidc': 'byo_oidc',  # noqa: E501
         'cloud_provider': 'cloud_provider',  # noqa: E501
         'console': 'console',  # noqa: E501
         'creation_timestamp': 'creation_timestamp',  # noqa: E501
         'disable_user_workload_monitoring': 'disable_user_workload_monitoring',  # noqa: E501
-        'display_name': 'display_name',  # noqa: E501
         'etcd_encryption': 'etcd_encryption',  # noqa: E501
         'expiration_timestamp': 'expiration_timestamp',  # noqa: E501
         'external_id': 'external_id',  # noqa: E501
         'external_configuration': 'external_configuration',  # noqa: E501
         'flavour': 'flavour',  # noqa: E501
         'groups': 'groups',  # noqa: E501
         'health_state': 'health_state',  # noqa: E501
         'hypershift': 'hypershift',  # noqa: E501
         'identity_providers': 'identity_providers',  # noqa: E501
         'inflight_checks': 'inflight_checks',  # noqa: E501
+        'infra_id': 'infra_id',  # noqa: E501
         'ingresses': 'ingresses',  # noqa: E501
         'load_balancer_quota': 'load_balancer_quota',  # noqa: E501
         'machine_pools': 'machine_pools',  # noqa: E501
         'managed': 'managed',  # noqa: E501
         'managed_service': 'managed_service',  # noqa: E501
         'multi_az': 'multi_az',  # noqa: E501
         'name': 'name',  # noqa: E501
         'network': 'network',  # noqa: E501
         'node_drain_grace_period': 'node_drain_grace_period',  # noqa: E501
+        'node_pools': 'node_pools',  # noqa: E501
         'nodes': 'nodes',  # noqa: E501
         'openshift_version': 'openshift_version',  # noqa: E501
         'product': 'product',  # noqa: E501
         'properties': 'properties',  # noqa: E501
         'provision_shard': 'provision_shard',  # noqa: E501
         'proxy': 'proxy',  # noqa: E501
         'region': 'region',  # noqa: E501
@@ -307,42 +319,45 @@
             api (ClusterAPI): [optional]  # noqa: E501
             aws (AWS): [optional]  # noqa: E501
             aws_infrastructure_access_role_grants ([AWSInfrastructureAccessRoleGrant]): List of AWS infrastructure access role grants on this cluster.. [optional]  # noqa: E501
             ccs (CCS): [optional]  # noqa: E501
             dns (DNS): [optional]  # noqa: E501
             fips (bool): Create cluster that uses FIPS Validated / Modules in Process cryptographic libraries.. [optional]  # noqa: E501
             gcp (GCP): [optional]  # noqa: E501
+            gcp_encryption_key (GCPEncryptionKey): [optional]  # noqa: E501
             gcp_network (GCPNetwork): [optional]  # noqa: E501
             additional_trust_bundle (str): Additional trust bundle.. [optional]  # noqa: E501
             addons ([AddOnInstallation]): List of add-ons on this cluster.. [optional]  # noqa: E501
             billing_model (BillingModel): [optional]  # noqa: E501
+            byo_oidc (ByoOidc): [optional]  # noqa: E501
             cloud_provider (CloudProvider): [optional]  # noqa: E501
             console (ClusterConsole): [optional]  # noqa: E501
             creation_timestamp (datetime): Date and time when the cluster was initially created, using the format defined in [RFC3339](https://www.ietf.org/rfc/rfc3339.txt).. [optional]  # noqa: E501
             disable_user_workload_monitoring (bool): Indicates whether the User workload monitoring is enabled or not It is enabled by default. [optional]  # noqa: E501
-            display_name (str): Name of the cluster for display purposes. It can contain any characters, including spaces.. [optional]  # noqa: E501
             etcd_encryption (bool): Indicates whether that etcd is encrypted or not. This is set only during cluster creation.. [optional]  # noqa: E501
             expiration_timestamp (datetime): Date and time when the cluster will be automatically deleted, using the format defined in [RFC3339](https://www.ietf.org/rfc/rfc3339.txt). If no timestamp is provided, the cluster will never expire.  This option is unsupported.. [optional]  # noqa: E501
             external_id (str): External identifier of the cluster, generated by the installer.. [optional]  # noqa: E501
             external_configuration (ExternalConfiguration): [optional]  # noqa: E501
             flavour (Flavour): [optional]  # noqa: E501
             groups ([Group]): Link to the collection of groups of user of the cluster.. [optional]  # noqa: E501
             health_state (ClusterHealthState): [optional]  # noqa: E501
-            hypershift (HyperShift): [optional]  # noqa: E501
+            hypershift (Hypershift): [optional]  # noqa: E501
             identity_providers ([IdentityProvider]): Link to the collection of identity providers of the cluster.. [optional]  # noqa: E501
             inflight_checks ([InflightCheck]): List of inflight checks on this cluster.. [optional]  # noqa: E501
+            infra_id (str): InfraID is used for example to name the VPCs.. [optional]  # noqa: E501
             ingresses ([Ingress]): List of ingresses on this cluster.. [optional]  # noqa: E501
             load_balancer_quota (int): Load Balancer quota to be assigned to the cluster.. [optional]  # noqa: E501
             machine_pools ([MachinePool]): List of machine pools on this cluster.. [optional]  # noqa: E501
             managed (bool): Flag indicating if the cluster is managed (by Red Hat) or self-managed by the user.. [optional]  # noqa: E501
             managed_service (ManagedService): [optional]  # noqa: E501
             multi_az (bool): Flag indicating if the cluster should be created with nodes in different availability zones or all the nodes in a single one randomly selected.. [optional]  # noqa: E501
             name (str): Name of the cluster. This name is assigned by the user when the cluster is created.. [optional]  # noqa: E501
             network (Network): [optional]  # noqa: E501
             node_drain_grace_period (Value): [optional]  # noqa: E501
+            node_pools ([NodePool]): List of node pools on this cluster. NodePool is a scalable set of worker nodes attached to a hosted cluster.. [optional]  # noqa: E501
             nodes (ClusterNodes): [optional]  # noqa: E501
             openshift_version (str): Version of _OpenShift_ installed in the cluster, for example `4.0.0-0.2`.  When retrieving a cluster this will always be reported.  When provisioning a cluster this will be ignored, as the version to deploy will be determined internally.. [optional]  # noqa: E501
             product (Product): [optional]  # noqa: E501
             properties ({str: (str,)}): User defined properties for tagging and querying.. [optional]  # noqa: E501
             provision_shard (ProvisionShard): [optional]  # noqa: E501
             proxy (Proxy): [optional]  # noqa: E501
             region (CloudRegion): [optional]  # noqa: E501
@@ -442,42 +457,45 @@
             api (ClusterAPI): [optional]  # noqa: E501
             aws (AWS): [optional]  # noqa: E501
             aws_infrastructure_access_role_grants ([AWSInfrastructureAccessRoleGrant]): List of AWS infrastructure access role grants on this cluster.. [optional]  # noqa: E501
             ccs (CCS): [optional]  # noqa: E501
             dns (DNS): [optional]  # noqa: E501
             fips (bool): Create cluster that uses FIPS Validated / Modules in Process cryptographic libraries.. [optional]  # noqa: E501
             gcp (GCP): [optional]  # noqa: E501
+            gcp_encryption_key (GCPEncryptionKey): [optional]  # noqa: E501
             gcp_network (GCPNetwork): [optional]  # noqa: E501
             additional_trust_bundle (str): Additional trust bundle.. [optional]  # noqa: E501
             addons ([AddOnInstallation]): List of add-ons on this cluster.. [optional]  # noqa: E501
             billing_model (BillingModel): [optional]  # noqa: E501
+            byo_oidc (ByoOidc): [optional]  # noqa: E501
             cloud_provider (CloudProvider): [optional]  # noqa: E501
             console (ClusterConsole): [optional]  # noqa: E501
             creation_timestamp (datetime): Date and time when the cluster was initially created, using the format defined in [RFC3339](https://www.ietf.org/rfc/rfc3339.txt).. [optional]  # noqa: E501
             disable_user_workload_monitoring (bool): Indicates whether the User workload monitoring is enabled or not It is enabled by default. [optional]  # noqa: E501
-            display_name (str): Name of the cluster for display purposes. It can contain any characters, including spaces.. [optional]  # noqa: E501
             etcd_encryption (bool): Indicates whether that etcd is encrypted or not. This is set only during cluster creation.. [optional]  # noqa: E501
             expiration_timestamp (datetime): Date and time when the cluster will be automatically deleted, using the format defined in [RFC3339](https://www.ietf.org/rfc/rfc3339.txt). If no timestamp is provided, the cluster will never expire.  This option is unsupported.. [optional]  # noqa: E501
             external_id (str): External identifier of the cluster, generated by the installer.. [optional]  # noqa: E501
             external_configuration (ExternalConfiguration): [optional]  # noqa: E501
             flavour (Flavour): [optional]  # noqa: E501
             groups ([Group]): Link to the collection of groups of user of the cluster.. [optional]  # noqa: E501
             health_state (ClusterHealthState): [optional]  # noqa: E501
-            hypershift (HyperShift): [optional]  # noqa: E501
+            hypershift (Hypershift): [optional]  # noqa: E501
             identity_providers ([IdentityProvider]): Link to the collection of identity providers of the cluster.. [optional]  # noqa: E501
             inflight_checks ([InflightCheck]): List of inflight checks on this cluster.. [optional]  # noqa: E501
+            infra_id (str): InfraID is used for example to name the VPCs.. [optional]  # noqa: E501
             ingresses ([Ingress]): List of ingresses on this cluster.. [optional]  # noqa: E501
             load_balancer_quota (int): Load Balancer quota to be assigned to the cluster.. [optional]  # noqa: E501
             machine_pools ([MachinePool]): List of machine pools on this cluster.. [optional]  # noqa: E501
             managed (bool): Flag indicating if the cluster is managed (by Red Hat) or self-managed by the user.. [optional]  # noqa: E501
             managed_service (ManagedService): [optional]  # noqa: E501
             multi_az (bool): Flag indicating if the cluster should be created with nodes in different availability zones or all the nodes in a single one randomly selected.. [optional]  # noqa: E501
             name (str): Name of the cluster. This name is assigned by the user when the cluster is created.. [optional]  # noqa: E501
             network (Network): [optional]  # noqa: E501
             node_drain_grace_period (Value): [optional]  # noqa: E501
+            node_pools ([NodePool]): List of node pools on this cluster. NodePool is a scalable set of worker nodes attached to a hosted cluster.. [optional]  # noqa: E501
             nodes (ClusterNodes): [optional]  # noqa: E501
             openshift_version (str): Version of _OpenShift_ installed in the cluster, for example `4.0.0-0.2`.  When retrieving a cluster this will always be reported.  When provisioning a cluster this will be ignored, as the version to deploy will be determined internally.. [optional]  # noqa: E501
             product (Product): [optional]  # noqa: E501
             properties ({str: (str,)}): User defined properties for tagging and querying.. [optional]  # noqa: E501
             provision_shard (ProvisionShard): [optional]  # noqa: E501
             proxy (Proxy): [optional]  # noqa: E501
             region (CloudRegion): [optional]  # noqa: E501
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_api.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_api.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_configuration_mode.py` & `ocm_python_client-1.0.6/ocm_python_client/model/machine_type_size.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class ClusterConfigurationMode(ModelSimple):
+class MachineTypeSize(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,16 +49,17 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'FULL': "full",
-            'READ_ONLY': "read_only",
+            'LARGE': "large",
+            'MEDIUM': "medium",
+            'SMALL': "small",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -97,23 +98,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """ClusterConfigurationMode - a model defined in OpenAPI
+        """MachineTypeSize - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Configuration mode of a cluster.., must be one of ["full", "read_only", ]  # noqa: E501
+            args[0] (str): Machine type size.., must be one of ["large", "medium", "small", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Configuration mode of a cluster.., must be one of ["full", "read_only", ]  # noqa: E501
+            value (str): Machine type size.., must be one of ["large", "medium", "small", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -191,23 +192,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """ClusterConfigurationMode - a model defined in OpenAPI
+        """MachineTypeSize - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Configuration mode of a cluster.., must be one of ["full", "read_only", ]  # noqa: E501
+            args[0] (str): Machine type size.., must be one of ["large", "medium", "small", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Configuration mode of a cluster.., must be one of ["full", "read_only", ]  # noqa: E501
+            value (str): Machine type size.., must be one of ["large", "medium", "small", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_console.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_console.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_credentials.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_credentials.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_deployment.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_deployment.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_health_state.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_health_state.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_nodes.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_nodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,15 +94,17 @@
         return {
             'autoscale_compute': (MachinePoolAutoscaling,),  # noqa: E501
             'availability_zones': ([str],),  # noqa: E501
             'compute': (int,),  # noqa: E501
             'compute_labels': ({str: (str,)},),  # noqa: E501
             'compute_machine_type': (MachineType,),  # noqa: E501
             'infra': (int,),  # noqa: E501
+            'infra_machine_type': (MachineType,),  # noqa: E501
             'master': (int,),  # noqa: E501
+            'master_machine_type': (MachineType,),  # noqa: E501
             'security_group_filters': ([MachinePoolSecurityGroupFilter],),  # noqa: E501
             'total': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -111,15 +113,17 @@
     attribute_map = {
         'autoscale_compute': 'autoscale_compute',  # noqa: E501
         'availability_zones': 'availability_zones',  # noqa: E501
         'compute': 'compute',  # noqa: E501
         'compute_labels': 'compute_labels',  # noqa: E501
         'compute_machine_type': 'compute_machine_type',  # noqa: E501
         'infra': 'infra',  # noqa: E501
+        'infra_machine_type': 'infra_machine_type',  # noqa: E501
         'master': 'master',  # noqa: E501
+        'master_machine_type': 'master_machine_type',  # noqa: E501
         'security_group_filters': 'security_group_filters',  # noqa: E501
         'total': 'total',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
@@ -159,20 +163,22 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             autoscale_compute (MachinePoolAutoscaling): [optional]  # noqa: E501
             availability_zones ([str]): The availability zones upon which the nodes are created.. [optional]  # noqa: E501
-            compute (int): Number of compute nodes of the cluster. Compute and AutoscaleCompute cannot be used together.    . [optional]  # noqa: E501
+            compute (int): Number of compute nodes of the cluster. Compute and AutoscaleCompute cannot be used together.. [optional]  # noqa: E501
             compute_labels ({str: (str,)}): The labels set on the \"default\" compute machine pool.. [optional]  # noqa: E501
             compute_machine_type (MachineType): [optional]  # noqa: E501
             infra (int): Number of infrastructure nodes of the cluster.. [optional]  # noqa: E501
+            infra_machine_type (MachineType): [optional]  # noqa: E501
             master (int): Number of master nodes of the cluster.. [optional]  # noqa: E501
-            security_group_filters ([MachinePoolSecurityGroupFilter]): List of security groups to be applied to nodes (Optional). [optional]  # noqa: E501
+            master_machine_type (MachineType): [optional]  # noqa: E501
+            security_group_filters ([MachinePoolSecurityGroupFilter]): List of security groups to be applied to nodes (Optional).. [optional]  # noqa: E501
             total (int): Total number of nodes of the cluster.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -253,20 +259,22 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             autoscale_compute (MachinePoolAutoscaling): [optional]  # noqa: E501
             availability_zones ([str]): The availability zones upon which the nodes are created.. [optional]  # noqa: E501
-            compute (int): Number of compute nodes of the cluster. Compute and AutoscaleCompute cannot be used together.    . [optional]  # noqa: E501
+            compute (int): Number of compute nodes of the cluster. Compute and AutoscaleCompute cannot be used together.. [optional]  # noqa: E501
             compute_labels ({str: (str,)}): The labels set on the \"default\" compute machine pool.. [optional]  # noqa: E501
             compute_machine_type (MachineType): [optional]  # noqa: E501
             infra (int): Number of infrastructure nodes of the cluster.. [optional]  # noqa: E501
+            infra_machine_type (MachineType): [optional]  # noqa: E501
             master (int): Number of master nodes of the cluster.. [optional]  # noqa: E501
-            security_group_filters ([MachinePoolSecurityGroupFilter]): List of security groups to be applied to nodes (Optional). [optional]  # noqa: E501
+            master_machine_type (MachineType): [optional]  # noqa: E501
+            security_group_filters ([MachinePoolSecurityGroupFilter]): List of security groups to be applied to nodes (Optional).. [optional]  # noqa: E501
             total (int): Total number of nodes of the cluster.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_operator_info.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_operator_info.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_operator_state.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_operator_state.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_operators_info.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_operators_info.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_registration.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_registration.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,25 +78,27 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
+            'console_url': (str,),  # noqa: E501
             'external_id': (str,),  # noqa: E501
             'organization_id': (str,),  # noqa: E501
             'subscription_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
+        'console_url': 'console_url',  # noqa: E501
         'external_id': 'external_id',  # noqa: E501
         'organization_id': 'organization_id',  # noqa: E501
         'subscription_id': 'subscription_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
@@ -135,16 +137,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            external_id (str): Identifier of the cluster generated by the installer.  For example, to register a cluster that has been provisioned outside of this service, send a a request like this:  ```http POST /api/clusters_mgmt/v1/register_cluster HTTP/1.1 ```  With a request body like this:  ```json {   \"external_id\": \"d656aecf-11a6-4782-ad86-8f72638449ba\" } ```. [optional]  # noqa: E501
-            organization_id (str): Optional Organization identifier of the cluster generated by the account manager.. [optional]  # noqa: E501
+            console_url (str): Optional Console URL of the cluster.. [optional]  # noqa: E501
+            external_id (str): Identifier of the cluster generated by the installer.. [optional]  # noqa: E501
+            organization_id (str): Organization identifier of the cluster generated by the account manager.. [optional]  # noqa: E501
             subscription_id (str): Subscription identifier of the cluster generated by the account manager.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -223,16 +226,17 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            external_id (str): Identifier of the cluster generated by the installer.  For example, to register a cluster that has been provisioned outside of this service, send a a request like this:  ```http POST /api/clusters_mgmt/v1/register_cluster HTTP/1.1 ```  With a request body like this:  ```json {   \"external_id\": \"d656aecf-11a6-4782-ad86-8f72638449ba\" } ```. [optional]  # noqa: E501
-            organization_id (str): Optional Organization identifier of the cluster generated by the account manager.. [optional]  # noqa: E501
+            console_url (str): Optional Console URL of the cluster.. [optional]  # noqa: E501
+            external_id (str): Identifier of the cluster generated by the installer.. [optional]  # noqa: E501
+            organization_id (str): Organization identifier of the cluster generated by the account manager.. [optional]  # noqa: E501
             subscription_id (str): Subscription identifier of the cluster generated by the account manager.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_resources.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_resources.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_state.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_state.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cluster_status.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cluster_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,14 +92,15 @@
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
             'dns_ready': (bool,),  # noqa: E501
             'oidc_ready': (bool,),  # noqa: E501
             'configuration_mode': (ClusterConfigurationMode,),  # noqa: E501
+            'current_compute': (int,),  # noqa: E501
             'description': (str,),  # noqa: E501
             'limited_support_reason_count': (int,),  # noqa: E501
             'provision_error_code': (str,),  # noqa: E501
             'provision_error_message': (str,),  # noqa: E501
             'state': (ClusterState,),  # noqa: E501
         }
 
@@ -111,14 +112,15 @@
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
         'dns_ready': 'dns_ready',  # noqa: E501
         'oidc_ready': 'oidc_ready',  # noqa: E501
         'configuration_mode': 'configuration_mode',  # noqa: E501
+        'current_compute': 'current_compute',  # noqa: E501
         'description': 'description',  # noqa: E501
         'limited_support_reason_count': 'limited_support_reason_count',  # noqa: E501
         'provision_error_code': 'provision_error_code',  # noqa: E501
         'provision_error_message': 'provision_error_message',  # noqa: E501
         'state': 'state',  # noqa: E501
     }
 
@@ -165,14 +167,15 @@
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'ClusterStatus' if this is a complete object or 'ClusterStatusLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             dns_ready (bool): DNSReady from Provisioner. [optional]  # noqa: E501
             oidc_ready (bool): OIDCReady from user configuration.. [optional]  # noqa: E501
             configuration_mode (ClusterConfigurationMode): [optional]  # noqa: E501
+            current_compute (int): Current Replicas available for a Hosted Cluster. [optional]  # noqa: E501
             description (str): Detailed description of the cluster status.. [optional]  # noqa: E501
             limited_support_reason_count (int): Limited Support Reason Count. [optional]  # noqa: E501
             provision_error_code (str): Provisioning Error Code. [optional]  # noqa: E501
             provision_error_message (str): Provisioning Error Message. [optional]  # noqa: E501
             state (ClusterState): [optional]  # noqa: E501
         """
 
@@ -261,14 +264,15 @@
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'ClusterStatus' if this is a complete object or 'ClusterStatusLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
             dns_ready (bool): DNSReady from Provisioner. [optional]  # noqa: E501
             oidc_ready (bool): OIDCReady from user configuration.. [optional]  # noqa: E501
             configuration_mode (ClusterConfigurationMode): [optional]  # noqa: E501
+            current_compute (int): Current Replicas available for a Hosted Cluster. [optional]  # noqa: E501
             description (str): Detailed description of the cluster status.. [optional]  # noqa: E501
             limited_support_reason_count (int): Limited Support Reason Count. [optional]  # noqa: E501
             provision_error_code (str): Provisioning Error Code. [optional]  # noqa: E501
             provision_error_message (str): Provisioning Error Message. [optional]  # noqa: E501
             state (ClusterState): [optional]  # noqa: E501
         """
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cpu_total_node_role_os_metric_node.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cpu_total_node_role_os_metric_node.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/cpu_totals_node_role_os_metric_node.py` & `ocm_python_client-1.0.6/ocm_python_client/model/cpu_totals_node_role_os_metric_node.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/credential_request.py` & `ocm_python_client-1.0.6/ocm_python_client/model/credential_request.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/detection_type.py` & `ocm_python_client-1.0.6/ocm_python_client/model/detection_type.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/dns.py` & `ocm_python_client-1.0.6/ocm_python_client/model/dns.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/encryption_key.py` & `ocm_python_client-1.0.6/ocm_python_client/model/encryption_key.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/environment.py` & `ocm_python_client-1.0.6/ocm_python_client/model/environment.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/error.py` & `ocm_python_client-1.0.6/ocm_python_client/model/error.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/event.py` & `ocm_python_client-1.0.6/ocm_python_client/model/event.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/external_configuration.py` & `ocm_python_client-1.0.6/ocm_python_client/model/external_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,18 @@
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 def lazy_import():
     from ocm_python_client.model.label import Label
+    from ocm_python_client.model.manifest import Manifest
     from ocm_python_client.model.syncset import Syncset
     globals()['Label'] = Label
+    globals()['Manifest'] = Manifest
     globals()['Syncset'] = Syncset
 
 
 class ExternalConfiguration(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
@@ -87,24 +89,26 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'labels': ([Label],),  # noqa: E501
+            'manifests': ([Manifest],),  # noqa: E501
             'syncsets': ([Syncset],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'labels': 'labels',  # noqa: E501
+        'manifests': 'manifests',  # noqa: E501
         'syncsets': 'syncsets',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -142,14 +146,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             labels ([Label]): list of labels externally configured on the clusterdeployment.. [optional]  # noqa: E501
+            manifests ([Manifest]): list of manifest externally configured for a hosted cluster.. [optional]  # noqa: E501
             syncsets ([Syncset]): list of syncsets externally configured on the cluster.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -229,14 +234,15 @@
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             labels ([Label]): list of labels externally configured on the clusterdeployment.. [optional]  # noqa: E501
+            manifests ([Manifest]): list of manifest externally configured for a hosted cluster.. [optional]  # noqa: E501
             syncsets ([Syncset]): list of syncsets externally configured on the cluster.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/flavour.py` & `ocm_python_client-1.0.6/ocm_python_client/model/flavour.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/flavour_nodes.py` & `ocm_python_client-1.0.6/ocm_python_client/model/flavour_nodes.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/gcp.py` & `ocm_python_client-1.0.6/ocm_python_client/model/gcp.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/gcp_flavour.py` & `ocm_python_client-1.0.6/ocm_python_client/model/value.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class GCPFlavour(ModelNormal):
+class Value(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,39 +78,37 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'compute_instance_type': (str,),  # noqa: E501
-            'infra_instance_type': (str,),  # noqa: E501
-            'master_instance_type': (str,),  # noqa: E501
+            'unit': (str,),  # noqa: E501
+            'value': (float,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'compute_instance_type': 'compute_instance_type',  # noqa: E501
-        'infra_instance_type': 'infra_instance_type',  # noqa: E501
-        'master_instance_type': 'master_instance_type',  # noqa: E501
+        'unit': 'unit',  # noqa: E501
+        'value': 'value',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GCPFlavour - a model defined in OpenAPI
+        """Value - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +133,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            compute_instance_type (str): GCP default instance type for the worker volume.  User can be overridden specifying in the cluster itself a type for compute node.. [optional]  # noqa: E501
-            infra_instance_type (str): GCP default instance type for the infra volume.. [optional]  # noqa: E501
-            master_instance_type (str): GCP default instance type for the master volume.. [optional]  # noqa: E501
+            unit (str): Name of the unit used to measure the value.. [optional]  # noqa: E501
+            value (float): Numeric value.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +187,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GCPFlavour - a model defined in OpenAPI
+        """Value - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,17 +220,16 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            compute_instance_type (str): GCP default instance type for the worker volume.  User can be overridden specifying in the cluster itself a type for compute node.. [optional]  # noqa: E501
-            infra_instance_type (str): GCP default instance type for the infra volume.. [optional]  # noqa: E501
-            master_instance_type (str): GCP default instance type for the master volume.. [optional]  # noqa: E501
+            unit (str): Name of the unit used to measure the value.. [optional]  # noqa: E501
+            value (float): Numeric value.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/gcp_network.py` & `ocm_python_client-1.0.6/ocm_python_client/model/gcp_network.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/github_identity_provider.py` & `ocm_python_client-1.0.6/ocm_python_client/model/github_identity_provider.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/gitlab_identity_provider.py` & `ocm_python_client-1.0.6/ocm_python_client/model/gitlab_identity_provider.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/google_identity_provider.py` & `ocm_python_client-1.0.6/ocm_python_client/model/google_identity_provider.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/group.py` & `ocm_python_client-1.0.6/ocm_python_client/model/group.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/ht_passwd_identity_provider.py` & `ocm_python_client-1.0.6/ocm_python_client/model/ht_passwd_identity_provider.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/ht_passwd_user.py` & `ocm_python_client-1.0.6/ocm_python_client/model/ht_passwd_user.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/hyper_shift.py` & `ocm_python_client-1.0.6/ocm_python_client/model/hypershift.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class HyperShift(ModelNormal):
+class Hypershift(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -98,15 +98,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """HyperShift - a model defined in OpenAPI
+        """Hypershift - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -131,15 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            enabled (bool): Boolean flag indicating if the cluster should be creating using _HyperShift_.  By default this is `false`.  To enable it the cluster needs to be ROSA cluster and the organization of the user needs to have the `hypershift` capability enabled.. [optional]  # noqa: E501
+            enabled (bool): Boolean flag indicating if the cluster should be creating using _Hypershift_.  By default this is `false`.  To enable it the cluster needs to be ROSA cluster and the organization of the user needs to have the `hypershift` capability enabled.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -184,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """HyperShift - a model defined in OpenAPI
+        """Hypershift - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -217,15 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            enabled (bool): Boolean flag indicating if the cluster should be creating using _HyperShift_.  By default this is `false`.  To enable it the cluster needs to be ROSA cluster and the organization of the user needs to have the `hypershift` capability enabled.. [optional]  # noqa: E501
+            enabled (bool): Boolean flag indicating if the cluster should be creating using _Hypershift_.  By default this is `false`.  To enable it the cluster needs to be ROSA cluster and the organization of the user needs to have the `hypershift` capability enabled.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/identity_provider.py` & `ocm_python_client-1.0.6/ocm_python_client/model/identity_provider.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/identity_provider_mapping_method.py` & `ocm_python_client-1.0.6/ocm_python_client/model/identity_provider_mapping_method.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/identity_provider_type.py` & `ocm_python_client-1.0.6/ocm_python_client/model/identity_provider_type.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/inflight_check.py` & `ocm_python_client-1.0.6/ocm_python_client/model/inflight_check.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/inflight_check_state.py` & `ocm_python_client-1.0.6/ocm_python_client/model/inflight_check_state.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/ingress.py` & `ocm_python_client-1.0.6/ocm_python_client/model/ingress.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/instance_iam_roles.py` & `ocm_python_client-1.0.6/ocm_python_client/model/instance_iam_roles.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/key_ring.py` & `ocm_python_client-1.0.6/ocm_python_client/model/key_ring.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/label.py` & `ocm_python_client-1.0.6/ocm_python_client/model/label.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/ldap_attributes.py` & `ocm_python_client-1.0.6/ocm_python_client/model/ldap_attributes.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/ldap_identity_provider.py` & `ocm_python_client-1.0.6/ocm_python_client/model/ldap_identity_provider.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/limited_support_reason.py` & `ocm_python_client-1.0.6/ocm_python_client/model/limited_support_reason.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/limited_support_reason_template.py` & `ocm_python_client-1.0.6/ocm_python_client/model/limited_support_reason_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'LimitedSupportReasonTemplate' if this is a complete object or 'LimitedSupportReasonTemplateLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
-            details (str): URL with a link to a detailed description of the reason.. [optional]  # noqa: E501
+            details (str): A detailed description of the reason.. [optional]  # noqa: E501
             summary (str): Summary of the reason.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -232,15 +232,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'LimitedSupportReasonTemplate' if this is a complete object or 'LimitedSupportReasonTemplateLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
-            details (str): URL with a link to a detailed description of the reason.. [optional]  # noqa: E501
+            details (str): A detailed description of the reason.. [optional]  # noqa: E501
             summary (str): Summary of the reason.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/listening_method.py` & `ocm_python_client-1.0.6/ocm_python_client/model/listening_method.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/log.py` & `ocm_python_client-1.0.6/ocm_python_client/model/log.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/machine_pool.py` & `ocm_python_client-1.0.6/ocm_python_client/model/machine_pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -103,14 +103,15 @@
             'autoscaling': (MachinePoolAutoscaling,),  # noqa: E501
             'availability_zones': ([str],),  # noqa: E501
             'cluster': (Cluster,),  # noqa: E501
             'instance_type': (str,),  # noqa: E501
             'labels': ({str: (str,)},),  # noqa: E501
             'replicas': (int,),  # noqa: E501
             'security_group_filters': ([MachinePoolSecurityGroupFilter],),  # noqa: E501
+            'subnets': ([str],),  # noqa: E501
             'taints': ([Taint],),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
@@ -123,14 +124,15 @@
         'autoscaling': 'autoscaling',  # noqa: E501
         'availability_zones': 'availability_zones',  # noqa: E501
         'cluster': 'cluster',  # noqa: E501
         'instance_type': 'instance_type',  # noqa: E501
         'labels': 'labels',  # noqa: E501
         'replicas': 'replicas',  # noqa: E501
         'security_group_filters': 'security_group_filters',  # noqa: E501
+        'subnets': 'subnets',  # noqa: E501
         'taints': 'taints',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -178,14 +180,15 @@
             autoscaling (MachinePoolAutoscaling): [optional]  # noqa: E501
             availability_zones ([str]): The availability zones upon which the nodes are created.. [optional]  # noqa: E501
             cluster (Cluster): [optional]  # noqa: E501
             instance_type (str): The instance type of Nodes to create.. [optional]  # noqa: E501
             labels ({str: (str,)}): The labels set on the Nodes created.. [optional]  # noqa: E501
             replicas (int): The number of Machines (and Nodes) to create. Replicas and autoscaling cannot be used together.    . [optional]  # noqa: E501
             security_group_filters ([MachinePoolSecurityGroupFilter]): List of security groups to be applied to MachinePool (Optional). [optional]  # noqa: E501
+            subnets ([str]): The subnets upon which the nodes are created.. [optional]  # noqa: E501
             taints ([Taint]): The taints set on the Nodes created.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -275,14 +278,15 @@
             autoscaling (MachinePoolAutoscaling): [optional]  # noqa: E501
             availability_zones ([str]): The availability zones upon which the nodes are created.. [optional]  # noqa: E501
             cluster (Cluster): [optional]  # noqa: E501
             instance_type (str): The instance type of Nodes to create.. [optional]  # noqa: E501
             labels ({str: (str,)}): The labels set on the Nodes created.. [optional]  # noqa: E501
             replicas (int): The number of Machines (and Nodes) to create. Replicas and autoscaling cannot be used together.    . [optional]  # noqa: E501
             security_group_filters ([MachinePoolSecurityGroupFilter]): List of security groups to be applied to MachinePool (Optional). [optional]  # noqa: E501
+            subnets ([str]): The subnets upon which the nodes are created.. [optional]  # noqa: E501
             taints ([Taint]): The taints set on the Nodes created.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/machine_pool_autoscaling.py` & `ocm_python_client-1.0.6/ocm_python_client/model/machine_pool_autoscaling.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/machine_pool_security_group_filter.py` & `ocm_python_client-1.0.6/ocm_python_client/model/machine_pool_security_group_filter.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/machine_type.py` & `ocm_python_client-1.0.6/ocm_python_client/model/machine_type.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/machine_type_category.py` & `ocm_python_client-1.0.6/ocm_python_client/model/machine_type_category.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/machine_type_size.py` & `ocm_python_client-1.0.6/ocm_python_client/model/node_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class MachineTypeSize(ModelSimple):
+class NodeType(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,17 +49,17 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'LARGE': "large",
-            'MEDIUM': "medium",
-            'SMALL': "small",
+            'COMPUTE': "compute",
+            'INFRA': "infra",
+            'MASTER': "master",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -98,23 +98,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """MachineTypeSize - a model defined in OpenAPI
+        """NodeType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Machine type size.., must be one of ["large", "medium", "small", ]  # noqa: E501
+            args[0] (str): Type of node received via telemetry.., must be one of ["compute", "infra", "master", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Machine type size.., must be one of ["large", "medium", "small", ]  # noqa: E501
+            value (str): Type of node received via telemetry.., must be one of ["compute", "infra", "master", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -192,23 +192,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """MachineTypeSize - a model defined in OpenAPI
+        """NodeType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Machine type size.., must be one of ["large", "medium", "small", ]  # noqa: E501
+            args[0] (str): Type of node received via telemetry.., must be one of ["compute", "infra", "master", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Machine type size.., must be one of ["large", "medium", "small", ]  # noqa: E501
+            value (str): Type of node received via telemetry.., must be one of ["compute", "infra", "master", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/managed_service.py` & `ocm_python_client-1.0.6/ocm_python_client/model/managed_service.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/metadata.py` & `ocm_python_client-1.0.6/ocm_python_client/model/metadata.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/network.py` & `ocm_python_client-1.0.6/ocm_python_client/model/network.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/node_info.py` & `ocm_python_client-1.0.6/ocm_python_client/model/node_info.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/node_type.py` & `ocm_python_client-1.0.6/ocm_python_client/model/billing_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class NodeType(ModelSimple):
+class BillingModel(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -49,17 +49,19 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'COMPUTE': "compute",
-            'INFRA': "infra",
-            'MASTER': "master",
+            'MARKETPLACE': "marketplace",
+            'MARKETPLACE-AWS': "marketplace-aws",
+            'MARKETPLACE-RHM': "marketplace-rhm",
+            'MARKETPLACE-AZURE': "marketplace-azure",
+            'STANDARD': "standard",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
@@ -98,23 +100,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """NodeType - a model defined in OpenAPI
+        """BillingModel - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Type of node received via telemetry.., must be one of ["compute", "infra", "master", ]  # noqa: E501
+            args[0] (str): Billing model for cluster resources.., must be one of ["marketplace", "marketplace-aws", "marketplace-rhm", "marketplace-azure", "standard", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Type of node received via telemetry.., must be one of ["compute", "infra", "master", ]  # noqa: E501
+            value (str): Billing model for cluster resources.., must be one of ["marketplace", "marketplace-aws", "marketplace-rhm", "marketplace-azure", "standard", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
@@ -192,23 +194,23 @@
                 path_to_item=_path_to_item,
                 valid_classes=(self.__class__,),
             )
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):
-        """NodeType - a model defined in OpenAPI
+        """BillingModel - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): Type of node received via telemetry.., must be one of ["compute", "infra", "master", ]  # noqa: E501
+            args[0] (str): Billing model for cluster resources.., must be one of ["marketplace", "marketplace-aws", "marketplace-rhm", "marketplace-azure", "standard", ]  # noqa: E501
 
         Keyword Args:
-            value (str): Type of node received via telemetry.., must be one of ["compute", "infra", "master", ]  # noqa: E501
+            value (str): Billing model for cluster resources.., must be one of ["marketplace", "marketplace-aws", "marketplace-rhm", "marketplace-azure", "standard", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/nodes_info.py` & `ocm_python_client-1.0.6/ocm_python_client/model/nodes_info.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/open_id_claims.py` & `ocm_python_client-1.0.6/ocm_python_client/model/open_id_claims.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/open_id_identity_provider.py` & `ocm_python_client-1.0.6/ocm_python_client/model/open_id_identity_provider.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/operator_iam_role.py` & `ocm_python_client-1.0.6/ocm_python_client/model/operator_iam_role.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/product.py` & `ocm_python_client-1.0.6/ocm_python_client/model/product.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/provision_shard.py` & `ocm_python_client-1.0.6/ocm_python_client/model/version_gate.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,24 +26,16 @@
     none_type,
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
-def lazy_import():
-    from ocm_python_client.model.cloud_provider import CloudProvider
-    from ocm_python_client.model.cloud_region import CloudRegion
-    from ocm_python_client.model.server_config import ServerConfig
-    globals()['CloudProvider'] = CloudProvider
-    globals()['CloudRegion'] = CloudRegion
-    globals()['ServerConfig'] = ServerConfig
 
-
-class ProvisionShard(ModelNormal):
+class VersionGate(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -71,72 +63,70 @@
 
     @cached_property
     def additional_properties_type():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
         """
-        lazy_import()
         return (bool, date, datetime, dict, float, int, list, str, none_type,)  # noqa: E501
 
     _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
-        lazy_import()
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
-            'aws_account_operator_config': (ServerConfig,),  # noqa: E501
-            'aws_base_domain': (str,),  # noqa: E501
-            'gcp_base_domain': (str,),  # noqa: E501
-            'gcp_project_operator': (ServerConfig,),  # noqa: E501
-            'cloud_provider': (CloudProvider,),  # noqa: E501
-            'hive_config': (ServerConfig,),  # noqa: E501
-            'management_cluster': (str,),  # noqa: E501
-            'region': (CloudRegion,),  # noqa: E501
+            'sts_only': (bool,),  # noqa: E501
+            'creation_timestamp': (datetime,),  # noqa: E501
+            'description': (str,),  # noqa: E501
+            'documentation_url': (str,),  # noqa: E501
+            'label': (str,),  # noqa: E501
+            'value': (str,),  # noqa: E501
+            'version_raw_id_prefix': (str,),  # noqa: E501
+            'warning_message': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
-        'aws_account_operator_config': 'aws_account_operator_config',  # noqa: E501
-        'aws_base_domain': 'aws_base_domain',  # noqa: E501
-        'gcp_base_domain': 'gcp_base_domain',  # noqa: E501
-        'gcp_project_operator': 'gcp_project_operator',  # noqa: E501
-        'cloud_provider': 'cloud_provider',  # noqa: E501
-        'hive_config': 'hive_config',  # noqa: E501
-        'management_cluster': 'management_cluster',  # noqa: E501
-        'region': 'region',  # noqa: E501
+        'sts_only': 'sts_only',  # noqa: E501
+        'creation_timestamp': 'creation_timestamp',  # noqa: E501
+        'description': 'description',  # noqa: E501
+        'documentation_url': 'documentation_url',  # noqa: E501
+        'label': 'label',  # noqa: E501
+        'value': 'value',  # noqa: E501
+        'version_raw_id_prefix': 'version_raw_id_prefix',  # noqa: E501
+        'warning_message': 'warning_message',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """ProvisionShard - a model defined in OpenAPI
+        """VersionGate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -161,25 +151,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kind (str): Indicates the type of this object. Will be 'ProvisionShard' if this is a complete object or 'ProvisionShardLink' if it is just a link.. [optional]  # noqa: E501
+            kind (str): Indicates the type of this object. Will be 'VersionGate' if this is a complete object or 'VersionGateLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
-            aws_account_operator_config (ServerConfig): [optional]  # noqa: E501
-            aws_base_domain (str): Contains the AWS base domain. [optional]  # noqa: E501
-            gcp_base_domain (str): Contains the GCP base domain. [optional]  # noqa: E501
-            gcp_project_operator (ServerConfig): [optional]  # noqa: E501
-            cloud_provider (CloudProvider): [optional]  # noqa: E501
-            hive_config (ServerConfig): [optional]  # noqa: E501
-            management_cluster (str): Contains the name of the managment cluster for Hypershift clusters that are assigned to this shard. This field is populated by OCM, and must not be overwritten via API.. [optional]  # noqa: E501
-            region (CloudRegion): [optional]  # noqa: E501
+            sts_only (bool): STSOnly indicates if this version gate is for STS clusters only. [optional]  # noqa: E501
+            creation_timestamp (datetime): CreationTimestamp is the date and time when the version gate was created, format defined in https://www.ietf.org/rfc/rfc3339.txt[RC3339].. [optional]  # noqa: E501
+            description (str): Description of the version gate.. [optional]  # noqa: E501
+            documentation_url (str): DocumentationURL is the URL for the documentation of the version gate.. [optional]  # noqa: E501
+            label (str): Label representing the version gate in OpenShift.. [optional]  # noqa: E501
+            value (str): Value represents the required value of the label.. [optional]  # noqa: E501
+            version_raw_id_prefix (str): VersionRawIDPrefix represents the versions prefix that the gate applies to.. [optional]  # noqa: E501
+            warning_message (str): WarningMessage is a warning that will be displayed to the user before they acknowledge the gate. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -224,15 +214,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """ProvisionShard - a model defined in OpenAPI
+        """VersionGate - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -257,25 +247,25 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kind (str): Indicates the type of this object. Will be 'ProvisionShard' if this is a complete object or 'ProvisionShardLink' if it is just a link.. [optional]  # noqa: E501
+            kind (str): Indicates the type of this object. Will be 'VersionGate' if this is a complete object or 'VersionGateLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
-            aws_account_operator_config (ServerConfig): [optional]  # noqa: E501
-            aws_base_domain (str): Contains the AWS base domain. [optional]  # noqa: E501
-            gcp_base_domain (str): Contains the GCP base domain. [optional]  # noqa: E501
-            gcp_project_operator (ServerConfig): [optional]  # noqa: E501
-            cloud_provider (CloudProvider): [optional]  # noqa: E501
-            hive_config (ServerConfig): [optional]  # noqa: E501
-            management_cluster (str): Contains the name of the managment cluster for Hypershift clusters that are assigned to this shard. This field is populated by OCM, and must not be overwritten via API.. [optional]  # noqa: E501
-            region (CloudRegion): [optional]  # noqa: E501
+            sts_only (bool): STSOnly indicates if this version gate is for STS clusters only. [optional]  # noqa: E501
+            creation_timestamp (datetime): CreationTimestamp is the date and time when the version gate was created, format defined in https://www.ietf.org/rfc/rfc3339.txt[RC3339].. [optional]  # noqa: E501
+            description (str): Description of the version gate.. [optional]  # noqa: E501
+            documentation_url (str): DocumentationURL is the URL for the documentation of the version gate.. [optional]  # noqa: E501
+            label (str): Label representing the version gate in OpenShift.. [optional]  # noqa: E501
+            value (str): Value represents the required value of the label.. [optional]  # noqa: E501
+            version_raw_id_prefix (str): VersionRawIDPrefix represents the versions prefix that the gate applies to.. [optional]  # noqa: E501
+            warning_message (str): WarningMessage is a warning that will be displayed to the user before they acknowledge the gate. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/proxy.py` & `ocm_python_client-1.0.6/ocm_python_client/model/proxy.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/server_config.py` & `ocm_python_client-1.0.6/ocm_python_client/model/server_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,26 +81,28 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
+            'kubeconfig': (str,),  # noqa: E501
             'server': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
+        'kubeconfig': 'kubeconfig',  # noqa: E501
         'server': 'server',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -140,14 +142,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'ServerConfig' if this is a complete object or 'ServerConfigLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
+            kubeconfig (str): The kubeconfig of the server. [optional]  # noqa: E501
             server (str): The URL of the server. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -229,14 +232,15 @@
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             kind (str): Indicates the type of this object. Will be 'ServerConfig' if this is a complete object or 'ServerConfigLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
+            kubeconfig (str): The kubeconfig of the server. [optional]  # noqa: E501
             server (str): The URL of the server. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/socket_total_node_role_os_metric_node.py` & `ocm_python_client-1.0.6/ocm_python_client/model/socket_total_node_role_os_metric_node.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/socket_totals_node_role_os_metric_node.py` & `ocm_python_client-1.0.6/ocm_python_client/model/socket_totals_node_role_os_metric_node.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/ssh_credentials.py` & `ocm_python_client-1.0.6/ocm_python_client/model/ssh_credentials.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/sts.py` & `ocm_python_client-1.0.6/ocm_python_client/model/sts.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,16 +88,19 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
             'oidc_endpoint_url': (str,),  # noqa: E501
             'auto_mode': (bool,),  # noqa: E501
+            'enabled': (bool,),  # noqa: E501
             'external_id': (str,),  # noqa: E501
             'instance_iam_roles': (InstanceIAMRoles,),  # noqa: E501
+            'managed_policies': (bool,),  # noqa: E501
+            'oidc_private_key_secret_arn': (str,),  # noqa: E501
             'operator_iam_roles': ([OperatorIAMRole],),  # noqa: E501
             'operator_role_prefix': (str,),  # noqa: E501
             'permission_boundary': (str,),  # noqa: E501
             'role_arn': (str,),  # noqa: E501
             'support_role_arn': (str,),  # noqa: E501
         }
 
@@ -105,16 +108,19 @@
     def discriminator():
         return None
 
 
     attribute_map = {
         'oidc_endpoint_url': 'oidc_endpoint_url',  # noqa: E501
         'auto_mode': 'auto_mode',  # noqa: E501
+        'enabled': 'enabled',  # noqa: E501
         'external_id': 'external_id',  # noqa: E501
         'instance_iam_roles': 'instance_iam_roles',  # noqa: E501
+        'managed_policies': 'managed_policies',  # noqa: E501
+        'oidc_private_key_secret_arn': 'oidc_private_key_secret_arn',  # noqa: E501
         'operator_iam_roles': 'operator_iam_roles',  # noqa: E501
         'operator_role_prefix': 'operator_role_prefix',  # noqa: E501
         'permission_boundary': 'permission_boundary',  # noqa: E501
         'role_arn': 'role_arn',  # noqa: E501
         'support_role_arn': 'support_role_arn',  # noqa: E501
     }
 
@@ -157,16 +163,19 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             oidc_endpoint_url (str): URL of the location where OIDC configuration and keys are available. [optional]  # noqa: E501
             auto_mode (bool): Auto creation mode for cluster - OCM will create the operator roles and OIDC provider. false by default.. [optional]  # noqa: E501
+            enabled (bool): If STS is enabled or disabled. [optional]  # noqa: E501
             external_id (str): Optional unique identifier when assuming role in another account. [optional]  # noqa: E501
             instance_iam_roles (InstanceIAMRoles): [optional]  # noqa: E501
+            managed_policies (bool): If true, cluster account and operator roles have managed policies attached.. [optional]  # noqa: E501
+            oidc_private_key_secret_arn (str): Secrets Manager ARN for the OIDC private key key.. [optional]  # noqa: E501
             operator_iam_roles ([OperatorIAMRole]): List of roles necessary to access the AWS resources of the various operators used during installation. [optional]  # noqa: E501
             operator_role_prefix (str): Optional user provided prefix for operator roles.. [optional]  # noqa: E501
             permission_boundary (str): Optional user provided permission boundary.. [optional]  # noqa: E501
             role_arn (str): ARN of the AWS role to assume when installing the cluster. [optional]  # noqa: E501
             support_role_arn (str): ARN of the AWS role used by SREs to access the cluster AWS account in order to provide support. [optional]  # noqa: E501
         """
 
@@ -251,16 +260,19 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             oidc_endpoint_url (str): URL of the location where OIDC configuration and keys are available. [optional]  # noqa: E501
             auto_mode (bool): Auto creation mode for cluster - OCM will create the operator roles and OIDC provider. false by default.. [optional]  # noqa: E501
+            enabled (bool): If STS is enabled or disabled. [optional]  # noqa: E501
             external_id (str): Optional unique identifier when assuming role in another account. [optional]  # noqa: E501
             instance_iam_roles (InstanceIAMRoles): [optional]  # noqa: E501
+            managed_policies (bool): If true, cluster account and operator roles have managed policies attached.. [optional]  # noqa: E501
+            oidc_private_key_secret_arn (str): Secrets Manager ARN for the OIDC private key key.. [optional]  # noqa: E501
             operator_iam_roles ([OperatorIAMRole]): List of roles necessary to access the AWS resources of the various operators used during installation. [optional]  # noqa: E501
             operator_role_prefix (str): Optional user provided prefix for operator roles.. [optional]  # noqa: E501
             permission_boundary (str): Optional user provided permission boundary.. [optional]  # noqa: E501
             role_arn (str): ARN of the AWS role to assume when installing the cluster. [optional]  # noqa: E501
             support_role_arn (str): ARN of the AWS role used by SREs to access the cluster AWS account in order to provide support. [optional]  # noqa: E501
         """
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/sts_credential_request.py` & `ocm_python_client-1.0.6/ocm_python_client/model/sts_credential_request.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/sts_operator.py` & `ocm_python_client-1.0.6/ocm_python_client/model/sts_operator.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/subnetwork.py` & `ocm_python_client-1.0.6/ocm_python_client/model/subnetwork.py`

 * *Files 3% similar despite different names*

```diff
@@ -80,25 +80,27 @@
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'availability_zone': (str,),  # noqa: E501
             'name': (str,),  # noqa: E501
+            'public': (bool,),  # noqa: E501
             'subnet_id': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'availability_zone': 'availability_zone',  # noqa: E501
         'name': 'name',  # noqa: E501
+        'public': 'public',  # noqa: E501
         'subnet_id': 'subnet_id',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
@@ -137,14 +139,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             availability_zone (str): The availability zone to which the subnet is related. [optional]  # noqa: E501
             name (str): Name of the subnet according to its `Name` tag on AWS. [optional]  # noqa: E501
+            public (bool): Whether it is a public subnet. [optional]  # noqa: E501
             subnet_id (str): The subnet id to be used while installing a cluster. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
@@ -225,14 +228,15 @@
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
             availability_zone (str): The availability zone to which the subnet is related. [optional]  # noqa: E501
             name (str): Name of the subnet according to its `Name` tag on AWS. [optional]  # noqa: E501
+            public (bool): Whether it is a public subnet. [optional]  # noqa: E501
             subnet_id (str): The subnet id to be used while installing a cluster. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/subscription.py` & `ocm_python_client-1.0.6/ocm_python_client/model/user.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class Subscription(ModelNormal):
+class User(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -102,15 +102,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Subscription - a model defined in OpenAPI
+        """User - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,15 +135,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kind (str): Indicates the type of this object. Will be 'Subscription' if this is a complete object or 'SubscriptionLink' if it is just a link.. [optional]  # noqa: E501
+            kind (str): Indicates the type of this object. Will be 'User' if this is a complete object or 'UserLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -190,15 +190,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Subscription - a model defined in OpenAPI
+        """User - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,15 +223,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kind (str): Indicates the type of this object. Will be 'Subscription' if this is a complete object or 'SubscriptionLink' if it is just a link.. [optional]  # noqa: E501
+            kind (str): Indicates the type of this object. Will be 'User' if this is a complete object or 'UserLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/syncset.py` & `ocm_python_client-1.0.6/ocm_python_client/model/syncset.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/taint.py` & `ocm_python_client-1.0.6/ocm_python_client/model/taint.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/upgrade_policy.py` & `ocm_python_client-1.0.6/ocm_python_client/model/upgrade_policy.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/upgrade_policy_state.py` & `ocm_python_client-1.0.6/ocm_python_client/model/upgrade_policy_state.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/upgrade_policy_state_value.py` & `ocm_python_client-1.0.6/ocm_python_client/model/upgrade_policy_state_value.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/user.py` & `ocm_python_client-1.0.6/ocm_python_client/model/additional_catalog_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class User(ModelNormal):
+class AdditionalCatalogSource(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,39 +78,41 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
-            'href': (str,),  # noqa: E501
+            'enabled': (bool,),  # noqa: E501
+            'image': (str,),  # noqa: E501
+            'name': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
-        'href': 'href',  # noqa: E501
+        'enabled': 'enabled',  # noqa: E501
+        'image': 'image',  # noqa: E501
+        'name': 'name',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+        """AdditionalCatalogSource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -135,17 +137,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kind (str): Indicates the type of this object. Will be 'User' if this is a complete object or 'UserLink' if it is just a link.. [optional]  # noqa: E501
-            id (str): Unique identifier of the object.. [optional]  # noqa: E501
-            href (str): Self link.. [optional]  # noqa: E501
+            id (str): ID of the additional catalog source. [optional]  # noqa: E501
+            enabled (bool): Indicates is this additional catalog source is enabled for the addon. [optional]  # noqa: E501
+            image (str): Image of the additional catalog source.. [optional]  # noqa: E501
+            name (str): Name of the additional catalog source.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -190,15 +193,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """User - a model defined in OpenAPI
+        """AdditionalCatalogSource - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -223,17 +226,18 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kind (str): Indicates the type of this object. Will be 'User' if this is a complete object or 'UserLink' if it is just a link.. [optional]  # noqa: E501
-            id (str): Unique identifier of the object.. [optional]  # noqa: E501
-            href (str): Self link.. [optional]  # noqa: E501
+            id (str): ID of the additional catalog source. [optional]  # noqa: E501
+            enabled (bool): Indicates is this additional catalog source is enabled for the addon. [optional]  # noqa: E501
+            image (str): Image of the additional catalog source.. [optional]  # noqa: E501
+            name (str): Name of the additional catalog source.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/value.py` & `ocm_python_client-1.0.6/ocm_python_client/model/gcp_volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class Value(ModelNormal):
+class GCPVolume(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -78,37 +78,35 @@
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
-            'unit': (str,),  # noqa: E501
-            'value': (float,),  # noqa: E501
+            'size': (int,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
-        'unit': 'unit',  # noqa: E501
-        'value': 'value',  # noqa: E501
+        'size': 'size',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Value - a model defined in OpenAPI
+        """GCPVolume - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -133,16 +131,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            unit (str): Name of the unit used to measure the value.. [optional]  # noqa: E501
-            value (float): Numeric value.. [optional]  # noqa: E501
+            size (int): Volume size in Gib.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -187,15 +184,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Value - a model defined in OpenAPI
+        """GCPVolume - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -220,16 +217,15 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            unit (str): Name of the unit used to measure the value.. [optional]  # noqa: E501
-            value (float): Numeric value.. [optional]  # noqa: E501
+            size (int): Volume size in Gib.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/version.py` & `ocm_python_client-1.0.6/ocm_python_client/model/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,15 @@
             'href': (str,),  # noqa: E501
             'rosa_enabled': (bool,),  # noqa: E501
             'available_upgrades': ([str],),  # noqa: E501
             'channel_group': (str,),  # noqa: E501
             'default': (bool,),  # noqa: E501
             'enabled': (bool,),  # noqa: E501
             'end_of_life_timestamp': (datetime,),  # noqa: E501
+            'hypershift_enabled': (bool,),  # noqa: E501
             'raw_id': (str,),  # noqa: E501
             'release_image': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
@@ -106,14 +107,15 @@
         'href': 'href',  # noqa: E501
         'rosa_enabled': 'rosa_enabled',  # noqa: E501
         'available_upgrades': 'available_upgrades',  # noqa: E501
         'channel_group': 'channel_group',  # noqa: E501
         'default': 'default',  # noqa: E501
         'enabled': 'enabled',  # noqa: E501
         'end_of_life_timestamp': 'end_of_life_timestamp',  # noqa: E501
+        'hypershift_enabled': 'hypershift_enabled',  # noqa: E501
         'raw_id': 'raw_id',  # noqa: E501
         'release_image': 'release_image',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
@@ -160,14 +162,15 @@
             href (str): Self link.. [optional]  # noqa: E501
             rosa_enabled (bool): ROSAEnabled indicates whether this version can be used to create ROSA clusters.. [optional]  # noqa: E501
             available_upgrades ([str]): AvailableUpgrades is the list of versions this version can be upgraded to.. [optional]  # noqa: E501
             channel_group (str): ChannelGroup is the name of the group where this image belongs. ChannelGroup is a mechanism to partition the images to different groups, each image belongs to only a single group.. [optional]  # noqa: E501
             default (bool): Indicates if this should be selected as the default version when a cluster is created without specifying explicitly the version.. [optional]  # noqa: E501
             enabled (bool): Indicates if this version can be used to create clusters.. [optional]  # noqa: E501
             end_of_life_timestamp (datetime): EndOfLifeTimestamp is the date and time when the version will get to End of Life, using the format defined in https://www.ietf.org/rfc/rfc3339.txt[RC3339].. [optional]  # noqa: E501
+            hypershift_enabled (bool): HypershiftEnabled indicates whether this version can be used to create Hypershift clusters.. [optional]  # noqa: E501
             raw_id (str): RawID is the id of the version - without channel group and prefix.. [optional]  # noqa: E501
             release_image (str): ReleaseImage contains the URI of Openshift release image. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
@@ -256,14 +259,15 @@
             href (str): Self link.. [optional]  # noqa: E501
             rosa_enabled (bool): ROSAEnabled indicates whether this version can be used to create ROSA clusters.. [optional]  # noqa: E501
             available_upgrades ([str]): AvailableUpgrades is the list of versions this version can be upgraded to.. [optional]  # noqa: E501
             channel_group (str): ChannelGroup is the name of the group where this image belongs. ChannelGroup is a mechanism to partition the images to different groups, each image belongs to only a single group.. [optional]  # noqa: E501
             default (bool): Indicates if this should be selected as the default version when a cluster is created without specifying explicitly the version.. [optional]  # noqa: E501
             enabled (bool): Indicates if this version can be used to create clusters.. [optional]  # noqa: E501
             end_of_life_timestamp (datetime): EndOfLifeTimestamp is the date and time when the version will get to End of Life, using the format defined in https://www.ietf.org/rfc/rfc3339.txt[RC3339].. [optional]  # noqa: E501
+            hypershift_enabled (bool): HypershiftEnabled indicates whether this version can be used to create Hypershift clusters.. [optional]  # noqa: E501
             raw_id (str): RawID is the id of the version - without channel group and prefix.. [optional]  # noqa: E501
             release_image (str): ReleaseImage contains the URI of Openshift release image. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/version_gate.py` & `ocm_python_client-1.0.6/ocm_python_client/model/addon_upgrade_policy.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from ocm_python_client.exceptions import ApiAttributeError
 
 
 
-class VersionGate(ModelNormal):
+class AddonUpgradePolicy(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -81,52 +81,50 @@
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         return {
             'kind': (str,),  # noqa: E501
             'id': (str,),  # noqa: E501
             'href': (str,),  # noqa: E501
-            'sts_only': (bool,),  # noqa: E501
-            'creation_timestamp': (datetime,),  # noqa: E501
-            'description': (str,),  # noqa: E501
-            'documentation_url': (str,),  # noqa: E501
-            'label': (str,),  # noqa: E501
-            'value': (str,),  # noqa: E501
-            'version_raw_id_prefix': (str,),  # noqa: E501
-            'warning_message': (str,),  # noqa: E501
+            'addon_id': (str,),  # noqa: E501
+            'cluster_id': (str,),  # noqa: E501
+            'next_run': (datetime,),  # noqa: E501
+            'schedule': (str,),  # noqa: E501
+            'schedule_type': (str,),  # noqa: E501
+            'upgrade_type': (str,),  # noqa: E501
+            'version': (str,),  # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
     attribute_map = {
         'kind': 'kind',  # noqa: E501
         'id': 'id',  # noqa: E501
         'href': 'href',  # noqa: E501
-        'sts_only': 'sts_only',  # noqa: E501
-        'creation_timestamp': 'creation_timestamp',  # noqa: E501
-        'description': 'description',  # noqa: E501
-        'documentation_url': 'documentation_url',  # noqa: E501
-        'label': 'label',  # noqa: E501
-        'value': 'value',  # noqa: E501
-        'version_raw_id_prefix': 'version_raw_id_prefix',  # noqa: E501
-        'warning_message': 'warning_message',  # noqa: E501
+        'addon_id': 'addon_id',  # noqa: E501
+        'cluster_id': 'cluster_id',  # noqa: E501
+        'next_run': 'next_run',  # noqa: E501
+        'schedule': 'schedule',  # noqa: E501
+        'schedule_type': 'schedule_type',  # noqa: E501
+        'upgrade_type': 'upgrade_type',  # noqa: E501
+        'version': 'version',  # noqa: E501
     }
 
     read_only_vars = {
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """VersionGate - a model defined in OpenAPI
+        """AddonUpgradePolicy - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -151,25 +149,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kind (str): Indicates the type of this object. Will be 'VersionGate' if this is a complete object or 'VersionGateLink' if it is just a link.. [optional]  # noqa: E501
+            kind (str): Indicates the type of this object. Will be 'AddonUpgradePolicy' if this is a complete object or 'AddonUpgradePolicyLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
-            sts_only (bool): STSOnly indicates if this version gate is for STS clusters only. [optional]  # noqa: E501
-            creation_timestamp (datetime): CreationTimestamp is the date and time when the version gate was created, format defined in https://www.ietf.org/rfc/rfc3339.txt[RC3339].. [optional]  # noqa: E501
-            description (str): Description of the version gate.. [optional]  # noqa: E501
-            documentation_url (str): DocumentationURL is the URL for the documentation of the version gate.. [optional]  # noqa: E501
-            label (str): Label representing the version gate in OpenShift.. [optional]  # noqa: E501
-            value (str): Value represents the required value of the label.. [optional]  # noqa: E501
-            version_raw_id_prefix (str): VersionRawIDPrefix represents the versions prefix that the gate applies to.. [optional]  # noqa: E501
-            warning_message (str): WarningMessage is a warning that will be displayed to the user before they acknowledge the gate. [optional]  # noqa: E501
+            addon_id (str): Addon ID this upgrade policy is defined for. [optional]  # noqa: E501
+            cluster_id (str): Cluster ID this upgrade policy is defined for.. [optional]  # noqa: E501
+            next_run (datetime): Next time the upgrade should run.. [optional]  # noqa: E501
+            schedule (str): Schedule cron expression that defines automatic upgrade scheduling.. [optional]  # noqa: E501
+            schedule_type (str): Schedule type can be either \"manual\" (single execution) or \"automatic\" (re-occurring).. [optional]  # noqa: E501
+            upgrade_type (str): Upgrade type specify the type of the upgrade. Must be \"ADDON\".. [optional]  # noqa: E501
+            version (str): Version is the desired upgrade version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', True)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
@@ -214,15 +211,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """VersionGate - a model defined in OpenAPI
+        """AddonUpgradePolicy - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -247,25 +244,24 @@
                                 petType and we pass in "Dog", and the class Dog
                                 allOf includes Animal, we move through Animal
                                 once using the discriminator, and pick Dog.
                                 Then in Dog, we will make an instance of the
                                 Animal class but this time we won't travel
                                 through its discriminator because we passed in
                                 _visited_composed_classes = (Animal,)
-            kind (str): Indicates the type of this object. Will be 'VersionGate' if this is a complete object or 'VersionGateLink' if it is just a link.. [optional]  # noqa: E501
+            kind (str): Indicates the type of this object. Will be 'AddonUpgradePolicy' if this is a complete object or 'AddonUpgradePolicyLink' if it is just a link.. [optional]  # noqa: E501
             id (str): Unique identifier of the object.. [optional]  # noqa: E501
             href (str): Self link.. [optional]  # noqa: E501
-            sts_only (bool): STSOnly indicates if this version gate is for STS clusters only. [optional]  # noqa: E501
-            creation_timestamp (datetime): CreationTimestamp is the date and time when the version gate was created, format defined in https://www.ietf.org/rfc/rfc3339.txt[RC3339].. [optional]  # noqa: E501
-            description (str): Description of the version gate.. [optional]  # noqa: E501
-            documentation_url (str): DocumentationURL is the URL for the documentation of the version gate.. [optional]  # noqa: E501
-            label (str): Label representing the version gate in OpenShift.. [optional]  # noqa: E501
-            value (str): Value represents the required value of the label.. [optional]  # noqa: E501
-            version_raw_id_prefix (str): VersionRawIDPrefix represents the versions prefix that the gate applies to.. [optional]  # noqa: E501
-            warning_message (str): WarningMessage is a warning that will be displayed to the user before they acknowledge the gate. [optional]  # noqa: E501
+            addon_id (str): Addon ID this upgrade policy is defined for. [optional]  # noqa: E501
+            cluster_id (str): Cluster ID this upgrade policy is defined for.. [optional]  # noqa: E501
+            next_run (datetime): Next time the upgrade should run.. [optional]  # noqa: E501
+            schedule (str): Schedule cron expression that defines automatic upgrade scheduling.. [optional]  # noqa: E501
+            schedule_type (str): Schedule type can be either \"manual\" (single execution) or \"automatic\" (re-occurring).. [optional]  # noqa: E501
+            upgrade_type (str): Upgrade type specify the type of the upgrade. Must be \"ADDON\".. [optional]  # noqa: E501
+            version (str): Version is the desired upgrade version.. [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model/version_gate_agreement.py` & `ocm_python_client-1.0.6/ocm_python_client/model/version_gate_agreement.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/model_utils.py` & `ocm_python_client-1.0.6/ocm_python_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client/models/__init__.py` & `ocm_python_client-1.0.6/ocm_python_client/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,37 @@
 from ocm_python_client.model.aws import AWS
 from ocm_python_client.model.aws_flavour import AWSFlavour
 from ocm_python_client.model.aws_infrastructure_access_role import AWSInfrastructureAccessRole
 from ocm_python_client.model.aws_infrastructure_access_role_grant import AWSInfrastructureAccessRoleGrant
 from ocm_python_client.model.aws_infrastructure_access_role_grant_state import AWSInfrastructureAccessRoleGrantState
 from ocm_python_client.model.aws_infrastructure_access_role_state import AWSInfrastructureAccessRoleState
 from ocm_python_client.model.aws_machine_pool import AWSMachinePool
+from ocm_python_client.model.aws_node_pool import AWSNodePool
 from ocm_python_client.model.awssts_policy import AWSSTSPolicy
 from ocm_python_client.model.aws_spot_market_options import AWSSpotMarketOptions
 from ocm_python_client.model.aws_volume import AWSVolume
 from ocm_python_client.model.add_on import AddOn
 from ocm_python_client.model.add_on_config import AddOnConfig
 from ocm_python_client.model.add_on_environment_variable import AddOnEnvironmentVariable
 from ocm_python_client.model.add_on_install_mode import AddOnInstallMode
 from ocm_python_client.model.add_on_installation import AddOnInstallation
+from ocm_python_client.model.add_on_installation_billing import AddOnInstallationBilling
 from ocm_python_client.model.add_on_installation_parameter import AddOnInstallationParameter
 from ocm_python_client.model.add_on_installation_state import AddOnInstallationState
+from ocm_python_client.model.add_on_namespace import AddOnNamespace
 from ocm_python_client.model.add_on_parameter import AddOnParameter
 from ocm_python_client.model.add_on_parameter_option import AddOnParameterOption
 from ocm_python_client.model.add_on_requirement import AddOnRequirement
 from ocm_python_client.model.add_on_requirement_status import AddOnRequirementStatus
+from ocm_python_client.model.add_on_secret_propagation import AddOnSecretPropagation
 from ocm_python_client.model.add_on_sub_operator import AddOnSubOperator
 from ocm_python_client.model.add_on_version import AddOnVersion
+from ocm_python_client.model.additional_catalog_source import AdditionalCatalogSource
+from ocm_python_client.model.addon_upgrade_policy import AddonUpgradePolicy
+from ocm_python_client.model.addon_upgrade_policy_state import AddonUpgradePolicyState
 from ocm_python_client.model.admin_credentials import AdminCredentials
 from ocm_python_client.model.alert_info import AlertInfo
 from ocm_python_client.model.alert_severity import AlertSeverity
 from ocm_python_client.model.alerts_info import AlertsInfo
 from ocm_python_client.model.api_clusters_mgmt_v1_addons_addon_id_versions_get200_response import ApiClustersMgmtV1AddonsAddonIdVersionsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_addons_get200_response import ApiClustersMgmtV1AddonsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_infrastructure_access_roles_get200_response import ApiClustersMgmtV1AwsInfrastructureAccessRolesGet200Response
@@ -43,42 +50,49 @@
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_regions_post200_response import ApiClustersMgmtV1AwsInquiriesRegionsPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_sts_credential_requests_get200_response import ApiClustersMgmtV1AwsInquiriesStsCredentialRequestsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_sts_policies_get200_response import ApiClustersMgmtV1AwsInquiriesStsPoliciesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_aws_inquiries_vpcs_post200_response import ApiClustersMgmtV1AwsInquiriesVpcsPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post200_response import ApiClustersMgmtV1CloudProvidersCloudProviderIdAvailableRegionsPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get200_response import ApiClustersMgmtV1CloudProvidersCloudProviderIdRegionsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_cloud_providers_get200_response import ApiClustersMgmtV1CloudProvidersGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get200_response import ApiClustersMgmtV1ClustersClusterIdAddonUpgradePoliciesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_addons_get200_response import ApiClustersMgmtV1ClustersClusterIdAddonsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get200_response import ApiClustersMgmtV1ClustersClusterIdAwsInfrastructureAccessRoleGrantsGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get200_response import ApiClustersMgmtV1ClustersClusterIdAwsPrivateLinkConfigurationPrincipalsGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get200_response import ApiClustersMgmtV1ClustersClusterIdControlPlaneUpgradePoliciesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get200_response import ApiClustersMgmtV1ClustersClusterIdExternalConfigurationLabelsGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get200_response import ApiClustersMgmtV1ClustersClusterIdExternalConfigurationManifestsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get200_response import ApiClustersMgmtV1ClustersClusterIdExternalConfigurationSyncsetsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get200_response import ApiClustersMgmtV1ClustersClusterIdGateAgreementsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_groups_get200_response import ApiClustersMgmtV1ClustersClusterIdGroupsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get200_response import ApiClustersMgmtV1ClustersClusterIdGroupsGroupIdUsersGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get200_response import ApiClustersMgmtV1ClustersClusterIdIdentityProvidersGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get200_response import ApiClustersMgmtV1ClustersClusterIdIdentityProvidersIdentityProviderIdHtpasswdUsersGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post200_response import ApiClustersMgmtV1ClustersClusterIdIdentityProvidersIdentityProviderIdHtpasswdUsersImportPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request import ApiClustersMgmtV1ClustersClusterIdIdentityProvidersIdentityProviderIdHtpasswdUsersImportPostRequest
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get200_response import ApiClustersMgmtV1ClustersClusterIdIngressesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get200_response import ApiClustersMgmtV1ClustersClusterIdLimitedSupportReasonsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_logs_get200_response import ApiClustersMgmtV1ClustersClusterIdLogsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get200_response import ApiClustersMgmtV1ClustersClusterIdMachinePoolsGet200Response
+from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get200_response import ApiClustersMgmtV1ClustersClusterIdNodePoolsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get200_response import ApiClustersMgmtV1ClustersClusterIdStsOperatorRolesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get200_response import ApiClustersMgmtV1ClustersClusterIdUpgradePoliciesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_clusters_get200_response import ApiClustersMgmtV1ClustersGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_flavours_get200_response import ApiClustersMgmtV1FlavoursGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_gcp_inquiries_encryption_keys_post200_response import ApiClustersMgmtV1GcpInquiriesEncryptionKeysPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_gcp_inquiries_key_rings_post200_response import ApiClustersMgmtV1GcpInquiriesKeyRingsPost200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_limited_support_reason_templates_get200_response import ApiClustersMgmtV1LimitedSupportReasonTemplatesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_machine_types_get200_response import ApiClustersMgmtV1MachineTypesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_products_get200_response import ApiClustersMgmtV1ProductsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_provision_shards_get200_response import ApiClustersMgmtV1ProvisionShardsGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_version_gates_get200_response import ApiClustersMgmtV1VersionGatesGet200Response
 from ocm_python_client.model.api_clusters_mgmt_v1_versions_get200_response import ApiClustersMgmtV1VersionsGet200Response
+from ocm_python_client.model.aws_etcd_encryption import AwsEtcdEncryption
 from ocm_python_client.model.billing_model import BillingModel
+from ocm_python_client.model.byo_oidc import ByoOidc
 from ocm_python_client.model.ccs import CCS
 from ocm_python_client.model.cpu_total_node_role_os_metric_node import CPUTotalNodeRoleOSMetricNode
 from ocm_python_client.model.cpu_totals_node_role_os_metric_node import CPUTotalsNodeRoleOSMetricNode
 from ocm_python_client.model.cloud_provider import CloudProvider
 from ocm_python_client.model.cloud_provider_data import CloudProviderData
 from ocm_python_client.model.cloud_region import CloudRegion
 from ocm_python_client.model.cloud_vpc import CloudVPC
@@ -93,34 +107,38 @@
 from ocm_python_client.model.cluster_operator_info import ClusterOperatorInfo
 from ocm_python_client.model.cluster_operator_state import ClusterOperatorState
 from ocm_python_client.model.cluster_operators_info import ClusterOperatorsInfo
 from ocm_python_client.model.cluster_registration import ClusterRegistration
 from ocm_python_client.model.cluster_resources import ClusterResources
 from ocm_python_client.model.cluster_state import ClusterState
 from ocm_python_client.model.cluster_status import ClusterStatus
+from ocm_python_client.model.control_plane_upgrade_policy import ControlPlaneUpgradePolicy
 from ocm_python_client.model.credential_request import CredentialRequest
 from ocm_python_client.model.dns import DNS
 from ocm_python_client.model.detection_type import DetectionType
 from ocm_python_client.model.encryption_key import EncryptionKey
 from ocm_python_client.model.environment import Environment
 from ocm_python_client.model.error import Error
 from ocm_python_client.model.event import Event
 from ocm_python_client.model.external_configuration import ExternalConfiguration
 from ocm_python_client.model.flavour import Flavour
 from ocm_python_client.model.flavour_nodes import FlavourNodes
 from ocm_python_client.model.gcp import GCP
+from ocm_python_client.model.gcp_encryption_key import GCPEncryptionKey
 from ocm_python_client.model.gcp_flavour import GCPFlavour
 from ocm_python_client.model.gcp_network import GCPNetwork
+from ocm_python_client.model.gcp_volume import GCPVolume
 from ocm_python_client.model.github_identity_provider import GithubIdentityProvider
 from ocm_python_client.model.gitlab_identity_provider import GitlabIdentityProvider
 from ocm_python_client.model.google_identity_provider import GoogleIdentityProvider
 from ocm_python_client.model.group import Group
 from ocm_python_client.model.ht_passwd_identity_provider import HTPasswdIdentityProvider
 from ocm_python_client.model.ht_passwd_user import HTPasswdUser
-from ocm_python_client.model.hyper_shift import HyperShift
+from ocm_python_client.model.hypershift import Hypershift
+from ocm_python_client.model.hypershift_config import HypershiftConfig
 from ocm_python_client.model.identity_provider import IdentityProvider
 from ocm_python_client.model.identity_provider_mapping_method import IdentityProviderMappingMethod
 from ocm_python_client.model.identity_provider_type import IdentityProviderType
 from ocm_python_client.model.inflight_check import InflightCheck
 from ocm_python_client.model.inflight_check_state import InflightCheckState
 from ocm_python_client.model.ingress import Ingress
 from ocm_python_client.model.instance_iam_roles import InstanceIAMRoles
@@ -135,22 +153,30 @@
 from ocm_python_client.model.machine_pool import MachinePool
 from ocm_python_client.model.machine_pool_autoscaling import MachinePoolAutoscaling
 from ocm_python_client.model.machine_pool_security_group_filter import MachinePoolSecurityGroupFilter
 from ocm_python_client.model.machine_type import MachineType
 from ocm_python_client.model.machine_type_category import MachineTypeCategory
 from ocm_python_client.model.machine_type_size import MachineTypeSize
 from ocm_python_client.model.managed_service import ManagedService
+from ocm_python_client.model.manifest import Manifest
 from ocm_python_client.model.metadata import Metadata
 from ocm_python_client.model.network import Network
 from ocm_python_client.model.node_info import NodeInfo
+from ocm_python_client.model.node_pool import NodePool
+from ocm_python_client.model.node_pool_autoscaling import NodePoolAutoscaling
+from ocm_python_client.model.node_pool_status import NodePoolStatus
 from ocm_python_client.model.node_type import NodeType
 from ocm_python_client.model.nodes_info import NodesInfo
 from ocm_python_client.model.open_id_claims import OpenIDClaims
 from ocm_python_client.model.open_id_identity_provider import OpenIDIdentityProvider
 from ocm_python_client.model.operator_iam_role import OperatorIAMRole
+from ocm_python_client.model.private_link_cluster_configuration import PrivateLinkClusterConfiguration
+from ocm_python_client.model.private_link_configuration import PrivateLinkConfiguration
+from ocm_python_client.model.private_link_principal import PrivateLinkPrincipal
+from ocm_python_client.model.private_link_principals import PrivateLinkPrincipals
 from ocm_python_client.model.product import Product
 from ocm_python_client.model.provision_shard import ProvisionShard
 from ocm_python_client.model.proxy import Proxy
 from ocm_python_client.model.ssh_credentials import SSHCredentials
 from ocm_python_client.model.sts import STS
 from ocm_python_client.model.sts_credential_request import STSCredentialRequest
 from ocm_python_client.model.sts_operator import STSOperator
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client/rest.py` & `ocm_python_client-1.0.6/ocm_python_client/rest.py`

 * *Files identical despite different names*

### Comparing `ocm_python_client-1.0.5/ocm_python_client.egg-info/PKG-INFO` & `ocm_python_client-1.0.6/ocm_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: ocm-python-client
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python client for https://api.openshift.com/api/ APIs
 Home-page: https://github.com/RedHatQE/openshift-cluster-management-python-client
-Download-URL: https://github.com/RedHatQE/openshift-cluster-management-python-client/archive/refs/tags/v1.0.5.tar.gz
+Download-URL: https://github.com/RedHatQE/openshift-cluster-management-python-client/archive/refs/tags/v1.0.6.tar.gz
 Author: Ruth Netser
 Author-email: rnetser@redhat.com
 License: apache-2.0
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-cluster-management-python-client/tree/main/docs
 Keywords: Openshift,ocm
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `ocm_python_client-1.0.5/ocm_python_client.egg-info/SOURCES.txt` & `ocm_python_client-1.0.6/ocm_python_client.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,22 +19,28 @@
 ocm_python_client/apis/__init__.py
 ocm_python_client/model/__init__.py
 ocm_python_client/model/add_on.py
 ocm_python_client/model/add_on_config.py
 ocm_python_client/model/add_on_environment_variable.py
 ocm_python_client/model/add_on_install_mode.py
 ocm_python_client/model/add_on_installation.py
+ocm_python_client/model/add_on_installation_billing.py
 ocm_python_client/model/add_on_installation_parameter.py
 ocm_python_client/model/add_on_installation_state.py
+ocm_python_client/model/add_on_namespace.py
 ocm_python_client/model/add_on_parameter.py
 ocm_python_client/model/add_on_parameter_option.py
 ocm_python_client/model/add_on_requirement.py
 ocm_python_client/model/add_on_requirement_status.py
+ocm_python_client/model/add_on_secret_propagation.py
 ocm_python_client/model/add_on_sub_operator.py
 ocm_python_client/model/add_on_version.py
+ocm_python_client/model/additional_catalog_source.py
+ocm_python_client/model/addon_upgrade_policy.py
+ocm_python_client/model/addon_upgrade_policy_state.py
 ocm_python_client/model/admin_credentials.py
 ocm_python_client/model/alert_info.py
 ocm_python_client/model/alert_severity.py
 ocm_python_client/model/alerts_info.py
 ocm_python_client/model/api_clusters_mgmt_v1_addons_addon_id_versions_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_addons_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_aws_infrastructure_access_roles_get200_response.py
@@ -42,52 +48,60 @@
 ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_regions_post200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_credential_requests_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_policies_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_vpcs_post200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_get200_response.py
+ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addons_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get200_response.py
+ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get200_response.py
+ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get200_response.py
+ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_logs_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get200_response.py
+ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_clusters_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_flavours_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_encryption_keys_post200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_key_rings_post200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_limited_support_reason_templates_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_machine_types_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_products_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_provision_shards_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_version_gates_get200_response.py
 ocm_python_client/model/api_clusters_mgmt_v1_versions_get200_response.py
 ocm_python_client/model/aws.py
+ocm_python_client/model/aws_etcd_encryption.py
 ocm_python_client/model/aws_flavour.py
 ocm_python_client/model/aws_infrastructure_access_role.py
 ocm_python_client/model/aws_infrastructure_access_role_grant.py
 ocm_python_client/model/aws_infrastructure_access_role_grant_state.py
 ocm_python_client/model/aws_infrastructure_access_role_state.py
 ocm_python_client/model/aws_machine_pool.py
+ocm_python_client/model/aws_node_pool.py
 ocm_python_client/model/aws_spot_market_options.py
 ocm_python_client/model/aws_volume.py
 ocm_python_client/model/awssts_policy.py
 ocm_python_client/model/billing_model.py
+ocm_python_client/model/byo_oidc.py
 ocm_python_client/model/ccs.py
 ocm_python_client/model/cloud_provider.py
 ocm_python_client/model/cloud_provider_data.py
 ocm_python_client/model/cloud_region.py
 ocm_python_client/model/cloud_vpc.py
 ocm_python_client/model/cluster.py
 ocm_python_client/model/cluster_api.py
@@ -100,36 +114,40 @@
 ocm_python_client/model/cluster_operator_info.py
 ocm_python_client/model/cluster_operator_state.py
 ocm_python_client/model/cluster_operators_info.py
 ocm_python_client/model/cluster_registration.py
 ocm_python_client/model/cluster_resources.py
 ocm_python_client/model/cluster_state.py
 ocm_python_client/model/cluster_status.py
+ocm_python_client/model/control_plane_upgrade_policy.py
 ocm_python_client/model/cpu_total_node_role_os_metric_node.py
 ocm_python_client/model/cpu_totals_node_role_os_metric_node.py
 ocm_python_client/model/credential_request.py
 ocm_python_client/model/detection_type.py
 ocm_python_client/model/dns.py
 ocm_python_client/model/encryption_key.py
 ocm_python_client/model/environment.py
 ocm_python_client/model/error.py
 ocm_python_client/model/event.py
 ocm_python_client/model/external_configuration.py
 ocm_python_client/model/flavour.py
 ocm_python_client/model/flavour_nodes.py
 ocm_python_client/model/gcp.py
+ocm_python_client/model/gcp_encryption_key.py
 ocm_python_client/model/gcp_flavour.py
 ocm_python_client/model/gcp_network.py
+ocm_python_client/model/gcp_volume.py
 ocm_python_client/model/github_identity_provider.py
 ocm_python_client/model/gitlab_identity_provider.py
 ocm_python_client/model/google_identity_provider.py
 ocm_python_client/model/group.py
 ocm_python_client/model/ht_passwd_identity_provider.py
 ocm_python_client/model/ht_passwd_user.py
-ocm_python_client/model/hyper_shift.py
+ocm_python_client/model/hypershift.py
+ocm_python_client/model/hypershift_config.py
 ocm_python_client/model/identity_provider.py
 ocm_python_client/model/identity_provider_mapping_method.py
 ocm_python_client/model/identity_provider_type.py
 ocm_python_client/model/inflight_check.py
 ocm_python_client/model/inflight_check_state.py
 ocm_python_client/model/ingress.py
 ocm_python_client/model/instance_iam_roles.py
@@ -144,22 +162,30 @@
 ocm_python_client/model/machine_pool.py
 ocm_python_client/model/machine_pool_autoscaling.py
 ocm_python_client/model/machine_pool_security_group_filter.py
 ocm_python_client/model/machine_type.py
 ocm_python_client/model/machine_type_category.py
 ocm_python_client/model/machine_type_size.py
 ocm_python_client/model/managed_service.py
+ocm_python_client/model/manifest.py
 ocm_python_client/model/metadata.py
 ocm_python_client/model/network.py
 ocm_python_client/model/node_info.py
+ocm_python_client/model/node_pool.py
+ocm_python_client/model/node_pool_autoscaling.py
+ocm_python_client/model/node_pool_status.py
 ocm_python_client/model/node_type.py
 ocm_python_client/model/nodes_info.py
 ocm_python_client/model/open_id_claims.py
 ocm_python_client/model/open_id_identity_provider.py
 ocm_python_client/model/operator_iam_role.py
+ocm_python_client/model/private_link_cluster_configuration.py
+ocm_python_client/model/private_link_configuration.py
+ocm_python_client/model/private_link_principal.py
+ocm_python_client/model/private_link_principals.py
 ocm_python_client/model/product.py
 ocm_python_client/model/provision_shard.py
 ocm_python_client/model/proxy.py
 ocm_python_client/model/server_config.py
 ocm_python_client/model/socket_total_node_role_os_metric_node.py
 ocm_python_client/model/socket_totals_node_role_os_metric_node.py
 ocm_python_client/model/ssh_credentials.py
```

### Comparing `ocm_python_client-1.0.5/setup.cfg` & `ocm_python_client-1.0.6/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = openshift-cluster-management-python-client
-version = 1.0.5
+version = 1.0.6
 author = Ruth Netser
 author_email = rnetser@redhat.com
 description = A python client for https://api.openshift.com/api/ APIs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RedHatQE/openshift-cluster-management-python-client
-download_url = https://github.com/RedHatQE/openshift-cluster-management-python-client/archive/refs/tags/v1.0.5.tar.gz
+download_url = https://github.com/RedHatQE/openshift-cluster-management-python-client/archive/refs/tags/v1.0.6.tar.gz
 project_urls = 
 	Documentation = https://github.com/RedHatQE/openshift-cluster-management-python-client/tree/main/docs
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
 
 [egg_info]
```

