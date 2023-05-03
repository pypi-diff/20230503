# Comparing `tmp/gaia-core-0.0.1.tar.gz` & `tmp/gaia-core-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\gaia-core-0.0.1.tar", last modified: Wed May  3 07:53:07 2023, max compression
+gzip compressed data, was "dist\gaia-core-0.0.2.tar", last modified: Wed May  3 07:54:28 2023, max compression
```

## Comparing `gaia-core-0.0.1.tar` & `gaia-core-0.0.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.816771 gaia-core-0.0.1/
--rw-rw-rw-   0        0        0     1169 2023-05-03 07:53:07.816771 gaia-core-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      959 2023-05-03 05:54:50.000000 gaia-core-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.723022 gaia-core-0.0.1/gaia/
--rw-rw-rw-   0        0        0      153 2023-05-03 05:53:58.000000 gaia-core-0.0.1/gaia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.723022 gaia-core-0.0.1/gaia/base/
--rw-rw-rw-   0        0        0        2 2023-04-30 18:12:38.000000 gaia-core-0.0.1/gaia/base/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.723022 gaia-core-0.0.1/gaia/base/vendors/
--rw-rw-rw-   0        0        0        0 2023-04-20 07:59:12.000000 gaia-core-0.0.1/gaia/base/vendors/__init__.py
--rw-rw-rw-   0        0        0      438 2023-04-20 08:38:23.000000 gaia-core-0.0.1/gaia/base/vendors/base.py
--rw-rw-rw-   0        0        0     2872 2023-04-20 08:33:18.000000 gaia-core-0.0.1/gaia/base/vendors/chat_gpt.py
--rw-rw-rw-   0        0        0     1817 2023-04-20 08:46:10.000000 gaia-core-0.0.1/gaia/base/vendors/co_here.py
--rw-rw-rw-   0        0        0     8295 2023-05-03 05:53:58.000000 gaia-core-0.0.1/gaia/base/vendors/vendors_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.738649 gaia-core-0.0.1/gaia/cli/
--rw-rw-rw-   0        0        0     2196 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/.gitignore
--rw-rw-rw-   0        0        0      258 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/__init__.py
--rw-rw-rw-   0        0        0       84 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/allow_commands.py
--rw-rw-rw-   0        0        0      265 2023-03-27 06:15:44.000000 gaia-core-0.0.1/gaia/cli/config.json
--rw-rw-rw-   0        0        0       65 2022-06-15 14:26:55.000000 gaia-core-0.0.1/gaia/cli/cors_allowed_origins.json
--rw-rw-rw-   0        0        0      764 2023-03-30 09:46:44.000000 gaia-core-0.0.1/gaia/cli/forcer_template.py
--rw-rw-rw-   0        0        0     1248 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/labelizer_template.py
--rw-rw-rw-   0        0        0     2748 2023-03-29 15:58:50.000000 gaia-core-0.0.1/gaia/cli/main_template.py
--rw-rw-rw-   0        0        0     3479 2023-03-30 10:01:09.000000 gaia-core-0.0.1/gaia/cli/pipeline_template.py
--rw-rw-rw-   0        0        0     1570 2023-03-30 10:48:08.000000 gaia-core-0.0.1/gaia/cli/pipeline_test_template.py
--rw-rw-rw-   0        0        0     2928 2023-03-30 09:44:46.000000 gaia-core-0.0.1/gaia/cli/postprocess_template.py
--rw-rw-rw-   0        0        0      904 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/predictable_template.py
--rw-rw-rw-   0        0        0     2283 2023-03-30 09:45:17.000000 gaia-core-0.0.1/gaia/cli/predictor_template.py
--rw-rw-rw-   0        0        0     4184 2023-03-30 09:45:41.000000 gaia-core-0.0.1/gaia/cli/preprocess_template.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.754273 gaia-core-0.0.1/gaia/cli/schema/
--rw-rw-rw-   0        0        0      113 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/schema/__init__.py
--rw-rw-rw-   0        0        0       87 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/schema/__init___template.py
--rw-rw-rw-   0        0        0      127 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/schema/inputs_template.py
--rw-rw-rw-   0        0        0      127 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/schema/outputs_template.py
--rw-rw-rw-   0        0        0      554 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/schema/test_input_template.py
--rw-rw-rw-   0        0        0      881 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/schema/test_output_template.py
--rw-rw-rw-   0        0        0      525 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/shared_artifacts_template.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.754273 gaia-core-0.0.1/gaia/cli/tester/
--rw-rw-rw-   0        0        0      170 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.769918 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/
--rw-rw-rw-   0        0        0      148 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/.cloud_eval_env
--rw-rw-rw-   0        0        0      301 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/Dockerfile_base
--rw-rw-rw-   0        0        0     3375 2023-02-19 16:01:10.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/Dockerfile_batch_processor
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/__init__.py
--rw-rw-rw-   0        0        0      581 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/auto_model_eval.sh
--rw-rw-rw-   0        0        0      184 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/batch_entrypoint.sh
--rw-rw-rw-   0        0        0      741 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/build_worker.sh
--rw-rw-rw-   0        0        0     1155 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/cloud_eval_client.py
--rw-rw-rw-   0        0        0      286 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/create_ecr_repo_if_needed.sh
--rw-rw-rw-   0        0        0      359 2023-03-27 09:49:11.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/dvc_download_artifacts_s3.sh
--rw-rw-rw-   0        0        0       87 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/eval_on_cloud.sh
--rw-rw-rw-   0        0        0     1829 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/eval_on_cloud_proc.sh
--rw-rw-rw-   0        0        0      492 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/gunicorn.conf.py
--rw-rw-rw-   0        0        0      752 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/tag_version.sh
--rw-rw-rw-   0        0        0      228 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/cloud_eval/untag_version.sh
--rw-rw-rw-   0        0        0     1725 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/tester/dataset_template.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.801167 gaia-core-0.0.1/gaia/cli/tester/deploy_files/
--rw-rw-rw-   0        0        0     3013 2023-02-19 16:01:09.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/Dockerfile
--rw-rw-rw-   0        0        0        0 2022-06-15 14:26:55.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/Jenkinsfile
--rw-rw-rw-   0        0        0        0 2022-06-15 14:26:55.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/Jenkinsfile_dozi
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.801167 gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/
--rw-rw-rw-   0        0        0      476 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-pr.yaml
--rw-rw-rw-   0        0        0      649 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-prd.yaml
--rw-rw-rw-   0        0        0      421 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-rollback.yaml
--rw-rw-rw-   0        0        0      646 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-stg.yaml
--rw-rw-rw-   0        0        0      745 2022-06-15 14:26:55.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/jenkins.env
--rw-rw-rw-   0        0        0      234 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/docker_build_run.sh
--rw-rw-rw-   0        0        0      313 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/dvc_add.sh
--rw-rw-rw-   0        0        0      412 2023-03-29 09:05:51.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/dvc_download_artifacts.sh
--rw-rw-rw-   0        0        0      412 2023-03-29 08:32:38.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/dvc_download_artifacts_google.sh
--rw-rw-rw-   0        0        0      603 2023-03-29 09:04:57.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/dvc_init.sh
--rw-rw-rw-   0        0        0      603 2023-03-29 08:33:10.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/dvc_init_google.sh
--rw-rw-rw-   0        0        0       73 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/dvc_push.sh
--rw-rw-rw-   0        0        0      239 2023-03-27 07:13:27.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/git_init.sh
--rw-rw-rw-   0        0        0      491 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/gunicorn.conf.py
--rw-rw-rw-   0        0        0     1183 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/locustfile.py
--rw-rw-rw-   0        0        0       23 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/requirements_docker.txt
--rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/deploy_files/sample.csv
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.801167 gaia-core-0.0.1/gaia/cli/tester/dsp/
--rw-rw-rw-   0        0        0      877 2022-06-15 14:26:55.000000 gaia-core-0.0.1/gaia/cli/tester/dsp/add_experiment_template.py
--rw-rw-rw-   0        0        0      941 2022-06-15 14:26:55.000000 gaia-core-0.0.1/gaia/cli/tester/dsp/get_dataset_options_template.py
--rw-rw-rw-   0        0        0      993 2023-02-19 16:02:38.000000 gaia-core-0.0.1/gaia/cli/tester/dsp/get_model_options_template.py
--rw-rw-rw-   0        0        0      379 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/tester/evaluator_template.py
--rw-rw-rw-   0        0        0     9122 2023-03-29 15:58:50.000000 gaia-core-0.0.1/gaia/cli/tester/general_tester_template.py
--rw-rw-rw-   0        0        0     3578 2023-03-29 15:58:51.000000 gaia-core-0.0.1/gaia/cli/tester/reporter_template.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.816771 gaia-core-0.0.1/gaia/cli/tester/server/
--rw-rw-rw-   0        0        0      260 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/server/__init__.py
--rw-rw-rw-   0        0        0       71 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/server/__init___template.py
--rw-rw-rw-   0        0        0     5872 2023-03-30 10:48:25.000000 gaia-core-0.0.1/gaia/cli/tester/server/main_template.py
--rw-rw-rw-   0        0        0      657 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/server/pool_template.py
--rw-rw-rw-   0        0        0     4105 2023-03-29 15:58:50.000000 gaia-core-0.0.1/gaia/cli/tester/server/server_template_old.py
--rw-rw-rw-   0        0        0     1739 2023-03-30 10:26:37.000000 gaia-core-0.0.1/gaia/cli/tester/server/test_server_post_stream_template.py
--rw-rw-rw-   0        0        0     1823 2022-06-15 12:42:01.000000 gaia-core-0.0.1/gaia/cli/tester/server/test_server_post_template.py
--rw-rw-rw-   0        0        0     4468 2023-03-27 09:49:11.000000 gaia-core-0.0.1/gaia/cli/tester/server/token_generator_template.py
--rw-rw-rw-   0        0        0    17998 2023-03-29 15:58:50.000000 gaia-core-0.0.1/gaia/cli/tester/tester_template.py
--rw-rw-rw-   0        0        0      398 2023-03-29 15:58:50.000000 gaia-core-0.0.1/gaia/cli/tester/trainer_template.py
--rw-rw-rw-   0        0        0     2596 2023-05-03 05:53:58.000000 gaia-core-0.0.1/gaia/gaia.py
--rw-rw-rw-   0        0        0    28324 2023-03-30 10:27:08.000000 gaia-core-0.0.1/gaia_cli.py
-drwxrwxrwx   0        0        0        0 2023-05-03 07:53:07.816771 gaia-core-0.0.1/gaia_core.egg-info/
--rw-rw-rw-   0        0        0     1169 2023-05-03 07:53:07.000000 gaia-core-0.0.1/gaia_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3564 2023-05-03 07:53:07.000000 gaia-core-0.0.1/gaia_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 07:53:07.000000 gaia-core-0.0.1/gaia_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-03 07:53:07.000000 gaia-core-0.0.1/gaia_core.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       56 2023-05-03 07:53:07.000000 gaia-core-0.0.1/gaia_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-03 07:53:07.000000 gaia-core-0.0.1/gaia_core.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 07:53:07.816771 gaia-core-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     3006 2023-05-03 07:53:00.000000 gaia-core-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.518541 gaia-core-0.0.2/
+-rw-rw-rw-   0        0        0     1170 2023-05-03 07:54:28.518541 gaia-core-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      960 2023-05-03 07:53:57.000000 gaia-core-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.331036 gaia-core-0.0.2/gaia/
+-rw-rw-rw-   0        0        0      153 2023-05-03 05:53:58.000000 gaia-core-0.0.2/gaia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.331036 gaia-core-0.0.2/gaia/base/
+-rw-rw-rw-   0        0        0        2 2023-04-30 18:12:38.000000 gaia-core-0.0.2/gaia/base/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.331036 gaia-core-0.0.2/gaia/base/vendors/
+-rw-rw-rw-   0        0        0        0 2023-04-20 07:59:12.000000 gaia-core-0.0.2/gaia/base/vendors/__init__.py
+-rw-rw-rw-   0        0        0      438 2023-04-20 08:38:23.000000 gaia-core-0.0.2/gaia/base/vendors/base.py
+-rw-rw-rw-   0        0        0     2872 2023-04-20 08:33:18.000000 gaia-core-0.0.2/gaia/base/vendors/chat_gpt.py
+-rw-rw-rw-   0        0        0     1817 2023-04-20 08:46:10.000000 gaia-core-0.0.2/gaia/base/vendors/co_here.py
+-rw-rw-rw-   0        0        0     8295 2023-05-03 05:53:58.000000 gaia-core-0.0.2/gaia/base/vendors/vendors_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.346661 gaia-core-0.0.2/gaia/cli/
+-rw-rw-rw-   0        0        0     2196 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/.gitignore
+-rw-rw-rw-   0        0        0      258 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/__init__.py
+-rw-rw-rw-   0        0        0       84 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/allow_commands.py
+-rw-rw-rw-   0        0        0      265 2023-03-27 06:15:44.000000 gaia-core-0.0.2/gaia/cli/config.json
+-rw-rw-rw-   0        0        0       65 2022-06-15 14:26:55.000000 gaia-core-0.0.2/gaia/cli/cors_allowed_origins.json
+-rw-rw-rw-   0        0        0      764 2023-03-30 09:46:44.000000 gaia-core-0.0.2/gaia/cli/forcer_template.py
+-rw-rw-rw-   0        0        0     1248 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/labelizer_template.py
+-rw-rw-rw-   0        0        0     2748 2023-03-29 15:58:50.000000 gaia-core-0.0.2/gaia/cli/main_template.py
+-rw-rw-rw-   0        0        0     3479 2023-03-30 10:01:09.000000 gaia-core-0.0.2/gaia/cli/pipeline_template.py
+-rw-rw-rw-   0        0        0     1570 2023-03-30 10:48:08.000000 gaia-core-0.0.2/gaia/cli/pipeline_test_template.py
+-rw-rw-rw-   0        0        0     2928 2023-03-30 09:44:46.000000 gaia-core-0.0.2/gaia/cli/postprocess_template.py
+-rw-rw-rw-   0        0        0      904 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/predictable_template.py
+-rw-rw-rw-   0        0        0     2283 2023-03-30 09:45:17.000000 gaia-core-0.0.2/gaia/cli/predictor_template.py
+-rw-rw-rw-   0        0        0     4184 2023-03-30 09:45:41.000000 gaia-core-0.0.2/gaia/cli/preprocess_template.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.346661 gaia-core-0.0.2/gaia/cli/schema/
+-rw-rw-rw-   0        0        0      113 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/schema/__init__.py
+-rw-rw-rw-   0        0        0       87 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/schema/__init___template.py
+-rw-rw-rw-   0        0        0      127 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/schema/inputs_template.py
+-rw-rw-rw-   0        0        0      127 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/schema/outputs_template.py
+-rw-rw-rw-   0        0        0      554 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/schema/test_input_template.py
+-rw-rw-rw-   0        0        0      881 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/schema/test_output_template.py
+-rw-rw-rw-   0        0        0      525 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/shared_artifacts_template.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.362286 gaia-core-0.0.2/gaia/cli/tester/
+-rw-rw-rw-   0        0        0      170 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.377913 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/
+-rw-rw-rw-   0        0        0      148 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/.cloud_eval_env
+-rw-rw-rw-   0        0        0      301 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/Dockerfile_base
+-rw-rw-rw-   0        0        0     3375 2023-02-19 16:01:10.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/Dockerfile_batch_processor
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/__init__.py
+-rw-rw-rw-   0        0        0      581 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/auto_model_eval.sh
+-rw-rw-rw-   0        0        0      184 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/batch_entrypoint.sh
+-rw-rw-rw-   0        0        0      741 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/build_worker.sh
+-rw-rw-rw-   0        0        0     1155 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/cloud_eval_client.py
+-rw-rw-rw-   0        0        0      286 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/create_ecr_repo_if_needed.sh
+-rw-rw-rw-   0        0        0      359 2023-03-27 09:49:11.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/dvc_download_artifacts_s3.sh
+-rw-rw-rw-   0        0        0       87 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/eval_on_cloud.sh
+-rw-rw-rw-   0        0        0     1829 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/eval_on_cloud_proc.sh
+-rw-rw-rw-   0        0        0      492 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/gunicorn.conf.py
+-rw-rw-rw-   0        0        0      752 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/tag_version.sh
+-rw-rw-rw-   0        0        0      228 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/cloud_eval/untag_version.sh
+-rw-rw-rw-   0        0        0     1725 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/tester/dataset_template.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.409166 gaia-core-0.0.2/gaia/cli/tester/deploy_files/
+-rw-rw-rw-   0        0        0     3013 2023-02-19 16:01:09.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/Dockerfile
+-rw-rw-rw-   0        0        0        0 2022-06-15 14:26:55.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/Jenkinsfile
+-rw-rw-rw-   0        0        0        0 2022-06-15 14:26:55.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/Jenkinsfile_dozi
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.424791 gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/
+-rw-rw-rw-   0        0        0      476 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-pr.yaml
+-rw-rw-rw-   0        0        0      649 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-prd.yaml
+-rw-rw-rw-   0        0        0      421 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-rollback.yaml
+-rw-rw-rw-   0        0        0      646 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-stg.yaml
+-rw-rw-rw-   0        0        0      745 2022-06-15 14:26:55.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/jenkins.env
+-rw-rw-rw-   0        0        0      234 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/docker_build_run.sh
+-rw-rw-rw-   0        0        0      313 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/dvc_add.sh
+-rw-rw-rw-   0        0        0      412 2023-03-29 09:05:51.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/dvc_download_artifacts.sh
+-rw-rw-rw-   0        0        0      412 2023-03-29 08:32:38.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/dvc_download_artifacts_google.sh
+-rw-rw-rw-   0        0        0      603 2023-03-29 09:04:57.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/dvc_init.sh
+-rw-rw-rw-   0        0        0      603 2023-03-29 08:33:10.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/dvc_init_google.sh
+-rw-rw-rw-   0        0        0       73 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/dvc_push.sh
+-rw-rw-rw-   0        0        0      239 2023-03-27 07:13:27.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/git_init.sh
+-rw-rw-rw-   0        0        0      491 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/gunicorn.conf.py
+-rw-rw-rw-   0        0        0     1183 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/locustfile.py
+-rw-rw-rw-   0        0        0       23 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/requirements_docker.txt
+-rw-rw-rw-   0        0        0        0 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/deploy_files/sample.csv
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.440414 gaia-core-0.0.2/gaia/cli/tester/dsp/
+-rw-rw-rw-   0        0        0      877 2022-06-15 14:26:55.000000 gaia-core-0.0.2/gaia/cli/tester/dsp/add_experiment_template.py
+-rw-rw-rw-   0        0        0      941 2022-06-15 14:26:55.000000 gaia-core-0.0.2/gaia/cli/tester/dsp/get_dataset_options_template.py
+-rw-rw-rw-   0        0        0      993 2023-02-19 16:02:38.000000 gaia-core-0.0.2/gaia/cli/tester/dsp/get_model_options_template.py
+-rw-rw-rw-   0        0        0      379 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/tester/evaluator_template.py
+-rw-rw-rw-   0        0        0     9122 2023-03-29 15:58:50.000000 gaia-core-0.0.2/gaia/cli/tester/general_tester_template.py
+-rw-rw-rw-   0        0        0     3578 2023-03-29 15:58:51.000000 gaia-core-0.0.2/gaia/cli/tester/reporter_template.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.471666 gaia-core-0.0.2/gaia/cli/tester/server/
+-rw-rw-rw-   0        0        0      260 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/server/__init__.py
+-rw-rw-rw-   0        0        0       71 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/server/__init___template.py
+-rw-rw-rw-   0        0        0     5872 2023-03-30 10:48:25.000000 gaia-core-0.0.2/gaia/cli/tester/server/main_template.py
+-rw-rw-rw-   0        0        0      657 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/server/pool_template.py
+-rw-rw-rw-   0        0        0     4105 2023-03-29 15:58:50.000000 gaia-core-0.0.2/gaia/cli/tester/server/server_template_old.py
+-rw-rw-rw-   0        0        0     1739 2023-03-30 10:26:37.000000 gaia-core-0.0.2/gaia/cli/tester/server/test_server_post_stream_template.py
+-rw-rw-rw-   0        0        0     1823 2022-06-15 12:42:01.000000 gaia-core-0.0.2/gaia/cli/tester/server/test_server_post_template.py
+-rw-rw-rw-   0        0        0     4468 2023-03-27 09:49:11.000000 gaia-core-0.0.2/gaia/cli/tester/server/token_generator_template.py
+-rw-rw-rw-   0        0        0    17998 2023-03-29 15:58:50.000000 gaia-core-0.0.2/gaia/cli/tester/tester_template.py
+-rw-rw-rw-   0        0        0      398 2023-03-29 15:58:50.000000 gaia-core-0.0.2/gaia/cli/tester/trainer_template.py
+-rw-rw-rw-   0        0        0     2596 2023-05-03 05:53:58.000000 gaia-core-0.0.2/gaia/gaia.py
+-rw-rw-rw-   0        0        0    28324 2023-03-30 10:27:08.000000 gaia-core-0.0.2/gaia_cli.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:54:28.502915 gaia-core-0.0.2/gaia_core.egg-info/
+-rw-rw-rw-   0        0        0     1170 2023-05-03 07:54:28.000000 gaia-core-0.0.2/gaia_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3564 2023-05-03 07:54:28.000000 gaia-core-0.0.2/gaia_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:54:28.000000 gaia-core-0.0.2/gaia_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-03 07:54:28.000000 gaia-core-0.0.2/gaia_core.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       56 2023-05-03 07:54:28.000000 gaia-core-0.0.2/gaia_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-03 07:54:28.000000 gaia-core-0.0.2/gaia_core.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:54:28.518541 gaia-core-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     3025 2023-05-03 07:54:20.000000 gaia-core-0.0.2/setup.py
```

### Comparing `gaia-core-0.0.1/PKG-INFO` & `gaia-core-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gaia-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: Gaia SDK library
 Home-page: UNKNOWN
 Author: oribrau@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # gaia-sdk
 gaia sdk
 
 #how to install
