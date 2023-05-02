# Comparing `tmp/iambic_core-0.4.1.tar.gz` & `tmp/iambic_core-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iambic_core-0.4.1.tar", max compression
+gzip compressed data, was "iambic_core-0.5.1.tar", max compression
```

## Comparing `iambic_core-0.4.1.tar` & `iambic_core-0.5.1.tar`

### file list

```diff
@@ -1,158 +1,158 @@
--rw-r--r--   0        0        0    11356 2023-05-01 22:30:16.826649 iambic_core-0.4.1/LICENSE.md
--rw-r--r--   0        0        0    10551 2023-05-01 22:30:16.826649 iambic_core-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/__init__.py
--rw-r--r--   0        0        0    20099 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/dynamic_config.py
--rw-r--r--   0        0        0      460 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/templates.py
--rw-r--r--   0        0        0     1955 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/utils.py
--rw-r--r--   0        0        0    69560 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/config/wizard.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/core/__init__.py
--rw-r--r--   0        0        0     3010 2023-05-01 22:30:16.858641 iambic_core-0.4.1/iambic/core/aio_utils/__init__.py
--rw-r--r--   0        0        0      290 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/context.py
--rw-r--r--   0        0        0      609 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/exceptions.py
--rw-r--r--   0        0        0    15217 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/git.py
--rw-r--r--   0        0        0      758 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/iambic_enum.py
--rw-r--r--   0        0        0     4592 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/iambic_plugin.py
--rw-r--r--   0        0        0     1685 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/logger.py
--rw-r--r--   0        0        0    24862 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/models.py
--rw-r--r--   0        0        0     1782 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/noq_json.py
--rw-r--r--   0        0        0     5244 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/parser.py
--rw-r--r--   0        0        0    46094 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/template_generation.py
--rw-r--r--   0        0        0    26626 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/core/utils.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/__init__.py
--rw-r--r--   0        0        0      607 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/templates/iambic-detect.yml
--rw-r--r--   0        0        0      654 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/templates/iambic-enforce.yml
--rw-r--r--   0        0        0      658 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/templates/iambic-expire.yml
--rw-r--r--   0        0        0      656 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/templates/iambic-import.yml
--rw-r--r--   0        0        0     1042 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/github/utils.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/lambda/__init__.py
--rw-r--r--   0        0        0     4307 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/lambda/app.py
--rw-r--r--   0        0        0    13644 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/main.py
--rw-r--r--   0        0        0      664 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/filters.py
--rw-r--r--   0        0        0      480 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/markdown.py
--rw-r--r--   0        0        0    12556 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/models.py
--rw-r--r--   0        0        0     4736 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/templates/github_summary.jinja2
--rw-r--r--   0        0        0     1086 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/templates/text_file_summary.jinja2
--rw-r--r--   0        0        0     1082 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/templates/text_screen_summary.jinja2
--rw-r--r--   0        0        0     1040 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/output/text.py
--rw-r--r--   0        0        0     1240 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/README.md
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/__init__.py
--rw-r--r--   0        0        0       62 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
--rw-r--r--   0        0        0     1753 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
--rw-r--r--   0        0        0     2149 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
--rw-r--r--   0        0        0     2276 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
--rw-r--r--   0        0        0     2498 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
--rw-r--r--   0        0        0     1902 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
--rw-r--r--   0        0        0    13572 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
--rw-r--r--   0        0        0      660 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
--rw-r--r--   0        0        0    33240 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/handlers.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
--rw-r--r--   0        0        0    10334 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
--rw-r--r--   0        0        0    17683 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
--rw-r--r--   0        0        0    13616 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
--rw-r--r--   0        0        0     1254 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/models.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
--rw-r--r--   0        0        0    15824 2023-05-01 22:30:16.862640 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
--rw-r--r--   0        0        0    17544 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
--rw-r--r--   0        0        0    10649 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
--rw-r--r--   0        0        0       35 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
--rw-r--r--   0        0        0    16135 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
--rw-r--r--   0        0        0    21304 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
--rw-r--r--   0        0        0    24395 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
--rw-r--r--   0        0        0    14064 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
--rw-r--r--   0        0        0    20623 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
--rw-r--r--   0        0        0    22579 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
--rw-r--r--   0        0        0     4534 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
--rw-r--r--   0        0        0     4968 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
--rw-r--r--   0        0        0    31350 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
--rw-r--r--   0        0        0    20296 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
--rw-r--r--   0        0        0    35369 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
--rw-r--r--   0        0        0    28215 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/models.py
--rw-r--r--   0        0        0     1086 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/sqs/util.py
--rw-r--r--   0        0        0     2973 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/template_generation.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
--rw-r--r--   0        0        0    11950 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
--rw-r--r--   0        0        0     3550 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
--rw-r--r--   0        0        0    10183 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/utils.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
--rw-r--r--   0        0        0    13766 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
--rw-r--r--   0        0        0     3746 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
--rw-r--r--   0        0        0    14891 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
--rw-r--r--   0        0        0     2267 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
--rw-r--r--   0        0        0     1795 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
--rw-r--r--   0        0        0     8455 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/models.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
--rw-r--r--   0        0        0     8648 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
--rw-r--r--   0        0        0     3709 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
--rw-r--r--   0        0        0     7179 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
--rw-r--r--   0        0        0      258 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/utils.py
--rw-r--r--   0        0        0       82 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/README.md
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/__init__.py
--rw-r--r--   0        0        0      413 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/handlers.py
--rw-r--r--   0        0        0      908 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
--rw-r--r--   0        0        0     1514 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_database/models.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
--rw-r--r--   0        0        0     3366 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_file/models.py
--rw-r--r--   0        0        0      284 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/README.md
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/__init__.py
--rw-r--r--   0        0        0    31334 2023-05-01 22:30:16.866639 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/github.py
--rw-r--r--   0        0        0    11851 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/github_app.py
--rw-r--r--   0        0        0     1349 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/handlers.py
--rw-r--r--   0        0        0     1553 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
--rw-r--r--   0        0        0     9806 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
--rw-r--r--   0        0        0     5345 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
--rw-r--r--   0        0        0    14549 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
--rw-r--r--   0        0        0     2030 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
--rw-r--r--   0        0        0     5066 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
--rw-r--r--   0        0        0     4409 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/models.py
--rw-r--r--   0        0        0     1154 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
--rw-r--r--   0        0        0     7852 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
--rw-r--r--   0        0        0    14373 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
--rw-r--r--   0        0        0    11307 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
--rw-r--r--   0        0        0     3020 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
--rw-r--r--   0        0        0     3167 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/__init__.py
--rw-r--r--   0        0        0     9282 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/models.py
--rw-r--r--   0        0        0     3105 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
--rw-r--r--   0        0        0    17906 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/utils.py
--rw-r--r--   0        0        0       91 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/__init__.py
--rw-r--r--   0        0        0    11393 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/models.py
--rw-r--r--   0        0        0     3535 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
--rw-r--r--   0        0        0    20065 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/utils.py
--rw-r--r--   0        0        0     2478 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/handlers.py
--rw-r--r--   0        0        0     2687 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
--rw-r--r--   0        0        0     6720 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/models.py
--rw-r--r--   0        0        0     1085 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/__init__.py
--rw-r--r--   0        0        0     9405 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/models.py
--rw-r--r--   0        0        0     3424 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
--rw-r--r--   0        0        0    13563 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/utils.py
--rw-r--r--   0        0        0     1536 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/utils.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/request_handler/__init__.py
--rw-r--r--   0        0        0      864 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/request_handler/expire_resources.py
--rw-r--r--   0        0        0     4110 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/request_handler/git_apply.py
--rw-r--r--   0        0        0      977 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/request_handler/git_plan.py
--rw-r--r--   0        0        0        0 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/__init__.py
--rw-r--r--   0        0        0      168 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
--rw-r--r--   0        0        0     1069 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/LICENSE
--rw-r--r--   0        0        0      137 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/__init__.py
--rw-r--r--   0        0        0    12636 2023-05-01 22:30:16.870638 iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/main.py
--rw-r--r--   0        0        0     1922 2023-05-01 22:30:16.874637 iambic_core-0.4.1/pyproject.toml
--rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 iambic_core-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-05-02 23:20:35.556413 iambic_core-0.5.1/LICENSE.md
+-rw-r--r--   0        0        0    10551 2023-05-02 23:20:35.556413 iambic_core-0.5.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/config/__init__.py
+-rw-r--r--   0        0        0    20099 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/config/dynamic_config.py
+-rw-r--r--   0        0        0      460 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/config/templates.py
+-rw-r--r--   0        0        0     1955 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/config/utils.py
+-rw-r--r--   0        0        0    71912 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/config/wizard.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/__init__.py
+-rw-r--r--   0        0        0     3010 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/aio_utils/__init__.py
+-rw-r--r--   0        0        0      290 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/context.py
+-rw-r--r--   0        0        0      609 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/exceptions.py
+-rw-r--r--   0        0        0    15217 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/git.py
+-rw-r--r--   0        0        0      758 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/iambic_enum.py
+-rw-r--r--   0        0        0     4592 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/iambic_plugin.py
+-rw-r--r--   0        0        0     1685 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/logger.py
+-rw-r--r--   0        0        0    24862 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/models.py
+-rw-r--r--   0        0        0     1782 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/noq_json.py
+-rw-r--r--   0        0        0     5244 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/parser.py
+-rw-r--r--   0        0        0    46094 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/template_generation.py
+-rw-r--r--   0        0        0    26626 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/core/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/github/__init__.py
+-rw-r--r--   0        0        0      607 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/github/templates/iambic-detect.yml
+-rw-r--r--   0        0        0      654 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/github/templates/iambic-enforce.yml
+-rw-r--r--   0        0        0      658 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/github/templates/iambic-expire.yml
+-rw-r--r--   0        0        0      656 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/github/templates/iambic-import.yml
+-rw-r--r--   0        0        0     1042 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/github/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/lambda/__init__.py
+-rw-r--r--   0        0        0     4307 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/lambda/app.py
+-rw-r--r--   0        0        0    13644 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/main.py
+-rw-r--r--   0        0        0      664 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/output/__init__.py
+-rw-r--r--   0        0        0     2799 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/output/filters.py
+-rw-r--r--   0        0        0      480 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/output/markdown.py
+-rw-r--r--   0        0        0    12556 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/output/models.py
+-rw-r--r--   0        0        0     4736 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/output/templates/github_summary.jinja2
+-rw-r--r--   0        0        0     1086 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/output/templates/text_file_summary.jinja2
+-rw-r--r--   0        0        0     1082 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/output/templates/text_screen_summary.jinja2
+-rw-r--r--   0        0        0     1040 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/output/text.py
+-rw-r--r--   0        0        0     1240 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/plugins/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/plugins/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/plugins/v0_1_0/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.584414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/__init__.py
+-rw-r--r--   0        0        0     1753 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml
+-rw-r--r--   0        0        0     2149 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml
+-rw-r--r--   0        0        0     2276 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml
+-rw-r--r--   0        0        0     2483 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml
+-rw-r--r--   0        0        0     1902 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml
+-rw-r--r--   0        0        0    14846 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/event_bridge/__init__.py
+-rw-r--r--   0        0        0      660 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py
+-rw-r--r--   0        0        0    33240 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/handlers.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/group/__init__.py
+-rw-r--r--   0        0        0    10334 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/group/models.py
+-rw-r--r--   0        0        0    17683 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py
+-rw-r--r--   0        0        0    13616 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py
+-rw-r--r--   0        0        0     1254 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/models.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/policy/__init__.py
+-rw-r--r--   0        0        0    15824 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py
+-rw-r--r--   0        0        0    17544 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py
+-rw-r--r--   0        0        0    10649 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py
+-rw-r--r--   0        0        0       35 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/role/__init__.py
+-rw-r--r--   0        0        0    16135 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/role/models.py
+-rw-r--r--   0        0        0    21304 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py
+-rw-r--r--   0        0        0    24395 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/user/__init__.py
+-rw-r--r--   0        0        0    14064 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/user/models.py
+-rw-r--r--   0        0        0    20623 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py
+-rw-r--r--   0        0        0    22579 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py
+-rw-r--r--   0        0        0     4534 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py
+-rw-r--r--   0        0        0     4968 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/__init__.py
+-rw-r--r--   0        0        0    31619 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py
+-rw-r--r--   0        0        0    20296 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py
+-rw-r--r--   0        0        0    35514 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py
+-rw-r--r--   0        0        0    28308 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/models.py
+-rw-r--r--   0        0        0     1086 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/sqs/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/sqs/util.py
+-rw-r--r--   0        0        0     2973 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/template_generation.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/tests/__init__.py
+-rw-r--r--   0        0        0    11950 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py
+-rw-r--r--   0        0        0     3550 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/tests/test_models.py
+-rw-r--r--   0        0        0    10183 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/group/__init__.py
+-rw-r--r--   0        0        0    13766 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/group/models.py
+-rw-r--r--   0        0        0     3746 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py
+-rw-r--r--   0        0        0    14891 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py
+-rw-r--r--   0        0        0     2267 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/handlers.py
+-rw-r--r--   0        0        0     1795 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py
+-rw-r--r--   0        0        0     8515 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/models.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.588414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/user/__init__.py
+-rw-r--r--   0        0        0     8648 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/user/models.py
+-rw-r--r--   0        0        0     3709 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py
+-rw-r--r--   0        0        0     7179 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py
+-rw-r--r--   0        0        0      258 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/utils.py
+-rw-r--r--   0        0        0       82 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/example/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/example/__init__.py
+-rw-r--r--   0        0        0      413 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/example/handlers.py
+-rw-r--r--   0        0        0      908 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/example/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/example/local_database/__init__.py
+-rw-r--r--   0        0        0     1514 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/example/local_database/models.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/example/local_file/__init__.py
+-rw-r--r--   0        0        0     3366 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/example/local_file/models.py
+-rw-r--r--   0        0        0      284 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/github/README.md
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/github/__init__.py
+-rw-r--r--   0        0        0    31334 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/github/github.py
+-rw-r--r--   0        0        0    11851 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/github/github_app.py
+-rw-r--r--   0        0        0     1349 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/github/handlers.py
+-rw-r--r--   0        0        0     1553 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/github/iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/group/__init__.py
+-rw-r--r--   0        0        0     9806 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/group/models.py
+-rw-r--r--   0        0        0     5345 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py
+-rw-r--r--   0        0        0    14549 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py
+-rw-r--r--   0        0        0     2030 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/handlers.py
+-rw-r--r--   0        0        0     5247 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py
+-rw-r--r--   0        0        0     4409 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/models.py
+-rw-r--r--   0        0        0     1154 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/__init__.py
+-rw-r--r--   0        0        0     7852 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py
+-rw-r--r--   0        0        0    14373 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py
+-rw-r--r--   0        0        0    11307 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py
+-rw-r--r--   0        0        0     3020 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py
+-rw-r--r--   0        0        0     3167 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/app/__init__.py
+-rw-r--r--   0        0        0     9282 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/app/models.py
+-rw-r--r--   0        0        0     3105 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/app/template_generation.py
+-rw-r--r--   0        0        0    17906 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/app/utils.py
+-rw-r--r--   0        0        0       91 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/group/__init__.py
+-rw-r--r--   0        0        0    11393 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/group/models.py
+-rw-r--r--   0        0        0     3535 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/group/template_generation.py
+-rw-r--r--   0        0        0    20065 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/group/utils.py
+-rw-r--r--   0        0        0     2478 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/handlers.py
+-rw-r--r--   0        0        0     2685 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py
+-rw-r--r--   0        0        0     6720 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/models.py
+-rw-r--r--   0        0        0     1085 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/user/__init__.py
+-rw-r--r--   0        0        0     9492 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/user/models.py
+-rw-r--r--   0        0        0     3424 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/user/template_generation.py
+-rw-r--r--   0        0        0    13610 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/user/utils.py
+-rw-r--r--   0        0        0     1536 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/utils.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/request_handler/__init__.py
+-rw-r--r--   0        0        0      864 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/request_handler/expire_resources.py
+-rw-r--r--   0        0        0     4110 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/request_handler/git_apply.py
+-rw-r--r--   0        0        0      977 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/request_handler/git_plan.py
+-rw-r--r--   0        0        0        0 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/vendor/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/vendor/lambda_multiprocessing/ATTRIBUTION
+-rw-r--r--   0        0        0     1069 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/vendor/lambda_multiprocessing/LICENSE
+-rw-r--r--   0        0        0      137 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/vendor/lambda_multiprocessing/__init__.py
+-rw-r--r--   0        0        0    12636 2023-05-02 23:20:35.592414 iambic_core-0.5.1/iambic/vendor/lambda_multiprocessing/main.py
+-rw-r--r--   0        0        0     1922 2023-05-02 23:20:35.596414 iambic_core-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0    12874 1970-01-01 00:00:00.000000 iambic_core-0.5.1/PKG-INFO
```

### Comparing `iambic_core-0.4.1/LICENSE.md` & `iambic_core-0.5.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/README.md` & `iambic_core-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/config/dynamic_config.py` & `iambic_core-0.5.1/iambic/config/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/config/utils.py` & `iambic_core-0.5.1/iambic/config/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/config/wizard.py` & `iambic_core-0.5.1/iambic/config/wizard.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 import json
 import os
 import re
 import select
 import sys
 import uuid
 from enum import Enum
