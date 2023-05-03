# Comparing `tmp/aws-cfn-update-0.8.1.tar.gz` & `tmp/aws-cfn-update-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-cfn-update-0.8.1.tar", last modified: Tue Mar 28 19:37:34 2023, max compression
+gzip compressed data, was "aws-cfn-update-0.8.2.tar", last modified: Wed May  3 17:42:40 2023, max compression
```

## Comparing `aws-cfn-update-0.8.1.tar` & `aws-cfn-update-0.8.2.tar`

### file list

```diff
@@ -1,126 +1,126 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.984872 aws-cfn-update-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.956872 aws-cfn-update-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.964872 aws-cfn-update-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.github/workflows/release-image.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.964872 aws-cfn-update-0.8.1/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/aws-cfn-update.iml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/cfnlintPlugin.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.964872 aws-cfn-update-0.8.1/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.964872 aws-cfn-update-0.8.1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.make-release-support
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/.release
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/Makefile.mk
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-03-28 19:37:34.984872 aws-cfn-update-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)    77257 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.960872 aws-cfn-update-0.8.1/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.968872 aws-cfn-update-0.8.1/samples/add-new-resources/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/add-new-resources/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/add-new-resources/storage-server-new.json
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/add-new-resources/storage-server-new.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/add-new-resources/storage-server.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/add-new-resources/storage-server.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.968872 aws-cfn-update-0.8.1/samples/config-rule-inline-code/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/config-rule-inline-code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/config-rule-inline-code/dynamodb-pitr-enabled.guard
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/config-rule-inline-code/template.json
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/config-rule-inline-code/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.968872 aws-cfn-update-0.8.1/samples/container-image/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/container-image/paas-monitor.json
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/container-image/paas-monitor.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.968872 aws-cfn-update-0.8.1/samples/cron-schedule-expression/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/cron-schedule-expression/cron.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.968872 aws-cfn-update-0.8.1/samples/lambda-inline-code/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/lambda-inline-code/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/lambda-inline-code/cfn-listener-rule-provider.json
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/lambda-inline-code/cfn-listener-rule-provider.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/lambda-inline-code/cfn_listener_rule_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.968872 aws-cfn-update-0.8.1/samples/latest-ami-update/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/latest-ami-update/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/latest-ami-update/template.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.968872 aws-cfn-update-0.8.1/samples/oidc-provider/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/oidc-provider/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/oidc-provider/oidc-provider.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/oidc-provider/oidc-provider.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.968872 aws-cfn-update-0.8.1/samples/packer-latest-ami/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/packer-latest-ami/packer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.972872 aws-cfn-update-0.8.1/samples/remove-resource/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/remove-resource/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/remove-resource/storage-server.json
--rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/remove-resource/storage-server.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.972872 aws-cfn-update-0.8.1/samples/rest-api-body/
--rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/rest-api-body/api-specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/rest-api-body/aws-extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/rest-api-body/rest-api.json
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/rest-api-body/rest-api.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.972872 aws-cfn-update-0.8.1/samples/state-machine-definition/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/state-machine-definition/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/state-machine-definition/definition.json
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/state-machine-definition/definition.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/samples/state-machine-definition/helloworld.json
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-28 19:37:34.984872 aws-cfn-update-0.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.960872 aws-cfn-update-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.976872 aws-cfn-update-0.8.1/src/aws_cfn_update/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/add_missing_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/add_new_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5193 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/cfn_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/config_rule_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/container_image_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/cron_schedule_expression_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/lambda_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/latest_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/oidc_provider_thumbprints_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/packer_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/remove_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/replace_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/rest_api_body_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/src/aws_cfn_update/statemachine_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.976872 aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-03-28 19:37:34.000000 aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-03-28 19:37:34.000000 aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 19:37:34.000000 aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-28 19:37:34.000000 aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-28 19:37:34.000000 aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 19:37:34.000000 aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 19:36:31.000000 aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.980872 aws-cfn-update-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/api-specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/aws-extensions.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   204302 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/dummy_responses.json
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_add_new_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_config_rule_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_cron_schedule_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_lambda_inline_code_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_latest_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_oidc_provider_thumbprint_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_packer_ami_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_remove_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_replace_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_rest_api_body_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/test_statemachine_definition_updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.980872 aws-cfn-update-0.8.1/tests/update_packer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/update_packer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/update_packer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:37:34.980872 aws-cfn-update-0.8.1/tests/update_packer/call_00001_describe_images/
--rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/update_packer/call_00001_describe_images/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tests/update_packer/test_update_packer.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-28 19:35:57.000000 aws-cfn-update-0.8.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.391731 aws-cfn-update-0.8.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.github/workflows/release-image.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/aws-cfn-update.iml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/cfnlintPlugin.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.make-release-support
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/.release
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Makefile.mk
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)    77208 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.391731 aws-cfn-update-0.8.2/samples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/samples/add-new-resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/storage-server-new.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/storage-server-new.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/storage-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/add-new-resources/storage-server.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/samples/config-rule-inline-code/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/config-rule-inline-code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/config-rule-inline-code/dynamodb-pitr-enabled.guard
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/config-rule-inline-code/template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/config-rule-inline-code/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/samples/container-image/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/container-image/paas-monitor.json
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/container-image/paas-monitor.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.395731 aws-cfn-update-0.8.2/samples/cron-schedule-expression/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/cron-schedule-expression/cron.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/lambda-inline-code/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/lambda-inline-code/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn-listener-rule-provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn-listener-rule-provider.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn_listener_rule_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/latest-ami-update/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/latest-ami-update/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/latest-ami-update/template.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/oidc-provider/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/oidc-provider/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/oidc-provider/oidc-provider.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/oidc-provider/oidc-provider.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/packer-latest-ami/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/packer-latest-ami/packer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/remove-resource/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/remove-resource/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/remove-resource/storage-server.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/remove-resource/storage-server.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/rest-api-body/
+-rw-r--r--   0 runner    (1001) docker     (123)    17590 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/rest-api-body/api-specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/rest-api-body/aws-extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/rest-api-body/rest-api.json
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/rest-api-body/rest-api.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.399731 aws-cfn-update-0.8.2/samples/state-machine-definition/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/state-machine-definition/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/state-machine-definition/definition.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/state-machine-definition/definition.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/samples/state-machine-definition/helloworld.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.391731 aws-cfn-update-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.403731 aws-cfn-update-0.8.2/src/aws_cfn_update/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/add_missing_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/add_new_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5279 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/cfn_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/config_rule_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/container_image_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/cron_schedule_expression_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/lambda_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9569 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/latest_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/oidc_provider_thumbprints_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/packer_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/remove_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/replace_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/rest_api_body_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/src/aws_cfn_update/statemachine_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.403731 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10952 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-03 17:42:40.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 17:41:54.000000 aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.403731 aws-cfn-update-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/api-specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/aws-extensions.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   204302 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/dummy_responses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_add_new_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2873 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_config_rule_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_cron_schedule_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_lambda_inline_code_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_latest_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_oidc_provider_thumbprint_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_packer_ami_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5027 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_remove_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_replace_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_rest_api_body_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/test_statemachine_definition_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/tests/update_packer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/update_packer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/update_packer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 17:42:40.407731 aws-cfn-update-0.8.2/tests/update_packer/call_00001_describe_images/
+-rw-r--r--   0 runner    (1001) docker     (123)    17592 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/update_packer/call_00001_describe_images/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tests/update_packer/test_update_packer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 17:41:34.000000 aws-cfn-update-0.8.2/tox.ini
```

### Comparing `aws-cfn-update-0.8.1/.github/workflows/release-image.yaml` & `aws-cfn-update-0.8.2/.github/workflows/release-image.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/.github/workflows/release.yml` & `aws-cfn-update-0.8.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/.idea/aws-cfn-update.iml` & `aws-cfn-update-0.8.2/.idea/aws-cfn-update.iml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/.idea/codeStyles/Project.xml` & `aws-cfn-update-0.8.2/.idea/codeStyles/Project.xml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/.idea/inspectionProfiles/Project_Default.xml` & `aws-cfn-update-0.8.2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/.make-release-support` & `aws-cfn-update-0.8.2/.make-release-support`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/LICENSE` & `aws-cfn-update-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/Makefile.mk` & `aws-cfn-update-0.8.2/Makefile.mk`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/PKG-INFO` & `aws-cfn-update-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-update
-Version: 0.8.1
+Version: 0.8.2
 Summary: Programmatically update CloudFormation templates
 Home-page: https://github.com/binxio/aws-cfn-update
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-cfn-update-0.8.1/Pipfile.lock` & `aws-cfn-update-0.8.2/Pipfile.lock`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9806832694763731%*

 * *Differences: {"'default'": "{'attrs': {'hashes': "*

 * *              "['sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04', "*

 * *              "'sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015'], "*

 * *              '\'markers\': "python_version >= \'3.7\'", \'version\': \'==23.1.0\'}, \'boto3\': '*

 * *              "{'hashes': "*

 * *              "['sha256:6648aff15d19927cd26db47eb56362ccd313a1ddbd7aaa3235ef05d05d398252', "*

 * *              "'sha256:fe8248b80c4f0fdaed8b8779467c4431a5e52177e02ccd […]*

```diff
@@ -14,39 +14,39 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "attrs": {
             "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
+                "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04",
+                "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1.0"
         },
         "aws-cfn-update": {
             "editable": true,
             "path": "."
         },
         "boto3": {
             "hashes": [
-                "sha256:567f03ac638c3a6f4af00d88d081df7d6b8de4d127a26543c4ec1e7509e1a626",
-                "sha256:b5be5bcffe17d70a72622f8ecbb428df7b11ef8d1facdfa984e94c6fc9fa301b"
+                "sha256:6648aff15d19927cd26db47eb56362ccd313a1ddbd7aaa3235ef05d05d398252",
+                "sha256:fe8248b80c4f0fdaed8b8779467c4431a5e52177e02ccd137d51ec51194ebb00"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.100"
+            "version": "==1.26.125"
         },
         "botocore": {
             "hashes": [
-                "sha256:d5c4c5bbbbf0ec62a4235ccac1b9bbb579558f7bb3231d7fb6054e1f64d3a623",
-                "sha256:ff6585df3dcef2057be5e54b45d254608d3769d726ea4ccd4e17f77825e5b13d"
+                "sha256:3005a7ffee083315e69938acdf1bfeaf9e21fe1fe1643d6573ee817721f4ffcd",
+                "sha256:ac87b63e9aa4231cd28941945024a0c4470c184c60334ebe5e1cae3544c785ed"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.100"
+            "version": "==1.29.125"
         },
         "certifi": {
             "hashes": [
                 "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
                 "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
             ],
             "markers": "python_version >= '3.6'",
@@ -215,44 +215,44 @@
                 "sha256:bb4d8133cb15a609f44e8213d9b391b0809795062913b383c62be0ee95b1db48"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==8.1.3"
         },
         "croniter": {
             "hashes": [
-                "sha256:32a5ec04e97ec0837bcdf013767abd2e71cceeefd3c2e14c804098ce51ad6cd9",
-                "sha256:d6ed8386d5f4bbb29419dc1b65c4909c04a2322bd15ec0dc5b2877bfa1b75c7a"
+                "sha256:d067b1f95b553c6e82d95a983c465695913dcd12f47a8b9aa938a0450d94dd5e",
+                "sha256:da1a1a7ca977b38e952ab0a119576e002bc4c05d058d644e81fc06ef7e995bb0"
             ],
             "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.8"
+            "version": "==1.3.14"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
-                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
-                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
-                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
-                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
-                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
-                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
-                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
-                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
-                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
-                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
-                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
-                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
-                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
-                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
-                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
-                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
-                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
-                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==40.0.1"
+            "version": "==40.0.2"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -326,18 +326,18 @@
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pytz": {
             "hashes": [
-                "sha256:8a8baaf1e237175b02f5c751eea67168043a749c843989e2b3015aa1ad9db68b",
-                "sha256:a27dcf612c05d2ebde626f7d506555f10dfc815b3eddccfaadfc7d99b11c9a07"
+                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
+                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
-            "version": "==2023.2"
+            "version": "==2023.3"
         },
         "pytz-deprecation-shim": {
             "hashes": [
                 "sha256:8314c9692a636c8eb3bda879b9f119e350e93223ae83e70e80c31675a0fdc1a6",
                 "sha256:af097bae1b616dde5c5744441e2ddc69e74dfdcb0c263129610d85b87445a59d"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
@@ -387,27 +387,27 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.30.0"
         },
         "ruamel.yaml": {
             "hashes": [
-                "sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7",
-                "sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af"
+                "sha256:b4c6e66d103d8af198aa6139580ab735169be4922eb4c515ac121bdabf6f9361",
+                "sha256:c22ec58aaca5105f771cb8f7ac45ad631b5e8b00454ebe1822d442fb696e9e62"
             ],
             "markers": "python_version >= '3'",
-            "version": "==0.17.21"
+            "version": "==0.17.22"
         },
         "ruamel.yaml.clib": {
             "hashes": [
                 "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
                 "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
                 "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
                 "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
@@ -461,19 +461,19 @@
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "tzdata": {
             "hashes": [
-                "sha256:905ae9e6744dd9ef5ce94d2aaa2dd00282fee38b670b2133407f23c388f110a1",
-                "sha256:c3b51b235b07f9f1889089c2264bcbeaaba260a63f89bea09e350ea4205eb95f"
+                "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a",
+                "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.2"
+            "version": "==2023.3"
         },
         "tzlocal": {
             "hashes": [
                 "sha256:3f21d09e1b2aa9f2dacca12da240ca37de3ba5237a93addfd6d593afe9073355",
                 "sha256:b44c4388f3d34f25862cfbb387578a4d70fec417649da694a132f628a23367e2"
             ],
             "markers": "python_version >= '3.7'",
@@ -487,19 +487,19 @@
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.15"
         }
     },
     "develop": {
         "attrs": {
             "hashes": [
-                "sha256:29e95c7f6778868dbd49170f98f8818f78f3dc5e0e37c0b1f474e3561b240836",
-                "sha256:c9227bfc2f01993c03f68db37d1d15c9690188323c067c641f1a35ca58185f99"
+                "sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04",
+                "sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==22.2.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==23.1.0"
         },
         "aws-cfn-update": {
             "editable": true,
             "path": "."
         },
         "bleach": {
             "hashes": [
@@ -507,27 +507,27 @@
                 "sha256:33c16e3353dbd13028ab4799a0f89a83f113405c766e9c122df8a06f5b85b3f4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==6.0.0"
         },
         "boto3": {
             "hashes": [
-                "sha256:567f03ac638c3a6f4af00d88d081df7d6b8de4d127a26543c4ec1e7509e1a626",
-                "sha256:b5be5bcffe17d70a72622f8ecbb428df7b11ef8d1facdfa984e94c6fc9fa301b"
+                "sha256:6648aff15d19927cd26db47eb56362ccd313a1ddbd7aaa3235ef05d05d398252",
+                "sha256:fe8248b80c4f0fdaed8b8779467c4431a5e52177e02ccd137d51ec51194ebb00"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.26.100"
+            "version": "==1.26.125"
         },
         "botocore": {
             "hashes": [
-                "sha256:d5c4c5bbbbf0ec62a4235ccac1b9bbb579558f7bb3231d7fb6054e1f64d3a623",
-                "sha256:ff6585df3dcef2057be5e54b45d254608d3769d726ea4ccd4e17f77825e5b13d"
+                "sha256:3005a7ffee083315e69938acdf1bfeaf9e21fe1fe1643d6573ee817721f4ffcd",
+                "sha256:ac87b63e9aa4231cd28941945024a0c4470c184c60334ebe5e1cae3544c785ed"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==1.29.100"
+            "version": "==1.29.125"
         },
         "build": {
             "hashes": [
                 "sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171",
                 "sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269"
             ],
             "index": "pypi",
@@ -728,44 +728,44 @@
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==0.4.6"
         },
         "croniter": {
             "hashes": [
-                "sha256:32a5ec04e97ec0837bcdf013767abd2e71cceeefd3c2e14c804098ce51ad6cd9",
-                "sha256:d6ed8386d5f4bbb29419dc1b65c4909c04a2322bd15ec0dc5b2877bfa1b75c7a"
+                "sha256:d067b1f95b553c6e82d95a983c465695913dcd12f47a8b9aa938a0450d94dd5e",
+                "sha256:da1a1a7ca977b38e952ab0a119576e002bc4c05d058d644e81fc06ef7e995bb0"
             ],
             "markers": "python_version >= '2.6' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==1.3.8"
+            "version": "==1.3.14"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
-                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
-                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
-                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
-                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
-                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
-                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
-                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
-                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
-                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
-                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
-                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
-                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
-                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
-                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
-                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
-                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
-                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
-                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==40.0.1"
+            "version": "==40.0.2"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -784,35 +784,35 @@
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:892be14aa8efc01673b5ed6589dbccb95f9a8596f0507e232626155495c18105",
-                "sha256:bde48477b15fde2c7e5a0713cbe72721cb5a5ad32ee0b8f419907960b9d75536"
+                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
+                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.10.7"
+            "version": "==3.12.0"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "importlib-metadata": {
             "hashes": [
-                "sha256:43ce9281e097583d758c2c708c4376371261a02c34682491a8e98352365aad20",
-                "sha256:ff80f3b5394912eb1b108fcfd444dc78b7f1f3e16b16188054bd01cb9cb86f09"
+                "sha256:43dd286a2cd8995d5eaef7fee2066340423b818ed3fd70adf0bad5f1fac53fed",
+                "sha256:92501cdf9cc66ebd3e612f1b4f0c0765dfa42f0fa38ffb319b6bd84dd675d705"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==6.1.0"
+            "version": "==6.6.0"
         },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
@@ -878,35 +878,35 @@
                 "sha256:d2bc7f02446e86a68911e58ded76d6561eea00cddfb2a91e7019bbb586c799f3"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==9.1.0"
         },
         "packaging": {
             "hashes": [
-                "sha256:714ac14496c3e68c99c29b00845f7a2b85f3bb6f1078fd9f72fd20f0570002b2",
-                "sha256:b6ad297f8907de0fa2fe1ccbd26fdaf387f5f47c7275fedf8cce89f99446cf97"
+                "sha256:994793af429502c4ea2ebf6bf664629d07c1a9fe974af92966e4b8d2df7edc61",
+                "sha256:a392980d2b6cffa644431898be54b0045151319d1e7ec34f0cfed48767dd334f"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==23.0"
+            "version": "==23.1"
         },
         "pkginfo": {
             "hashes": [
                 "sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546",
                 "sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==1.9.6"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
-                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
+                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
+                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.2.0"
+            "version": "==3.5.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
@@ -917,19 +917,19 @@
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pygments": {
             "hashes": [
-                "sha256:b3ed06a9e8ac9a9aae5a6f5dbe78a8a58655d17b43b93c078f094ddc476ae297",
-                "sha256:fa7bd7bd2771287c0de303af8bfdfc731f51bd2c6a47ab69d117138893b82717"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
-            "markers": "python_version >= '3.6'",
-            "version": "==2.14.0"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.15.1"
         },
         "pyproject-api": {
             "hashes": [
                 "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
                 "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
             ],
             "markers": "python_version >= '3.7'",
@@ -974,34 +974,34 @@
                 "sha256:f0e7c4b2f77593871e918be000b96c8107da48444d57005b6a6bc61fb4331b2c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.19.3"
         },
         "pytest": {
             "hashes": [
-                "sha256:130328f552dcfac0b1cec75c12e3f005619dc5f874f0a06e8ff7263f0ee6225e",
-                "sha256:c99ab0c73aceb050f68929bc93af19ab6db0558791c6a0715723abe9d0ade9d4"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
-            "version": "==7.2.2"
+            "version": "==7.3.1"
         },
         "python-dateutil": {
             "hashes": [
                 "sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86",
                 "sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==2.8.2"
         },
         "pytz": {
             "hashes": [
-                "sha256:8a8baaf1e237175b02f5c751eea67168043a749c843989e2b3015aa1ad9db68b",
-                "sha256:a27dcf612c05d2ebde626f7d506555f10dfc815b3eddccfaadfc7d99b11c9a07"
+                "sha256:1d8ce29db189191fb55338ee6d0387d82ab59f3d00eac103412d64e0ebd0c588",
+                "sha256:a151b3abb88eda1d4e34a9814df37de2a80e301e68ba0fd856fb9b46bfbbbffb"
             ],
-            "version": "==2023.2"
+            "version": "==2023.3"
         },
         "pytz-deprecation-shim": {
             "hashes": [
                 "sha256:8314c9692a636c8eb3bda879b9f119e350e93223ae83e70e80c31675a0fdc1a6",
                 "sha256:af097bae1b616dde5c5744441e2ddc69e74dfdcb0c263129610d85b87445a59d"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
@@ -1059,51 +1059,51 @@
                 "sha256:f67a16caedfa71eef48a31b39708637a6f4664c4394801a7b0d6432d13907343"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==37.3"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
-            "markers": "python_version >= '3.7' and python_version < '4'",
-            "version": "==2.28.2"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.30.0"
         },
         "requests-toolbelt": {
             "hashes": [
-                "sha256:18565aa58116d9951ac39baa288d3adb5b3ff975c4f25eee78555d89e8f247f7",
-                "sha256:62e09f7ff5ccbda92772a29f394a49c3ad6cb181d568b1337626b2abb628a63d"
+                "sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6",
+                "sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
-            "version": "==0.10.1"
+            "version": "==1.0.0"
         },
         "rfc3986": {
             "hashes": [
                 "sha256:50b1502b60e289cb37883f3dfd34532b8873c7de9f49bb546641ce9cbd256ebd",
                 "sha256:97aacf9dbd4bfd829baad6e6309fa6573aaf1be3f6fa735c8ab05e46cecb261c"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
         },
         "rich": {
             "hashes": [
-                "sha256:540c7d6d26a1178e8e8b37e9ba44573a3cd1464ff6348b99ee7061b95d1c6333",
-                "sha256:dc84400a9d842b3a9c5ff74addd8eb798d155f36c1c91303888e0a66850d2a15"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "markers": "python_full_version >= '3.7.0'",
-            "version": "==13.3.3"
+            "version": "==13.3.5"
         },
         "ruamel.yaml": {
             "hashes": [
-                "sha256:742b35d3d665023981bd6d16b3d24248ce5df75fdb4e2924e93a05c1f8b61ca7",
-                "sha256:8b7ce697a2f212752a35c1ac414471dc16c424c9573be4926b56ff3f5d23b7af"
+                "sha256:b4c6e66d103d8af198aa6139580ab735169be4922eb4c515ac121bdabf6f9361",
+                "sha256:c22ec58aaca5105f771cb8f7ac45ad631b5e8b00454ebe1822d442fb696e9e62"
             ],
             "markers": "python_version >= '3'",
-            "version": "==0.17.21"
+            "version": "==0.17.22"
         },
         "ruamel.yaml.clib": {
             "hashes": [
                 "sha256:045e0626baf1c52e5527bd5db361bc83180faaba2ff586e763d3d5982a876a9e",
                 "sha256:15910ef4f3e537eea7fe45f8a5d19997479940d9196f357152a09031c5be59f3",
                 "sha256:184faeaec61dbaa3cace407cffc5819f7b977e75360e8d5ca19461cd851a5fc5",
                 "sha256:1f08fd5a2bea9c4180db71678e850b995d2a5f4537be0e94557668cf0f5f9497",
@@ -1149,19 +1149,19 @@
                 "sha256:2ed07d3866f523cc561bf4a00fc5535827981b117dd7876f036b0c1aca42c947"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.6.0"
         },
         "setuptools": {
             "hashes": [
-                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
-                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
+                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
+                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.6.1"
+            "version": "==67.7.2"
         },
         "setuptools-scm": {
             "hashes": [
                 "sha256:6c508345a771aad7d56ebff0e70628bf2b0ec7573762be9960214730de278f27",
                 "sha256:73988b6d848709e2af142aa48c986ea29592bbcfca5375678064708205253d8e"
             ],
             "index": "pypi",
@@ -1181,19 +1181,19 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version < '3.11'",
             "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
-                "sha256:12fe562b8992ea63b1e92556b7e28600cd1b70c9e01ce08984f60ce2d32c243c",
-                "sha256:524640254de8b0f03facbdc6b7c18a35700592e3ada0ede42f509b3504b745ff"
+                "sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56",
+                "sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046"
             ],
             "index": "pypi",
-            "version": "==4.4.8"
+            "version": "==4.5.1"
         },
         "twine": {
             "hashes": [
                 "sha256:929bc3c280033347a00f847236564d1c52a3e61b1ac2516c97c48f3ceab756d8",
                 "sha256:9e102ef5fdd5a20661eb88fad46338806c3bd32cf1db729603fe3697b1bc83c8"
             ],
             "index": "pypi",
@@ -1205,19 +1205,19 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "tzdata": {
             "hashes": [
-                "sha256:905ae9e6744dd9ef5ce94d2aaa2dd00282fee38b670b2133407f23c388f110a1",
-                "sha256:c3b51b235b07f9f1889089c2264bcbeaaba260a63f89bea09e350ea4205eb95f"
+                "sha256:11ef1e08e54acb0d4f95bdb1be05da659673de4acbd21bf9c69e94cc5e907a3a",
+                "sha256:7e65763eef3120314099b6939b5546db7adce1e7d6f2e179e3df563c70511eda"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2023.2"
+            "version": "==2023.3"
         },
         "tzlocal": {
             "hashes": [
                 "sha256:3f21d09e1b2aa9f2dacca12da240ca37de3ba5237a93addfd6d593afe9073355",
                 "sha256:b44c4388f3d34f25862cfbb387578a4d70fec417649da694a132f628a23367e2"
             ],
             "markers": "python_version >= '3.7'",
@@ -1229,19 +1229,19 @@
                 "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
             "version": "==1.26.15"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
-                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.21.0"
+            "version": "==20.23.0"
         },
         "webencodings": {
             "hashes": [
                 "sha256:a0af1213f3c2226497a97e2b3aa01a7e4bee4f403f95be16fc9acd2947514a78",
                 "sha256:b36a1c245f2d304965eb4e0a82848379241dc04b865afcc4aab16748587e1923"
             ],
             "version": "==0.5.1"
```

### Comparing `aws-cfn-update-0.8.1/README.md` & `aws-cfn-update-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/add-new-resources/storage-server-new.json` & `aws-cfn-update-0.8.2/samples/add-new-resources/storage-server-new.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/add-new-resources/storage-server-new.yaml` & `aws-cfn-update-0.8.2/samples/add-new-resources/storage-server-new.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/add-new-resources/storage-server.json` & `aws-cfn-update-0.8.2/samples/add-new-resources/storage-server.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/add-new-resources/storage-server.yaml` & `aws-cfn-update-0.8.2/samples/add-new-resources/storage-server.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/container-image/paas-monitor.json` & `aws-cfn-update-0.8.2/samples/container-image/paas-monitor.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/lambda-inline-code/cfn-listener-rule-provider.json` & `aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn-listener-rule-provider.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/lambda-inline-code/cfn-listener-rule-provider.yaml` & `aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn-listener-rule-provider.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/lambda-inline-code/cfn_listener_rule_provider.py` & `aws-cfn-update-0.8.2/samples/lambda-inline-code/cfn_listener_rule_provider.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/latest-ami-update/template.yaml` & `aws-cfn-update-0.8.2/samples/latest-ami-update/template.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/packer-latest-ami/packer.json` & `aws-cfn-update-0.8.2/samples/packer-latest-ami/packer.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/remove-resource/storage-server.json` & `aws-cfn-update-0.8.2/samples/remove-resource/storage-server.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/remove-resource/storage-server.yaml` & `aws-cfn-update-0.8.2/samples/remove-resource/storage-server.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/rest-api-body/api-specification.yaml` & `aws-cfn-update-0.8.2/samples/rest-api-body/api-specification.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/rest-api-body/aws-extensions.yaml` & `aws-cfn-update-0.8.2/samples/rest-api-body/aws-extensions.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/rest-api-body/rest-api.json` & `aws-cfn-update-0.8.2/samples/rest-api-body/rest-api.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/state-machine-definition/definition.json` & `aws-cfn-update-0.8.2/samples/state-machine-definition/definition.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/samples/state-machine-definition/definition.yaml` & `aws-cfn-update-0.8.2/samples/state-machine-definition/definition.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/setup.cfg` & `aws-cfn-update-0.8.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aws-cfn-update
-version = 0.8.1
+version = 0.8.2
 author = Mark van Holsteijn
 url = https://github.com/binxio/aws-cfn-update
 author_email = mark.vanholsteijn@xebia.com
 description = Programmatically update CloudFormation templates
 long_description = file: README.md
 long_description_content_type = text/markdown
 test_suite = tests
```

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/add_new_resources.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/add_new_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/cfn_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/cfn_updater.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         self.template = None
         with open(self.filename, 'r') as f:
             if self.template_format == '.json':
                 self.template = json.load(f, object_pairs_hook=collections.OrderedDict)
             else:
                 yaml = YAML(typ='rt')
                 yaml.preserve_quotes = True
+                yaml.explicit_start = True
                 self.template = yaml.load(f)
 
     def is_cloudformation_template(self):
         """
         returns true if the `self.template` is a AWS CloudFormation template
         """
         return self.template and 'AWSTemplateFormatVersion' in self.template
@@ -102,14 +103,15 @@
 
         if self.dry_run:
             return
 
         with open(self.filename, 'w') as f:
             if self.template_format == '.yaml':
                 yaml = YAML()
+                yaml.explicit_start = True
                 yaml.indent(mapping=2, sequence=4, offset=2)
                 yaml.dump(self.template, f)
             else:
                 json.dump(self.template, f, separators=(',', ': '), indent=2)
 
     def update_template(self):
         """
```

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/cli.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/cli.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/config_rule_inline_code_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/config_rule_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/container_image_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/container_image_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/cron_schedule_expression_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/cron_schedule_expression_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/lambda_inline_code_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/lambda_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/latest_ami_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/latest_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/oidc_provider_thumbprints_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/oidc_provider_thumbprints_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/packer_ami_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/packer_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/remove_resource.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/remove_resource.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/replace_references.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/replace_references.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/rest_api_body_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/rest_api_body_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update/statemachine_updater.py` & `aws-cfn-update-0.8.2/src/aws_cfn_update/statemachine_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/PKG-INFO` & `aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-cfn-update
-Version: 0.8.1
+Version: 0.8.2
 Summary: Programmatically update CloudFormation templates
 Home-page: https://github.com/binxio/aws-cfn-update
 Author: Mark van Holsteijn
 Author-email: mark.vanholsteijn@xebia.com
 License: BSD 3-Clause License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `aws-cfn-update-0.8.1/src/aws_cfn_update.egg-info/SOURCES.txt` & `aws-cfn-update-0.8.2/src/aws_cfn_update.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/api-specification.yaml` & `aws-cfn-update-0.8.2/tests/api-specification.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/aws-extensions.yaml` & `aws-cfn-update-0.8.2/tests/aws-extensions.yaml`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/dummy_responses.json` & `aws-cfn-update-0.8.2/tests/dummy_responses.json`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_add_new_resources.py` & `aws-cfn-update-0.8.2/tests/test_add_new_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_config_rule_inline_code_updater.py` & `aws-cfn-update-0.8.2/tests/test_config_rule_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_cron_schedule_expression.py` & `aws-cfn-update-0.8.2/tests/test_cron_schedule_expression.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_lambda_inline_code_updater.py` & `aws-cfn-update-0.8.2/tests/test_lambda_inline_code_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_latest_ami_updater.py` & `aws-cfn-update-0.8.2/tests/test_latest_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_oidc_provider_thumbprint_updater.py` & `aws-cfn-update-0.8.2/tests/test_oidc_provider_thumbprint_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_packer_ami_updater.py` & `aws-cfn-update-0.8.2/tests/test_packer_ami_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_remove_resources.py` & `aws-cfn-update-0.8.2/tests/test_remove_resources.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_replace_references.py` & `aws-cfn-update-0.8.2/tests/test_replace_references.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_rest_api_body_updater.py` & `aws-cfn-update-0.8.2/tests/test_rest_api_body_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/test_statemachine_definition_updater.py` & `aws-cfn-update-0.8.2/tests/test_statemachine_definition_updater.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/update_packer/base.py` & `aws-cfn-update-0.8.2/tests/update_packer/base.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/update_packer/call_00001_describe_images/__init__.py` & `aws-cfn-update-0.8.2/tests/update_packer/call_00001_describe_images/__init__.py`

 * *Files identical despite different names*

### Comparing `aws-cfn-update-0.8.1/tests/update_packer/test_update_packer.py` & `aws-cfn-update-0.8.2/tests/update_packer/test_update_packer.py`

 * *Files identical despite different names*