-pip install gaia-sdk
+pip install gaia-core
 
 #how to use
 ```python
 
 # add .vendors_keys file including
 # OPEN_AI_KEY=
 # COHERE_AI_KEY=
```

### Comparing `gaia-core-0.0.1/README.md` & `gaia-core-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # gaia-sdk
 gaia sdk
 
 #how to install
-pip install gaia-sdk
+pip install gaia-core
 
 #how to use
 ```python
 
 # add .vendors_keys file including
 # OPEN_AI_KEY=
 # COHERE_AI_KEY=
```

### Comparing `gaia-core-0.0.1/gaia/base/vendors/chat_gpt.py` & `gaia-core-0.0.2/gaia/base/vendors/chat_gpt.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/base/vendors/co_here.py` & `gaia-core-0.0.2/gaia/base/vendors/co_here.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/base/vendors/vendors_manager.py` & `gaia-core-0.0.2/gaia/base/vendors/vendors_manager.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/.gitignore` & `gaia-core-0.0.2/gaia/cli/.gitignore`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/forcer_template.py` & `gaia-core-0.0.2/gaia/cli/forcer_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/labelizer_template.py` & `gaia-core-0.0.2/gaia/cli/labelizer_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/main_template.py` & `gaia-core-0.0.2/gaia/cli/main_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/pipeline_template.py` & `gaia-core-0.0.2/gaia/cli/pipeline_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/pipeline_test_template.py` & `gaia-core-0.0.2/gaia/cli/pipeline_test_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/postprocess_template.py` & `gaia-core-0.0.2/gaia/cli/postprocess_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/predictable_template.py` & `gaia-core-0.0.2/gaia/cli/predictable_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/predictor_template.py` & `gaia-core-0.0.2/gaia/cli/predictor_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/preprocess_template.py` & `gaia-core-0.0.2/gaia/cli/preprocess_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/schema/test_input_template.py` & `gaia-core-0.0.2/gaia/cli/schema/test_input_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/schema/test_output_template.py` & `gaia-core-0.0.2/gaia/cli/schema/test_output_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/shared_artifacts_template.py` & `gaia-core-0.0.2/gaia/cli/shared_artifacts_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/cloud_eval/Dockerfile_batch_processor` & `gaia-core-0.0.2/gaia/cli/tester/cloud_eval/Dockerfile_batch_processor`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/cloud_eval/auto_model_eval.sh` & `gaia-core-0.0.2/gaia/cli/tester/cloud_eval/auto_model_eval.sh`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/cloud_eval/build_worker.sh` & `gaia-core-0.0.2/gaia/cli/tester/cloud_eval/build_worker.sh`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/cloud_eval/cloud_eval_client.py` & `gaia-core-0.0.2/gaia/cli/tester/cloud_eval/cloud_eval_client.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/cloud_eval/eval_on_cloud_proc.sh` & `gaia-core-0.0.2/gaia/cli/tester/cloud_eval/eval_on_cloud_proc.sh`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/cloud_eval/tag_version.sh` & `gaia-core-0.0.2/gaia/cli/tester/cloud_eval/tag_version.sh`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/dataset_template.py` & `gaia-core-0.0.2/gaia/cli/tester/dataset_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/deploy_files/Dockerfile` & `gaia-core-0.0.2/gaia/cli/tester/deploy_files/Dockerfile`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-prd.yaml` & `gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-prd.yaml`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-stg.yaml` & `gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/app-gcp_gae-stg.yaml`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/deploy_files/deploy/jenkins.env` & `gaia-core-0.0.2/gaia/cli/tester/deploy_files/deploy/jenkins.env`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/deploy_files/dvc_init.sh` & `gaia-core-0.0.2/gaia/cli/tester/deploy_files/dvc_init.sh`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/deploy_files/dvc_init_google.sh` & `gaia-core-0.0.2/gaia/cli/tester/deploy_files/dvc_init_google.sh`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/deploy_files/locustfile.py` & `gaia-core-0.0.2/gaia/cli/tester/deploy_files/locustfile.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/dsp/add_experiment_template.py` & `gaia-core-0.0.2/gaia/cli/tester/dsp/add_experiment_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/dsp/get_dataset_options_template.py` & `gaia-core-0.0.2/gaia/cli/tester/dsp/get_dataset_options_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/dsp/get_model_options_template.py` & `gaia-core-0.0.2/gaia/cli/tester/dsp/get_model_options_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/general_tester_template.py` & `gaia-core-0.0.2/gaia/cli/tester/general_tester_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/reporter_template.py` & `gaia-core-0.0.2/gaia/cli/tester/reporter_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/server/main_template.py` & `gaia-core-0.0.2/gaia/cli/tester/server/main_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/server/pool_template.py` & `gaia-core-0.0.2/gaia/cli/tester/server/pool_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/server/server_template_old.py` & `gaia-core-0.0.2/gaia/cli/tester/server/server_template_old.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/server/test_server_post_stream_template.py` & `gaia-core-0.0.2/gaia/cli/tester/server/test_server_post_stream_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/server/test_server_post_template.py` & `gaia-core-0.0.2/gaia/cli/tester/server/test_server_post_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/server/token_generator_template.py` & `gaia-core-0.0.2/gaia/cli/tester/server/token_generator_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/cli/tester/tester_template.py` & `gaia-core-0.0.2/gaia/cli/tester/tester_template.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia/gaia.py` & `gaia-core-0.0.2/gaia/gaia.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia_cli.py` & `gaia-core-0.0.2/gaia_cli.py`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/gaia_core.egg-info/PKG-INFO` & `gaia-core-0.0.2/gaia_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gaia-core
-Version: 0.0.1
+Version: 0.0.2
 Summary: Gaia SDK library
 Home-page: UNKNOWN
 Author: oribrau@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # gaia-sdk
 gaia sdk
 
 #how to install