+from pathlib import Path
 from textwrap import dedent
-from typing import Union
+from typing import Optional, Union
 
 import boto3
 import questionary
 from aws_error_utils.aws_error_utils import errors
 from botocore.exceptions import ClientError, NoCredentialsError
 from pydantic.json import pydantic_encoder
 from pydantic.types import SecretStr
@@ -44,15 +45,14 @@
     create_iambic_eventbridge_stacks,
     create_iambic_role_stacks,
     create_spoke_role_stack,
 )
 from iambic.plugins.v0_1_0.aws.handlers import apply as aws_apply
 from iambic.plugins.v0_1_0.aws.handlers import import_aws_resources
 from iambic.plugins.v0_1_0.aws.handlers import load as aws_load
-from iambic.plugins.v0_1_0.aws.iam.policy.models import PolicyDocument, PolicyStatement
 from iambic.plugins.v0_1_0.aws.iam.role.models import (
     AWS_IAM_ROLE_TEMPLATE_TYPE,
     AwsIamRoleTemplate,
 )
 from iambic.plugins.v0_1_0.aws.iambic_plugin import AWSConfig
 from iambic.plugins.v0_1_0.aws.models import (
     ARN_RE,
@@ -78,14 +78,17 @@
     GoogleProject,
     GoogleSubject,
     GoogleWorkspaceConfig,
 )
 from iambic.plugins.v0_1_0.okta.handlers import import_okta_resources
 from iambic.plugins.v0_1_0.okta.iambic_plugin import OktaConfig, OktaOrganization
 
+AWS_SECRETS = "AWS Secrets"
+LOCALLY = "Locally"
+
 CUSTOM_AUTO_COMPLETE_STYLE = questionary.Style(
     [
         ("answer", "fg:#0A886A"),
         ("selected", "bold bg:#000000"),
     ]
 )
 
@@ -178,25 +181,49 @@
             log.warning(
                 "The role ARN must be a valid ARN for the account you are configuring.",
                 expected_account_id=account_id,
                 provided_role_arn=role_arn,
             )
 
 
+def set_aws_is_read_only() -> bool:
+    return not bool(
+        questionary.confirm(
+            "Grant IambicSpokeRole write access to IAM and IdentityCenter?\n"
+            "If set to 'no', this will limit IAMbic's capabilities to import-only.",
+            default=True,
+        ).unsafe_ask()
+    )
+
+
 def set_required_text_value(human_readable_name: str, default_val: str = None):
     while True:
         if response := questionary.text(
             human_readable_name,
             default=default_val or "",
         ).unsafe_ask():
             return response
         else:
             print("Please enter a valid response.")
 
 
+def set_required_secure_text_value(
+    human_readable_name: str,
+    default_val: Optional[SecretStr] = None,
+):
+    while True:
+        if response := questionary.text(
+            human_readable_name,
+            default=SecretStr(default_val or "").get_secret_value(),
+        ).unsafe_ask():
+            return SecretStr(response.replace("\\n", "\n"))
+        else:
+            print("Please enter a valid response.")
+
+
 def set_idp_name(default_val: str = None):
     return set_required_text_value("What is the Identity Provider Name?", default_val)
 
 
 def set_tenant_id(default_val: str = None):
     return set_required_text_value("What is the Tenant ID?", default_val)
 
@@ -232,16 +259,16 @@
     )
 
 
 def set_google_project_id(default_val: str = None):
     return set_required_text_value("What is the Project ID?", default_val)
 
 
-def set_google_private_key(default_val: str = None):
-    return set_required_text_value("What is the Private Key?", default_val)
+def set_google_private_key(default_val: SecretStr = None):
+    return set_required_secure_text_value("What is the Private Key?", default_val)
 
 
 def set_google_private_key_id(default_val: str = None):
     return set_required_text_value("What is the Private Key ID?", default_val)
 
 
 def set_google_client_email(default_val: str = None):
@@ -305,96 +332,38 @@
             log.info("Exiting...")
             sys.exit(0)
 
 
 class ConfigurationWizard:
     def __init__(self, repo_dir: str):
         # TODO: Handle the case where the config file exists but is not valid
-        self.default_region = "us-east-1"
-        try:
-            self.boto3_session = boto3.Session(region_name=self.default_region)
-        except Exception as exc:
-            log.error(f"Unable to access your AWS account: {exc}")
-            sys.exit(1)
-
-        self.autodetected_org_settings = {}
         self.existing_role_template_map = {}
         self.aws_account_map = {}
         self.repo_dir = repo_dir
         self._has_cf_permissions = None
         self._cf_role_arn = None
         self._assume_as_arn = None
         self.caller_identity = {}
         self.profile_name = ""
+        self._default_region = None
 
         asyncio.run(self.set_config_details())
 
