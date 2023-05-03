# Comparing `tmp/infra-buddy-too-60.tar.gz` & `tmp/infra-buddy-too-61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infra-buddy-too-60.tar", last modified: Tue Jan 24 20:46:22 2023, max compression
+gzip compressed data, was "infra-buddy-too-61.tar", last modified: Wed May  3 18:24:16 2023, max compression
```

## Comparing `infra-buddy-too-60.tar` & `infra-buddy-too-61.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.738276 infra-buddy-too-60/
--rw-rw-r--   0 runner    (1001) docker     (123)       56 2023-01-24 20:46:22.000000 infra-buddy-too-60/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-24 20:46:22.738276 infra-buddy-too-60/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.726276 infra-buddy-too-60/infra_buddy_too/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/aws/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/aws/cloudwatch_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/aws/ecs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5271 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/aws/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commandline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too/commands/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/bootstrap/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too/commands/deploy_cloudformation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/deploy_cloudformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/deploy_cloudformation/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too/commands/deploy_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/deploy_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/deploy_service/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too/commands/generate_artifact_manifest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/generate_artifact_manifest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/generate_artifact_manifest/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too/commands/generate_service_definition/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/generate_service_definition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/generate_service_definition/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too/commands/introspect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/introspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/introspect/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.734276 infra-buddy-too-60/infra_buddy_too/commands/validate_template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/validate_template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/commands/validate_template/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.734276 infra-buddy-too-60/infra_buddy_too/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/context/artifact_definition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14172 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/context/deploy_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/context/monitor_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/context/service_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.734276 infra-buddy-too-60/infra_buddy_too/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/deploy/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16879 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/deploy/cloudformation_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/deploy/datadog_monitor_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/deploy/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/deploy/ecs_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/deploy/s3_deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.734276 infra-buddy-too-60/infra_buddy_too/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/notifier/datadog_notifier.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.734276 infra-buddy-too-60/infra_buddy_too/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/template/builtin-templates.json
--rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/template/template.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8950 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/template/template_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.738276 infra-buddy-too-60/infra_buddy_too/utility/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/utility/exception.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9442 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/utility/helper_functions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/utility/print_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-01-24 20:45:44.000000 infra-buddy-too-60/infra_buddy_too/utility/waitfor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.730276 infra-buddy-too-60/infra_buddy_too.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-01-24 20:46:22.000000 infra-buddy-too-60/infra_buddy_too.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-01-24 20:46:22.000000 infra-buddy-too-60/infra_buddy_too.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:46:22.000000 infra-buddy-too-60/infra_buddy_too.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:46:22.000000 infra-buddy-too-60/infra_buddy_too.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-24 20:46:22.000000 infra-buddy-too-60/infra_buddy_too.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-24 20:46:22.000000 infra-buddy-too-60/infra_buddy_too.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 20:46:22.000000 infra-buddy-too-60/infra_buddy_too.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 20:46:22.738276 infra-buddy-too-60/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-01-24 20:46:22.000000 infra-buddy-too-60/scripts/infra-buddy
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-24 20:46:22.738276 infra-buddy-too-60/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2385 2023-01-24 20:46:22.000000 infra-buddy-too-60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.656896 infra-buddy-too-61/
+-rw-rw-r--   0 runner    (1001) docker     (123)       56 2023-05-03 18:24:15.000000 infra-buddy-too-61/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-03 18:24:16.656896 infra-buddy-too-61/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.648896 infra-buddy-too-61/infra_buddy_too/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14525 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/aws/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/aws/cloudwatch_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/aws/ecs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5271 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/aws/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commandline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/commands/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/bootstrap/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/commands/deploy_cloudformation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/deploy_cloudformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/deploy_cloudformation/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/commands/deploy_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/deploy_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/deploy_service/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/commands/generate_artifact_manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/generate_artifact_manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/generate_artifact_manifest/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/commands/generate_service_definition/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/generate_service_definition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/generate_service_definition/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/commands/introspect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/introspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/introspect/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/commands/validate_template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/validate_template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/commands/validate_template/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5786 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/context/artifact_definition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14267 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/context/deploy_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/context/monitor_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/context/service_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.656896 infra-buddy-too-61/infra_buddy_too/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/deploy/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16987 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/deploy/cloudformation_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/deploy/datadog_monitor_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/deploy/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/deploy/ecs_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/deploy/s3_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.656896 infra-buddy-too-61/infra_buddy_too/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/notifier/datadog_notifier.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.656896 infra-buddy-too-61/infra_buddy_too/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/template/builtin-templates.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12347 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/template/template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8950 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/template/template_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.656896 infra-buddy-too-61/infra_buddy_too/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/utility/exception.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9442 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/utility/helper_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1233 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/utility/print_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-03 18:23:37.000000 infra-buddy-too-61/infra_buddy_too/utility/waitfor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.652896 infra-buddy-too-61/infra_buddy_too.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-03 18:24:16.000000 infra-buddy-too-61/infra_buddy_too.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-05-03 18:24:16.000000 infra-buddy-too-61/infra_buddy_too.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:24:16.000000 infra-buddy-too-61/infra_buddy_too.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:24:16.000000 infra-buddy-too-61/infra_buddy_too.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 18:24:16.000000 infra-buddy-too-61/infra_buddy_too.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 18:24:16.000000 infra-buddy-too-61/infra_buddy_too.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 18:24:16.000000 infra-buddy-too-61/infra_buddy_too.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 18:24:16.656896 infra-buddy-too-61/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 18:24:15.000000 infra-buddy-too-61/scripts/infra-buddy
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 18:24:16.656896 infra-buddy-too-61/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2385 2023-05-03 18:24:15.000000 infra-buddy-too-61/setup.py
```

### Comparing `infra-buddy-too-60/infra_buddy_too/aws/cloudformation.py` & `infra-buddy-too-61/infra_buddy_too/aws/cloudformation.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/aws/cloudwatch_logs.py` & `infra-buddy-too-61/infra_buddy_too/aws/cloudwatch_logs.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/aws/config.py` & `infra-buddy-too-61/infra_buddy_too/aws/config.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/aws/ecs.py` & `infra-buddy-too-61/infra_buddy_too/aws/ecs.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/aws/s3.py` & `infra-buddy-too-61/infra_buddy_too/aws/s3.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/commandline.py` & `infra-buddy-too-61/infra_buddy_too/commandline.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/commands/bootstrap/command.py` & `infra-buddy-too-61/infra_buddy_too/commands/bootstrap/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/commands/deploy_cloudformation/command.py` & `infra-buddy-too-61/infra_buddy_too/commands/deploy_cloudformation/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/commands/deploy_service/command.py` & `infra-buddy-too-61/infra_buddy_too/commands/deploy_service/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/commands/generate_artifact_manifest/command.py` & `infra-buddy-too-61/infra_buddy_too/commands/generate_artifact_manifest/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/commands/generate_service_definition/command.py` & `infra-buddy-too-61/infra_buddy_too/commands/generate_service_definition/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/commands/introspect/command.py` & `infra-buddy-too-61/infra_buddy_too/commands/introspect/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/commands/validate_template/command.py` & `infra-buddy-too-61/infra_buddy_too/commands/validate_template/command.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/context/artifact_definition.py` & `infra-buddy-too-61/infra_buddy_too/context/artifact_definition.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/context/deploy_ctx.py` & `infra-buddy-too-61/infra_buddy_too/context/deploy_ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,17 @@
 
     def get_deploy_templates(self):
         return self.get('service-templates', {})
 
     def get_service_modification_templates(self):
         return self.get('service-modification-templates', {})
 