-pip install gaia-sdk
+pip install gaia-core
 
 #how to use
 ```python
 
 # add .vendors_keys file including
 # OPEN_AI_KEY=
 # COHERE_AI_KEY=
```

### Comparing `gaia-core-0.0.1/gaia_core.egg-info/SOURCES.txt` & `gaia-core-0.0.2/gaia_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gaia-core-0.0.1/setup.py` & `gaia-core-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging as log
 from shutil import rmtree
 from setuptools import find_packages, setup
 from distutils.command.clean import clean
 from distutils.cmd import Command
 
 package_name = 'gaia-core'
+version = '0.0.2'
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 
 class CleanCommand(clean):
     """
     Custom implementation of ``clean`` setuptools command."""
@@ -47,15 +48,15 @@
 
     packages=find_packages(include=['gaia*']),
     package_data={'': ['config.json', 'cors_allowed_origins.json', '.gitignore'] + extra_files + cloud_eval_extra_files + dsp_files},
     entry_points='''
         [console_scripts]
         gaia-cli=gaia_cli:cli
     ''',
-    version='0.0.1',
+    version=version,
     description='Gaia SDK library',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
     # url='http://pypi.python.org/pypi/PackageName/',
     author='oribrau@gmail.com',
     license='MIT',
     install_requires=required,
```