-        if self.config.aws:
-            self.hub_account_id = self.config.aws.hub_role_arn.split(":")[4]
-            self.spoke_role_is_read_only = self.config.aws.spoke_role_is_read_only
-        else:
-            self.hub_account_id = None
-
-        try:
-            default_caller_identity = self.boto3_session.client(
-                "sts"
-            ).get_caller_identity()
-            caller_arn = get_identity_arn(default_caller_identity)
-            default_hub_account_id = caller_arn.split(":")[4]
-        except (
-            AttributeError,
-            IndexError,
-            NoCredentialsError,
-            ClientError,
-            FileNotFoundError,
-        ):
-            default_hub_account_id = None
-            default_caller_identity = {}
-
-        if not self.hub_account_id:
-            while True:
-                self.hub_account_id = set_required_text_value(
-                    "To get started with the IAMbic setup wizard, you'll need an AWS account.\n"
-                    "This is where IAMbic will deploy its main role. If you have an AWS Organization, "
-                    "that account will be your hub account.\n"
-                    "Review to-be-created IAMbic roles at https://docs.iambic.org/reference/aws_hub_and_spoke_roles\n"
-                    "Which Account ID should we use to deploy the IAMbic hub role?",
-                    default_val=default_hub_account_id,
-                )
-                if is_valid_account_id(self.hub_account_id):
-                    break
-
-        if self.hub_account_id == default_hub_account_id:
-            identity_arn = get_identity_arn(default_caller_identity)
-            if questionary.confirm(
-                f"IAMbic detected you are using {identity_arn} for AWS access.\n"
-                f"This identity will require the ability to create"
-                f"CloudFormation stacks, stack sets, and stack set instances.\n"
-                f"Would you like to use this identity?"
-            ).ask():
-                self.caller_identity = default_caller_identity
-            else:
-                self.set_boto3_session()
-        else:
-            self.set_boto3_session()
-
-        asyncio.run(self.sync_config_aws_org())
-
         log.debug("Starting configuration wizard", config_path=self.config_path)
 
     @property
     def has_cf_permissions(self):
         if self._has_cf_permissions is None:
             try:
                 self._has_cf_permissions = questionary.confirm(
                     f"This requires that you have the ability to "
                     f"create CloudFormation stacks, stack sets, and stack set instances.\n"
                     f"If you are using an AWS Organization, be sure that trusted access is enabled.\n"
                     f"You can check this using the AWS Console:\n  "
-                    f"https://{self.default_region}.console.aws.amazon.com/organizations/v2/home/services/CloudFormation%20StackSets\n"
+                    f"https://{self.aws_default_region}.console.aws.amazon.com/organizations/v2/home/services/CloudFormation%20StackSets\n"
                     f"Proceed?"
                 ).unsafe_ask()
             except KeyboardInterrupt:
                 log.info("Exiting...")
                 sys.exit(0)
 
         return self._has_cf_permissions
@@ -414,14 +383,79 @@
     @property
     def cf_role_arn(self):
         if self._cf_role_arn is None:
             self._cf_role_arn = set_aws_role_arn(self.hub_account_id)
 
         return self._cf_role_arn
 
+    @property
+    def has_aws_account_or_organizations(self) -> bool:
+        return self.config.aws and (
+            self.config.aws.accounts or self.config.aws.organizations
+        )
+
+    @property
+    def aws_default_region(self) -> str:
+        default_val = RegionName.us_east_1.value
+
+        if self._default_region:
+            return self._default_region
+        elif self.has_aws_account_or_organizations:
+            if self.config.aws.organizations:
+                self._default_region = self.config.aws.organizations[0].region_name
+            else:
+                hub_account = [
+                    account
+                    for account in self.config.aws.accounts
+                    if account.hub_role_arn
+                ]
+                if hub_account:
+                    self._default_region = hub_account[0].region_name
+                else:
+                    self._default_region = set_aws_region(
+                        "What region should IAMbic use?", default_val
+                    )
+        else:
+            self._default_region = set_aws_region(
+                "What region should IAMbic use?", default_val
+            )
+
+        return self._default_region
+
+    @property
+    def secrets_message(self) -> tuple[str, bool]:
+        """Returns if secrets are configured"""
+        secret_in_config = bool(self.config.extends)
+
+        if (
+            secret_in_config
+            and self.config.extends[0].key == ExtendsConfigKey.AWS_SECRETS_MANAGER
+        ):
+            secret_question_text = (
+                "This requires the ability to update the AWS Secrets Manager secret."
+            )
+        elif (
+            secret_in_config
+            and self.config.extends[0].key == ExtendsConfigKey.LOCAL_FILE
+        ):
+            secret_question_text = (
+                "This requires permissions to update secrets in your secrets file."
+            )
+        else:
+            secret_question_text = "Secrets must be created."
+
+        return (secret_question_text, secret_in_config)
+
+    @property
+    def has_okta_configured(self) -> bool:
+        return self.config.okta and self.config.okta.organizations
+
+    def secret_config_dir(self, secrets_file: str = "secrets.yaml") -> str:
+        return f"{Path(self.config_path).parent.joinpath(secrets_file)}"
+
     async def set_config_details(self):
         try:
             self.config_path = str((await resolve_config_template_path(self.repo_dir)))
         except RuntimeError:
             self.config_path = f"{self.repo_dir}/iambic_config.yaml"
 
         if os.path.exists(self.config_path) and os.path.getsize(self.config_path) != 0:
@@ -442,19 +476,14 @@
                 file_path=self.config_path, version=CURRENT_IAMBIC_VERSION
             )
 
             self.config = await process_config(
                 base_config, self.config_path, base_config.dict()
             )
 
-        with contextlib.suppress(ClientError, NoCredentialsError, FileNotFoundError):
-            self.autodetected_org_settings = self.boto3_session.client(
-                "organizations"
-            ).describe_organization()["Organization"]
-
     def resolve_aws_profile_defaults_from_env(self) -> str:
         if "AWS_ACCESS_KEY_ID" in os.environ:
             # Environment variables has 1st priority
             profile_name = "None"
             log.info("Using AWS credentials from environment", profile=profile_name)
         elif profile_name := os.environ.get("AWS_PROFILE"):
             # Explicit profile has 2nd priority
@@ -473,15 +502,16 @@
 
         return profile_name
 
     def set_aws_profile_name(
         self, question_text: str = None, allow_none: bool = False
     ) -> Union[str, None]:
         questionary_params = {}
-        available_profiles = self.boto3_session.available_profiles
+        boto3_session = boto3.Session(region_name=self.aws_default_region)
+        available_profiles = boto3_session.available_profiles
         if allow_none:
             available_profiles.insert(0, "None")
 
         default_profile = self.resolve_aws_profile_defaults_from_env()
         if default_profile != "None":
             questionary_params["default"] = default_profile
             available_profiles.append(default_profile)
@@ -523,18 +553,18 @@
 
     def set_boto3_session(self):
         self._has_cf_permissions = True
         while True:
             try:
                 profile_name = self.set_aws_profile_name()
                 self.boto3_session = boto3.Session(
-                    profile_name=profile_name, region_name=self.default_region
+                    profile_name=profile_name, region_name=self.aws_default_region
                 )
                 self.caller_identity = self.boto3_session.client(
-                    "sts"
+                    "sts", region_name=self.aws_default_region
                 ).get_caller_identity()
                 selected_hub_account_id = self.caller_identity.get("Arn").split(":")[4]
                 if selected_hub_account_id != self.hub_account_id:
                     log.error(
                         "The selected profile does not have access to the Hub Account. Please try again.",
                         required_account_id=self.hub_account_id,
                         selected_account_id=selected_hub_account_id,
@@ -574,20 +604,23 @@
                 continue
 
             self.profile_name = profile_name
             with contextlib.suppress(
                 ClientError, NoCredentialsError, FileNotFoundError
             ):
                 self.autodetected_org_settings = self.boto3_session.client(
-                    "organizations"
+                    "organizations", region_name=self.aws_default_region
                 ).describe_organization()["Organization"]
             break
 
-    def get_boto3_session_for_account(self, account_id: str):
+    def get_boto3_session_for_account(self, account_id: str, region_name: str = None):
         # This need to follow standard credentials provider chain
+        if not region_name:
+            region_name = self.aws_default_region
+
         if account_id == self.hub_account_id:
             if not self.profile_name:
                 if os.getenv("AWS_ACCESS_KEY_ID"):
                     # environment variables credentials detected
                     self.profile_name = None
                 elif profile_name := os.getenv("AWS_PROFILE"):
                     self.profile_name = profile_name
@@ -603,17 +636,15 @@
                 "If None is selected the AWS Account will be skipped.",
                 allow_none=True,
             )
             if not profile_name:
                 log.info("Unable to add the AWS Account without a session.")
                 return None, None
             return (
-                boto3.Session(
-                    profile_name=profile_name, region_name=self.default_region
-                ),
+                boto3.Session(profile_name=profile_name, region_name=region_name),
                 profile_name,
             )
 
     async def run_import_aws_resources(self):
         log.info("Importing AWS identities")
         current_command = ctx.command
         ctx.command = Command.IMPORT
@@ -658,15 +689,15 @@
             await aws_apply(exe_message, sub_config, load_templates(templates))
             ctx.command = current_command
 
         await self.run_import_aws_resources()
 
     async def sync_config_aws_org(self, run_config_discovery: bool = True):
         if not self.config.aws:
-            return
+            self.config.aws = AWSConfig()
 
         self.aws_account_map = {}
         current_command = ctx.command
 
         try:
             if run_config_discovery:
                 exe_message = ExecutionMessage(
@@ -768,31 +799,26 @@
         )
 
         if is_hub_account:
             account_id = self.hub_account_id
             account_name = set_required_text_value(
                 "What is the name of the AWS Account?"
             )
+            default_region = self.aws_default_region
             if not questionary.confirm(
                 "Create required Hub and Spoke roles via CloudFormation?\n"
                 "The templates that will be used can be found here:\n"
                 "  https://github.com/noqdev/iambic/tree/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates"
             ).unsafe_ask():
                 log.info(
                     "Unable to add the AWS Account without creating the required roles."
                 )
                 return
 
