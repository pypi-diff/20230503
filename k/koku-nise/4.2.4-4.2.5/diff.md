# Comparing `tmp/koku-nise-4.2.4.tar.gz` & `tmp/koku-nise-4.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koku-nise-4.2.4.tar", last modified: Thu Apr 20 18:41:41 2023, max compression
+gzip compressed data, was "koku-nise-4.2.5.tar", last modified: Wed May  3 13:35:50 2023, max compression
```

## Comparing `koku-nise-4.2.4.tar` & `koku-nise-4.2.5.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-04-20 18:41:18.000000 koku-nise-4.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-20 18:41:18.000000 koku-nise-4.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 18:41:41.721258 koku-nise-4.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-04-20 18:41:18.000000 koku-nise-4.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.713257 koku-nise-4.2.4/koku_nise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-20 18:41:41.000000 koku-nise-4.2.4/koku_nise.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/aws-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/extract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/aws_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/aws_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/data_transfer_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/ebs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/ec2_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/marketplace_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/rds_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/route53_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/s3_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/aws/vpc_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/azure/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/azure_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/bandwidth_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/ccsp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/sql_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/virtual_machine_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/azure/virtual_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/cloud_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/compute_engine_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/gcp_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/gcp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/gcp_network_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/hcs_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/gcp/project_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.717258 koku-nise-4.2.4/nise/generators/oci/
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_block_storage_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_compute_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_database_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/oci/oci_network_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39500 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/generators/ocp/ocp_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/ocp-template-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    52710 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/report.py
--rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/util/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71376 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/ec2_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/rds_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/aws/regions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/azure/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/azure/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/gcp/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/oci/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/oci/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/oci/oci_yaml_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/ocp/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/ocp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/ocp/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/ocp_on_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/ocp_on_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/ocp_on_cloud/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 18:41:41.721258 koku-nise-4.2.4/nise/yaml_generators/static/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/aws_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/aws_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/azure_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/azure_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/gcp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/gcp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/oci_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/oci_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/ocp_generator_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/ocp_on_cloud_options.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/static/ocp_static_data.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-04-20 18:41:18.000000 koku-nise-4.2.4/nise/yaml_generators/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 18:41:41.721258 koku-nise-4.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-20 18:41:18.000000 koku-nise-4.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.351198 koku-nise-4.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-05-03 13:35:23.000000 koku-nise-4.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 13:35:23.000000 koku-nise-4.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 13:35:50.351198 koku-nise-4.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9816 2023-05-03 13:35:23.000000 koku-nise-4.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.339198 koku-nise-4.2.5/koku_nise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-03 13:35:50.000000 koku-nise-4.2.5/koku_nise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-03 13:35:50.000000 koku-nise-4.2.5/koku_nise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:35:50.000000 koku-nise-4.2.5/koku_nise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 13:35:50.000000 koku-nise-4.2.5/koku_nise.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:35:50.000000 koku-nise-4.2.5/koku_nise.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 13:35:50.000000 koku-nise-4.2.5/koku_nise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-03 13:35:50.000000 koku-nise-4.2.5/koku_nise.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.343198 koku-nise-4.2.5/nise/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26044 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/aws-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/extract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.343198 koku-nise-4.2.5/nise/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.343198 koku-nise-4.2.5/nise/generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/aws_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/aws_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/data_transfer_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/ebs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/ec2_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/marketplace_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/rds_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/route53_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/s3_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/aws/vpc_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.343198 koku-nise-4.2.5/nise/generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/azure/azure_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/azure/bandwidth_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/azure/ccsp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/azure/sql_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/azure/storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/azure/virtual_machine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/azure/virtual_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.347198 koku-nise-4.2.5/nise/generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/gcp/cloud_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/gcp/compute_engine_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/gcp/gcp_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/gcp/gcp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/gcp/gcp_network_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/gcp/hcs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4384 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/gcp/project_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.347198 koku-nise-4.2.5/nise/generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/oci/oci_block_storage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/oci/oci_compute_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/oci/oci_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/oci/oci_database_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10817 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/oci/oci_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/oci/oci_network_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.347198 koku-nise-4.2.5/nise/generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39548 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/generators/ocp/ocp_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/ocp-template-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    52710 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15635 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.347198 koku-nise-4.2.5/nise/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/util/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7688 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.347198 koku-nise-4.2.5/nise/yaml_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.347198 koku-nise-4.2.5/nise/yaml_generators/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71376 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/aws/ec2_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/aws/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13953 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/aws/rds_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/aws/regions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.351198 koku-nise-4.2.5/nise/yaml_generators/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7923 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/azure/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.351198 koku-nise-4.2.5/nise/yaml_generators/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/gcp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.351198 koku-nise-4.2.5/nise/yaml_generators/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/oci/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/oci/oci_yaml_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.351198 koku-nise-4.2.5/nise/yaml_generators/ocp/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/ocp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/ocp/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.351198 koku-nise-4.2.5/nise/yaml_generators/ocp_on_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/ocp_on_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/ocp_on_cloud/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:35:50.351198 koku-nise-4.2.5/nise/yaml_generators/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/aws_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/aws_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/azure_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/azure_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/gcp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/gcp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/oci_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/oci_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/ocp_generator_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/ocp_on_cloud_options.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/static/ocp_static_data.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     4366 2023-05-03 13:35:23.000000 koku-nise-4.2.5/nise/yaml_generators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 13:35:50.351198 koku-nise-4.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-05-03 13:35:23.000000 koku-nise-4.2.5/setup.py
```

### Comparing `koku-nise-4.2.4/LICENSE` & `koku-nise-4.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/README.md` & `koku-nise-4.2.5/README.md`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/koku_nise.egg-info/SOURCES.txt` & `koku-nise-4.2.5/koku_nise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/__main__.py` & `koku-nise-4.2.5/nise/__main__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/aws-template-manifest.json` & `koku-nise-4.2.5/nise/aws-template-manifest.json`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/copy.py` & `koku-nise-4.2.5/nise/copy.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/extract.py` & `koku-nise-4.2.5/nise/extract.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/__init__.py` & `koku-nise-4.2.5/nise/generators/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/aws_constants.py` & `koku-nise-4.2.5/nise/generators/aws/aws_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/aws_generator.py` & `koku-nise-4.2.5/nise/generators/aws/aws_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/data_transfer_generator.py` & `koku-nise-4.2.5/nise/generators/aws/data_transfer_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/ebs_generator.py` & `koku-nise-4.2.5/nise/generators/aws/ebs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/ec2_generator.py` & `koku-nise-4.2.5/nise/generators/aws/ec2_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/marketplace_generator.py` & `koku-nise-4.2.5/nise/generators/aws/marketplace_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/rds_generator.py` & `koku-nise-4.2.5/nise/generators/aws/rds_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/route53_generator.py` & `koku-nise-4.2.5/nise/generators/aws/route53_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/s3_generator.py` & `koku-nise-4.2.5/nise/generators/aws/s3_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/aws/vpc_generator.py` & `koku-nise-4.2.5/nise/generators/aws/vpc_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/azure/__init__.py` & `koku-nise-4.2.5/nise/generators/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/azure/azure_generator.py` & `koku-nise-4.2.5/nise/generators/azure/azure_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/azure/bandwidth_generator.py` & `koku-nise-4.2.5/nise/generators/azure/bandwidth_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/azure/ccsp_generator.py` & `koku-nise-4.2.5/nise/generators/azure/ccsp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/azure/sql_database_generator.py` & `koku-nise-4.2.5/nise/generators/azure/sql_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/azure/storage_generator.py` & `koku-nise-4.2.5/nise/generators/azure/storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/azure/virtual_machine_generator.py` & `koku-nise-4.2.5/nise/generators/azure/virtual_machine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/azure/virtual_network_generator.py` & `koku-nise-4.2.5/nise/generators/azure/virtual_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/gcp/__init__.py` & `koku-nise-4.2.5/nise/generators/gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/gcp/cloud_storage_generator.py` & `koku-nise-4.2.5/nise/generators/gcp/cloud_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/gcp/compute_engine_generator.py` & `koku-nise-4.2.5/nise/generators/gcp/compute_engine_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/gcp/gcp_database_generator.py` & `koku-nise-4.2.5/nise/generators/gcp/gcp_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/gcp/gcp_generator.py` & `koku-nise-4.2.5/nise/generators/gcp/gcp_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/gcp/gcp_network_generator.py` & `koku-nise-4.2.5/nise/generators/gcp/gcp_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/gcp/hcs_generator.py` & `koku-nise-4.2.5/nise/generators/gcp/hcs_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/gcp/project_generator.py` & `koku-nise-4.2.5/nise/generators/gcp/project_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/generator.py` & `koku-nise-4.2.5/nise/generators/generator.py`

 * *Files 21% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """Defines a abstract class for generators."""
 
     def __init__(self, start_date, end_date):
         """Initialize the generator."""
         self.start_date = start_date
         self.end_date = end_date
         self.hours = self._set_hours()
+        self.quarter_hours = self._set_quarter_hours()
         self.days = self._set_days()
         self.fake = Faker()
         super().__init__()
 
     def _set_hours(self):
         """Create a list of hours between the start and end dates for hourly aws data."""
         hours = []
@@ -52,14 +53,35 @@
         cur_date = self.start_date
         while (cur_date + one_hour) <= self.end_date:
             cur_hours = {"start": cur_date, "end": cur_date + one_hour}
             hours.append(cur_hours)
             cur_date = cur_date + one_hour
         return hours
 
+    def _set_quarter_hours(self):
+        """Create a list of times between the start and end dates for 15 min intervals data."""
+        quarter_hours = []
+        if not self.start_date or not self.end_date:
+            raise ValueError("start_date and end_date must be date objects.")
+        if not isinstance(self.start_date, datetime.datetime):
+            raise ValueError("start_date must be a date object.")
+        if not isinstance(self.end_date, datetime.datetime):
+            raise ValueError("end_date must be a date object.")
+        if self.end_date < self.start_date:
+            raise ValueError("start_date must be a date object less than end_date.")
+
+        one_quarter_hour = datetime.timedelta(minutes=15)
+        one_second = datetime.timedelta(seconds=1)
+        cur_date = self.start_date
+        while (cur_date + one_quarter_hour) <= self.end_date:
+            cur_quarter_hours = {"start": cur_date + one_second, "end": cur_date + one_quarter_hour}
+            quarter_hours.append(cur_quarter_hours)
+            cur_date = cur_date + one_quarter_hour
+        return quarter_hours
+
     def _set_days(self):
         """Create a list of days between the start and end dates for daily azure data."""
         days = []
         if not self.start_date or not self.end_date:
             raise ValueError("start_date and end_date must be date objects.")
         if not isinstance(self.start_date, datetime.datetime):
             raise ValueError("start_date must be a date object.")
```

