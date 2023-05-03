# Comparing `tmp/openshift-cluster-management-python-client-1.0.21.tar.gz` & `tmp/openshift-cluster-management-python-client-1.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-cluster-management-python-client-1.0.21.tar", last modified: Wed May  3 12:36:18 2023, max compression
+gzip compressed data, was "openshift-cluster-management-python-client-1.0.22.tar", last modified: Wed May  3 14:51:21 2023, max compression
```

## Comparing `openshift-cluster-management-python-client-1.0.21.tar` & `openshift-cluster-management-python-client-1.0.22.tar`

### file list

```diff
@@ -1,20 +1,209 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:36:18.034265 openshift-cluster-management-python-client-1.0.21/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/LICENSE
--rw-r--r--   0 root         (0) root         (0)    58148 2023-05-03 12:36:18.034265 openshift-cluster-management-python-client-1.0.21/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    57407 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:36:18.033265 openshift-cluster-management-python-client-1.0.21/ocm_python_client/
--rw-r--r--   0 root         (0) root         (0)      830 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39265 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/api_client.py
--rw-r--r--   0 root         (0) root         (0)    16702 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5138 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    82559 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/model_utils.py
--rw-r--r--   0 root         (0) root         (0)    14345 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/ocm_python_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 12:36:18.034265 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)    58148 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 12:36:18.000000 openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1352 2023-05-03 12:36:15.000000 openshift-cluster-management-python-client-1.0.21/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 12:36:18.034265 openshift-cluster-management-python-client-1.0.21/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 14:51:21.255781 openshift-cluster-management-python-client-1.0.22/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    58148 2023-05-03 14:51:21.255781 openshift-cluster-management-python-client-1.0.22/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    57407 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/README.md
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 14:51:21.242781 openshift-cluster-management-python-client-1.0.22/ocm_python_client/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 14:51:21.243781 openshift-cluster-management-python-client-1.0.22/ocm_python_client/api/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1011822 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/api/default_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 14:51:21.243781 openshift-cluster-management-python-client-1.0.22/ocm_python_client/apis/
+-rw-r--r--   0 root         (0) root         (0)      487 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 14:51:21.255781 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20643 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on.py
+-rw-r--r--   0 root         (0) root         (0)    13404 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_config.py
+-rw-r--r--   0 root         (0) root         (0)    12719 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_environment_variable.py
+-rw-r--r--   0 root         (0) root         (0)    12283 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_install_mode.py
+-rw-r--r--   0 root         (0) root         (0)    16036 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_installation.py
+-rw-r--r--   0 root         (0) root         (0)    13049 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_installation_billing.py
+-rw-r--r--   0 root         (0) root         (0)    12503 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_installation_parameter.py
+-rw-r--r--   0 root         (0) root         (0)    12491 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_installation_state.py
+-rw-r--r--   0 root         (0) root         (0)    13047 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_namespace.py
+-rw-r--r--   0 root         (0) root         (0)    16731 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_parameter.py
+-rw-r--r--   0 root         (0) root         (0)    12743 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_parameter_option.py
+-rw-r--r--   0 root         (0) root         (0)    13071 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_requirement.py
+-rw-r--r--   0 root         (0) root         (0)    11960 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_requirement_status.py
+-rw-r--r--   0 root         (0) root         (0)    12551 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_secret_propagation.py
+-rw-r--r--   0 root         (0) root         (0)    12227 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_sub_operator.py
+-rw-r--r--   0 root         (0) root         (0)    16317 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/add_on_version.py
+-rw-r--r--   0 root         (0) root         (0)    12426 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/additional_catalog_source.py
+-rw-r--r--   0 root         (0) root         (0)    14457 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/addon_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)    12981 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/addon_upgrade_policy_state.py
+-rw-r--r--   0 root         (0) root         (0)    11814 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/admin_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    11993 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/alert_info.py
+-rw-r--r--   0 root         (0) root         (0)    12282 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/alert_severity.py
+-rw-r--r--   0 root         (0) root         (0)    11662 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/alerts_info.py
+-rw-r--r--   0 root         (0) root         (0)    12916 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_addons_addon_id_versions_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12805 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_addons_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13023 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_aws_infrastructure_access_roles_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12916 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_machine_types_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13541 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_regions_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13000 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_credential_requests_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12907 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_sts_policies_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13503 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_aws_inquiries_vpcs_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13631 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_available_regions_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13585 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_cloud_provider_id_regions_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12901 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_cloud_providers_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12840 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addon_upgrade_policies_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12967 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_addons_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13189 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_infrastructure_access_role_grants_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12885 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_aws_private_link_configuration_principals_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12899 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_control_plane_upgrade_policies_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12740 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_labels_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12776 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_manifests_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12764 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_external_configuration_syncsets_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12840 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_gate_agreements_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12677 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12704 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_groups_group_id_users_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12812 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12874 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12891 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12610 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_identity_providers_identity_provider_id_htpasswd_users_import_post_request.py
+-rw-r--r--   0 root         (0) root         (0)    12706 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_ingresses_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12833 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_limited_support_reasons_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12663 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_logs_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12752 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_machine_pools_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12716 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_node_pools_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12955 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_sts_operator_roles_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12777 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_cluster_id_upgrade_policies_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_clusters_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_flavours_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13592 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_encryption_keys_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    13528 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_gcp_inquiries_key_rings_post200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12863 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_limited_support_reason_templates_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12881 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_machine_types_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12826 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_products_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12783 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_provision_shards_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12927 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_version_gates_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    12876 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/api_clusters_mgmt_v1_versions_get200_response.py
+-rw-r--r--   0 root         (0) root         (0)    14709 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws.py
+-rw-r--r--   0 root         (0) root         (0)    11622 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_etcd_encryption.py
+-rw-r--r--   0 root         (0) root         (0)    13404 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_flavour.py
+-rw-r--r--   0 root         (0) root         (0)    13419 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_infrastructure_access_role.py
+-rw-r--r--   0 root         (0) root         (0)    14273 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_infrastructure_access_role_grant.py
+-rw-r--r--   0 root         (0) root         (0)    12502 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_infrastructure_access_role_grant_state.py
+-rw-r--r--   0 root         (0) root         (0)    12307 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_infrastructure_access_role_state.py
+-rw-r--r--   0 root         (0) root         (0)    12700 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_machine_pool.py
+-rw-r--r--   0 root         (0) root         (0)    13400 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_node_pool.py
+-rw-r--r--   0 root         (0) root         (0)    12599 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_spot_market_options.py
+-rw-r--r--   0 root         (0) root         (0)    11733 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/aws_volume.py
+-rw-r--r--   0 root         (0) root         (0)    12196 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/awssts_policy.py
+-rw-r--r--   0 root         (0) root         (0)    12573 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/billing_model.py
+-rw-r--r--   0 root         (0) root         (0)    11957 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/byo_oidc.py
+-rw-r--r--   0 root         (0) root         (0)    12890 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/ccs.py
+-rw-r--r--   0 root         (0) root         (0)    12911 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cloud_provider.py
+-rw-r--r--   0 root         (0) root         (0)    13274 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cloud_provider_data.py
+-rw-r--r--   0 root         (0) root         (0)    14932 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cloud_region.py
+-rw-r--r--   0 root         (0) root         (0)    12568 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cloud_vpc.py
+-rw-r--r--   0 root         (0) root         (0)    31402 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster.py
+-rw-r--r--   0 root         (0) root         (0)    11972 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_api.py
+-rw-r--r--   0 root         (0) root         (0)    12167 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_configuration_mode.py
+-rw-r--r--   0 root         (0) root         (0)    11551 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_console.py
+-rw-r--r--   0 root         (0) root         (0)    13262 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    12668 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_deployment.py
+-rw-r--r--   0 root         (0) root         (0)    12329 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_health_state.py
+-rw-r--r--   0 root         (0) root         (0)    15343 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_nodes.py
+-rw-r--r--   0 root         (0) root         (0)    13020 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_operator_info.py
+-rw-r--r--   0 root         (0) root         (0)    12363 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_operator_state.py
+-rw-r--r--   0 root         (0) root         (0)    11778 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_operators_info.py
+-rw-r--r--   0 root         (0) root         (0)    12687 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_registration.py
+-rw-r--r--   0 root         (0) root         (0)    13164 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_resources.py
+-rw-r--r--   0 root         (0) root         (0)    12927 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_state.py
+-rw-r--r--   0 root         (0) root         (0)    15209 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cluster_status.py
+-rw-r--r--   0 root         (0) root         (0)    15946 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/control_plane_upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)    12492 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cpu_total_node_role_os_metric_node.py
+-rw-r--r--   0 root         (0) root         (0)    11877 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/cpu_totals_node_role_os_metric_node.py
+-rw-r--r--   0 root         (0) root         (0)    12643 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/credential_request.py
+-rw-r--r--   0 root         (0) root         (0)    11980 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/detection_type.py
+-rw-r--r--   0 root         (0) root         (0)    14444 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/dns.py
+-rw-r--r--   0 root         (0) root         (0)    12415 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/encryption_key.py
+-rw-r--r--   0 root         (0) root         (0)    12363 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/environment.py
+-rw-r--r--   0 root         (0) root         (0)    13472 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/error.py
+-rw-r--r--   0 root         (0) root         (0)    12186 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/event.py
+-rw-r--r--   0 root         (0) root         (0)    12656 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/external_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    13903 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/flavour.py
+-rw-r--r--   0 root         (0) root         (0)    11560 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/flavour_nodes.py
+-rw-r--r--   0 root         (0) root         (0)    14027 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/gcp.py
+-rw-r--r--   0 root         (0) root         (0)    12519 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/gcp_encryption_key.py
+-rw-r--r--   0 root         (0) root         (0)    13404 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/gcp_flavour.py
+-rw-r--r--   0 root         (0) root         (0)    12192 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/gcp_network.py
+-rw-r--r--   0 root         (0) root         (0)    11503 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/gcp_volume.py
+-rw-r--r--   0 root         (0) root         (0)    13824 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/github_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12527 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/gitlab_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12261 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/google_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12516 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/group.py
+-rw-r--r--   0 root         (0) root         (0)    12407 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/ht_passwd_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12204 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/ht_passwd_user.py
+-rw-r--r--   0 root         (0) root         (0)    11968 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/hypershift.py
+-rw-r--r--   0 root         (0) root         (0)    12468 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/hypershift_config.py
+-rw-r--r--   0 root         (0) root         (0)    16717 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12512 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/identity_provider_mapping_method.py
+-rw-r--r--   0 root         (0) root         (0)    12989 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/identity_provider_type.py
+-rw-r--r--   0 root         (0) root         (0)    14233 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/inflight_check.py
+-rw-r--r--   0 root         (0) root         (0)    12279 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/inflight_check_state.py
+-rw-r--r--   0 root         (0) root         (0)    13725 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/ingress.py
+-rw-r--r--   0 root         (0) root         (0)    12010 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/instance_iam_roles.py
+-rw-r--r--   0 root         (0) root         (0)    12361 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/key_ring.py
+-rw-r--r--   0 root         (0) root         (0)    12585 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/label.py
+-rw-r--r--   0 root         (0) root         (0)    12539 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/ldap_attributes.py
+-rw-r--r--   0 root         (0) root         (0)    13633 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/ldap_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    14000 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/limited_support_reason.py
+-rw-r--r--   0 root         (0) root         (0)    12796 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/limited_support_reason_template.py
+-rw-r--r--   0 root         (0) root         (0)    12174 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/listening_method.py
+-rw-r--r--   0 root         (0) root         (0)    12344 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/log.py
+-rw-r--r--   0 root         (0) root         (0)    15964 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/machine_pool.py
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/machine_pool_autoscaling.py
+-rw-r--r--   0 root         (0) root         (0)    11707 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/machine_pool_security_group_filter.py
+-rw-r--r--   0 root         (0) root         (0)    15218 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/machine_type.py
+-rw-r--r--   0 root         (0) root         (0)    12520 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/machine_type_category.py
+-rw-r--r--   0 root         (0) root         (0)    12138 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/machine_type_size.py
+-rw-r--r--   0 root         (0) root         (0)    11894 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/managed_service.py
+-rw-r--r--   0 root         (0) root         (0)    12655 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/manifest.py
+-rw-r--r--   0 root         (0) root         (0)    11556 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/metadata.py
+-rw-r--r--   0 root         (0) root         (0)    13120 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/network.py
+-rw-r--r--   0 root         (0) root         (0)    11903 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/node_info.py
+-rw-r--r--   0 root         (0) root         (0)    15956 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/node_pool.py
+-rw-r--r--   0 root         (0) root         (0)    12851 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/node_pool_autoscaling.py
+-rw-r--r--   0 root         (0) root         (0)    12939 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/node_pool_status.py
+-rw-r--r--   0 root         (0) root         (0)    12201 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/node_type.py
+-rw-r--r--   0 root         (0) root         (0)    11647 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/nodes_info.py
+-rw-r--r--   0 root         (0) root         (0)    12525 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/open_id_claims.py
+-rw-r--r--   0 root         (0) root         (0)    13872 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/open_id_identity_provider.py
+-rw-r--r--   0 root         (0) root         (0)    12823 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/operator_iam_role.py
+-rw-r--r--   0 root         (0) root         (0)    11927 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/private_link_cluster_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    11803 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/private_link_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    12551 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/private_link_principal.py
+-rw-r--r--   0 root         (0) root         (0)    12813 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/private_link_principals.py
+-rw-r--r--   0 root         (0) root         (0)    12359 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/product.py
+-rw-r--r--   0 root         (0) root         (0)    16784 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/provision_shard.py
+-rw-r--r--   0 root         (0) root         (0)    12302 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/proxy.py
+-rw-r--r--   0 root         (0) root         (0)    12674 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/server_config.py
+-rw-r--r--   0 root         (0) root         (0)    12522 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/socket_total_node_role_os_metric_node.py
+-rw-r--r--   0 root         (0) root         (0)    11922 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/socket_totals_node_role_os_metric_node.py
+-rw-r--r--   0 root         (0) root         (0)    11849 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/ssh_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    16007 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/sts.py
+-rw-r--r--   0 root         (0) root         (0)    11930 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/sts_credential_request.py
+-rw-r--r--   0 root         (0) root         (0)    12570 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/sts_operator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/subnetwork.py
+-rw-r--r--   0 root         (0) root         (0)    12172 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/subscription.py
+-rw-r--r--   0 root         (0) root         (0)    12646 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/syncset.py
+-rw-r--r--   0 root         (0) root         (0)    12119 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/taint.py
+-rw-r--r--   0 root         (0) root         (0)    14668 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/upgrade_policy.py
+-rw-r--r--   0 root         (0) root         (0)    12946 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/upgrade_policy_state.py
+-rw-r--r--   0 root         (0) root         (0)    12630 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/upgrade_policy_state_value.py
+-rw-r--r--   0 root         (0) root         (0)    12116 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/user.py
+-rw-r--r--   0 root         (0) root         (0)    11760 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/value.py
+-rw-r--r--   0 root         (0) root         (0)    15973 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/version.py
+-rw-r--r--   0 root         (0) root         (0)    15119 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/version_gate.py
+-rw-r--r--   0 root         (0) root         (0)    12987 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/model/version_gate_agreement.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 14:51:21.255781 openshift-cluster-management-python-client-1.0.22/ocm_python_client/models/
+-rw-r--r--   0 root         (0) root         (0)    17685 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/ocm_python_client/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 14:51:21.255781 openshift-cluster-management-python-client-1.0.22/openshift_cluster_management_python_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    58148 2023-05-03 14:51:21.000000 openshift-cluster-management-python-client-1.0.22/openshift_cluster_management_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11198 2023-05-03 14:51:21.000000 openshift-cluster-management-python-client-1.0.22/openshift_cluster_management_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 14:51:21.000000 openshift-cluster-management-python-client-1.0.22/openshift_cluster_management_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-05-03 14:51:21.000000 openshift-cluster-management-python-client-1.0.22/openshift_cluster_management_python_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-03 14:51:21.000000 openshift-cluster-management-python-client-1.0.22/openshift_cluster_management_python_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-05-03 14:51:18.000000 openshift-cluster-management-python-client-1.0.22/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 14:51:21.255781 openshift-cluster-management-python-client-1.0.22/setup.cfg
```

### Comparing `openshift-cluster-management-python-client-1.0.21/LICENSE` & `openshift-cluster-management-python-client-1.0.22/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.21/PKG-INFO` & `openshift-cluster-management-python-client-1.0.22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-client
-Version: 1.0.21
+Version: 1.0.22
 Summary: A python client for https://api.openshift.com/api/ APIs
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-cluster-management-python-client
 Project-URL: Download, https://pypi.org/project/openshift-cluster-management-python-client/
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-cluster-management-python-client/blob/main/README.md
 Keywords: Openshift,OCM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openshift-cluster-management-python-client-1.0.21/README.md` & `openshift-cluster-management-python-client-1.0.22/README.md`

 * *Files identical despite different names*

### Comparing `openshift-cluster-management-python-client-1.0.21/openshift_cluster_management_python_client.egg-info/PKG-INFO` & `openshift-cluster-management-python-client-1.0.22/openshift_cluster_management_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-cluster-management-python-client
-Version: 1.0.21
+Version: 1.0.22
 Summary: A python client for https://api.openshift.com/api/ APIs
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-cluster-management-python-client
 Project-URL: Download, https://pypi.org/project/openshift-cluster-management-python-client/
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-cluster-management-python-client/blob/main/README.md
 Keywords: Openshift,OCM
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openshift-cluster-management-python-client-1.0.21/pyproject.toml` & `openshift-cluster-management-python-client-1.0.22/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -52,8 +52,8 @@
 Download = "https://pypi.org/project/openshift-cluster-management-python-client/"
 Documentation = "https://github.com/RedHatQE/openshift-cluster-management-python-client/blob/main/README.md"
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-include = ["ocm_python_client"]
+include = ["ocm_python_client.*"]
```