-            self.config.aws.spoke_role_is_read_only = bool(
-                questionary.confirm(
-                    "Do you want to restrict IambicSpokeRole to read-only IAM and IdentityCenter service?\n"
-                    "This will limit IAMbic capability to import",
-                    default=False,
-                ).unsafe_ask()
-            )
+            self.config.aws.spoke_role_is_read_only = set_aws_is_read_only()
 
         else:
             if requires_sync:
                 if not questionary.confirm(
                     "Adding this account will require a sync to be run.\n"
                     "This is to apply any matching templates to the account if the resource does not already exist.\n"
                     "Then, the account resources will be imported into Iambic.\n"
@@ -812,35 +838,41 @@
             if not is_valid_account_id(account_id):
                 log.info("Invalid AWS Account ID")
                 return
             elif account_id in list(self.aws_account_map.keys()):
                 log.info("AWS Account already exists in the configuration")
                 return
 
+            default_region = set_aws_region(
+                "What region should IAMbic use?", self.aws_default_region
+            )
+
             if not questionary.confirm(
                 "Create required Spoke role via CloudFormation?\n"
                 "The template that will be used can be found here:\n"
                 "  https://github.com/noqdev/iambic/blob/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml"
             ).unsafe_ask():
                 log.info(
                     "Unable to add the AWS account without creating the required role."
                 )
                 return
 
         read_only = self.config.aws.spoke_role_is_read_only
-        session, profile_name = self.get_boto3_session_for_account(account_id)
+        session, profile_name = self.get_boto3_session_for_account(
+            account_id, region_name=default_region
+        )
         if not session:
             return
 
         if is_hub_account and not profile_name:
             profile_name = self.profile_name
         elif not is_hub_account:
             profile_name = None
 
-        cf_client = session.client("cloudformation")
+        cf_client = session.client("cloudformation", region_name=default_region)
         role_arn = set_aws_role_arn(account_id)
 
         if is_hub_account:
             created_successfully = asyncio.run(
                 create_iambic_role_stacks(
                     cf_client=cf_client,
                     hub_account_id=account_id,
@@ -869,14 +901,15 @@
 
         account = AWSAccount(
             account_id=account_id,
             account_name=account_name,
             spoke_role_arn=get_spoke_role_arn(account_id, read_only=read_only),
             iambic_managed=IambicManaged.READ_AND_WRITE,
             aws_profile=profile_name,
+            default_region=default_region,
         )
         if is_hub_account:
             account.hub_role_arn = get_hub_role_arn(account_id)
         # account.partition = set_aws_account_partition(account.partition)
 
         confirm_command_exe("AWS Account", Operation.ADDED, requires_sync=requires_sync)
 
@@ -923,39 +956,95 @@
                 "No editable accounts found.\n"
                 "TIP: An AWS account cannot be edited if it attached to an Organization in the config."
             )
             return
         else:
             account = self.config.aws.accounts[0]
 
-        choices = ["Go back", "Update IAMbic control"]
+        choices = ["Go back", "Update IAMbic control", "Update Region"]
         if not account.org_id:
             choices.append("Update name")
 
         while True:
             action = questionary.select(
                 "What would you like to do?",
                 choices=choices,
             ).unsafe_ask()
             if action == "Go back":
                 return
             elif action == "Update name":
+                account.default_region = set_aws_region(
+                    "What region should IAMbic use?", account.default_region
+                )
+            elif action == "Update name":
                 account.account_name = questionary.text(
                     "What is the name of the AWS Account?",
                     default=account.account_name,
                 ).unsafe_ask()
 
             confirm_command_exe("AWS Account", Operation.UPDATED)
 
             self.config.aws.accounts[
                 account_id_to_config_elem_map[account.account_id]
             ] = account
             asyncio.run(self.run_import_aws_resources())
             self.config.write()
 
+    def setup_aws_configuration(self):
+        if self.has_aws_account_or_organizations:
+            self.hub_account_id = self.config.aws.hub_role_arn.split(":")[4]
+            self.spoke_role_is_read_only = self.config.aws.spoke_role_is_read_only
+        else:
+            self.hub_account_id = None
+
+        try:
+            default_caller_identity = self.boto3_session.client(
+                "sts", region_name=self.aws_default_region
+            ).get_caller_identity()
+            caller_arn = get_identity_arn(default_caller_identity)
+            default_hub_account_id = caller_arn.split(":")[4]
+        except (
+            AttributeError,
+            IndexError,
+            NoCredentialsError,
+            ClientError,
+            FileNotFoundError,
+        ):
+            default_hub_account_id = None
+            default_caller_identity = {}
+
+        if not self.hub_account_id:
+            while True:
+                self.hub_account_id = set_required_text_value(
+                    "To get started with the IAMbic setup wizard, you'll need an AWS account.\n"
+                    "This is where IAMbic will deploy its main role. If you have an AWS Organization, "
+                    "that account will be your hub account.\n"
+                    "Review to-be-created IAMbic roles at https://docs.iambic.org/reference/aws_hub_and_spoke_roles\n"
+                    "Which Account ID should we use to deploy the IAMbic hub role?",
+                    default_val=default_hub_account_id,
+                )
+                if is_valid_account_id(self.hub_account_id):
+                    break
+
+        if self.hub_account_id == default_hub_account_id:
+            identity_arn = get_identity_arn(default_caller_identity)
+            if questionary.confirm(
+                f"IAMbic detected you are using {identity_arn} for AWS access.\n"
+                f"This identity will require the ability to create"
+                f"CloudFormation stacks, stack sets, and stack set instances.\n"
+                f"Would you like to use this identity?"
+            ).ask():
+                self.caller_identity = default_caller_identity
+            else:
+                self.set_boto3_session()
+        else:
+            self.set_boto3_session()
+
+        asyncio.run(self.sync_config_aws_org())
+
     def configuration_wizard_aws_accounts(self):
         while True:
             if self.config.aws and self.config.aws.accounts:
                 action = questionary.select(
                     "What would you like to do?",
                     choices=["Go back", "Add AWS Account", "Edit AWS Account"],
                 ).unsafe_ask()
@@ -990,22 +1079,27 @@
         else:
             org_to_edit = self.config.aws.organizations[0]
 
         choices = [
             "Go back",
             "Update IdentityCenter",
             "Update IAMbic control",
+            "Update Region",
         ]
         while True:
             action = questionary.select(
                 "What would you like to do?",
                 choices=choices,
             ).unsafe_ask()
             if action == "Go back":
                 return
+            elif action == "Update Region":
+                org_to_edit.default_region = set_aws_region(
+                    "What region should IAMbic use?", org_to_edit.default_region
+                )
             elif action == "Update IdentityCenter":
                 org_to_edit.identity_center = set_identity_center()
                 asyncio.run(self.sync_config_aws_org(False))
 
             confirm_command_exe("AWS Organization", Operation.UPDATED)
             self.config.aws.organizations[
                 org_id_to_config_elem_map[org_to_edit.org_id]
@@ -1015,16 +1109,15 @@
     def configuration_wizard_aws_organizations_add(self):
         if not self.has_cf_permissions:
             log.info(
                 "Unable to edit this attribute without CloudFormation permissions."
             )
             return
 
-        org_region = "us-east-1"  # Orgs are only available in us-east-1
-        org_console_url = f"https://{org_region}.console.aws.amazon.com/organizations/v2/home/accounts"
+        org_console_url = f"https://{self.aws_default_region}.console.aws.amazon.com/organizations/v2/home/accounts"
         org_id = questionary.text(
             f"What is the AWS Organization ID? It can be found here {org_console_url}",
             default=self.autodetected_org_settings.get("Id", ""),
         ).unsafe_ask()
 
         account_id = self.hub_account_id
         session, profile_name = self.get_boto3_session_for_account(account_id)
@@ -1035,44 +1128,43 @@
             "Create required Hub and Spoke roles via CloudFormation?\n"
             "The templates that will be used can be found here:\n"
             "  https://github.com/noqdev/iambic/tree/main/iambic/plugins/v0_1_0/aws/cloud_formation/templates"
         ).unsafe_ask():
             log.info("Unable to add the AWS Org without creating the required roles.")
             return
 
-        read_only = bool(
-            questionary.confirm(
-                "Do you want to restrict IambicSpokeRole to read-only IAM and IdentityCenter service?\n"
-                "This will limit IAMbic capability to import",
-                default=False,
-            ).unsafe_ask()
-        )
+        read_only = set_aws_is_read_only()
         self.config.aws.spoke_role_is_read_only = read_only
 
         created_successfully = asyncio.run(
             create_iambic_role_stacks(
-                cf_client=session.client("cloudformation"),
+                cf_client=session.client(
+                    "cloudformation", region_name=self.aws_default_region
+                ),
                 hub_account_id=account_id,
                 assume_as_arn=self.assume_as_arn,
                 role_arn=self.cf_role_arn,
-                org_client=session.client("organizations"),
+                org_client=session.client(
+                    "organizations", region_name=self.aws_default_region
+                ),
                 read_only=read_only,
             )
         )
         if not created_successfully:
             log.error("Failed to create the required IAMbic roles. Exiting.")
             sys.exit(0)
 
         aws_org = AWSOrganization(
             org_id=org_id,
             org_account_id=account_id,
             default_rule=BaseAWSOrgRule(),
             hub_role_arn=get_hub_role_arn(account_id),
             aws_profile=profile_name,
             spoke_role_is_read_only=read_only,
+            default_region=self.aws_default_region,
         )
         aws_org.default_rule.iambic_managed = IambicManaged.READ_AND_WRITE
 
         self.config.aws.organizations.append(aws_org)
 
         log.debug("Attempting to get a session on the AWS org", org_id=org_id)
         try:
@@ -1120,98 +1212,159 @@
         ).unsafe_ask():
             if self.config.aws and self.config.aws.organizations:
                 self.configuration_wizard_aws_organizations_edit()
             else:
                 self.configuration_wizard_aws_organizations_add()
 
     def configuration_wizard_aws(self):
+        self.setup_aws_configuration()
+
         while True:
             action = questionary.select(
                 "What would you like to configure in AWS?\n"
                 "We recommend configuring IAMbic with AWS Organizations, "
                 "but you may also manually configure accounts.",
                 choices=["Go back", "AWS Organizations", "AWS Accounts"],
             ).unsafe_ask()
             if action == "Go back":
                 return
             elif action == "AWS Organizations":
                 self.configuration_wizard_aws_organizations()
             elif action == "AWS Accounts":
                 self.configuration_wizard_aws_accounts()
 
-    def create_secret(self):
-        region = set_aws_region(
-            "What region should the secret be created in?",
-            self.default_region,
-        )
-
-        question_text = "Create the secret"
-        role_name = IAMBIC_SPOKE_ROLE_NAME
-        role_account_id = self.hub_account_id
-
-        if not questionary.confirm(f"{question_text}?").unsafe_ask():
-            self.config.secrets = {}
-            return
-
-        if role_name and (aws_account := self.aws_account_map.get(role_account_id)):
-            session = asyncio.run(aws_account.get_boto3_session(region_name=region))
-        else:
-            session = boto3.Session(region_name=region)
-
-        client = session.client(service_name="secretsmanager")
-        response = client.create_secret(
-            Name=f"iambic-config-secrets-{str(uuid.uuid4())}",
-            Description="IAMbic managed secret used to store protected config values",
-            SecretString=yaml.dump({"secrets": self.config.secrets}),
-        )
-
-        self.config.extends = [
-            ExtendsConfig(
-                key=ExtendsConfigKey.AWS_SECRETS_MANAGER,
-                value=response["ARN"],
-                assume_role_arn=get_spoke_role_arn(
-                    self.hub_account_id, read_only=self.spoke_role_is_read_only
-                ),
-            )
-        ]
-        self.config.write()
-
-    def update_secret(self):
+    def upsert_secret(self):
         if not self.config.secrets:
             self.config.secrets = {}
 
         if self.config.okta:
             self.config.secrets["okta"] = get_secret_dict_with_val(
-                self.config.okta, exclude={"client"}
+                self.config.okta,
+                exclude={"organizations": {"__all__": {"client"}}},
+                exclude_unset=True,
             )
 
         if self.config.azure_ad:
             self.config.secrets["azure_ad"] = get_secret_dict_with_val(
-                self.config.azure_ad
+                self.config.azure_ad, exclude_unset=True
             )
 
         if self.config.google_workspace:
             self.config.secrets["google_workspace"] = get_secret_dict_with_val(
-                self.config.google_workspace, exclude={"_service_connection_map"}
+                self.config.google_workspace,
+                exclude={"_service_connection_map"},
+                exclude_unset=True,
             )
+
+        if len(self.config.extends) == 0:
+            self.create_secret()
+        else:
+            self.update_secret()
+
+    def create_secret(self):
+        response = None
+
+        if len(self.config.extends) == 0:
+            if self.aws_account_map:
+                response = questionary.select(
+                    "Where do you want to store your secrets?",
+                    choices=[
+                        LOCALLY,
+                        AWS_SECRETS,
+                    ],
+                ).ask()
+            else:
+                # TODO: ask if they want to create the file
+                response = LOCALLY
+        elif self.config.extends[0].key == ExtendsConfigKey.AWS_SECRETS_MANAGER:
+            response = AWS_SECRETS
+        elif self.config.extends[0].key == ExtendsConfigKey.LOCAL_FILE:
+            response = LOCALLY
+
+        if response == AWS_SECRETS:
+            region = set_aws_region(
+                "What region should the secret be created in?",
+                self.aws_default_region,
+            )
+
+            question_text = "Create the secret"
+            role_name = IAMBIC_SPOKE_ROLE_NAME
+            role_account_id = self.hub_account_id
+
+            if not questionary.confirm(f"{question_text}?").unsafe_ask():
+                self.config.secrets = {}
+                return
+
+            if role_name and (aws_account := self.aws_account_map.get(role_account_id)):
+                session = asyncio.run(aws_account.get_boto3_session(region_name=region))
+            else:
+                session = boto3.Session(region_name=region)
+
+            client = session.client(service_name="secretsmanager", region_name=region)
+            response = client.create_secret(
+                Name=f"iambic-config-secrets-{str(uuid.uuid4())}",
+                Description="IAMbic managed secret used to store protected config values",
+                SecretString=yaml.dump({"secrets": self.config.secrets}),
+            )
+
+            self.config.extends = [
+                ExtendsConfig(
+                    key=ExtendsConfigKey.AWS_SECRETS_MANAGER,
+                    value=response["ARN"],
+                    assume_role_arn=get_spoke_role_arn(
+                        self.hub_account_id, read_only=self.spoke_role_is_read_only
+                    ),
+                )  # type: ignore
+            ]
+            self.config.write()
+        elif response == LOCALLY:
+            # TODO: add check to gitignore the file
+            with open(self.secret_config_dir(), "w") as f:
+                f.write(yaml.dump({"secrets": self.config.secrets}))  # type: ignore
+
+            self.config.extends = [
+                ExtendsConfig(
+                    key=ExtendsConfigKey.LOCAL_FILE,
+                    value="secrets.yaml",
+                )  # type: ignore
+            ]
+
+            self.config.write()
+
+    def update_secret(self):
+        response = None
+
+        if self.config.extends[0].key == ExtendsConfigKey.AWS_SECRETS_MANAGER:
+            response = AWS_SECRETS
+        elif self.config.extends[0].key == ExtendsConfigKey.LOCAL_FILE:
+            response = LOCALLY
+
         secret_details = self.config.extends[0]
-        secret_arn = secret_details.value
-        region = secret_arn.split(":")[3]
-        secret_account_id = secret_arn.split(":")[4]
-
-        if aws_account := self.aws_account_map.get(secret_account_id):
-            session = asyncio.run(aws_account.get_boto3_session(region_name=region))
-        else:
-            session = boto3.Session(region_name=region)
-
-        client = session.client(service_name="secretsmanager")
-        client.put_secret_value(
-            SecretId=secret_arn,
-            SecretString=yaml.dump({"secrets": self.config.secrets}),
-        )
+
+        if response == AWS_SECRETS:
+            secret_arn = secret_details.value
+            region = secret_arn.split(":")[3]
+            secret_account_id = secret_arn.split(":")[4]
+
+            if aws_account := self.aws_account_map.get(secret_account_id):
+                session = asyncio.run(aws_account.get_boto3_session(region_name=region))
+            else:
+                session = boto3.Session(region_name=region)
+
+            client = session.client(service_name="secretsmanager", region_name=region)
+            client.put_secret_value(
+                SecretId=secret_arn,
+                SecretString=yaml.dump({"secrets": self.config.secrets}),
+            )
+        elif response == LOCALLY:
+            secrets_config_path = self.secret_config_dir(secret_details.value)
+            with open(secrets_config_path, "w") as f:
+                f.write(yaml.dump({"secrets": self.config.secrets}))  # type: ignore
+
+            self.config.write()
 
     def configuration_wizard_google_workspace_add(self):
         google_obj = {
             "subjects": [set_google_subject()],
             "type": set_google_project_type(),
             "project_id": set_google_project_id(),
             "private_key_id": set_google_private_key_id(),
@@ -1222,40 +1375,23 @@
             "token_uri": set_google_token_uri(),
             "auth_provider_x509_cert_url": set_google_auth_provider_cert_url(),
             "client_x509_cert_url": set_google_client_cert_url(),
         }
 
         confirm_command_exe("Google Workspace", Operation.ADDED)
 
-        if self.config.secrets:
-            if self.config.google_workspace:
-                self.config.google_workspace.workspaces.append(
-                    GoogleProject(**google_obj)
-                )
-            else:
-                self.config.google_workspace = GoogleWorkspaceConfig(
-                    workspaces=[
-                        GoogleProject(
-                            iambic_managed=IambicManaged.READ_AND_WRITE, **google_obj
-                        )
-                    ]
-                )
-            asyncio.run(self.run_import_google_workspace_resources())
-            self.update_secret()
+        project = GoogleProject(**google_obj)
+
+        if self.config.secrets and self.config.google_workspace:
+            self.config.google_workspace.workspaces.append(project)
         else:
-            self.config.google_workspace = GoogleWorkspaceConfig(
-                workspaces=[
-                    GoogleProject(
-                        iambic_managed=IambicManaged.READ_AND_WRITE, **google_obj
-                    )
-                ]
-            )
-            asyncio.run(self.run_import_google_workspace_resources())
-            self.config.secrets = {"google_workspace": {"workspaces": [google_obj]}}
-            self.create_secret()
+            self.config.google_workspace = GoogleWorkspaceConfig(workspaces=[project])
+
+        asyncio.run(self.run_import_google_workspace_resources())
+        self.upsert_secret()
 
     def configuration_wizard_google_workspace_edit(self):
         project_ids = [
             project.project_id for project in self.config.google_workspace.workspaces
         ]
         project_id_to_config_elem_map = {
             project.project_id: elem
@@ -1349,15 +1485,15 @@
             confirm_command_exe("Google Workspace", Operation.UPDATED)
 
             self.config.google_workspace.workspaces[
                 project_id_to_config_elem_map[project_id]
             ] = project_to_edit
 
             asyncio.run(self.run_import_google_workspace_resources())
-            self.update_secret()
+            self.upsert_secret()
             self.config.write()
 
     def configuration_wizard_google_workspace(self):
         log.info(
             "For details on how to retrieve the information required to add a Google Workspace "
             "to IAMbic check out our docs: https://docs.iambic.org/getting_started/google/"
         )
@@ -1381,38 +1517,23 @@
             "idp_name": set_idp_name(),
             "org_url": set_okta_org_url(),
             "api_token": set_okta_api_token(),
         }
 
         confirm_command_exe("Okta Organization", Operation.ADDED)
 
-        if self.config.secrets:
-            if self.config.okta and self.config.okta.organizations:
-                self.config.okta.organizations.append(OktaOrganization(**okta_obj))
-            else:
-                self.config.okta = OktaConfig(
-                    organizations=[
-                        OktaOrganization(
-                            iambic_managed=IambicManaged.READ_AND_WRITE, **okta_obj
-                        )
-                    ]
-                )
-            asyncio.run(self.run_import_okta_resources())
-            self.update_secret()
+        organization = OktaOrganization(**okta_obj)
+
+        if self.config.secrets and self.has_okta_configured:
+            self.config.okta.organizations.append(organization)
         else:
-            self.config.okta = OktaConfig(
-                organizations=[
-                    OktaOrganization(
-                        iambic_managed=IambicManaged.READ_AND_WRITE, **okta_obj
-                    )
-                ]
-            )
-            self.config.secrets = {"okta": {"organizations": [okta_obj]}}
-            asyncio.run(self.run_import_okta_resources())
-            self.create_secret()
+            self.config.okta = OktaConfig(organizations=[organization])
+
+        asyncio.run(self.run_import_okta_resources())
+        self.upsert_secret()
 
     def configuration_wizard_okta_organization_edit(self):
         org_names = [org.idp_name for org in self.config.okta.organizations]
         org_name_to_config_elem_map = {
             org.idp_name: elem
             for elem, org in enumerate(self.config.okta.organizations)
         }
@@ -1460,15 +1581,15 @@
 
             confirm_command_exe("Okta Organization", Operation.UPDATED)
             self.config.okta.organizations[
                 org_name_to_config_elem_map[org_name]
             ] = org_to_edit
 
             asyncio.run(self.run_import_okta_resources())
-            self.update_secret()
+            self.upsert_secret()
             self.config.write()
 
     def configuration_wizard_okta(self):
         log.info(
             "For details on how to retrieve the information required to add an Okta Organization "
             "to IAMbic check out our docs: https://docs.iambic.org/getting_started/okta/"
         )
@@ -1492,44 +1613,27 @@
             "tenant_id": set_tenant_id(),
             "client_id": set_client_id(),
             "client_secret": set_client_secret(),
         }
 
         confirm_command_exe("Azure AD Organization", Operation.ADDED)
 
