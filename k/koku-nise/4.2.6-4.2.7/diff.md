# Comparing `tmp/koku-nise-4.2.6.tar.gz` & `tmp/koku-nise-4.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koku-nise-4.2.6.tar", last modified: Wed May  3 15:36:52 2023, max compression
+gzip compressed data, was "koku-nise-4.2.7.tar", last modified: Wed May  3 18:29:13 2023, max compression
```

## Comparing `koku-nise-4.2.6.tar` & `koku-nise-4.2.7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.265869 koku-nise-4.2.6/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-05-03 15:36:29.000000 koku-nise-4.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 15:36:29.000000 koku-nise-4.2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 15:36:52.265869 koku-nise-4.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-05-03 15:36:29.000000 koku-nise-4.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.253869 koku-nise-4.2.6/koku_nise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 15:36:51.000000 koku-nise-4.2.6/koku_nise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-03 15:36:52.000000 koku-nise-4.2.6/koku_nise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:36:51.000000 koku-nise-4.2.6/koku_nise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 15:36:51.000000 koku-nise-4.2.6/koku_nise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:36:51.000000 koku-nise-4.2.6/koku_nise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 15:36:51.000000 koku-nise-4.2.6/koku_nise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 15:36:51.000000 koku-nise-4.2.6/koku_nise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.253869 koku-nise-4.2.6/nise/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/aws-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.253869 koku-nise-4.2.6/nise/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.257869 koku-nise-4.2.6/nise/generators/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/aws_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/aws_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/ebs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/ec2_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/marketplace_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/rds_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/route53_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/s3_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/aws/vpc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.257869 koku-nise-4.2.6/nise/generators/azure/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/azure/azure_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/azure/bandwidth_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/azure/ccsp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/azure/sql_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/azure/storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/azure/virtual_machine_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/azure/virtual_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.257869 koku-nise-4.2.6/nise/generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/gcp/cloud_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/gcp/compute_engine_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/gcp/gcp_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/gcp/gcp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/gcp/gcp_network_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/gcp/hcs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/gcp/project_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.257869 koku-nise-4.2.6/nise/generators/oci/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/oci/oci_block_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/oci/oci_compute_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/oci/oci_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/oci/oci_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/oci/oci_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/oci/oci_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.257869 koku-nise-4.2.6/nise/generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39961 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/generators/ocp/ocp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/ocp-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    52710 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.257869 koku-nise-4.2.6/nise/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/util/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.261869 koku-nise-4.2.6/nise/yaml_generators/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.261869 koku-nise-4.2.6/nise/yaml_generators/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71376 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/aws/ec2_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/aws/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/aws/rds_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/aws/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.261869 koku-nise-4.2.6/nise/yaml_generators/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/azure/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.261869 koku-nise-4.2.6/nise/yaml_generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/gcp/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.261869 koku-nise-4.2.6/nise/yaml_generators/oci/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/oci/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/oci/oci_yaml_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.261869 koku-nise-4.2.6/nise/yaml_generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/ocp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.261869 koku-nise-4.2.6/nise/yaml_generators/ocp_on_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/ocp_on_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/ocp_on_cloud/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:36:52.265869 koku-nise-4.2.6/nise/yaml_generators/static/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/aws_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/aws_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/azure_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/azure_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/gcp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/gcp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/oci_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/oci_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/ocp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/ocp_on_cloud_options.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/static/ocp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-03 15:36:29.000000 koku-nise-4.2.6/nise/yaml_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:36:52.265869 koku-nise-4.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-03 15:36:29.000000 koku-nise-4.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.411058 koku-nise-4.2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-05-03 18:28:53.000000 koku-nise-4.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 18:28:53.000000 koku-nise-4.2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 18:29:13.411058 koku-nise-4.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-05-03 18:28:53.000000 koku-nise-4.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.403057 koku-nise-4.2.7/koku_nise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 18:29:13.000000 koku-nise-4.2.7/koku_nise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-03 18:29:13.000000 koku-nise-4.2.7/koku_nise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:29:13.000000 koku-nise-4.2.7/koku_nise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 18:29:13.000000 koku-nise-4.2.7/koku_nise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:29:13.000000 koku-nise-4.2.7/koku_nise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 18:29:13.000000 koku-nise-4.2.7/koku_nise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 18:29:13.000000 koku-nise-4.2.7/koku_nise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.403057 koku-nise-4.2.7/nise/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/aws-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.403057 koku-nise-4.2.7/nise/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.407057 koku-nise-4.2.7/nise/generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/aws_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/aws_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/ebs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/ec2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/marketplace_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/rds_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/route53_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/s3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/aws/vpc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.407057 koku-nise-4.2.7/nise/generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16574 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/azure/azure_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/azure/bandwidth_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/azure/ccsp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/azure/sql_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/azure/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/azure/virtual_machine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/azure/virtual_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.407057 koku-nise-4.2.7/nise/generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/gcp/cloud_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/gcp/compute_engine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/gcp/gcp_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/gcp/gcp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/gcp/gcp_network_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/gcp/hcs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/gcp/project_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.407057 koku-nise-4.2.7/nise/generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/oci/oci_block_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/oci/oci_compute_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/oci/oci_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/oci/oci_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/oci/oci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/oci/oci_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.407057 koku-nise-4.2.7/nise/generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39961 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/generators/ocp/ocp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/ocp-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    52710 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.407057 koku-nise-4.2.7/nise/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.407057 koku-nise-4.2.7/nise/yaml_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.407057 koku-nise-4.2.7/nise/yaml_generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71376 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/aws/ec2_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/aws/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/aws/rds_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/aws/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.411058 koku-nise-4.2.7/nise/yaml_generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/azure/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.411058 koku-nise-4.2.7/nise/yaml_generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/gcp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.411058 koku-nise-4.2.7/nise/yaml_generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/oci/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/oci/oci_yaml_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.411058 koku-nise-4.2.7/nise/yaml_generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/ocp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.411058 koku-nise-4.2.7/nise/yaml_generators/ocp_on_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/ocp_on_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/ocp_on_cloud/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:29:13.411058 koku-nise-4.2.7/nise/yaml_generators/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/aws_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/aws_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/azure_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/azure_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/gcp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/gcp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/oci_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/oci_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/ocp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/ocp_on_cloud_options.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/static/ocp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-03 18:28:53.000000 koku-nise-4.2.7/nise/yaml_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:29:13.411058 koku-nise-4.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-03 18:28:53.000000 koku-nise-4.2.7/setup.py
```

### Comparing `koku-nise-4.2.6/LICENSE` & `koku-nise-4.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/README.md` & `koku-nise-4.2.7/README.md`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/koku_nise.egg-info/SOURCES.txt` & `koku-nise-4.2.7/koku_nise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/__main__.py` & `koku-nise-4.2.7/nise/__main__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/aws-template-manifest.json` & `koku-nise-4.2.7/nise/aws-template-manifest.json`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/copy.py` & `koku-nise-4.2.7/nise/copy.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/extract.py` & `koku-nise-4.2.7/nise/extract.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/__init__.py` & `koku-nise-4.2.7/nise/generators/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/aws_constants.py` & `koku-nise-4.2.7/nise/generators/aws/aws_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/aws_generator.py` & `koku-nise-4.2.7/nise/generators/aws/aws_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/data_transfer_generator.py` & `koku-nise-4.2.7/nise/generators/aws/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/ebs_generator.py` & `koku-nise-4.2.7/nise/generators/aws/ebs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/ec2_generator.py` & `koku-nise-4.2.7/nise/generators/aws/ec2_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/marketplace_generator.py` & `koku-nise-4.2.7/nise/generators/aws/marketplace_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/rds_generator.py` & `koku-nise-4.2.7/nise/generators/aws/rds_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/route53_generator.py` & `koku-nise-4.2.7/nise/generators/aws/route53_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/s3_generator.py` & `koku-nise-4.2.7/nise/generators/aws/s3_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/aws/vpc_generator.py` & `koku-nise-4.2.7/nise/generators/aws/vpc_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/azure/__init__.py` & `koku-nise-4.2.7/nise/generators/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/azure/azure_generator.py` & `koku-nise-4.2.7/nise/generators/azure/azure_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,17 @@
         # row['ProductOrderName'] =
         # row['AvailabilityZone'] =
         # row['Term'] =
         row["PublisherName"] = publisher_name
         # row['PlanName'] =
         # row['PartNumber'] =
         # row['CostCenter'] =