-    def generate_modification_stack_name(self, mod_name):
-        return "{ENVIRONMENT}-{APPLICATION}-{ROLE}-{mod_name}".format(mod_name=mod_name, **self)
+    def generate_modification_stack_name(self, mod_name, ending=None):
+        name__format = '{ENVIRONMENT}-{APPLICATION}-{ROLE}-{mod_name}'.format(mod_name=mod_name, **self)
+        return name__format if not ending else f"{name__format}-{ending}"
 
     def generate_modification_resource_stack_name(self, mod_name):
         return "{ENVIRONMENT}-{APPLICATION}-{ROLE}-{mod_name}-resources".format(mod_name=mod_name, **self)
 
     def get_region(self):
         return self._get_required_default_configuration(REGION)
```

### Comparing `infra-buddy-too-60/infra_buddy_too/context/monitor_definition.py` & `infra-buddy-too-61/infra_buddy_too/context/monitor_definition.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/context/service_definition.py` & `infra-buddy-too-61/infra_buddy_too/context/service_definition.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import datetime
 from jsonschema import validate
 from pprint import pformat
 from infra_buddy_too.deploy.cloudformation_deploy import CloudFormationDeploy
 from infra_buddy_too.template.template_manager import TemplateManager
 from infra_buddy_too.utility import print_utility
 
+STACK_NAME_SUFFIX = "stack-name-suffix"
+
 _SERVICE_DEFINITION_FILE = "service.json"
 
 _MODIFICATIONS = 'service-modifications'