-        if self.config.secrets:
-            if self.config.azure_ad and self.config.azure_ad.organizations:
-                self.config.azure_ad.organizations.append(
-                    AzureADOrganization(**azure_ad_obj)
-                )
-            else:
-                self.config.azure_ad = AzureADConfig(
-                    organizations=[
-                        AzureADOrganization(
-                            iambic_managed=IambicManaged.READ_AND_WRITE, **azure_ad_obj
-                        )
-                    ]
-                )
+        organization = AzureADOrganization(**azure_ad_obj)
 
-            asyncio.run(self.run_import_azure_ad_resources())
-            self.update_secret()
+        if (
+            self.config.secrets
+            and self.config.azure_ad
+            and self.config.azure_ad.organizations
+        ):
+            self.config.azure_ad.organizations.append(organization)
         else:
-            self.config.azure_ad = AzureADConfig(
-                organizations=[
-                    AzureADOrganization(
-                        iambic_managed=IambicManaged.READ_AND_WRITE, **azure_ad_obj
-                    )
-                ]
-            )
-            self.config.secrets = {
-                "azure_ad": get_secret_dict_with_val(self.config.azure_ad)
-            }
+            self.config.azure_ad = AzureADConfig(organizations=[organization])
 
-            asyncio.run(self.run_import_azure_ad_resources())
-            self.create_secret()
+        asyncio.run(self.run_import_azure_ad_resources())
+        self.upsert_secret()
 
     def configuration_wizard_azure_ad_organization_edit(self):
         org_names = [org.idp_name for org in self.config.azure_ad.organizations]
         org_name_to_config_elem_map = {
             org.idp_name: elem
             for elem, org in enumerate(self.config.azure_ad.organizations)
         }