### Comparing `koku-nise-4.2.4/nise/generators/oci/__init__.py` & `koku-nise-4.2.5/nise/generators/oci/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/oci/oci_block_storage_generator.py` & `koku-nise-4.2.5/nise/generators/oci/oci_block_storage_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/oci/oci_compute_generator.py` & `koku-nise-4.2.5/nise/generators/oci/oci_compute_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/oci/oci_constants.py` & `koku-nise-4.2.5/nise/generators/oci/oci_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/oci/oci_database_generator.py` & `koku-nise-4.2.5/nise/generators/oci/oci_database_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/oci/oci_generator.py` & `koku-nise-4.2.5/nise/generators/oci/oci_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/oci/oci_network_generator.py` & `koku-nise-4.2.5/nise/generators/oci/oci_network_generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/ocp/__init__.py` & `koku-nise-4.2.5/nise/generators/ocp/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/generators/ocp/ocp_generator.py` & `koku-nise-4.2.5/nise/generators/ocp/ocp_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
             },
         }
 
         if self.ros_ocp_info:
             self.ocp_report_generation.update(
                 {
                     OCP_ROS_USAGE: {
-                        "_generate_hourly_data": self._gen_hourly_ros_ocp_pods_usage,
+                        "_generate_hourly_data": self._gen_quarter_hourly_ros_ocp_pods_usage,
                         "_update_data": self._update_ros_ocp_pod_data,
                     }
                 }
             )
 
     @staticmethod
     def timestamp(in_date):