+_MODIFICATIONS_EXT = 'service-modification-definitions'
 _ENVIRONMENTS = 'deploy-environments'
 
 _DEPLOYMENT_PARAMETERS = 'deployment-parameters'
 _CI_DEPLOYMENT_PARAMETERS = 'ci-deployment-parameters'
 _PROD_DEPLOYMENT_PARAMETERS = 'prod-deployment-parameters'
 _DEV_DEPLOYMENT_PARAMETERS = 'dev-deployment-parameters'
 _UNIT_TEST_DEPLOYMENT_PARAMETERS = 'unit-test-deployment-parameters'
@@ -47,45 +50,68 @@
                     },
                     "required": ["type"]
                 }
             },
             _ENVIRONMENTS: {
                 "type": "object",
                 "properties": {
-                    "skip": {"type": "array", "items": {
-                        "type": "string"
-                    }
-                 }
+                    "skip": {
+                        "type": "array",
+                        "items": {
+                            "type": "string"
+                        }
+                     }
                 },
                 "additionalProperties": True
             },
-            _DEPLOYMENT_PARAMETERS: {
-                "type": "object",
-                "properties": {
-                },
-                "additionalProperties": True
-            },
-            _CI_DEPLOYMENT_PARAMETERS: {
-                "type": "object",
-                "properties": {
-                },
-                "additionalProperties": True
-            },
-            _PROD_DEPLOYMENT_PARAMETERS: {
-                "type": "object",
-                "properties": {
-                },
-                "additionalProperties": True
+            _MODIFICATIONS:{
+                "type": "array", "items": {
+                    "type": "string"
+                }
             },
-            _DEV_DEPLOYMENT_PARAMETERS: {
-                "type": "object",
-                "properties": {
-                },
-                "additionalProperties": True
-            }
+             _MODIFICATIONS_EXT:{
+                 "type": "array",
+                  "items": {
+                      "type": "object",
+                      "properties": {
+                          "name": {"type": "string"},
+                          STACK_NAME_SUFFIX: {"type": "string"},
+                          _DEPLOYMENT_PARAMETERS: {
+                              "type": "object",
+                              "properties": {},
+                              "additionalProperties": True
+                          }
+                      },
+                      "required": [
+                          STACK_NAME_SUFFIX
+                      ],
+                      "additionalProperties": True
+                  }
+              },
+             _DEPLOYMENT_PARAMETERS: {
+                 "type": "object",
+                 "properties": {},
+                 "additionalProperties": True
+             },
+             _CI_DEPLOYMENT_PARAMETERS: {
+                 "type": "object",
+                 "properties": {},
+                 "additionalProperties": True
+             },
+             _PROD_DEPLOYMENT_PARAMETERS: {
+                 "type": "object",
+                 "properties": {},
+                 "additionalProperties": True
+             },
+             _DEV_DEPLOYMENT_PARAMETERS: {
+                 "type": "object",
+                 "properties": {},
+                 "additionalProperties": True
+             }
+
         },
         "required": [
             _APPLICATION,
             _ROLE,
             _DEPLOYMENT_PARAMETERS,
             _SERVICE_TYPE
         ]
@@ -121,14 +147,15 @@
             env_deployment_parameters = '{environment}-deployment-parameters'.format(environment=environment)
             if env_deployment_parameters in service_definition:
                 print_utility.info("Updating deployment params with environment"
                                    " specific settings - {}".format(env_deployment_parameters))
                 self.deployment_parameters.update(service_definition[env_deployment_parameters])
             print_utility.info("Loaded deployment parameters: " + pformat(self.deployment_parameters, indent=4))
             self.service_modifications = service_definition.get(_MODIFICATIONS, [])
+            self.service_modifications_ext = service_definition.get(_MODIFICATIONS_EXT, [])
 
     def generate_execution_plan(self, template_manager, deploy_ctx):
         # type: (TemplateManager) -> list(Deploy)
         ret = []
         template = template_manager.get_known_service(self.service_type)
         ret.append(CloudFormationDeploy(stack_name=deploy_ctx.stack_name,
                                         template=template,
@@ -143,16 +170,25 @@
         else:
             print_utility.info("Addition resource template not located (aws-resources.template).")
         for mod in self.service_modifications:
             template = template_manager.get_known_service_modification(self.service_type, mod)
             ret.append(CloudFormationDeploy(stack_name=deploy_ctx.generate_modification_stack_name(mod),
                                             template=template,
                                             deploy_ctx=deploy_ctx))
-            if template.has_monitor_definition():
-                ret.extend(template.get_monitor_artifact().generate_execution_plan(deploy_ctx))
+        for definition in self.service_modifications_ext:
+            mod = definition.get('name')
+            ending = definition.get(STACK_NAME_SUFFIX)
+            parameters = definition.get(_DEPLOYMENT_PARAMETERS)
+            template = template_manager.get_known_service_modification(self.service_type, mod)
+            ret.append(CloudFormationDeploy(stack_name=deploy_ctx.generate_modification_stack_name(mod,ending),
+                                            template=template,
+                                            deploy_ctx=deploy_ctx,
+                                            deployment_specific_parameters=parameters))
+        if template.has_monitor_definition():
+            ret.extend(template.get_monitor_artifact().generate_execution_plan(deploy_ctx))
         return ret
 
     @classmethod
     def save_to_file(cls, application, role, deploy_params, service_type, known_service_modifications, destination):
         # type: (str, str, dict,str) -> str
         if destination:
             service_file_path = os.path.join(destination, _SERVICE_DEFINITION_FILE)
```

### Comparing `infra-buddy-too-60/infra_buddy_too/deploy/cloudformation_deploy.py` & `infra-buddy-too-61/infra_buddy_too/deploy/cloudformation_deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,27 +39,27 @@
                 "key": {"type": "string"}
             },
             "required": ["type"]
         }
 
     }
 