@@ -1583,15 +1687,15 @@
             confirm_command_exe("Azure AD Organization", Operation.UPDATED)
             self.config.azure_ad.organizations[
                 org_name_to_config_elem_map[org_name]
             ] = org_to_edit
 
             asyncio.run(self.run_import_azure_ad_resources())
 
-            self.update_secret()
+            self.upsert_secret()
             self.config.write()
 
     def configuration_wizard_azure_ad(self):
         log.info(
             "For details on how to retrieve the information required to add an Azure AD Organization "
             "to IAMbic check out our docs: https://docs.iambic.org/getting_started/azure_ad/"
         )
@@ -1640,22 +1744,25 @@
             )
 
     def configuration_wizard_change_detection_setup(self, aws_org: AWSOrganization):
         if not questionary.confirm(
             "To setup change detection for iambic requires "
             "creating CloudFormation stacks "
             "and a CloudFormation stack set.\n"
-            "This will also update the IAMbic Hub Role to add the required policy to consume the changes.\n"
             "Proceed?"
         ).unsafe_ask():
             return
 
         session, _ = self.get_boto3_session_for_account(aws_org.org_account_id)
-        cf_client = session.client("cloudformation", region_name="us-east-1")
-        org_client = session.client("organizations", region_name="us-east-1")
+        cf_client = session.client(
+            "cloudformation", region_name=self.aws_default_region
+        )
+        org_client = session.client(
+            "organizations", region_name=self.aws_default_region
+        )
 
         successfully_created = asyncio.run(
             create_iambic_eventbridge_stacks(
                 cf_client,
                 org_client,
                 aws_org.org_id,
                 aws_org.org_account_id,
@@ -1663,82 +1770,60 @@
             )
         )
         if not successfully_created:
             return
 
         role_name = IAMBIC_SPOKE_ROLE_NAME
         hub_account_id = self.hub_account_id
-        sqs_arn = f"arn:aws:sqs:us-east-1:{hub_account_id}:IAMbicChangeDetectionQueue"
+        sqs_arn = f"arn:aws:sqs:{self.aws_default_region}:{hub_account_id}:IAMbicChangeDetectionQueue"
+
+        if not self.existing_role_template_map:
+            log.info("Loading AWS role templates...")
+            self.existing_role_template_map = asyncio.run(
+                get_existing_template_map(self.repo_dir, AWS_IAM_ROLE_TEMPLATE_TYPE)
+            )
+
         role_template: AwsIamRoleTemplate = self.existing_role_template_map.get(
             role_name
         )
-        role_template.properties.inline_policies.append(
-            PolicyDocument(
-                policy_name="consume_iambic_changes",
-                included_accounts=[hub_account_id],
-                statement=[
-                    PolicyStatement(
-                        effect="Allow",
-                        action=[
-                            "sqs:DeleteMessage",
-                            "sqs:ReceiveMessage",
-                            "sqs:GetQueueAttributes",
-                        ],
-                        resource=[sqs_arn],
-                    )
-                ],
-            )
-        )
 
         self.config.aws.sqs_cloudtrail_changes_queues = [sqs_arn]
         asyncio.run(self.save_and_deploy_changes(role_template))
 
     def run(self):  # noqa: C901
-        if "aws" not in self.config.__fields__:
-            log.info("The config wizard requires the IAMbic AWS plugin.")
-            return
-        elif not self.config.aws:
-            self.config.aws = AWSConfig()
+        """Run the configuration wizard.
 
-        while True:
-            choices = ["AWS", "Done"]
-            secret_in_config = bool(self.config.extends)
-            if secret_in_config:
-                secret_question_text = "This requires the ability to update the AWS Secrets Manager secret."
-            else:
-                secret_question_text = (
-                    "This requires permissions to create an AWS Secret."
-                )
+        This will prompt the user for the required information to configure IAMbic.
 
-            if self.config.aws.accounts or self.config.aws.organizations:
-                if not self.existing_role_template_map:
-                    log.info("Loading AWS role templates...")
-                    self.existing_role_template_map = asyncio.run(
-                        get_existing_template_map(
-                            self.repo_dir, AWS_IAM_ROLE_TEMPLATE_TYPE
-                        )
-                    )
-                if self.existing_role_template_map:
-                    choices = ["AWS"]
-                    # Currently, the config wizard only support IAMbic plugins
-                    if "azure_ad" in self.config.__fields__:
-                        choices.append("Azure AD")
-                    if "google_workspace" in self.config.__fields__:
-                        choices.append("Google Workspace")
-                    if "okta" in self.config.__fields__:
-                        choices.append("Okta")
+        Notes:
+        - AWS is not required to use IAMbic, but it is required to store to aws secrets.
+        """
+
+        while True:
+            choices = []
+            secret_question_text, _ = self.secrets_message
 
-                    choices.extend(["Generate Github Action Workflows", "Done"])
+            if "aws" in self.config.__fields__:
+                choices.append("AWS")
+            if "azure_ad" in self.config.__fields__:
+                choices.append("Azure AD")
+            if "google_workspace" in self.config.__fields__:
+                choices.append("Google Workspace")
+            if "okta" in self.config.__fields__:
+                choices.append("Okta")
 
+            if self.has_aws_account_or_organizations:
+                choices.append("Generate Github Action Workflows")
                 if (
                     self.config.aws.organizations
-                    and self.existing_role_template_map
                     and not self.config.aws.sqs_cloudtrail_changes_queues
                 ):
-                    choices.insert(-1, "Setup AWS change detection")
+                    choices.append("Setup AWS change detection")
+
+            choices.append("Done")
 
             try:
                 action = questionary.select(
                     "What would you like to configure?",
                     choices=choices,
                 ).unsafe_ask()
             except KeyboardInterrupt:
@@ -1770,17 +1855,17 @@
                 elif action == "Generate Github Action Workflows":
                     self.configuration_wizard_github_workflow()
                 elif action == "Setup AWS change detection":
                     if self.has_cf_permissions:
                         log.info(
                             f"IAMbic change detection relies on CloudTrail being enabled all IAMbic aware accounts. "
                             f"You can check that you have CloudTrail setup by going to "
-                            f"https://{self.default_region}.console.aws.amazon.com/cloudtrail/home\n"
+                            f"https://{self.aws_default_region}.console.aws.amazon.com/cloudtrail/home\n"
                             f"If you do not have CloudTrail setup, you can set it up by going to "
-                            f"https://{self.default_region}.console.aws.amazon.com/cloudtrail/home?region={self.default_region}#/create"
+                            f"https://{self.aws_default_region}.console.aws.amazon.com/cloudtrail/home?region={self.aws_default_region}#/create"
                         )
                         self.configuration_wizard_change_detection_setup(
                             self.config.aws.organizations[0]
                         )
                     else:
                         log.info(
                             "Unable to edit this attribute without CloudFormation permissions."
```

### Comparing `iambic_core-0.4.1/iambic/core/aio_utils/__init__.py` & `iambic_core-0.5.1/iambic/core/aio_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/exceptions.py` & `iambic_core-0.5.1/iambic/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/git.py` & `iambic_core-0.5.1/iambic/core/git.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/iambic_enum.py` & `iambic_core-0.5.1/iambic/core/iambic_enum.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/iambic_plugin.py` & `iambic_core-0.5.1/iambic/core/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/logger.py` & `iambic_core-0.5.1/iambic/core/logger.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/models.py` & `iambic_core-0.5.1/iambic/core/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/noq_json.py` & `iambic_core-0.5.1/iambic/core/noq_json.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/parser.py` & `iambic_core-0.5.1/iambic/core/parser.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/template_generation.py` & `iambic_core-0.5.1/iambic/core/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/core/utils.py` & `iambic_core-0.5.1/iambic/core/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/github/templates/iambic-detect.yml` & `iambic_core-0.5.1/iambic/github/templates/iambic-detect.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/github/templates/iambic-enforce.yml` & `iambic_core-0.5.1/iambic/github/templates/iambic-enforce.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/github/templates/iambic-expire.yml` & `iambic_core-0.5.1/iambic/github/templates/iambic-expire.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/github/templates/iambic-import.yml` & `iambic_core-0.5.1/iambic/github/templates/iambic-import.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/github/utils.py` & `iambic_core-0.5.1/iambic/github/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/lambda/app.py` & `iambic_core-0.5.1/iambic/lambda/app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/main.py` & `iambic_core-0.5.1/iambic/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/output/__init__.py` & `iambic_core-0.5.1/iambic/output/__init__.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/output/filters.py` & `iambic_core-0.5.1/iambic/output/filters.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from io import StringIO
 from typing import List
 
 from rich.console import Console
 from rich.style import Style
 from rich.table import Table
 from rich.text import Text
```

### Comparing `iambic_core-0.4.1/iambic/output/models.py` & `iambic_core-0.5.1/iambic/output/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/output/templates/github_summary.jinja2` & `iambic_core-0.5.1/iambic/output/templates/github_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/output/templates/text_file_summary.jinja2` & `iambic_core-0.5.1/iambic/output/templates/text_file_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/output/templates/text_screen_summary.jinja2` & `iambic_core-0.5.1/iambic/output/templates/text_screen_summary.jinja2`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/output/text.py` & `iambic_core-0.5.1/iambic/output/text.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/README.md` & `iambic_core-0.5.1/iambic/plugins/README.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicHubRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRole.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IambicSpokeRoleReadOnly.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleDestination.yml`

 * *Files 3% similar despite different names*

```diff
@@ -58,28 +58,28 @@
       - IAMbicEventBus
       - IAMbicChangeDetectionQueue
   IAMbicChangeDetectionQueue:
     Type: 'AWS::SQS::Queue'
     Properties:
       QueueName: IAMbicChangeDetectionQueue
       MessageRetentionPeriod: 604800
-  IAMbicChangeDetectionQueueSQSPolicy: 
+  IAMbicChangeDetectionQueueSQSPolicy:
     Type: AWS::SQS::QueuePolicy
-    Properties: 
-      Queues: 
+    Properties:
+      Queues:
         - !Ref IAMbicChangeDetectionQueue
-      PolicyDocument: 
-        Statement: 
-          - Action: 
-              - "sqs:SendMessage" 
+      PolicyDocument:
+        Statement:
+          - Action:
+              - "sqs:SendMessage"
             Effect: "Allow"
             Resource: !GetAtt IAMbicChangeDetectionQueue.Arn
-            Principal:  
+            Principal:
               Service:
                 - "events.amazonaws.com"
             Condition:
               ArnEquals:
                 aws:SourceArn: !GetAtt IAMbicEventRule.Arn
     DependsOn:
       - IAMbicEventRule
       - IAMbicChangeDetectionQueue
-      
+
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/templates/IdentityRuleForwarder.yml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/cloud_formation/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,26 +40,28 @@
     with open(template, "r") as f:
         return f.read()
 
 
 async def create_stack(
     client, stack_name: str, template_body: str, parameters: list[dict], **kwargs
 ) -> bool:
+    region = client.meta.region_name
+
     try:
         existing_stack = await legacy_paginated_search(
             client.describe_stacks,
             response_key="Stacks",
             StackName=stack_name,
         )
         if existing_stack:
             log.info(
                 "Stack already exists. Skipping creation. "
                 "If this is not the desired behavior, please delete the stack in the console and try again.\n",
                 stack_name=stack_name,
-                stack_url="https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks\n",
+                stack_url=f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacks\n",
             )
             return True
     except client.exceptions.ClientError as e:
         # ValidationError means the stack doesn't exist
         if e.response["Error"]["Code"] != "ValidationError":
             raise
 
@@ -98,43 +100,53 @@
             stack_details = {
                 "StackStatus": "CREATE_FAILED",
                 "StackStatusReason": f"Stack not found. Stack Name: {stack_name}, Stack ID: {stack_id}",
             }
         resource_status = stack_details.get("StackStatus")
 
     if resource_status == "CREATE_FAILED":
-        log.error(
-            "Unable to create AWS CloudFormation Stack",
-            stack_name=stack_name,
-            reason=stack_details.get("StackStatusReason"),
-        )
-        return False
+        soft_fail = bool("already exists." in stack_details.get("StackStatusReason"))
+        if soft_fail:
+            log.warning(
+                "Role already exists on account.",
+                stack_name=stack_name,
+                reason=stack_details.get("StackStatusReason"),
+            )
+        else:
+            log.error(
+                "Unable to create AWS CloudFormation Stack",
+                stack_name=stack_name,
+                reason=stack_details.get("StackStatusReason"),
+            )
+        return soft_fail
     return True
 
 
 async def create_stack_set(
     client,
     stack_set_name,
     template_body: str,
     parameters: list[dict],
     deployment_targets: dict,
     deployment_regions: list[str],
     operation_preferences: dict[str, Union[int, str]],
     **kwargs,
 ) -> bool:
+    region = client.meta.region_name
+
     try:
         await boto_crud_call(
             client.describe_stack_set,
             StackSetName=stack_set_name,
         )
         log.info(
             "StackSet already exists. Skipping creation. "
             "If this is not the desired behavior, please delete the stack in the console and try again.\n",
             stack_set_name=stack_set_name,
-            stack_set_url="https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacksets\n",
+            stack_set_url=f"https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacksets\n",
         )
         return True
     except client.exceptions.StackSetNotFoundException:
         pass
 
     await boto_crud_call(
         client.create_stack_set,
@@ -184,38 +196,54 @@
             continue
         elif all(
             instance.get("StackInstanceStatus", {}).get("DetailedStatus") == "SUCCEEDED"
             for instance in stack_instances
         ):
             return True
         else:
-            failed_instances = [
-                {
-                    "Account": instance["Account"],
-                    "Region": instance["Region"],
-                    "Status": instance.get("StackInstanceStatus", {}).get(
-                        "DetailedStatus"
-                    ),
-                    "StatusReason": instance.get("StatusReason"),
-                }
-                for instance in stack_instances
-                if instance.get("StackInstanceStatus", {}).get("DetailedStatus")
-                in ["FAILED", "CANCELLED"]
-            ]
-            log.error(
-                "Unable to create stack set instances",
-                stack_set_name=stack_set_name,
-                failed_instances=failed_instances,
-            )
-            return False
+            existing_instances = []
+            failed_instances = []
+            for instance in stack_instances:
+                if instance.get("StackInstanceStatus", {}).get("DetailedStatus") in [
+                    "FAILED",
+                    "CANCELLED",
+                ]:
+                    response_summary = {
+                        "Account": instance["Account"],
+                        "Region": instance["Region"],
+                        "Status": instance.get("StackInstanceStatus", {}).get(
+                            "DetailedStatus"
+                        ),
+                        "StatusReason": instance.get("StatusReason"),
+                    }
+                    if "already exists." in instance.get("StatusReason"):
+                        existing_instances.append(response_summary)
+                    else:
+                        failed_instances.append(response_summary)
+
+            if existing_instances:
+                log.warning(
+                    "Role already exists on account(s).",
+                    stack_set_name=stack_set_name,
+                    failed_instances=failed_instances,
+                )
+            if failed_instances:
+                log.error(
+                    "Unable to create stack set instances",
+                    stack_set_name=stack_set_name,
+                    failed_instances=failed_instances,
+                )
+
+            return not bool(failed_instances)
 
 
 async def create_change_detection_stacks(
     cf_client, org_id: str, org_account_id: str, role_arn: str = None
 ) -> bool:
+    region = cf_client.meta.region_name
     additional_kwargs = {"RoleARN": role_arn} if role_arn else {}
     stack_created = await create_stack(
         cf_client,
         stack_name="IAMbicCentralChangeRule",
         template_body=get_central_rule_template_body(),
         parameters=[{"ParameterKey": "OrgID", "ParameterValue": org_id}],
         **additional_kwargs,
@@ -224,79 +252,82 @@
         stack_created = await create_stack(
             cf_client,
             stack_name="IAMbicForwardEventRule",
             template_body=get_rule_forwarding_template_body(),
             parameters=[
                 {
                     "ParameterKey": "TargetEventBusArn",
-                    "ParameterValue": f"arn:aws:events:us-east-1:{org_account_id}:event-bus/IAMbicChangeDetectionEventBus",
+                    "ParameterValue": f"arn:aws:events:{region}:{org_account_id}:event-bus/IAMbicChangeDetectionEventBus",
                 }
             ],
             Capabilities=["CAPABILITY_NAMED_IAM"],
             **additional_kwargs,
         )
 
     return stack_created
 
 
 async def create_change_detection_stack_sets(
     cf_client, org_client, org_account_id: str
 ) -> bool:
+    region = cf_client.meta.region_name
     org_roots = await legacy_paginated_search(
         org_client.list_roots, response_key="Roots"
     )
 
     return await create_stack_set(
         cf_client,
         stack_set_name="IAMbicForwardEventRule",
         template_body=get_rule_forwarding_template_body(),
         parameters=[
             {
                 "ParameterKey": "TargetEventBusArn",
-                "ParameterValue": f"arn:aws:events:us-east-1:{org_account_id}:event-bus/IAMbicChangeDetectionEventBus",
+                "ParameterValue": f"arn:aws:events:{region}:{org_account_id}:event-bus/IAMbicChangeDetectionEventBus",
             }
         ],
         deployment_targets={
             "OrganizationalUnitIds": [root["Id"] for root in org_roots],
             "AccountFilterType": "NONE",
         },
-        deployment_regions=["us-east-1"],
+        deployment_regions=[region],
         operation_preferences={
             "MaxConcurrentCount": 1,
             "FailureToleranceCount": 1,
         },
         Capabilities=["CAPABILITY_NAMED_IAM"],
     )
 
 
 async def create_iambic_eventbridge_stacks(
     cf_client, org_client, org_id: str, account_id: str, role_arn: str = None
 ) -> bool:
+    region = cf_client.meta.region_name
     successfully_created = await create_change_detection_stacks(
         cf_client, org_id, account_id, role_arn
     )
     if successfully_created:
         log.info(
-            "Creating stack instances. "
-            "You can check the progress here: https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacksets/IAMbicForwardEventRule/stacks\n"
-            "WARNING: Don't Exit"
+            f"Creating stack instances. "
+            f"You can check the progress here: https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacksets/IAMbicForwardEventRule/stacks\n"
+            f"WARNING: Don't Exit"
         )
         return await create_change_detection_stack_sets(
             cf_client, org_client, account_id
         )
 
     return successfully_created
 
 
 async def create_spoke_role_stack_set(
     cf_client,
     org_client,
     hub_account_id: str,
     read_only=False,
 ) -> bool:
+    region = cf_client.meta.region_name
     org_roots = await legacy_paginated_search(
         org_client.list_roots, response_key="Roots"
     )
 
     return await create_stack_set(
         cf_client,
         stack_set_name="IambicSpokeRole",
@@ -308,15 +339,15 @@
             },
             {"ParameterKey": "SpokeRoleName", "ParameterValue": IAMBIC_SPOKE_ROLE_NAME},
         ],
         deployment_targets={
             "OrganizationalUnitIds": [root["Id"] for root in org_roots],
             "AccountFilterType": "NONE",
         },
-        deployment_regions=["us-east-1"],
+        deployment_regions=[region],
         operation_preferences={
             "RegionConcurrencyType": "PARALLEL",
             "MaxConcurrentCount": 10,
             "FailureToleranceCount": 10,
         },
         Capabilities=["CAPABILITY_NAMED_IAM"],
     )
@@ -391,18 +422,19 @@
         cf_client,
         hub_account_id,
         assume_as_arn,
         role_arn,
         spoke_role_read_only=read_only,
     )
     spoke_role_postfix = "ReadOnly" if read_only else ""
+    region = cf_client.meta.region_name
     if hub_role_created and org_client:
         log.info(
-            "Creating stack instances. "
-            f"You can check the progress here: https://us-east-1.console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacksets/IambicSpokeRole{spoke_role_postfix}/stacks"
-            "WARNING: Don't Exit"
+            f"Creating stack instances. "
+            f"You can check the progress here: https://{region}.console.aws.amazon.com/cloudformation/home?region={region}#/stacksets/IambicSpokeRole{spoke_role_postfix}/stacks\n"
+            f"WARNING: Don't Exit"
         )
         return await create_spoke_role_stack_set(
             cf_client, org_client, hub_account_id, read_only=read_only
         )
 
     return hub_role_created
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/event_bridge/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/handlers.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/policy/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/policy/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/policy/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/role/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/role/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/role/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iam/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/DESIGN_DECISIONS.md`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,18 @@
     arn: str
     region: str
     access_portal_url: str
     identity_store_id: str
 
 
 class CustomerManagedPolicyReference(BaseModel, ExpiryModel):
-    path: str
+    path: Optional[str] = Field(
+        "/",
+        description="The path to the IAM policy that you have configured in each account where you want to deploy your permission set. The default is /. For more information, see Friendly names and paths in the IAM User Guide.",
+    )
     name: str
 
     @property
     def resource_type(self) -> str:
         return "aws:iam:managed_policy"
 
     @property
@@ -100,23 +103,23 @@
     @property
     def resource_id(self) -> str:
         return self.arn
 
 
 class PermissionBoundary(BaseModel, ExpiryModel):
     customer_managed_policy_reference: Optional[CustomerManagedPolicyReference]
-    policy_arn: Optional[str]
+    managed_policy_arn: Optional[str]
 
     @property
     def resource_type(self):
         return "aws:identity_center:permission_boundary"
 
     @property
     def resource_id(self):
-        return self.customer_managed_policy_reference.name or self.policy_arn
+        return self.customer_managed_policy_reference.name or self.managed_policy_arn
 
 
 class SessionDuration(BaseModel):
     session_duration: str
 
 
 class InlinePolicy(BaseModel, ExpiryModel):
@@ -738,17 +741,15 @@
                 "Successfully finished scanning for drift on account for resource",
                 requires_changes=bool(account_change_details.proposed_changes),
                 **log_params,
             )
 
         return account_change_details
 