+
+        if hasattr(self, "product_id"):
+            row["ProductId"] = self.product_id
         return row
 
     def _map_header_to_report_version(self, row, meter_sub, amount, rate, cost, instance_id, service_tier):
         if self.azure_columns == AZURE_COLUMNS_V2:
             row["MeterSubCategory"] = meter_sub
             row["Quantity"] = amount
             row["EffectivePrice"] = rate
```

### Comparing `koku-nise-4.2.6/nise/generators/azure/bandwidth_generator.py` & `koku-nise-4.2.7/nise/generators/azure/bandwidth_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/azure/ccsp_generator.py` & `koku-nise-4.2.7/nise/generators/azure/ccsp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/azure/sql_database_generator.py` & `koku-nise-4.2.7/nise/generators/azure/sql_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/azure/storage_generator.py` & `koku-nise-4.2.7/nise/generators/azure/storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/azure/virtual_machine_generator.py` & `koku-nise-4.2.7/nise/generators/azure/virtual_machine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/azure/virtual_network_generator.py` & `koku-nise-4.2.7/nise/generators/azure/virtual_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/gcp/__init__.py` & `koku-nise-4.2.7/nise/generators/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/gcp/cloud_storage_generator.py` & `koku-nise-4.2.7/nise/generators/gcp/cloud_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/gcp/compute_engine_generator.py` & `koku-nise-4.2.7/nise/generators/gcp/compute_engine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/gcp/gcp_database_generator.py` & `koku-nise-4.2.7/nise/generators/gcp/gcp_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/gcp/gcp_generator.py` & `koku-nise-4.2.7/nise/generators/gcp/gcp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/gcp/gcp_network_generator.py` & `koku-nise-4.2.7/nise/generators/gcp/gcp_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/gcp/hcs_generator.py` & `koku-nise-4.2.7/nise/generators/gcp/hcs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/gcp/project_generator.py` & `koku-nise-4.2.7/nise/generators/gcp/project_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/generator.py` & `koku-nise-4.2.7/nise/generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/oci/__init__.py` & `koku-nise-4.2.7/nise/generators/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/oci/oci_block_storage_generator.py` & `koku-nise-4.2.7/nise/generators/oci/oci_block_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/oci/oci_compute_generator.py` & `koku-nise-4.2.7/nise/generators/oci/oci_compute_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/oci/oci_constants.py` & `koku-nise-4.2.7/nise/generators/oci/oci_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/oci/oci_database_generator.py` & `koku-nise-4.2.7/nise/generators/oci/oci_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/oci/oci_generator.py` & `koku-nise-4.2.7/nise/generators/oci/oci_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/oci/oci_network_generator.py` & `koku-nise-4.2.7/nise/generators/oci/oci_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/ocp/__init__.py` & `koku-nise-4.2.7/nise/generators/ocp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/generators/ocp/ocp_generator.py` & `koku-nise-4.2.7/nise/generators/ocp/ocp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/manifest.py` & `koku-nise-4.2.7/nise/manifest.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/report.py` & `koku-nise-4.2.7/nise/report.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/upload.py` & `koku-nise-4.2.7/nise/upload.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/util/__init__.py` & `koku-nise-4.2.7/nise/util/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/util/log.py` & `koku-nise-4.2.7/nise/util/log.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_gen.py` & `koku-nise-4.2.7/nise/yaml_gen.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/aws/ec2_instance_types.py` & `koku-nise-4.2.7/nise/yaml_generators/aws/ec2_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/aws/generator.py` & `koku-nise-4.2.7/nise/yaml_generators/aws/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/aws/rds_instance_types.py` & `koku-nise-4.2.7/nise/yaml_generators/aws/rds_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/aws/regions.py` & `koku-nise-4.2.7/nise/yaml_generators/aws/regions.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/azure/generator.py` & `koku-nise-4.2.7/nise/yaml_generators/azure/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/gcp/generator.py` & `koku-nise-4.2.7/nise/yaml_generators/gcp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/generator.py` & `koku-nise-4.2.7/nise/yaml_generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/oci/generator.py` & `koku-nise-4.2.7/nise/yaml_generators/oci/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/oci/oci_yaml_constants.py` & `koku-nise-4.2.7/nise/yaml_generators/oci/oci_yaml_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/ocp/generator.py` & `koku-nise-4.2.7/nise/yaml_generators/ocp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/ocp_on_cloud/generator.py` & `koku-nise-4.2.7/nise/yaml_generators/ocp_on_cloud/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/aws_generator_config.yml` & `koku-nise-4.2.7/nise/yaml_generators/static/aws_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/aws_static_data.yml.j2` & `koku-nise-4.2.7/nise/yaml_generators/static/aws_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/azure_generator_config.yml` & `koku-nise-4.2.7/nise/yaml_generators/static/azure_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/azure_static_data.yml.j2` & `koku-nise-4.2.7/nise/yaml_generators/static/azure_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/gcp_static_data.yml.j2` & `koku-nise-4.2.7/nise/yaml_generators/static/gcp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/oci_static_data.yml.j2` & `koku-nise-4.2.7/nise/yaml_generators/static/oci_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/ocp_generator_config.yml` & `koku-nise-4.2.7/nise/yaml_generators/static/ocp_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/ocp_on_cloud_options.yml` & `koku-nise-4.2.7/nise/yaml_generators/static/ocp_on_cloud_options.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/static/ocp_static_data.yml.j2` & `koku-nise-4.2.7/nise/yaml_generators/static/ocp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/nise/yaml_generators/utils.py` & `koku-nise-4.2.7/nise/yaml_generators/utils.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.6/setup.py` & `koku-nise-4.2.7/setup.py`

 * *Files identical despite different names*