-    def __init__(self, stack_name, template, deploy_ctx):
+    def __init__(self, stack_name, template, deploy_ctx, deployment_specific_parameters=None):
         # type: (str, Template,DeployContext) -> None
-        super(CloudFormationDeploy, self).__init__(deploy_ctx)
+        super(CloudFormationDeploy, self).__init__(deploy_ctx,deployment_specific_parameters)
         self.stack_name = stack_name
         self.config_directory = template.get_config_dir()
         self.lambda_directory = template.get_lambda_dir()
         self.parameter_file = template.get_parameter_file_path()
         self.template_file = template.get_template_file_path()
         self.default_path = template.get_defaults_file_path()
         self._load_defaults(template.get_default_env_values())
 
     def _load_defaults(self, default_env_values):
-        self.defaults = {}
+        self.defaults = {} if not self.defaults else self.defaults
         if self.default_path and os.path.exists(self.default_path):
             with open(self.default_path, 'r') as default_fp:
                 def_obj = json.load(default_fp)
                 validate(def_obj, self.schema)
             self._process_default_dict(def_obj)
         self.defaults.update(default_env_values)
```

### Comparing `infra-buddy-too-60/infra_buddy_too/deploy/datadog_monitor_deploy.py` & `infra-buddy-too-61/infra_buddy_too/deploy/datadog_monitor_deploy.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/deploy/deploy.py` & `infra-buddy-too-61/infra_buddy_too/deploy/deploy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 
 class Deploy(object):
 
 
     
-    def __init__(self,deploy_ctx):
+    def __init__(self,deploy_ctx, defaults=None):
         super(Deploy, self).__init__()
         self.deploy_ctx = deploy_ctx
         self.stack_name = None
-        self.defaults = {}
+        self.defaults = defaults if defaults else {}
         # Flag to indicate that we should not actually deploy (see deploy-environments['skip'])
         self.dry_run = False
 
     def do_deploy(self,dry_run=False):
         self.deploy_ctx.push_deploy_ctx(self)
         try:
             return self._internal_deploy(dry_run or self.dry_run)
```

### Comparing `infra-buddy-too-60/infra_buddy_too/deploy/ecs_deploy.py` & `infra-buddy-too-61/infra_buddy_too/deploy/ecs_deploy.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/deploy/s3_deploy.py` & `infra-buddy-too-61/infra_buddy_too/deploy/s3_deploy.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/notifier/datadog_notifier.py` & `infra-buddy-too-61/infra_buddy_too/notifier/datadog_notifier.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/template/builtin-templates.json` & `infra-buddy-too-61/infra_buddy_too/template/builtin-templates.json`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/template/template.py` & `infra-buddy-too-61/infra_buddy_too/template/template.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/template/template_manager.py` & `infra-buddy-too-61/infra_buddy_too/template/template_manager.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/utility/helper_functions.py` & `infra-buddy-too-61/infra_buddy_too/utility/helper_functions.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/utility/print_utility.py` & `infra-buddy-too-61/infra_buddy_too/utility/print_utility.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too/utility/waitfor.py` & `infra-buddy-too-61/infra_buddy_too/utility/waitfor.py`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/infra_buddy_too.egg-info/SOURCES.txt` & `infra-buddy-too-61/infra_buddy_too.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `infra-buddy-too-60/setup.py` & `infra-buddy-too-61/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         _install.run(self)
 
         self.post_install_script()
 
 if __name__ == '__main__':
     setup(
         name = 'infra-buddy-too',
-        version = '60',
+        version = '61',
         description = 'CLI for deploying micro-services',
         long_description = 'CLI for deploying micro-services',
         long_description_content_type = None,
         classifiers = [
             'Development Status :: 3 - Alpha',
             'Programming Language :: Python'
         ],
```

