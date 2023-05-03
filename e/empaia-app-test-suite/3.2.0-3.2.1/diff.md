# Comparing `tmp/empaia_app_test_suite-3.2.0.tar.gz` & `tmp/empaia_app_test_suite-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empaia_app_test_suite-3.2.0.tar", max compression
+gzip compressed data, was "empaia_app_test_suite-3.2.1.tar", max compression
```

## Comparing `empaia_app_test_suite-3.2.0.tar` & `empaia_app_test_suite-3.2.1.tar`

### file list

```diff
@@ -1,154 +1,152 @@
--rw-r--r--   0        0        0     1288 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/LICENSE
--rw-r--r--   0        0        0     6610 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/README.md
--rw-r--r--   0        0        0       87 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/__init__.py
--rw-r--r--   0        0        0     2624 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/__init__.py
--rw-r--r--   0        0        0     2944 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/apps_cli.py
--rw-r--r--   0        0        0     1305 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/cases_cli.py
--rw-r--r--   0        0        0     5646 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/jobs_cli.py
--rw-r--r--   0        0        0     4579 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/main_cli.py
--rw-r--r--   0        0        0     3899 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/services_cli.py
--rw-r--r--   0        0        0     2386 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/slides_cli.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/__init__.py
--rw-r--r--   0        0        0     5244 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/apps_commands.py
--rw-r--r--   0        0        0      921 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/cases_commands.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/__init__.py
--rw-r--r--   0        0        0     4204 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/app_helper.py
--rw-r--r--   0        0        0     4324 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/data_helper.py
--rw-r--r--   0        0        0     2784 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/job_helper.py
--rw-r--r--   0        0        0    10601 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/job_validation_helper.py
--rw-r--r--   0        0        0     4201 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/wsi_helper.py
--rw-r--r--   0        0        0    13309 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/jobs_commands.py
--rw-r--r--   0        0        0     8804 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/services_commands.py
--rw-r--r--   0        0        0     2973 2023-03-31 14:14:09.305022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/slides_commands.py
--rw-r--r--   0        0        0     4818 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/constants.py
--rw-r--r--   0        0        0     3881 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/custom_models.py
--rw-r--r--   0        0        0       56 2022-11-30 10:14:50.710744 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.git
--rw-r--r--   0        0        0       32 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitignore
--rw-r--r--   0        0        0      845 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      699 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0     1447 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab-ci.yml
--rw-r--r--   0        0        0     2258 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/LICENSE
--rw-r--r--   0        0        0      302 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/README.md
--rw-r--r--   0        0        0        0 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/__init__.py
--rw-r--r--   0        0        0      692 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/commons.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/marketplace/__init__.py
--rw-r--r--   0        0        0    17434 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/marketplace/app.py
--rw-r--r--   0        0        0    36937 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/poetry.lock
--rw-r--r--   0        0        0      780 2023-03-30 12:45:35.128584 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/pyproject.toml
--rw-r--r--   0        0        0       36 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/setup.cfg
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/__init__.py
--rw-r--r--   0        0        0     3983 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/access_token_tools.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/tests/__init__.py
--rw-r--r--   0        0        0     8405 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/__init__.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/__init__.py
--rw-r--r--   0        0        0    12040 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/annotations.py
--rw-r--r--   0        0        0     3587 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/classes.py
--rw-r--r--   0        0        0    11262 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/collections.py
--rw-r--r--   0        0        0     2341 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/jobs.py
--rw-r--r--   0        0        0     5884 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/primitives.py
--rw-r--r--   0        0        0      423 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/server_settings.py
--rw-r--r--   0        0        0     6052 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/clinical.py
--rw-r--r--   0        0        0     3305 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/commons.py
--rw-r--r--   0        0        0     3826 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/examination.py
--rw-r--r--   0        0        0      922 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/id_mapper.py
--rw-r--r--   0        0        0     7516 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/job.py
--rw-r--r--   0        0        0     2156 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/slide.py
--rw-r--r--   0        0        0     2661 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/storage.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/tests/__init__.py
--rw-r--r--   0        0        0      448 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/tests/test_job_creator_type.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/__init__.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/__init__.py
--rw-r--r--   0        0        0    13252 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/annotations.py
--rw-r--r--   0        0        0     3747 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/classes.py
--rw-r--r--   0        0        0    17090 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/collections.py
--rw-r--r--   0        0        0      397 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/jobs.py
--rw-r--r--   0        0        0     6657 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/primitives.py
--rw-r--r--   0        0        0      423 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/server_settings.py
--rw-r--r--   0        0        0     6052 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/clinical.py
--rw-r--r--   0        0        0     3683 2023-03-23 06:54:41.599255 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/commons.py
--rw-r--r--   0        0        0     8591 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/examination.py
--rw-r--r--   0        0        0      922 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/id_mapper.py
--rw-r--r--   0        0        0    11686 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/job.py
--rw-r--r--   0        0        0     2329 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/slide.py
--rw-r--r--   0        0        0     2661 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/storage.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/__init__.py
--rw-r--r--   0        0        0      373 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_examination.py
--rw-r--r--   0        0        0      500 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_creator_type.py
--rw-r--r--   0        0        0     2829 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py
--rw-r--r--   0        0        0     1816 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py
--rw-r--r--   0        0        0     2445 2022-11-30 10:14:54.810743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py
--rw-r--r--   0        0        0       67 2022-11-30 10:14:51.720744 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.git
--rw-r--r--   0        0        0       31 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitignore
--rw-r--r--   0        0        0      845 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      699 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0      791 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml
--rw-r--r--   0        0        0      224 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitmodules
--rw-r--r--   0        0        0     1115 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md
--rw-r--r--   0        0        0     6254 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/README.md
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/__init__.py
--rw-r--r--   0        0        0     3482 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml
--rw-r--r--   0        0        0    16228 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/poetry.lock
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__init__.py
--rw-r--r--   0        0        0     1232 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py
--rw-r--r--   0        0        0      111 2022-11-30 10:14:56.020743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.git
--rw-r--r--   0        0        0        8 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitignore
--rw-r--r--   0        0        0      845 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md
--rw-r--r--   0        0        0      697 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md
--rw-r--r--   0        0        0     1505 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md
--rw-r--r--   0        0        0    12338 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json
--rw-r--r--   0        0        0    17247 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json
--rw-r--r--   0        0        0    18941 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json
--rw-r--r--   0        0        0      283 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead-settings.json
--rw-r--r--   0        0        0      170 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/namespaces/org.empaia.global.v1.json
--rw-r--r--   0        0        0     9133 2022-11-30 10:14:58.070743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv
--rw-r--r--   0        0        0     5744 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py
--rw-r--r--   0        0        0      457 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/exceptions.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/__init__.py
--rw-r--r--   0        0        0     2230 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/__init__.py
--rw-r--r--   0        0        0     2674 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/__init__.py
--rw-r--r--   0        0        0     4439 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py
--rw-r--r--   0        0        0    16713 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py
--rw-r--r--   0        0        0     2149 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py
--rw-r--r--   0        0        0      869 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/pyproject.toml
--rw-r--r--   0        0        0      260 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/sample.env
--rw-r--r--   0        0        0       36 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/setup.cfg
--rw-r--r--   0        0        0        0 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/__init__.py
--rw-r--r--   0        0        0     9099 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py
--rw-r--r--   0        0        0    23309 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py
--rw-r--r--   0        0        0    10278 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py
--rw-r--r--   0        0        0    35567 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py
--rw-r--r--   0        0        0    10465 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/__init__.py
--rw-r--r--   0        0        0    43792 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py
--rw-r--r--   0        0        0     2186 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py
--rw-r--r--   0        0        0    34033 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py
--rw-r--r--   0        0        0     2345 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py
--rw-r--r--   0        0        0    42502 2023-03-30 12:45:47.179368 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py
--rw-r--r--   0        0        0     3024 2023-03-23 06:54:58.329261 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py
--rw-r--r--   0        0        0      864 2022-11-30 10:14:54.820743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py
--rw-r--r--   0        0        0     2999 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/docker-compose.yml
--rw-r--r--   0        0        0       48 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/nginx/Dockerfile
--rw-r--r--   0        0        0     1134 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/nginx/nginx.conf
--rw-r--r--   0        0        0     1256 2023-04-17 06:03:21.906959 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile
--rw-r--r--   0        0        0        0 2022-11-30 10:14:58.080743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__init__.py
--rw-r--r--   0        0        0     5688 2022-11-30 10:14:58.080743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py
--rw-r--r--   0        0        0     9355 2023-04-17 06:03:21.906959 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py
--rw-r--r--   0        0        0      361 2023-04-17 06:03:21.906959 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/pyproject.toml
--rw-r--r--   0        0        0     1033 2023-04-17 07:10:52.894495 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/Dockerfile
--rw-r--r--   0        0        0       81 2023-04-17 07:10:52.894495 empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-mirax/mirax_backend/entrypoint.sh
--rw-r--r--   0        0        0    18174 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/empaia_app_test_suite/settings.py
--rw-r--r--   0        0        0        0 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/__init__.py
--rw-r--r--   0        0        0      511 2023-03-31 14:14:09.315022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_aaa.py
--rw-r--r--   0        0        0     2448 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_commons.py
--rw-r--r--   0        0        0     8016 2022-11-30 10:14:49.760743 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_mds.py
--rw-r--r--   0        0        0     2158 2023-03-23 08:17:05.515364 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_mps.py
--rw-r--r--   0        0        0     5671 2023-03-31 14:14:09.315022 empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_print.py
--rw-r--r--   0        0        0     3037 2023-04-17 13:48:35.451634 empaia_app_test_suite-3.2.0/pyproject.toml
--rw-r--r--   0        0        0     8304 1970-01-01 00:00:00.000000 empaia_app_test_suite-3.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1288 2022-08-11 14:24:58.326262 empaia_app_test_suite-3.2.1/LICENSE
+-rw-r--r--   0        0        0     6610 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/README.md
+-rw-r--r--   0        0        0       87 2022-08-11 14:24:58.326262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/__init__.py
+-rw-r--r--   0        0        0     2624 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/__init__.py
+-rw-r--r--   0        0        0     2944 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/apps_cli.py
+-rw-r--r--   0        0        0     1305 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/cases_cli.py
+-rw-r--r--   0        0        0     5646 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/jobs_cli.py
+-rw-r--r--   0        0        0     4579 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/main_cli.py
+-rw-r--r--   0        0        0     3899 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/services_cli.py
+-rw-r--r--   0        0        0     2386 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/slides_cli.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/__init__.py
+-rw-r--r--   0        0        0     5244 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/apps_commands.py
+-rw-r--r--   0        0        0      921 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/cases_commands.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/__init__.py
+-rw-r--r--   0        0        0     4204 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/app_helper.py
+-rw-r--r--   0        0        0     4324 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/data_helper.py
+-rw-r--r--   0        0        0     2784 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/job_helper.py
+-rw-r--r--   0        0        0    10601 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/job_validation_helper.py
+-rw-r--r--   0        0        0     4201 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/wsi_helper.py
+-rw-r--r--   0        0        0    13267 2023-05-03 13:39:28.376471 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/jobs_commands.py
+-rw-r--r--   0        0        0     8804 2023-05-03 11:39:03.407046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/services_commands.py
+-rw-r--r--   0        0        0     2973 2023-05-03 11:39:03.407046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/slides_commands.py
+-rw-r--r--   0        0        0     4818 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/constants.py
+-rw-r--r--   0        0        0     3881 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/custom_models.py
+-rw-r--r--   0        0        0       56 2022-08-11 14:24:59.076262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/.git
+-rw-r--r--   0        0        0       32 2022-08-11 14:25:02.656262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/.gitignore
+-rw-r--r--   0        0        0      845 2022-08-11 14:25:02.656262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      699 2022-08-11 14:25:02.656262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0     1447 2023-05-03 11:42:18.266045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2258 2023-05-03 11:42:18.266045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/CHANGELOG.md
+-rw-r--r--   0        0        0     1064 2022-08-11 14:25:02.656262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/LICENSE
+-rw-r--r--   0        0        0      302 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 11:42:18.266045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/__init__.py
+-rw-r--r--   0        0        0      692 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/commons.py
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/marketplace/__init__.py
+-rw-r--r--   0        0        0    17434 2023-05-03 11:42:18.266045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/marketplace/app.py
+-rw-r--r--   0        0        0    36937 2022-08-11 14:25:02.656262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/poetry.lock
+-rw-r--r--   0        0        0      780 2023-05-03 11:42:18.266045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/pyproject.toml
+-rw-r--r--   0        0        0       36 2022-08-11 14:25:02.656262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/setup.cfg
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/utils/__init__.py
+-rw-r--r--   0        0        0     3983 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/utils/access_token_tools.py
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/utils/tests/__init__.py
+-rw-r--r--   0        0        0     8405 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/__init__.py
+-rw-r--r--   0        0        0    12040 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/annotations.py
+-rw-r--r--   0        0        0     3587 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/classes.py
+-rw-r--r--   0        0        0    11262 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/collections.py
+-rw-r--r--   0        0        0     2341 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/jobs.py
+-rw-r--r--   0        0        0     5884 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/primitives.py
+-rw-r--r--   0        0        0      423 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/server_settings.py
+-rw-r--r--   0        0        0     6052 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/clinical.py
+-rw-r--r--   0        0        0     3305 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/commons.py
+-rw-r--r--   0        0        0     3826 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/examination.py
+-rw-r--r--   0        0        0      922 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/id_mapper.py
+-rw-r--r--   0        0        0     7516 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/job.py
+-rw-r--r--   0        0        0     2156 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/slide.py
+-rw-r--r--   0        0        0     2661 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/storage.py
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/tests/__init__.py
+-rw-r--r--   0        0        0      448 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/tests/test_job_creator_type.py
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/__init__.py
+-rw-r--r--   0        0        0    13252 2023-05-03 11:42:18.266045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/annotations.py
+-rw-r--r--   0        0        0     3747 2023-05-03 11:42:18.266045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/classes.py
+-rw-r--r--   0        0        0    17090 2023-05-03 11:42:18.276045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/collections.py
+-rw-r--r--   0        0        0      397 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/jobs.py
+-rw-r--r--   0        0        0     6657 2023-05-03 11:42:18.276045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/primitives.py
+-rw-r--r--   0        0        0      423 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/server_settings.py
+-rw-r--r--   0        0        0     6052 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/clinical.py
+-rw-r--r--   0        0        0     3683 2023-05-03 11:42:18.276045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/commons.py
+-rw-r--r--   0        0        0     8591 2023-05-03 11:42:18.276045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/examination.py
+-rw-r--r--   0        0        0      922 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/id_mapper.py
+-rw-r--r--   0        0        0    11686 2023-05-03 11:42:18.276045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/job.py
+-rw-r--r--   0        0        0     2329 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/slide.py
+-rw-r--r--   0        0        0     2661 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/storage.py
+-rw-r--r--   0        0        0        0 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/__init__.py
+-rw-r--r--   0        0        0      373 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/test_examination.py
+-rw-r--r--   0        0        0      500 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/test_job_creator_type.py
+-rw-r--r--   0        0        0     2829 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/test_job_mode.py
+-rw-r--r--   0        0        0     1816 2022-11-08 07:14:22.274111 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/test_job_progress.py
+-rw-r--r--   0        0        0     2445 2023-05-03 11:42:18.276045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py
+-rw-r--r--   0        0        0       67 2022-08-11 14:24:59.776262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.git
+-rw-r--r--   0        0        0       31 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.gitignore
+-rw-r--r--   0        0        0      845 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      699 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0      791 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml
+-rw-r--r--   0        0        0      224 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.gitmodules
+-rw-r--r--   0        0        0     1115 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/CHANGELOG.md
+-rw-r--r--   0        0        0     6254 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/README.md
+-rw-r--r--   0        0        0        0 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/__init__.py
+-rw-r--r--   0        0        0     3482 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/docker-compose.yml
+-rw-r--r--   0        0        0    16228 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/poetry.lock
+-rw-r--r--   0        0        0        0 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/__init__.py
+-rw-r--r--   0        0        0     1232 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py
+-rw-r--r--   0        0        0      111 2022-08-11 14:25:03.386262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.git
+-rw-r--r--   0        0        0        8 2022-08-11 14:25:03.406262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitignore
+-rw-r--r--   0        0        0      845 2022-08-16 06:55:50.883244 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md
+-rw-r--r--   0        0        0      697 2022-08-16 06:55:50.883244 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md
+-rw-r--r--   0        0        0     1505 2022-08-11 14:25:03.406262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md
+-rw-r--r--   0        0        0    12338 2022-08-11 14:25:03.406262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json
+-rw-r--r--   0        0        0    17247 2022-08-11 14:25:03.406262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json
+-rw-r--r--   0        0        0    18941 2023-05-03 11:42:28.356045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json
+-rw-r--r--   0        0        0      283 2022-11-08 07:14:44.583528 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead-settings.json
+-rw-r--r--   0        0        0      170 2022-08-11 14:25:03.406262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/namespaces/org.empaia.global.v1.json
+-rw-r--r--   0        0        0     9133 2023-05-03 11:42:28.356045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv
+-rw-r--r--   0        0        0     5744 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py
+-rw-r--r--   0        0        0      457 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/exceptions.py
+-rw-r--r--   0        0        0        0 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/__init__.py
+-rw-r--r--   0        0        0     2230 2022-08-16 06:55:45.873244 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/__init__.py
+-rw-r--r--   0        0        0     2674 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/__init__.py
+-rw-r--r--   0        0        0     4439 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py
+-rw-r--r--   0        0        0    16713 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py
+-rw-r--r--   0        0        0     2149 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py
+-rw-r--r--   0        0        0      869 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/sample.env
+-rw-r--r--   0        0        0       36 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/setup.cfg
+-rw-r--r--   0        0        0        0 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/__init__.py
+-rw-r--r--   0        0        0     9099 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py
+-rw-r--r--   0        0        0    23309 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py
+-rw-r--r--   0        0        0    10278 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py
+-rw-r--r--   0        0        0    35567 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py
+-rw-r--r--   0        0        0    10465 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:42:18.286045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/__init__.py
+-rw-r--r--   0        0        0    43792 2023-05-03 11:42:18.296045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py
+-rw-r--r--   0        0        0     2186 2023-05-03 11:42:18.296045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py
+-rw-r--r--   0        0        0    34033 2023-05-03 11:42:18.296045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py
+-rw-r--r--   0        0        0     2345 2023-05-03 11:42:18.296045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py
+-rw-r--r--   0        0        0    42502 2023-05-03 11:42:18.296045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py
+-rw-r--r--   0        0        0     3024 2023-05-03 11:42:18.296045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py
+-rw-r--r--   0        0        0      864 2022-08-11 14:25:02.666262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py
+-rw-r--r--   0        0        0     2999 2023-05-03 13:39:28.376471 empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/docker-compose.yml
+-rw-r--r--   0        0        0       48 2022-08-11 14:24:58.326262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/nginx/Dockerfile
+-rw-r--r--   0        0        0     1134 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/nginx/nginx.conf
+-rw-r--r--   0        0        0     1256 2023-05-03 13:39:35.501427 empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile
+-rw-r--r--   0        0        0        0 2022-08-11 14:25:03.416262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__init__.py
+-rw-r--r--   0        0        0     5688 2022-08-11 14:25:03.416262 empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py
+-rw-r--r--   0        0        0     9355 2023-05-03 11:42:18.306045 empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py
+-rw-r--r--   0        0        0      361 2023-05-03 13:39:35.501427 empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/pyproject.toml
+-rw-r--r--   0        0        0    18174 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/settings.py
+-rw-r--r--   0        0        0        0 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/__init__.py
+-rw-r--r--   0        0        0      511 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_aaa.py
+-rw-r--r--   0        0        0     2448 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_commons.py
+-rw-r--r--   0        0        0     8016 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_mds.py
+-rw-r--r--   0        0        0     2158 2023-05-03 11:39:03.387046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_mps.py
+-rw-r--r--   0        0        0     5671 2023-05-03 11:39:03.397046 empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_print.py
+-rw-r--r--   0        0        0     3015 2023-05-03 13:39:28.376471 empaia_app_test_suite-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     8297 1970-01-01 00:00:00.000000 empaia_app_test_suite-3.2.1/PKG-INFO
```

### Comparing `empaia_app_test_suite-3.2.0/LICENSE` & `empaia_app_test_suite-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/README.md` & `empaia_app_test_suite-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/apps_cli.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/apps_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/cases_cli.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/cases_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/jobs_cli.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/jobs_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/main_cli.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/main_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/services_cli.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/services_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/cli_definitions/slides_cli.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/cli_definitions/slides_cli.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/apps_commands.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/apps_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/cases_commands.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/cases_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/app_helper.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/app_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/data_helper.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/data_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/job_helper.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/job_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/job_validation_helper.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/job_validation_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/helper/wsi_helper.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/helper/wsi_helper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/jobs_commands.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/jobs_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,21 +114,21 @@
 
     with PrintStep("Retrieving app_id for job"):
         r = requests.get(f"{mds_url}/v3/jobs/{job_id}")
         r.raise_for_status()
         job_status = r.json()["status"]
         app_id = r.json()["app_id"]
 