-    async def apply(
-        self, config: AWSConfig  # noqa: C901
-    ) -> TemplateChangeDetails:
+    async def apply(self, config: AWSConfig) -> TemplateChangeDetails:  # noqa: C901
         tasks = []
         template_changes = TemplateChangeDetails(
             resource_id=self.resource_id,
             resource_type=self.resource_type,
             template_path=self.file_path,
             exceptions_seen=[],
         )
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/identity_center/permission_set/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,19 @@
                 identity_center_client.describe_permission_set,
                 InstanceArn=instance_arn,
                 PermissionSetArn=permission_set_arn,
             )
         ).get("PermissionSet", {})
     except identity_center_client.exceptions.ResourceNotFoundException:
         return {}
+    except ClientError as e:
+        if e.response["Error"]["Code"] == "ResourceNotFound":
+            return {}
+        else:
+            raise
 
 
 async def generate_permission_set_map(aws_accounts: list[AWSAccount], templates: list):
     """Generates the map of permission sets for AWS accounts that are referenced in at least 1 template
 
     :param aws_accounts:
     :param templates:
@@ -702,15 +707,15 @@
                     current_value=existing_permission_boundary,
                     new_value=template_permission_boundary,
                 )
             )
         else:
             response.append(
                 ProposedChange(
-                    change_type=ProposedChangeType.CREATE,
+                    change_type=ProposedChangeType.ATTACH,
                     resource_type="aws:identity_center:permission_set",
                     resource_id=permission_set_arn,
                     attribute="permissions_boundary",
                     new_value=template_permission_boundary,
                 )
             )
 
@@ -726,15 +731,15 @@
             response = await plugin_apply_wrapper(apply_awaitable, response)
 
         log.debug(log_str, **log_params)
     elif existing_permission_boundary and not template_permission_boundary:
         log_str = "Removing PermissionsBoundary discovered."
         response.append(
             ProposedChange(
-                change_type=ProposedChangeType.DELETE,
+                change_type=ProposedChangeType.DETACH,
                 resource_type="aws:identity_center:permission_set",
                 resource_id=permission_set_arn,
                 attribute="permissions_boundary",
                 current_value=existing_permission_boundary,
             )
         )
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,15 +199,15 @@
             try:
                 session = boto3.Session(
                     profile_name=self.aws_profile, region_name=region_name
                 )
             except Exception as err:
                 log.warning(err)
 
-        sts_client = session.client("sts")
+        sts_client = session.client("sts", region_name=region_name)
         if self.hub_role_arn and self.hub_role_arn != get_current_role_arn(sts_client):
             boto3_session = await create_assume_role_session(
                 session,
                 self.hub_role_arn,
                 region_name,
                 external_id=self.external_id,
                 session_name=os.environ.get("IAMBIC_SESSION_NAME", None),
@@ -229,15 +229,18 @@
             client := self.boto3_session_map.get("client", {})
             .get(service, {})
             .get(region_name)
         ):
             return client
 
         client = (await self.get_boto3_session(region_name)).client(
-            service, config=botocore.client.Config(max_pool_connections=50)
+            service,
+            config=botocore.client.Config(
+                max_pool_connections=50, region_name=region_name
+            ),
         )
         self.boto3_session_map.setdefault("client", {}).setdefault(service, {})[
             region_name
         ] = client
         return client
 
     async def get_active_regions(self) -> list[str]:
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/pyproject.toml` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/tests/test_aws_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/tests/test_models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/aws/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/aws/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/handlers.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from pydantic import BaseModel, Field, SecretStr
 
 from iambic.core.context import ctx
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.logger import log
 from iambic.core.models import BaseTemplate, TemplateChangeDetails
 
-if TYPE_CHECKING:
+if TYPE_CHECKING:  # pragma: no cover
     from iambic.plugins.v0_1_0.azure_ad.iambic_plugin import AzureADConfig
 
-    MappingIntStrAny = typing.Mapping[int | str, any]
+    MappingIntStrAny = typing.Mapping[int | str, Any]
     AbstractSetIntStr = typing.AbstractSet[int | str]
 
 
 class AzureADOrganization(BaseModel):
     idp_name: str
     tenant_id: str
     client_id: str
@@ -35,15 +35,15 @@
         description="If true, at next sign-in, the user must perform a multi-factor authentication (MFA) "
         "before being forced to change their password.",
     )
 
     class Config:
         arbitrary_types_allowed = True
 
-    async def set_azure_access_token(self):
+    async def set_azure_access_token(self):  # pragma: no cover
         if not self.access_token:
             # initialize the client here
             self.client = msal.ConfidentialClientApplication(
                 self.client_id,
                 authority=f"https://login.microsoftonline.com/{self.tenant_id}",
                 client_credential=self.client_secret.get_secret_value(),
             )
@@ -54,15 +54,15 @@
                 self.access_token = token_result["access_token"]
             else:
                 raise Exception("Access token was not successfully acquired")
         return self.access_token
 
     async def _make_request(
         self, request_type: str, endpoint: str, **kwargs
-    ) -> Union[dict, list, None]:
+    ) -> Union[dict, list, None]:  # pragma: no cover
         await self.set_azure_access_token()
 
         response = []
         is_list = bool(request_type == "list")
         if is_list:
             request_type = "get"
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/user/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/azure_ad/user/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/example/iambic_plugin.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/example/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_database/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/example/local_database/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/example/local_file/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/example/local_file/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/github/github.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/github/github.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/github/github_app.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/github/github_app.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/github/handlers.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/github/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/github/iambic_plugin.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/github/iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/handlers.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/iambic_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import os
-from typing import Optional
+import typing
+from typing import TYPE_CHECKING, Any, Optional
 
 import googleapiclient.discovery
 from google.oauth2 import service_account
 from pydantic import BaseModel, Field, SecretStr, validator
 
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.iambic_plugin import ProviderPlugin
@@ -16,14 +17,18 @@
     GoogleWorkspaceGroupTemplate,
 )
 from iambic.plugins.v0_1_0.google_workspace.handlers import (
     import_google_resources,
     load,
 )
 
+if TYPE_CHECKING:  # pragma: no cover
+    MappingIntStrAny = typing.Mapping[int | str, Any]
+    AbstractSetIntStr = typing.AbstractSet[int | str]
+
 
 class GoogleSubject(BaseModel):
     domain: str
     service_account: str
 
 
 class GoogleProject(BaseModel):
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_google_group_utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/group/test_template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/google_workspace/tests/test_iambic_plugin.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/app/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/app/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/app/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/app/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/group/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/group/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/group/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/group/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/handlers.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/handlers.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/iambic_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 from typing import Any, Optional
 
+from okta.client import Client as OktaClient
 from pydantic import BaseModel, Extra, Field, SecretStr, validator
 
 from iambic.core.iambic_enum import IambicManaged
 from iambic.core.iambic_plugin import ProviderPlugin
 from iambic.plugins.v0_1_0 import PLUGIN_VERSION
 from iambic.plugins.v0_1_0.okta.app.models import OktaAppTemplate
 from iambic.plugins.v0_1_0.okta.group.models import OktaGroupTemplate
 from iambic.plugins.v0_1_0.okta.handlers import import_okta_resources, load
 from iambic.plugins.v0_1_0.okta.user.models import OktaUserTemplate
-from okta.client import Client as OktaClient
 
 
 class OktaOrganization(BaseModel):
     idp_name: str
     org_url: str
     api_token: SecretStr
     request_timeout: int = 60
     client: Any = None  # OktaClient
     iambic_managed: Optional[IambicManaged] = Field(
-        IambicManaged.IMPORT_ONLY,
+        IambicManaged.UNDEFINED,
         description="Controls the directionality of iambic changes",
     )
 
     class Config:
         arbitrary_types_allowed = True
         extra = Extra.forbid
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/models.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/pyproject.toml` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/pyproject.toml`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/models.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/user/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -236,22 +236,26 @@
         ):
             log.info(
                 "User is already deprovisioned. Please delete the user in Okta.",
                 **log_params,
             )
             return change_details
 
-        tasks.extend(
-            [
+        if current_user and not self.deleted:
+            tasks.append(
                 update_user_status(
                     current_user,
                     self.properties.status.value,
                     okta_organization,
                     log_params,
                 ),
+            )
+
+        tasks.extend(
+            [
                 update_user_profile(
                     self,
                     current_user,
                     self.properties.profile,
                     okta_organization,
                     log_params,
                 ),
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/template_generation.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/user/template_generation.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/user/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/user/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 from typing import TYPE_CHECKING, Any, List, Optional
 
 import okta.models as models
+
 from iambic.core.context import ctx
 from iambic.core.exceptions import RateLimitException
 from iambic.core.logger import log
 from iambic.core.models import ProposedChange, ProposedChangeType
 from iambic.core.utils import GlobalRetryController
 from iambic.plugins.v0_1_0.okta.exceptions import UserProfileNotUpdatableYet
 from iambic.plugins.v0_1_0.okta.models import User
@@ -250,14 +251,17 @@
     """
     response: list = []
     if not user:
         return response
     current_status: str = user.status.value
     if current_status == new_status:
         return response
+    if user.deleted:
+        return response
+
     response.append(
         ProposedChange(
             change_type=ProposedChangeType.UPDATE,
             resource_id=user.user_id,
             resource_type=user.resource_type,
             attribute="status",
             change_summary={
```

### Comparing `iambic_core-0.4.1/iambic/plugins/v0_1_0/okta/utils.py` & `iambic_core-0.5.1/iambic/plugins/v0_1_0/okta/utils.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/request_handler/expire_resources.py` & `iambic_core-0.5.1/iambic/request_handler/expire_resources.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/request_handler/git_apply.py` & `iambic_core-0.5.1/iambic/request_handler/git_apply.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/request_handler/git_plan.py` & `iambic_core-0.5.1/iambic/request_handler/git_plan.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/LICENSE` & `iambic_core-0.5.1/iambic/vendor/lambda_multiprocessing/LICENSE`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/iambic/vendor/lambda_multiprocessing/main.py` & `iambic_core-0.5.1/iambic/vendor/lambda_multiprocessing/main.py`

 * *Files identical despite different names*

### Comparing `iambic_core-0.4.1/pyproject.toml` & `iambic_core-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "iambic-core"
 packages = [
     { include="iambic", from="." },
 ]
-version = "0.4.1"
+version = "0.5.1"
 license = "Apache-2.0"
 description = "The python package used to generate, parse, and execute noqform yaml templates."
 authors = ["Noq Software <hello@noq.dev>"]
 readme = "README.md"
 exclude = ["build_util/*"]
 include = ["iambic/output/templates/*"]
```

### Comparing `iambic_core-0.4.1/PKG-INFO` & `iambic_core-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iambic-core
-Version: 0.4.1
+Version: 0.5.1
 Summary: The python package used to generate, parse, and execute noqform yaml templates.
 License: Apache-2.0
 Author: Noq Software
 Author-email: hello@noq.dev
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