@@ -753,19 +753,19 @@
                 for pod_choice in pod_choices:
                     pod_name = pod_keys[pod_choice]
                     pod = deepcopy(self.pods[pod_name])
                     row = self._init_data_row(start, end, **kwargs)
                     row = self._update_data(row, start, end, pod=pod, **kwargs)
                     yield row
 
-    def _gen_hourly_ros_ocp_pods_usage(self, **kwargs):
+    def _gen_quarter_hourly_ros_ocp_pods_usage(self, **kwargs):
         """Create hourly data for pod usage."""
-        for hour in self.hours:
-            start = hour.get("start")
-            end = hour.get("end")
+        for quarter_hour in self.quarter_hours:
+            start = quarter_hour.get("start")
+            end = quarter_hour.get("end")
             if self._nodes:
                 for pod_name, _ in self.pods.items():
                     pod = deepcopy(self.ros_data[pod_name])
                     row = self._init_data_row(start, end, **kwargs)
                     yield self._update_data(row, start, end, pod=pod, **kwargs)
             else:
                 pod_count = len(self.pods)
```

### Comparing `koku-nise-4.2.4/nise/manifest.py` & `koku-nise-4.2.5/nise/manifest.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/report.py` & `koku-nise-4.2.5/nise/report.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/upload.py` & `koku-nise-4.2.5/nise/upload.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/util/__init__.py` & `koku-nise-4.2.5/nise/util/__init__.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/util/log.py` & `koku-nise-4.2.5/nise/util/log.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_gen.py` & `koku-nise-4.2.5/nise/yaml_gen.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/aws/ec2_instance_types.py` & `koku-nise-4.2.5/nise/yaml_generators/aws/ec2_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/aws/generator.py` & `koku-nise-4.2.5/nise/yaml_generators/aws/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/aws/rds_instance_types.py` & `koku-nise-4.2.5/nise/yaml_generators/aws/rds_instance_types.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/aws/regions.py` & `koku-nise-4.2.5/nise/yaml_generators/aws/regions.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/azure/generator.py` & `koku-nise-4.2.5/nise/yaml_generators/azure/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/gcp/generator.py` & `koku-nise-4.2.5/nise/yaml_generators/gcp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/generator.py` & `koku-nise-4.2.5/nise/yaml_generators/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/oci/generator.py` & `koku-nise-4.2.5/nise/yaml_generators/oci/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/oci/oci_yaml_constants.py` & `koku-nise-4.2.5/nise/yaml_generators/oci/oci_yaml_constants.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/ocp/generator.py` & `koku-nise-4.2.5/nise/yaml_generators/ocp/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/ocp_on_cloud/generator.py` & `koku-nise-4.2.5/nise/yaml_generators/ocp_on_cloud/generator.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/aws_generator_config.yml` & `koku-nise-4.2.5/nise/yaml_generators/static/aws_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/aws_static_data.yml.j2` & `koku-nise-4.2.5/nise/yaml_generators/static/aws_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/azure_generator_config.yml` & `koku-nise-4.2.5/nise/yaml_generators/static/azure_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/azure_static_data.yml.j2` & `koku-nise-4.2.5/nise/yaml_generators/static/azure_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/gcp_static_data.yml.j2` & `koku-nise-4.2.5/nise/yaml_generators/static/gcp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/oci_static_data.yml.j2` & `koku-nise-4.2.5/nise/yaml_generators/static/oci_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/ocp_generator_config.yml` & `koku-nise-4.2.5/nise/yaml_generators/static/ocp_generator_config.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/ocp_on_cloud_options.yml` & `koku-nise-4.2.5/nise/yaml_generators/static/ocp_on_cloud_options.yml`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/static/ocp_static_data.yml.j2` & `koku-nise-4.2.5/nise/yaml_generators/static/ocp_static_data.yml.j2`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/nise/yaml_generators/utils.py` & `koku-nise-4.2.5/nise/yaml_generators/utils.py`

 * *Files identical despite different names*

### Comparing `koku-nise-4.2.4/setup.py` & `koku-nise-4.2.5/setup.py`

 * *Files identical despite different names*