-    with PrintStep("Locking job inputs"):
-        lock_inputs_to_job(client, job_id, mds_url, mps_url)
-
     with PrintStep("Checking job status"):
         if job_status != "ASSEMBLY":
             raise Exception(f"Job has already been started. Current status: {job_status}")
 
+    with PrintStep("Locking job inputs"):
+        lock_inputs_to_job(client, job_id, mds_url, mps_url)
+
     with PrintStep("Starting app"):
         set_job_statuses(job_id, mds_url, ["READY"])
         exec_request = {
             "app_id": app_id,
             "job_id": job_id,
             "access_token": token,
             "app_service_url": app_api,
@@ -298,15 +298,15 @@
     class_ids = []
     if "classes" in partial_input_ead:
         annotation = get_annotation(input_id, mds_url)
         if len(annotation["classes"]) == 0:
             raise HTTPError("Class constraint for annotation not fullfilled")
         valid_classes = get_valid_class_values_for_constraint(ead_classes, partial_input_ead["classes"])
         for annot_class in annotation["classes"]:
-            if annot_class["value"] in valid_classes and annot_class["creator_id"] == scope_id:
+            if annot_class["value"] in valid_classes:
                 class_ids.append(annot_class["id"])
         if len(class_ids) == 0:
             raise HTTPError("Class constraint for annotation not fullfilled")
     if partial_input_ead["type"] == "collection":
         collection = get_collection(input_id, mds_url)
         for item in collection["items"]:
             ids = validate_ead_input_classes(partial_input_ead["items"], item["id"], scope_id, ead_classes, mds_url)
```

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/services_commands.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/services_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/commands/slides_commands.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/commands/slides_commands.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/constants.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/constants.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/custom_models.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/custom_models.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/.gitlab-ci.yml` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/CHANGELOG.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/LICENSE` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/LICENSE`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/commons.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/marketplace/app.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/marketplace/app.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/poetry.lock` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/poetry.lock`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/pyproject.toml` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/access_token_tools.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/utils/access_token_tools.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/utils/tests/test_access_token_tools.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/annotations.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/annotations.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/classes.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/classes.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/collections.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/collections.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/jobs.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/jobs.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/annotation/primitives.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/annotation/primitives.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/clinical.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/clinical.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/commons.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/examination.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/examination.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/id_mapper.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/id_mapper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/job.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/slide.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/slide.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v1/storage.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v1/storage.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/annotations.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/annotations.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/classes.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/classes.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/collections.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/collections.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/annotation/primitives.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/annotation/primitives.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/clinical.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/clinical.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/commons.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/examination.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/examination.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/id_mapper.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/id_mapper.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/job.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/slide.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/slide.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/storage.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/storage.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_mode.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/test_job_mode.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_progress.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/test_job_progress.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/models/v3/tests/test_job_validation_fields.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/CHANGELOG.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/README.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/README.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/docker-compose.yml` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/poetry.lock` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/poetry.lock`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/__main__.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/issue_templates/story_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/.gitlab/merge_request_templates/merge_request_qa_level_1.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/README.md`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft1.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v1-draft3.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/ead/ead-schema.v3.json`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/definitions/tags/tags.csv`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/ead_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/common.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v1_draft3/ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/indepth/ead_schema_v3/job.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/py_ead_validation/job_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/pyproject.toml` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/pyproject.toml`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/test_ead_validator.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v1/test_validate_ead_with_config.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/ead_validation/v3/test_validate_ead_v3_with_config.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/conftest.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_completeness.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_input_compliance.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_completeness.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_output_compliance.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/job_validation/v3/test_suitable_job_status.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/py_ead_validation/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/docker-compose.yml` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/docker-compose.yml`

 * *Files 14% similar despite different names*

```diff
@@ -2,36 +2,36 @@
   app-service:
     image: registry.gitlab.com/empaia/services/app-service:0.7.19@sha256:f2c1b638e9a1ecd0dc2e4766b66d801e544bd7da22998726b64daf359c13514b
   annotation-service:
     image: registry.gitlab.com/empaia/services/annotation-service:0.16.5@sha256:131da84de1a31cd31c7660583aac149288431e80b88f6a7ffa13ffd92c8f0c85
   job-service:
     image: registry.gitlab.com/empaia/services/job-service:0.7.2@sha256:615c90ce7b353208da06e5deefcebcd74c4705e976123b9b0d2a298505e815e4
   examination-service:
-    image: registry.gitlab.com/empaia/services/examination-service:0.7.25@sha256:a4ea5e8dfdc4acb91f30e416f21f4669d6d52ebd04ff02bc4f35fc6a9b60bdab
+    image: registry.gitlab.com/empaia/services/examination-service:0.7.26@sha256:8e80904c93ca3f1fd7bbc2f1475382659e2b4d63c3a61551a38c006689cfaa82
   clinical-data-service:
     image: registry.gitlab.com/empaia/services/clinical-data-service:0.3.2
   storage-mapper-service:
-    image: registry.gitlab.com/empaia/services/storage-mapper-service:0.2.13@sha256:1cc1198dbed37050b817afd0ed7ea9044751319abc296420bb6ca6d2c7f11a01
+    image: registry.gitlab.com/empaia/services/storage-mapper-service:0.2.14@sha256:fdc31a5855876d3e246a56f009f1093cbb2d123d5d6ca9db18745c2cf99cc588
   wsi-service:
-    image: registry.gitlab.com/empaia/services/wsi-service-plugin-integration:0.11.2@sha256:5f9aee9740c75dd96bca6ac622517da858198fb1cf0ef4eb8465b0d0358dc937
+    image: registry.gitlab.com/empaia/services/wsi-service-plugin-integration:0.11.9@sha256:9e683fc08717c422ef0953323a74a976e5dfb309793d74a14addf21d36325466
   medical-data-service:
-    image: registry.gitlab.com/empaia/services/medical-data-service:0.7.13@sha256:0058b21a96c3f512d73dc6514dc954184400669764e8e96ad21dd4e6ef882714
+    image: registry.gitlab.com/empaia/services/medical-data-service:0.7.15@sha256:57eca23c2f678f755de2c75c7c09ea68e9b19120f15b0d5f486ec99b07e29e4f
   marketplace-service-mock:
-    image: registry.gitlab.com/empaia/service-mocks/marketplace-service-mock:0.1.54@sha256:8398a236513e1a116b5914c9c954f0259452a37b0187a85cdb98f7d93a7d5e98
+    image: registry.gitlab.com/empaia/service-mocks/marketplace-service-mock:0.1.55@sha256:5f900557af56dc9849289bf96a9865ab99396c24ddeb50ae69dad78273af4286
   aaa-service-mock:
-    image: registry.gitlab.com/empaia/service-mocks/aaa-service-mock:0.1.41@sha256:98ac5973963f23c5a3f2f6ba333964fa5de4f82ee113b42d728d335de2ca232e
+    image: registry.gitlab.com/empaia/service-mocks/aaa-service-mock:0.1.43@sha256:f18bc6bb64dbbd4083b0f2828a277b3e0b4733a320b343c095a94ab2a028b7be
   job-execution-service:
     image: registry.gitlab.com/empaia/services/job-execution-service:0.5.34@sha256:c80551a992011e75626babf42deaa1bf4361de31937f532024988c2008422029
   workbench-daemon:
     image: registry.gitlab.com/empaia/services/workbench-service:0.9.5@sha256:3f7ebe644f003cd2c77023ef3dcf73a2aa82f5dd70d1990da29759ac6de6f138
   workbench-service:
     image: registry.gitlab.com/empaia/services/workbench-service:0.9.5@sha256:3f7ebe644f003cd2c77023ef3dcf73a2aa82f5dd70d1990da29759ac6de6f138
   workbench-client-v3:
-    image: registry.gitlab.com/empaia/integration/frontend-workspace/workbench-client-v3:3.0.6@sha256:bc94d9d1f960b4e6dd43e83473b58009aae0f666f4dcda1da58b692bcbbbff51
+    image: registry.gitlab.com/empaia/integration/frontend-workspace/workbench-client-v3:3.0.8@sha256:9e11880dcc9352980dede64c08dfcdfa7b701b980ae8bad3b1e38c5493aed6aa
   workbench-client-v3-sample-ui:
-    image: registry.gitlab.com/empaia/integration/frontend-workspace/sample-app-v3:3.0.4@sha256:9ef80b91aa2484bb064e0406290691f2ca92ebc66b4ad9523bb6b3aaa8dec190
+    image: registry.gitlab.com/empaia/integration/frontend-workspace/sample-app-v3:3.0.5@sha256:015fe0ee096e234d2c05fe23ce10b6403715cbaef7812eda4693a715eee94e6e
   workbench-client-v3-generic-ui:
-    image: registry.gitlab.com/empaia/integration/frontend-workspace/generic-app-ui-v3:3.2.2@sha256:b9704fae8c6f30a996e85ec3f8af1d091b82abd6cc2616bf782cbb5ec205b3e5
+    image: registry.gitlab.com/empaia/integration/frontend-workspace/generic-app-ui-v3:3.2.3@sha256:7ba9b80a013eb93bd7b5700d1cfa410d0d3224619b6d481df293db9f6121c1ba
   eats-postgres-db:
-    image: registry.gitlab.com/empaia/integration/ci-docker-images/custom-postgres:0.1.67@sha256:86ce606ee6e340c8f81fab89016a6005d52169bf20e10910f95b8d53041674ae
+    image: registry.gitlab.com/empaia/integration/ci-docker-images/custom-postgres:0.1.69@sha256:2dd53e1b737493c60349ae57d547621fdb1b21451abefe0f43c82bfc75bb333a
   eats-mongo-db:
-    image: mongo:5.0.16@sha256:6ea33882c70df83283a6ba0a89fdd304795ba42bcb2c714b49e3ad722dd41b62
+    image: mongo:5.0.17@sha256:7ad08ce66a554b84a4eddedb518ad0546356b419e88e0fe324f41c01a0b4122b
```

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/nginx/nginx.conf` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/nginx/nginx.conf`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/Dockerfile`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM registry.gitlab.com/empaia/integration/ci-docker-images/test-runner:0.1.72@sha256:a47beb9877f1ed561fbd7b93069902b9d56f70130bc6ec7b42cbfd0a692ad848 AS build0
+FROM registry.gitlab.com/empaia/integration/ci-docker-images/test-runner:0.1.74@sha256:1de4ef90546b19bc6bd8bd0fbd116fe952ed4e5b7a5e8d61fd81bef491146e56 AS build0
 
 ENV DEBIAN_FRONTEND=noninteractive
 ENV PYTHONDONTWRITEBYTECODE=1
 ENV PYTHONUNBUFFERED=1
 
 COPY isyntax_backend /isyntax/isyntax_backend
 COPY pyproject.toml /isyntax/pyproject.toml
```

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/__main__.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/services/wsi-service-plugin-isyntax/isyntax_backend/isyntax_backend/isyntax_reader.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/settings.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/settings.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_commons.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_commons.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_mds.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_mds.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_mps.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_mps.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/empaia_app_test_suite/utils/utils_print.py` & `empaia_app_test_suite-3.2.1/empaia_app_test_suite/utils/utils_print.py`

 * *Files identical despite different names*

### Comparing `empaia_app_test_suite-3.2.0/pyproject.toml` & `empaia_app_test_suite-3.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "empaia-app-test-suite"
-version = "3.2.0"
+version = "3.2.1"
 description = "The EMPAIA App Test Suite (EATS)"
 license = "MIT"
 
 # Authors / Maintainers
 authors = ["EMPAIA <dev-support@empaia.org>"]
 maintainers = ["EMPAIA <dev-support@empaia.org>"]
 
@@ -49,28 +49,27 @@
 empaia-app-test-suite = 'empaia_app_test_suite.cli:app'
 eats = 'empaia_app_test_suite.cli:app'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 jsonschema = "^4.4.0"
 pydantic = {extras = ["dotenv"], version = "^1.9.0"}
-requests = "^2.27.1"
 toml = "^0.10.2"
 docker = "^6.0.0"
 prettytable = "^3.2.0"
 typer = "^0.7.0"
 PyYAML = "^6.0"
+requests = "2.28.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pillow = "^9.5.0"
 pydantic = "^1.10.7"
 pytest = "^7.3.1"
 pycodestyle = "^2.10.0"
-requests = "^2.28.2"
 pylint = "^2.17.2"
 
 [tool.pytest.ini_options]
 norecursedirs = ["empaia_app_test_suite/services"]
 
 [tool.black]
 line-length = 120
```

### Comparing `empaia_app_test_suite-3.2.0/PKG-INFO` & `empaia_app_test_suite-3.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empaia-app-test-suite
-Version: 3.2.0
+Version: 3.2.1
 Summary: The EMPAIA App Test Suite (EATS)
 Home-page: https://developer.empaia.org/app_developer_docs/#/
 License: MIT
 Author: EMPAIA
 Author-email: dev-support@empaia.org
 Maintainer: EMPAIA
 Maintainer-email: dev-support@empaia.org
@@ -25,15 +25,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: docker (>=6.0.0,<7.0.0)
 Requires-Dist: jsonschema (>=4.4.0,<5.0.0)
 Requires-Dist: prettytable (>=3.2.0,<4.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.9.0,<2.0.0)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: requests (==2.28.2)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Bug Tracker, https://gitlab.com/empaia/integration/empaia-app-test-suite/-/issues
 Project-URL: Documentation, https://developer.empaia.org/app_developer_docs/#/
 Project-URL: Repository, https://gitlab.com/empaia/integration/empaia-app-test-suite
 Description-Content-Type: text/markdown
```

