# Comparing `tmp/truss-0.4.4.dev3.tar.gz` & `tmp/truss-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "truss-0.4.4.dev3.tar", max compression
+gzip compressed data, was "truss-0.4.5.tar", max compression
```

## Comparing `truss-0.4.4.dev3.tar` & `truss-0.4.5.tar`

### file list

```diff
@@ -1,164 +1,168 @@
--rw-r--r--   0        0        0     5483 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2576 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/CONTRIBUTING.md
--rw-r--r--   0        0        0     1064 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/LICENSE
--rw-r--r--   0        0        0     5958 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/README.md
--rw-r--r--   0        0        0     3316 2023-04-21 04:27:43.127092 truss-0.4.4.dev3/ROADMAP.md
--rw-r--r--   0        0        0      465 2023-04-21 04:27:43.131092 truss-0.4.4.dev3/context_builder.Dockerfile
--rw-r--r--   0        0        0     2209 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/pyproject.toml
--rw-r--r--   0        0        0      330 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/__init__.py
--rw-r--r--   0        0        0      252 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/blob_backend.py
--rw-r--r--   0        0        0      733 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/blob_backend_registry.py
--rw-r--r--   0        0        0      648 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/blob/http_public_blob_backend.py
--rw-r--r--   0        0        0    13295 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/build.py
--rw-r--r--   0        0        0    10452 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/cli.py
--rw-r--r--   0        0        0     2742 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/constants.py
--rw-r--r--   0        0        0     1237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/image_builder.py
--rw-r--r--   0        0        0     5130 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/serving_image_builder.py
--rw-r--r--   0        0        0     4511 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/training_image_builder.py
--rw-r--r--   0        0        0     1976 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/image_builder/util.py
--rw-r--r--   0        0        0     1686 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/load_model_local.py
--rw-r--r--   0        0        0     2239 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/train_local.py
--rw-r--r--   0        0        0     5801 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/truss_module_loader.py
--rw-r--r--   0        0        0      853 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/local_loader/utils.py
--rw-r--r--   0        0        0      436 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/contexts/truss_context.py
--rw-r--r--   0        0        0      394 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/decorators.py
--rw-r--r--   0        0        0     3641 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/docker.py
--rw-r--r--   0        0        0     3759 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/environment_inference/requirements_inference.py
--rw-r--r--   0        0        0      643 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/errors.py
--rw-r--r--   0        0        0      824 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/local/local_config.py
--rw-r--r--   0        0        0     3896 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/local/local_config_handler.py
--rw-r--r--   0        0        0     2713 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_framework.py
--rw-r--r--   0        0        0     1687 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/__init__.py
--rw-r--r--   0        0        0     1895 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/huggingface_transformer.py
--rw-r--r--   0        0        0      918 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/keras.py
--rw-r--r--   0        0        0     1237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/lightgbm.py
--rw-r--r--   0        0        0     2410 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/mlflow.py
--rw-r--r--   0        0        0     2441 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/pytorch.py
--rw-r--r--   0        0        0     1232 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/sklearn.py
--rw-r--r--   0        0        0     1027 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_frameworks/xgboost.py
--rw-r--r--   0        0        0     6565 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/model_inference.py
--rw-r--r--   0        0        0      510 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/notebook.py
--rw-r--r--   0        0        0    10874 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/calc_patch.py
--rw-r--r--   0        0        0      774 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/dir_signature.py
--rw-r--r--   0        0        0     2388 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/hash.py
--rw-r--r--   0        0        0      468 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/signature.py
--rw-r--r--   0        0        0      937 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/patch/types.py
--rw-r--r--   0        0        0      237 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/pytest.ini
--rw-r--r--   0        0        0      705 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/readme_generator.py
--rw-r--r--   0        0        0     2482 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/README.md.jinja
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/__init__.py
--rw-r--r--   0        0        0     1409 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/base.Dockerfile.jinja
--rw-r--r--   0        0        0     2190 2023-04-21 04:27:43.235093 truss-0.4.4.dev3/truss/templates/control/control/application.py
--rw-r--r--   0        0        0     4083 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/endpoints.py
--rw-r--r--   0        0        0      413 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/context_managers.py
--rw-r--r--   0        0        0      877 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/errors.py
--rw-r--r--   0        0        0     5801 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_controller.py
--rw-r--r--   0        0        0     2596 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_process_controller.py
--rw-r--r--   0        0        0     2399 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_starter.py
--rw-r--r--   0        0        0     5389 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/patch_applier.py
--rw-r--r--   0        0        0     3070 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/helpers/types.py
--rw-r--r--   0        0        0     1849 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/control/server.py
--rw-r--r--   0        0        0       82 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/control/requirements.txt
--rw-r--r--   0        0        0       48 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/examples.yaml
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/model/__init__.py
--rw-r--r--   0        0        0      979 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/model/model.py
--rw-r--r--   0        0        0      460 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/custom/train/train.py
--rw-r--r--   0        0        0     2616 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/docs/README.md
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/__init__.py
--rw-r--r--   0        0        0     2272 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/model.py
--rw-r--r--   0        0        0       47 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/huggingface_transformer/requirements.txt
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/keras/model/__init__.py
--rw-r--r--   0        0        0     1173 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/keras/model/model.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/lightgbm/model/__init__.py
--rw-r--r--   0        0        0     1696 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/lightgbm/model/model.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/mlflow/model/__init__.py
--rw-r--r--   0        0        0     1196 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/mlflow/model/model.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pipeline/model/__init__.py
--rw-r--r--   0        0        0      875 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pipeline/model/model.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pytorch/model/__init__.py
--rw-r--r--   0        0        0     1708 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/pytorch/model/model.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/__init__.py
--rw-r--r--   0        0        0       85 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/__init__.py
--rw-r--r--   0        0        0      237 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/errors.py
--rw-r--r--   0        0        0     1892 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/external_data_resolver.py
--rw-r--r--   0        0        0     1352 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/logging.py
--rw-r--r--   0        0        0     3318 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/serialization.py
--rw-r--r--   0        0        0     5511 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/truss_server.py
--rw-r--r--   0        0        0      416 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/common/util.py
--rw-r--r--   0        0        0      733 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/inference_server.py
--rw-r--r--   0        0        0     5384 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/model_wrapper.py
--rw-r--r--   0        0        0      162 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server/requirements.txt
--rw-r--r--   0        0        0     1054 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/server.Dockerfile.jinja
--rw-r--r--   0        0        0      138 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/README.md
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/__init__.py
--rw-r--r--   0        0        0     1430 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/shared/secrets_resolver.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/sklearn/model/__init__.py
--rw-r--r--   0        0        0     1666 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/sklearn/model/model.py
--rw-r--r--   0        0        0     3400 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training/job.py
--rw-r--r--   0        0        0       12 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training/requirements.txt
--rw-r--r--   0        0        0      491 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/training.Dockerfile.jinja
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/xgboost/model/__init__.py
--rw-r--r--   0        0        0     1898 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/templates/xgboost/model/model.py
--rw-r--r--   0        0        0    30286 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/auto-mpg.data
--rw-r--r--   0        0        0      216 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/context_builder_image_test/Dockerfile
--rw-r--r--   0        0        0       72 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/context_builder_image_test/test.py
--rw-r--r--   0        0        0     1394 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/happy.ipynb
--rw-r--r--   0        0        0     1267 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/patch_ping_test_server/app.py
--rw-r--r--   0        0        0    23279 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/pima-indians-diabetes.csv
--rw-r--r--   0        0        0     1586 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_int_example.md
--rw-r--r--   0        0        0     1607 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_no_example.md
--rw-r--r--   0        0        0     1726 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/readme_str_example.md
--rw-r--r--   0        0        0      669 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/config.yaml
--rw-r--r--   0        0        0       48 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/examples.yaml
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/dummy
--rw-r--r--   0        0        0     1006 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/test_data/test_truss/model/model.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/__init__.py
--rw-r--r--   0        0        0    19997 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/conftest.py
--rw-r--r--   0        0        0      783 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_load_local.py
--rw-r--r--   0        0        0     5337 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_truss_module_finder.py
--rw-r--r--   0        0        0      968 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/environments_inference/test_requirements_inference.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.239093 truss-0.4.4.dev3/truss/tests/local/__init__.py
--rw-r--r--   0        0        0     2245 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/local/test_local_config_handler.py
--rw-r--r--   0        0        0        0 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/__init__.py
--rw-r--r--   0        0        0     3293 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
--rw-r--r--   0        0        0     2789 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_keras_framework.py
--rw-r--r--   0        0        0     2409 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_lightgbm_framework.py
--rw-r--r--   0        0        0     1479 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_pytorch_framework.py
--rw-r--r--   0        0        0     2427 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_sklearn_framework.py
--rw-r--r--   0        0        0     2437 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/model_frameworks/test_xgboost_framework.py
--rw-r--r--   0        0        0    10483 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_calc_patch.py
--rw-r--r--   0        0        0      487 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_dir_signature.py
--rw-r--r--   0        0        0     5983 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_hash.py
--rw-r--r--   0        0        0      394 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_signature.py
--rw-r--r--   0        0        0      273 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/patch/test_types.py
--rw-r--r--   0        0        0    10415 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/samples.py
--rw-r--r--   0        0        0      283 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_context_managers.py
--rw-r--r--   0        0        0     1976 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_patch_applier.py
--rw-r--r--   0        0        0     6937 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/control/control/test_server.py
--rw-r--r--   0        0        0      750 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/core/server/common/test_util.py
--rw-r--r--   0        0        0     1539 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/core/server/test_secrets_resolver.py
--rw-r--r--   0        0        0     2157 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/templates/server/common/test_external_resolver.py
--rw-r--r--   0        0        0     1910 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_backward.py
--rw-r--r--   0        0        0     8260 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_build.py
--rw-r--r--   0        0        0     2359 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_config.py
--rw-r--r--   0        0        0     1188 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_context_builder_image.py
--rw-r--r--   0        0        0      517 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_docker.py
--rw-r--r--   0        0        0     2605 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_model_inference.py
--rw-r--r--   0        0        0      656 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_notebooks.py
--rw-r--r--   0        0        0     1483 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_testing_utilities_for_other_tests.py
--rw-r--r--   0        0        0     1252 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_gatherer.py
--rw-r--r--   0        0        0    31937 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_handle.py
--rw-r--r--   0        0        0      434 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_truss_util.py
--rw-r--r--   0        0        0     1865 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/tests/test_validation.py
--rw-r--r--   0        0        0    12070 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_config.py
--rw-r--r--   0        0        0     2845 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_gatherer.py
--rw-r--r--   0        0        0    40806 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_handle.py
--rw-r--r--   0        0        0     5331 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/truss_spec.py
--rw-r--r--   0        0        0     2124 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/types.py
--rw-r--r--   0        0        0      227 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/data_structures.py
--rw-r--r--   0        0        0      553 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/gpu.py
--rw-r--r--   0        0        0      333 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/jinja.py
--rw-r--r--   0        0        0     2018 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/util/path.py
--rw-r--r--   0        0        0     2317 2023-04-21 04:27:43.243093 truss-0.4.4.dev3/truss/validation.py
--rw-r--r--   0        0        0     7302 1970-01-01 00:00:00.000000 truss-0.4.4.dev3/PKG-INFO
+-rw-r--r--   0        0        0     5483 2023-05-03 21:08:21.549623 truss-0.4.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2576 2023-05-03 21:08:21.549623 truss-0.4.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1064 2023-05-03 21:08:21.553623 truss-0.4.5/LICENSE
+-rw-r--r--   0        0        0     5958 2023-05-03 21:08:21.553623 truss-0.4.5/README.md
+-rw-r--r--   0        0        0     3316 2023-05-03 21:08:21.553623 truss-0.4.5/ROADMAP.md
+-rw-r--r--   0        0        0      465 2023-05-03 21:08:21.553623 truss-0.4.5/context_builder.Dockerfile
+-rw-r--r--   0        0        0     2205 2023-05-03 21:08:21.625624 truss-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      330 2023-05-03 21:08:21.625624 truss-0.4.5/truss/__init__.py
+-rw-r--r--   0        0        0      252 2023-05-03 21:08:21.625624 truss-0.4.5/truss/blob/blob_backend.py
+-rw-r--r--   0        0        0      733 2023-05-03 21:08:21.625624 truss-0.4.5/truss/blob/blob_backend_registry.py
+-rw-r--r--   0        0        0      648 2023-05-03 21:08:21.625624 truss-0.4.5/truss/blob/http_public_blob_backend.py
+-rw-r--r--   0        0        0    13295 2023-05-03 21:08:21.625624 truss-0.4.5/truss/build.py
+-rw-r--r--   0        0        0    10452 2023-05-03 21:08:21.625624 truss-0.4.5/truss/cli.py
+-rw-r--r--   0        0        0     2813 2023-05-03 21:08:21.625624 truss-0.4.5/truss/constants.py
+-rw-r--r--   0        0        0     1294 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/image_builder/image_builder.py
+-rw-r--r--   0        0        0     5529 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/image_builder/serving_image_builder.py
+-rw-r--r--   0        0        0     4950 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/image_builder/training_image_builder.py
+-rw-r--r--   0        0        0     1976 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/image_builder/util.py
+-rw-r--r--   0        0        0     1686 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/local_loader/load_model_local.py
+-rw-r--r--   0        0        0     2239 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/local_loader/train_local.py
+-rw-r--r--   0        0        0     5801 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/local_loader/truss_module_loader.py
+-rw-r--r--   0        0        0      853 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/local_loader/utils.py
+-rw-r--r--   0        0        0      436 2023-05-03 21:08:21.625624 truss-0.4.5/truss/contexts/truss_context.py
+-rw-r--r--   0        0        0      394 2023-05-03 21:08:21.625624 truss-0.4.5/truss/decorators.py
+-rw-r--r--   0        0        0     3641 2023-05-03 21:08:21.625624 truss-0.4.5/truss/docker.py
+-rw-r--r--   0        0        0     3759 2023-05-03 21:08:21.625624 truss-0.4.5/truss/environment_inference/requirements_inference.py
+-rw-r--r--   0        0        0      643 2023-05-03 21:08:21.625624 truss-0.4.5/truss/errors.py
+-rw-r--r--   0        0        0      824 2023-05-03 21:08:21.625624 truss-0.4.5/truss/local/local_config.py
+-rw-r--r--   0        0        0     3896 2023-05-03 21:08:21.625624 truss-0.4.5/truss/local/local_config_handler.py
+-rw-r--r--   0        0        0     2713 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_framework.py
+-rw-r--r--   0        0        0     1687 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_frameworks/huggingface_transformer.py
+-rw-r--r--   0        0        0      918 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_frameworks/keras.py
+-rw-r--r--   0        0        0     1237 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_frameworks/lightgbm.py
+-rw-r--r--   0        0        0     2410 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_frameworks/mlflow.py
+-rw-r--r--   0        0        0     2441 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_frameworks/pytorch.py
+-rw-r--r--   0        0        0     1232 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_frameworks/sklearn.py
+-rw-r--r--   0        0        0     1027 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_frameworks/xgboost.py
+-rw-r--r--   0        0        0     6565 2023-05-03 21:08:21.625624 truss-0.4.5/truss/model_inference.py
+-rw-r--r--   0        0        0      510 2023-05-03 21:08:21.625624 truss-0.4.5/truss/notebook.py
+-rw-r--r--   0        0        0    11065 2023-05-03 21:08:21.625624 truss-0.4.5/truss/patch/calc_patch.py
+-rw-r--r--   0        0        0      774 2023-05-03 21:08:21.625624 truss-0.4.5/truss/patch/dir_signature.py
+-rw-r--r--   0        0        0     2388 2023-05-03 21:08:21.625624 truss-0.4.5/truss/patch/hash.py
+-rw-r--r--   0        0        0      468 2023-05-03 21:08:21.625624 truss-0.4.5/truss/patch/signature.py
+-rw-r--r--   0        0        0      937 2023-05-03 21:08:21.625624 truss-0.4.5/truss/patch/types.py
+-rw-r--r--   0        0        0      237 2023-05-03 21:08:21.625624 truss-0.4.5/truss/pytest.ini
+-rw-r--r--   0        0        0      705 2023-05-03 21:08:21.625624 truss-0.4.5/truss/readme_generator.py
+-rw-r--r--   0        0        0     2482 2023-05-03 21:08:21.625624 truss-0.4.5/truss/templates/README.md.jinja
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.625624 truss-0.4.5/truss/templates/__init__.py
+-rw-r--r--   0        0        0     1887 2023-05-03 21:08:21.625624 truss-0.4.5/truss/templates/_truss_build.Dockerfile.jinja
+-rw-r--r--   0        0        0     2023 2023-05-03 21:08:21.625624 truss-0.4.5/truss/templates/base.Dockerfile.jinja
+-rw-r--r--   0        0        0     2190 2023-05-03 21:08:21.625624 truss-0.4.5/truss/templates/control/control/application.py
+-rw-r--r--   0        0        0     4083 2023-05-03 21:08:21.625624 truss-0.4.5/truss/templates/control/control/endpoints.py
+-rw-r--r--   0        0        0      413 2023-05-03 21:08:21.625624 truss-0.4.5/truss/templates/control/control/helpers/context_managers.py
+-rw-r--r--   0        0        0      877 2023-05-03 21:08:21.625624 truss-0.4.5/truss/templates/control/control/helpers/errors.py
+-rw-r--r--   0        0        0     5801 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/control/control/helpers/inference_server_controller.py
+-rw-r--r--   0        0        0     2596 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/control/control/helpers/inference_server_process_controller.py
+-rw-r--r--   0        0        0     2399 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/control/control/helpers/inference_server_starter.py
+-rw-r--r--   0        0        0     5389 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/control/control/helpers/patch_applier.py
+-rw-r--r--   0        0        0     3070 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/control/control/helpers/types.py
+-rw-r--r--   0        0        0     1849 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/control/control/server.py
+-rw-r--r--   0        0        0       82 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/control/requirements.txt
+-rw-r--r--   0        0        0       48 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/custom/examples.yaml
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/custom/model/__init__.py
+-rw-r--r--   0        0        0      534 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/custom/model/model.py
+-rw-r--r--   0        0        0      460 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/custom/train/train.py
+-rw-r--r--   0        0        0     2616 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/docs/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/huggingface_transformer/model/__init__.py
+-rw-r--r--   0        0        0     1827 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/huggingface_transformer/model/model.py
+-rw-r--r--   0        0        0       47 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/huggingface_transformer/requirements.txt
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/keras/model/__init__.py
+-rw-r--r--   0        0        0      728 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/keras/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/lightgbm/model/__init__.py
+-rw-r--r--   0        0        0     1251 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/lightgbm/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/mlflow/model/__init__.py
+-rw-r--r--   0        0        0      751 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/mlflow/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/pipeline/model/__init__.py
+-rw-r--r--   0        0        0      430 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/pipeline/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/pytorch/model/__init__.py
+-rw-r--r--   0        0        0     1263 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/pytorch/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/__init__.py
+-rw-r--r--   0        0        0       85 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/common/__init__.py
+-rw-r--r--   0        0        0      237 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/common/errors.py
+-rw-r--r--   0        0        0     1892 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/common/external_data_resolver.py
+-rw-r--r--   0        0        0     1352 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/common/logging.py
+-rw-r--r--   0        0        0      593 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/common/retry.py
+-rw-r--r--   0        0        0     3318 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/common/serialization.py
+-rw-r--r--   0        0        0     5511 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/common/truss_server.py
+-rw-r--r--   0        0        0      416 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/common/util.py
+-rw-r--r--   0        0        0      733 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/inference_server.py
+-rw-r--r--   0        0        0     5674 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/model_wrapper.py
+-rw-r--r--   0        0        0      162 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server/requirements.txt
+-rw-r--r--   0        0        0     1054 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/server.Dockerfile.jinja
+-rw-r--r--   0        0        0      138 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/shared/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/shared/__init__.py
+-rw-r--r--   0        0        0     1430 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/shared/secrets_resolver.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/sklearn/model/__init__.py
+-rw-r--r--   0        0        0     1221 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/sklearn/model/model.py
+-rw-r--r--   0        0        0     3400 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/training/job.py
+-rw-r--r--   0        0        0       12 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/training/requirements.txt
+-rw-r--r--   0        0        0      491 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/training.Dockerfile.jinja
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/xgboost/model/__init__.py
+-rw-r--r--   0        0        0     1453 2023-05-03 21:08:21.629624 truss-0.4.5/truss/templates/xgboost/model/model.py
+-rw-r--r--   0        0        0    30286 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/auto-mpg.data
+-rw-r--r--   0        0        0      216 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/context_builder_image_test/Dockerfile
+-rw-r--r--   0        0        0       72 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/context_builder_image_test/test.py
+-rw-r--r--   0        0        0     1394 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/happy.ipynb
+-rw-r--r--   0        0        0     1267 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/patch_ping_test_server/app.py
+-rw-r--r--   0        0        0    23279 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/pima-indians-diabetes.csv
+-rw-r--r--   0        0        0     1586 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/readme_int_example.md
+-rw-r--r--   0        0        0     1607 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/readme_no_example.md
+-rw-r--r--   0        0        0     1726 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/readme_str_example.md
+-rw-r--r--   0        0        0      669 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/test_truss/config.yaml
+-rw-r--r--   0        0        0       48 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/test_truss/examples.yaml
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/test_truss/model/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/test_truss/model/dummy
+-rw-r--r--   0        0        0      534 2023-05-03 21:08:21.629624 truss-0.4.5/truss/test_data/test_truss/model/model.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/__init__.py
+-rw-r--r--   0        0        0    20835 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/conftest.py
+-rw-r--r--   0        0        0      783 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/contexts/local_loader/test_load_local.py
+-rw-r--r--   0        0        0     5337 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/contexts/local_loader/test_truss_module_finder.py
+-rw-r--r--   0        0        0      968 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/environments_inference/test_requirements_inference.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/local/__init__.py
+-rw-r--r--   0        0        0     2245 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/local/test_local_config_handler.py
+-rw-r--r--   0        0        0        0 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/model_frameworks/__init__.py
+-rw-r--r--   0        0        0     3293 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/model_frameworks/test_huggingface_transformer_framework.py
+-rw-r--r--   0        0        0     2789 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/model_frameworks/test_keras_framework.py
+-rw-r--r--   0        0        0     2409 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/model_frameworks/test_lightgbm_framework.py
+-rw-r--r--   0        0        0     1479 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/model_frameworks/test_pytorch_framework.py
+-rw-r--r--   0        0        0     2427 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/model_frameworks/test_sklearn_framework.py
+-rw-r--r--   0        0        0     2437 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/model_frameworks/test_xgboost_framework.py
+-rw-r--r--   0        0        0    11109 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/patch/test_calc_patch.py
+-rw-r--r--   0        0        0      487 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/patch/test_dir_signature.py
+-rw-r--r--   0        0        0     5983 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/patch/test_hash.py
+-rw-r--r--   0        0        0      394 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/patch/test_signature.py
+-rw-r--r--   0        0        0      273 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/patch/test_types.py
+-rw-r--r--   0        0        0    10415 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/samples.py
+-rw-r--r--   0        0        0      283 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/templates/control/control/helpers/test_context_managers.py
+-rw-r--r--   0        0        0     1976 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/templates/control/control/helpers/test_patch_applier.py
+-rw-r--r--   0        0        0     6937 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/templates/control/control/test_server.py
+-rw-r--r--   0        0        0      750 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/templates/core/server/common/test_util.py
+-rw-r--r--   0        0        0     1539 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/templates/core/server/test_secrets_resolver.py
+-rw-r--r--   0        0        0     2157 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/templates/server/common/test_external_resolver.py
+-rw-r--r--   0        0        0     2038 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/templates/server/common/test_retry.py
+-rw-r--r--   0        0        0     2252 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/templates/server/test_model_wrapper.py
+-rw-r--r--   0        0        0     1910 2023-05-03 21:08:21.629624 truss-0.4.5/truss/tests/test_backward.py
+-rw-r--r--   0        0        0     8260 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_build.py
+-rw-r--r--   0        0        0     2359 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_config.py
+-rw-r--r--   0        0        0     1188 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_context_builder_image.py
+-rw-r--r--   0        0        0      517 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_docker.py
+-rw-r--r--   0        0        0     2605 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_model_inference.py
+-rw-r--r--   0        0        0      656 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1483 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_testing_utilities_for_other_tests.py
+-rw-r--r--   0        0        0     1252 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_truss_gatherer.py
+-rw-r--r--   0        0        0    33011 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_truss_handle.py
+-rw-r--r--   0        0        0      434 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_truss_util.py
+-rw-r--r--   0        0        0     1865 2023-05-03 21:08:21.633624 truss-0.4.5/truss/tests/test_validation.py
+-rw-r--r--   0        0        0    12200 2023-05-03 21:08:21.633624 truss-0.4.5/truss/truss_config.py
+-rw-r--r--   0        0        0     2845 2023-05-03 21:08:21.633624 truss-0.4.5/truss/truss_gatherer.py
+-rw-r--r--   0        0        0    41070 2023-05-03 21:08:21.633624 truss-0.4.5/truss/truss_handle.py
+-rw-r--r--   0        0        0     5428 2023-05-03 21:08:21.633624 truss-0.4.5/truss/truss_spec.py
+-rw-r--r--   0        0        0     2124 2023-05-03 21:08:21.633624 truss-0.4.5/truss/types.py
+-rw-r--r--   0        0        0      227 2023-05-03 21:08:21.633624 truss-0.4.5/truss/util/data_structures.py
+-rw-r--r--   0        0        0      553 2023-05-03 21:08:21.633624 truss-0.4.5/truss/util/gpu.py
+-rw-r--r--   0        0        0      333 2023-05-03 21:08:21.633624 truss-0.4.5/truss/util/jinja.py
+-rw-r--r--   0        0        0     2018 2023-05-03 21:08:21.633624 truss-0.4.5/truss/util/path.py
+-rw-r--r--   0        0        0     2317 2023-05-03 21:08:21.633624 truss-0.4.5/truss/validation.py
+-rw-r--r--   0        0        0     7297 1970-01-01 00:00:00.000000 truss-0.4.5/PKG-INFO
```

### Comparing `truss-0.4.4.dev3/CODE_OF_CONDUCT.md` & `truss-0.4.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/CONTRIBUTING.md` & `truss-0.4.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/LICENSE` & `truss-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/README.md` & `truss-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/ROADMAP.md` & `truss-0.4.5/ROADMAP.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/pyproject.toml` & `truss-0.4.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "truss"
-version = "0.4.4dev3"
+version = "0.4.5"
 description = "A seamless bridge from model development to model delivery"
 license = "MIT"
 readme = "README.md"
 authors = ["Pankaj Gupta <pankaj@baseten.co>", "Phil Howes <phil@baseten.co>"]
 include = ["*.txt", "*.Dockerfile", "*.md"]
 repository = "https://github.com/basetenlabs/truss"
 keywords = ["MLOps", "AI", "Model Serving", "Model Deployment", "Machine Learning"]
```

### Comparing `truss-0.4.4.dev3/truss/blob/blob_backend_registry.py` & `truss-0.4.5/truss/blob/blob_backend_registry.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/blob/http_public_blob_backend.py` & `truss-0.4.5/truss/blob/http_public_blob_backend.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/build.py` & `truss-0.4.5/truss/build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/cli.py` & `truss-0.4.5/truss/cli.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/constants.py` & `truss-0.4.5/truss/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 SERVING_DIR: pathlib.Path = TEMPLATES_DIR
 
 REQUIREMENTS_TXT_FILENAME = "requirements.txt"
 SERVER_REQUIREMENTS_TXT_FILENAME = "server_requirements.txt"
 TRAINING_REQUIREMENTS_TXT_FILENAME = "training_requirements.txt"
 SYSTEM_PACKAGES_TXT_FILENAME = "system_packages.txt"
 
+TRUSS_BUILD_DOCKERFILE_TEMPLATE_NAME = "_truss_build.Dockerfile.jinja"
 SERVER_DOCKERFILE_TEMPLATE_NAME = "server.Dockerfile.jinja"
 TRAINING_DOCKERFILE_TEMPLATE_NAME = "training.Dockerfile.jinja"
 MODEL_DOCKERFILE_NAME = "Dockerfile"
 TRAINING_DOCKERFILE_NAME = "Dockerfile"
 
 README_TEMPLATE_NAME = "README.md.jinja"
 MODEL_README_NAME = "README.md"
```

### Comparing `truss-0.4.4.dev3/truss/contexts/image_builder/image_builder.py` & `truss-0.4.5/truss/contexts/image_builder/image_builder.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class ImageBuilder(ABC):
     def build_image(
         self,
         build_dir: Optional[Path] = None,
         tag: Optional[str] = None,
         labels: Optional[dict] = None,
+        cache: bool = True,
     ):
         """Build image.
 
         Arguments:
             build_dir(Path): Directory to use for building the docker image. If None
                              then a temporary directory is used.
             tag(str): A tag to assign to the docker image.
@@ -23,14 +24,15 @@
 
         with given_or_temporary_dir(build_dir) as build_dir_path:
             self.prepare_image_build_dir(build_dir_path)
             return Docker.client().build(
                 str(build_dir_path),
                 labels=labels if labels else {},
                 tags=tag or self.default_tag,
+                cache=cache,
             )
 
     @property
     @abstractmethod
     def default_tag(self):
         pass
```

### Comparing `truss-0.4.4.dev3/truss/contexts/image_builder/serving_image_builder.py` & `truss-0.4.5/truss/contexts/image_builder/serving_image_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     SERVER_CODE_DIR,
     SERVER_DOCKERFILE_TEMPLATE_NAME,
     SERVER_REQUIREMENTS_TXT_FILENAME,
     SHARED_SERVING_AND_TRAINING_CODE_DIR,
     SHARED_SERVING_AND_TRAINING_CODE_DIR_NAME,
     SYSTEM_PACKAGES_TXT_FILENAME,
     TEMPLATES_DIR,
+    TRUSS_BUILD_DOCKERFILE_TEMPLATE_NAME,
 )
 from truss.contexts.image_builder.image_builder import ImageBuilder
 from truss.contexts.image_builder.util import (
     TRUSS_BASE_IMAGE_VERSION_TAG,
     file_is_not_empty,
     to_dotted_python_version,
     truss_base_image_name,
@@ -100,34 +101,41 @@
     ):
         config = self._spec.config
         data_dir = build_dir / config.data_dir
         bundled_packages_dir = build_dir / config.bundled_packages_dir
         dockerfile_template = read_template_from_fs(
             TEMPLATES_DIR, SERVER_DOCKERFILE_TEMPLATE_NAME
         )
-        base_image_name = truss_base_image_name(job_type="server")
+        truss_build_template_path = TRUSS_BUILD_DOCKERFILE_TEMPLATE_NAME
         python_version = to_dotted_python_version(config.python_version)
-        tag = truss_base_image_tag(
-            python_version=python_version,
-            use_gpu=config.resources.use_gpu,
-            live_reload=config.live_reload,
-            version_tag=TRUSS_BASE_IMAGE_VERSION_TAG,
-        )
-        base_image_name_and_tag = f"{base_image_name}:{tag}"
+        if config.base_image:
+            base_image_name_and_tag = config.base_image
+        else:
+            base_image_name = truss_base_image_name(job_type="server")
+            tag = truss_base_image_tag(
+                python_version=python_version,
+                use_gpu=config.resources.use_gpu,
+                live_reload=config.live_reload,
+                version_tag=TRUSS_BASE_IMAGE_VERSION_TAG,
+            )
+            base_image_name_and_tag = f"{base_image_name}:{tag}"
         should_install_system_requirements = file_is_not_empty(
             build_dir / SYSTEM_PACKAGES_TXT_FILENAME
         )
         should_install_python_requirements = file_is_not_empty(
             build_dir / REQUIREMENTS_TXT_FILENAME
         )
         dockerfile_contents = dockerfile_template.render(
             should_install_server_requirements=should_install_server_requirements,
             base_image_name_and_tag=base_image_name_and_tag,
             should_install_system_requirements=should_install_system_requirements,
             should_install_requirements=should_install_python_requirements,
             config=config,
+            truss_build_template_path=truss_build_template_path,
+            python_version=python_version,
+            live_reload=config.live_reload,
             data_dir_exists=data_dir.exists(),
             bundled_packages_dir_exists=bundled_packages_dir.exists(),
             truss_hash=directory_content_hash(self._truss_dir),
         )
         docker_file_path = build_dir / MODEL_DOCKERFILE_NAME
         docker_file_path.write_text(dockerfile_contents)
```

### Comparing `truss-0.4.4.dev3/truss/contexts/image_builder/training_image_builder.py` & `truss-0.4.5/truss/contexts/image_builder/training_image_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     SYSTEM_PACKAGES_TXT_FILENAME,
     TEMPLATES_DIR,
     TRAINING_DOCKERFILE_NAME,
     TRAINING_DOCKERFILE_TEMPLATE_NAME,
     TRAINING_JOB_WRAPPER_CODE_DIR,
     TRAINING_JOB_WRAPPER_CODE_DIR_NAME,
     TRAINING_REQUIREMENTS_TXT_FILENAME,
+    TRUSS_BUILD_DOCKERFILE_TEMPLATE_NAME,
 )
 from truss.contexts.image_builder.image_builder import ImageBuilder
 from truss.contexts.image_builder.util import (
     TRUSS_BASE_IMAGE_VERSION_TAG,
     file_is_not_empty,
     to_dotted_python_version,
     truss_base_image_name,
@@ -88,32 +89,40 @@
             build_dir / self._spec.config.bundled_packages_dir
         ).exists()
         template_loader = FileSystemLoader(str(TEMPLATES_DIR))
         template_env = Environment(loader=template_loader)
         dockerfile_template = template_env.get_template(
             TRAINING_DOCKERFILE_TEMPLATE_NAME
         )
+        truss_build_template_path = TRUSS_BUILD_DOCKERFILE_TEMPLATE_NAME
         should_install_system_requirements = file_is_not_empty(
             build_dir / SYSTEM_PACKAGES_TXT_FILENAME
         )
         should_install_requirements = file_is_not_empty(
             build_dir / REQUIREMENTS_TXT_FILENAME
         )
         config = self._spec.config
-        base_image_name = truss_base_image_name(job_type="training")
-        tag = truss_base_image_tag(
-            python_version=to_dotted_python_version(config.python_version),
-            use_gpu=config.resources.use_gpu,
-            live_reload=config.live_reload,
-            version_tag=TRUSS_BASE_IMAGE_VERSION_TAG,
-        )
-        base_image_name_and_tag = f"{base_image_name}:{tag}"
+        python_version = to_dotted_python_version(config.python_version)
+        if config.base_image:
+            base_image_name_and_tag = config.base_image
+        else:
+            base_image_name = truss_base_image_name(job_type="training")
+            tag = truss_base_image_tag(
+                python_version=python_version,
+                use_gpu=config.resources.use_gpu,
+                live_reload=config.live_reload,
+                version_tag=TRUSS_BASE_IMAGE_VERSION_TAG,
+            )
+            base_image_name_and_tag = f"{base_image_name}:{tag}"
         dockerfile_contents = dockerfile_template.render(
             base_image_name_and_tag=base_image_name_and_tag,
             config=self._spec.config,
+            truss_build_template_path=truss_build_template_path,
+            python_version=python_version,
+            live_reload=config.live_reload,
             bundled_packages_dir_exists=bundled_packages_dir_exists,
             should_install_system_requirements=should_install_system_requirements,
             should_install_requirements=should_install_requirements,
         )
         docker_file_path = build_dir / TRAINING_DOCKERFILE_NAME
         with docker_file_path.open("w") as docker_file:
             docker_file.write(dockerfile_contents)
```

### Comparing `truss-0.4.4.dev3/truss/contexts/image_builder/util.py` & `truss-0.4.5/truss/contexts/image_builder/util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/contexts/local_loader/load_model_local.py` & `truss-0.4.5/truss/contexts/local_loader/load_model_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/contexts/local_loader/train_local.py` & `truss-0.4.5/truss/contexts/local_loader/train_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/contexts/local_loader/truss_module_loader.py` & `truss-0.4.5/truss/contexts/local_loader/truss_module_loader.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/contexts/local_loader/utils.py` & `truss-0.4.5/truss/contexts/local_loader/utils.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/docker.py` & `truss-0.4.5/truss/docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/environment_inference/requirements_inference.py` & `truss-0.4.5/truss/environment_inference/requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/errors.py` & `truss-0.4.5/truss/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/local/local_config.py` & `truss-0.4.5/truss/local/local_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/local/local_config_handler.py` & `truss-0.4.5/truss/local/local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_framework.py` & `truss-0.4.5/truss/model_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_frameworks/__init__.py` & `truss-0.4.5/truss/model_frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_frameworks/huggingface_transformer.py` & `truss-0.4.5/truss/model_frameworks/huggingface_transformer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_frameworks/keras.py` & `truss-0.4.5/truss/model_frameworks/keras.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_frameworks/lightgbm.py` & `truss-0.4.5/truss/model_frameworks/lightgbm.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_frameworks/mlflow.py` & `truss-0.4.5/truss/model_frameworks/mlflow.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_frameworks/pytorch.py` & `truss-0.4.5/truss/model_frameworks/pytorch.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_frameworks/sklearn.py` & `truss-0.4.5/truss/model_frameworks/sklearn.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_frameworks/xgboost.py` & `truss-0.4.5/truss/model_frameworks/xgboost.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/model_inference.py` & `truss-0.4.5/truss/model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/patch/calc_patch.py` & `truss-0.4.5/truss/patch/calc_patch.py`

 * *Files 5% similar despite different names*

```diff
@@ -130,22 +130,30 @@
     root: Path,
     previous_root_path_content_hashes: Dict[str, str],
     ignore_patterns: Optional[List[str]],
 ) -> Dict[str, List[str]]:
     """
     TODO(pankaj) add support for directory creation in patch
     """
-    unignored_paths = _calc_unignored_paths(root, ignore_patterns)
+    root_relative_new_paths = set(
+        (str(path.relative_to(root)) for path in root.glob("**/*"))
+    )
+    unignored_new_paths = _calc_unignored_paths(
+        root, root_relative_new_paths, ignore_patterns
+    )
     previous_root_relative_paths = set(previous_root_path_content_hashes.keys())
+    unignored_prev_paths = _calc_unignored_paths(
+        root, previous_root_relative_paths, ignore_patterns
+    )
 
-    added_paths = unignored_paths - previous_root_relative_paths
-    removed_paths = previous_root_relative_paths - unignored_paths
+    added_paths = unignored_new_paths - unignored_prev_paths
+    removed_paths = unignored_prev_paths - unignored_new_paths
 
     updated_paths = set()
-    common_paths = unignored_paths.intersection(previous_root_relative_paths)
+    common_paths = unignored_new_paths.intersection(unignored_prev_paths)
     for path in common_paths:
         full_path: Path = root / path
         if full_path.is_file():
             content_hash = file_content_hash_str(full_path)
             previous_content_hash = previous_root_path_content_hashes[path]
             if content_hash != previous_content_hash:
                 updated_paths.add(path)
@@ -154,27 +162,26 @@
         "added": list(added_paths),
         "updated": list(updated_paths),
         "removed": list(removed_paths),
     }
 
 
 def _calc_unignored_paths(
-    root: Path, ignore_patterns: Optional[List[str]] = None
+    root: Path,
+    root_relative_paths: Set[str],
+    ignore_patterns: Optional[List[str]] = None,
 ) -> Set[str]:
     root_relative_ignored_paths = set()
     if ignore_patterns is not None:
         for ignore_pattern in ignore_patterns:
             ignored_paths_for_pattern = set(
                 (str(path.relative_to(root)) for path in root.glob(ignore_pattern))
             )
             root_relative_ignored_paths.update(ignored_paths_for_pattern)
 
-    root_relative_paths = set(
-        (str(path.relative_to(root)) for path in root.glob("**/*"))
-    )
     return root_relative_paths - root_relative_ignored_paths
 
 
 def _calc_config_patches(
     prev_config: TrussConfig, new_config: TrussConfig
 ) -> Optional[List[Patch]]:
     """Calculate patch based on changes to config.
```

### Comparing `truss-0.4.4.dev3/truss/patch/dir_signature.py` & `truss-0.4.5/truss/patch/dir_signature.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/patch/hash.py` & `truss-0.4.5/truss/patch/hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/patch/types.py` & `truss-0.4.5/truss/patch/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/readme_generator.py` & `truss-0.4.5/truss/readme_generator.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/README.md.jinja` & `truss-0.4.5/truss/templates/README.md.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/application.py` & `truss-0.4.5/truss/templates/control/control/application.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/endpoints.py` & `truss-0.4.5/truss/templates/control/control/endpoints.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/helpers/errors.py` & `truss-0.4.5/truss/templates/control/control/helpers/errors.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_controller.py` & `truss-0.4.5/truss/templates/control/control/helpers/inference_server_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_process_controller.py` & `truss-0.4.5/truss/templates/control/control/helpers/inference_server_process_controller.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/helpers/inference_server_starter.py` & `truss-0.4.5/truss/templates/control/control/helpers/inference_server_starter.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/helpers/patch_applier.py` & `truss-0.4.5/truss/templates/control/control/helpers/patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/helpers/types.py` & `truss-0.4.5/truss/templates/control/control/helpers/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/control/control/server.py` & `truss-0.4.5/truss/templates/control/control/server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/docs/README.md` & `truss-0.4.5/truss/templates/docs/README.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/huggingface_transformer/model/model.py` & `truss-0.4.5/truss/templates/huggingface_transformer/model/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,28 +23,14 @@
             transformer_config["device"] = 0
 
         self._model = pipeline(
             task=self._config["model_type"],
             **transformer_config,
         )
 
-    def preprocess(self, model_input: Any) -> Any:
-        """
-        Incorporate pre-processing required by the model if desired here.
-
-        These might be feature transformations that are tightly coupled to the model.
-        """
-        return model_input
-
-    def postprocess(self, model_output: Any) -> Any:
-        """
-        Incorporate post-processing required by the model if desired here.
-        """
-        return model_output
-
     def predict(self, model_input: Any) -> Any:
         model_output = {}
         instances = model_input
 
         with torch.no_grad():
             if self._has_named_args:
                 result = [self._model(**instance) for instance in instances]
```

### Comparing `truss-0.4.4.dev3/truss/templates/keras/model/model.py` & `truss-0.4.5/truss/templates/pytorch/model/model.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 from typing import Any
 
-import numpy as np
-from tensorflow import keras
+import torch
+from torch import package
 
 
 class Model:
     def __init__(self, **kwargs) -> None:
         self._data_dir = kwargs["data_dir"]
         config = kwargs["config"]
-        model_metadata = config["model_metadata"]
-        self._model_binary_dir = model_metadata["model_binary_dir"]
+        self._model_metadata = config["model_metadata"]
         self._model = None
+        self._model_dtype = None
+        self._device = torch.device(
+            "cuda:0"
+            if torch.cuda.is_available() and config["resources"]["use_gpu"]
+            else "cpu"
+        )
 
     def load(self):
-        self._model = keras.models.load_model(
-            str(self._data_dir / self._model_binary_dir)
+        imp = package.PackageImporter(
+            self._data_dir / "model" / self._model_metadata["torch_package_file"]
         )
-
-    def preprocess(self, model_input: Any) -> Any:
-        """
-        Incorporate pre-processing required by the model if desired here.
-
-        These might be feature transformations that are tightly coupled to the model.
-        """
-        return model_input
-
-    def postprocess(self, model_output: Any) -> Any:
-        """
-        Incorporate post-processing required by the model if desired here.
-        """
-        return model_output
+        package_name = self._model_metadata["torch_model_package_name"]
+        model_pickle_filename = self._model_metadata["torch_model_pickle_filename"]
+        self._model = imp.load_pickle(package_name, model_pickle_filename)
+        self._model_dtype = list(self._model.parameters())[0].dtype
 
     def predict(self, model_input: Any) -> Any:
         model_output = {}
-        inputs = np.array(model_input)
-        result = self._model.predict(inputs).tolist()
-        model_output["predictions"] = result
-        return model_output
+        with torch.no_grad():
+            inputs = torch.tensor(
+                model_input, dtype=self._model_dtype, device=self._device
+            )
+            model_output["predictions"] = self._model(inputs).tolist()
+            return model_output
```

### Comparing `truss-0.4.4.dev3/truss/templates/lightgbm/model/model.py` & `truss-0.4.5/truss/templates/xgboost/model/model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,39 @@
 from typing import Any
 
+import xgboost as xgb
+
 MODEL_BASENAME = "model"
-MODEL_EXTENSIONS = [".joblib", ".pkl", ".pickle"]
+MODEL_EXTENSIONS = [".ubj"]
 
 
 class Model:
     def __init__(self, **kwargs) -> None:
         self._data_dir = kwargs["data_dir"]
         config = kwargs["config"]
         model_metadata = config["model_metadata"]
-        # LightGBM does not implement a `predict_proba` function
+        # XGBoost models, saved and loaded via the native save/load
+        # in XGBoost do not support predicting probabilities unless
+        # they are a multi-class classification problem.
+        # TODO: Integrate model_metadata field to determine model
+        # objective function to determine if an XGBoost model
+        # supports predicting probabilities.
         self._supports_predict_proba = False
         self._model_binary_dir = model_metadata["model_binary_dir"]
         self._model = None
 
     def load(self):
-        import joblib
-
         model_binary_dir_path = self._data_dir / self._model_binary_dir
         paths = [
             (model_binary_dir_path / MODEL_BASENAME).with_suffix(model_extension)
             for model_extension in MODEL_EXTENSIONS
         ]
         model_file_path = next(path for path in paths if path.exists())
-        self._model = joblib.load(model_file_path)
-
-    def preprocess(self, model_input: Any) -> Any:
-        """
-        Incorporate pre-processing required by the model if desired here.
-
-        These might be feature transformations that are tightly coupled to the model.
-        """
-        return model_input
-
-    def postprocess(self, model_output: Any) -> Any:
-        """
-        Incorporate post-processing required by the model if desired here.
-        """
-        return model_output
+        self._model = xgb.Booster()
+        self._model.load_model(model_file_path)
 
     def predict(self, model_input: Any) -> Any:
         model_output = {}
-        result = self._model.predict(model_input)
+        dmatrix_inputs = xgb.DMatrix(model_input)
+        result = self._model.predict(dmatrix_inputs)
         model_output["predictions"] = result
-        if self._supports_predict_proba:
-            model_output["probabilities"] = self._model.predict_proba(
-                model_input
-            ).tolist()
         return model_output
```

### Comparing `truss-0.4.4.dev3/truss/templates/server/common/external_data_resolver.py` & `truss-0.4.5/truss/templates/server/common/external_data_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/server/common/logging.py` & `truss-0.4.5/truss/templates/server/common/logging.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/server/common/serialization.py` & `truss-0.4.5/truss/templates/server/common/serialization.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/server/common/truss_server.py` & `truss-0.4.5/truss/templates/server/common/truss_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/server/inference_server.py` & `truss-0.4.5/truss/templates/server/inference_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/server/model_wrapper.py` & `truss-0.4.5/truss/templates/server/model_wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 import importlib
 import inspect
 import logging
+import os
 import sys
 import time
 import traceback
 from enum import Enum
 from pathlib import Path
 from threading import Lock, Thread
 from typing import Dict, Optional, Union
 
 import kserve
 from cloudevents.http import CloudEvent
 from common.external_data_resolver import download_external_data  # noqa: E402
+from common.retry import retry
 from kserve.grpc.grpc_predict_v2_pb2 import ModelInferRequest, ModelInferResponse
 from shared.secrets_resolver import SecretsResolver
 
 MODEL_BASENAME = "model"
 
+NUM_LOAD_RETRIES = int(os.environ.get("NUM_LOAD_RETRIES_TRUSS", "3"))
+
 
 class ModelWrapper(kserve.Model):
     class Status(Enum):
         NOT_READY = 0
         LOADING = 1
         READY = 2
         FAILED = 3
@@ -107,15 +111,21 @@
         if _signature_accepts_keyword_arg(model_class_signature, "data_dir"):
             model_init_params["data_dir"] = data_dir
         if _signature_accepts_keyword_arg(model_class_signature, "secrets"):
             model_init_params["secrets"] = SecretsResolver.get_secrets(self._config)
         self._model = model_class(**model_init_params)
 
         if hasattr(self._model, "load"):
-            self._model.load()
+            retry(
+                self._model.load,
+                NUM_LOAD_RETRIES,
+                self.logger.warn,
+                "Failed to load model.",
+                gap_seconds=1.0,
+            )
 
     def preprocess(
         self,
         payload: Union[Dict, CloudEvent, ModelInferRequest],
         headers: Optional[Dict[str, str]] = None,
     ) -> Union[Dict, ModelInferRequest]:
         if not hasattr(self._model, "preprocess"):
```

### Comparing `truss-0.4.4.dev3/truss/templates/server.Dockerfile.jinja` & `truss-0.4.5/truss/templates/server.Dockerfile.jinja`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/shared/secrets_resolver.py` & `truss-0.4.5/truss/templates/shared/secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/templates/sklearn/model/model.py` & `truss-0.4.5/truss/templates/sklearn/model/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -20,28 +20,14 @@
         paths = [
             (model_binary_dir_path / MODEL_BASENAME).with_suffix(model_extension)
             for model_extension in MODEL_EXTENSIONS
         ]
         model_file_path = next(path for path in paths if path.exists())
         self._model = joblib.load(model_file_path)
 
-    def preprocess(self, model_input: Any) -> Any:
-        """
-        Incorporate pre-processing required by the model if desired here.
-
-        These might be feature transformations that are tightly coupled to the model.
-        """
-        return model_input
-
-    def postprocess(self, model_output: Any) -> Any:
-        """
-        Incorporate post-processing required by the model if desired here.
-        """
-        return model_output
-
     def predict(self, model_input: Any) -> Any:
         model_output = {}
         result = self._model.predict(model_input)
         model_output["predictions"] = result
         if self._supports_predict_proba:
             model_output["probabilities"] = self._model.predict_proba(
                 model_input
```

### Comparing `truss-0.4.4.dev3/truss/templates/training/job.py` & `truss-0.4.5/truss/templates/training/job.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/test_data/auto-mpg.data` & `truss-0.4.5/truss/test_data/auto-mpg.data`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/test_data/happy.ipynb` & `truss-0.4.5/truss/test_data/happy.ipynb`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/test_data/patch_ping_test_server/app.py` & `truss-0.4.5/truss/test_data/patch_ping_test_server/app.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/test_data/pima-indians-diabetes.csv` & `truss-0.4.5/truss/test_data/pima-indians-diabetes.csv`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/test_data/readme_int_example.md` & `truss-0.4.5/truss/test_data/readme_int_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/test_data/readme_no_example.md` & `truss-0.4.5/truss/test_data/readme_no_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/test_data/readme_str_example.md` & `truss-0.4.5/truss/test_data/readme_str_example.md`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/test_data/test_truss/config.yaml` & `truss-0.4.5/truss/test_data/test_truss/config.yaml`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/conftest.py` & `truss-0.4.5/truss/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -771,7 +771,44 @@
 ) -> Path:
     dir_path = where_dir / truss_name
     handle = init(str(dir_path))
     if handle_ops is not None:
         handle_ops(handle)
     handle.spec.model_class_filepath.write_text(model_code)
     return dir_path
+
+
+class Helpers:
+    @staticmethod
+    @contextlib.contextmanager
+    def file_content(file_path: Path, content: str):
+        orig_content = file_path.read_text()
+        try:
+            file_path.write_text(content)
+            yield
+        finally:
+            file_path.write_text(orig_content)
+
+    @staticmethod
+    @contextlib.contextmanager
+    def sys_path(path: Path):
+        try:
+            sys.path.append(str(path))
+            yield
+        finally:
+            sys.path.pop()
+
+    @staticmethod
+    @contextlib.contextmanager
+    def env_var(var: str, value: str):
+        orig_environ = os.environ.copy()
+        try:
+            os.environ[var] = value
+            yield
+        finally:
+            os.environ.clear()
+            os.environ.update(orig_environ)
+
+
+@pytest.fixture
+def helpers():
+    return Helpers()
```

### Comparing `truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_load_local.py` & `truss-0.4.5/truss/tests/contexts/local_loader/test_load_local.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/contexts/local_loader/test_truss_module_finder.py` & `truss-0.4.5/truss/tests/contexts/local_loader/test_truss_module_finder.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/environments_inference/test_requirements_inference.py` & `truss-0.4.5/truss/tests/environments_inference/test_requirements_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/local/test_local_config_handler.py` & `truss-0.4.5/truss/tests/local/test_local_config_handler.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/model_frameworks/test_huggingface_transformer_framework.py` & `truss-0.4.5/truss/tests/model_frameworks/test_huggingface_transformer_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/model_frameworks/test_keras_framework.py` & `truss-0.4.5/truss/tests/model_frameworks/test_keras_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/model_frameworks/test_lightgbm_framework.py` & `truss-0.4.5/truss/tests/model_frameworks/test_lightgbm_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/model_frameworks/test_pytorch_framework.py` & `truss-0.4.5/truss/tests/model_frameworks/test_pytorch_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/model_frameworks/test_sklearn_framework.py` & `truss-0.4.5/truss/tests/model_frameworks/test_sklearn_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/model_frameworks/test_xgboost_framework.py` & `truss-0.4.5/truss/tests/model_frameworks/test_xgboost_framework.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/patch/test_calc_patch.py` & `truss-0.4.5/truss/tests/patch/test_calc_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -115,14 +115,31 @@
     patches = calc_truss_patch(
         custom_model_truss_dir,
         prev_sign,
     )
     assert len(patches) == 0
 
 
+def test_calc_truss_ignore_pycache_existing(custom_model_truss_dir: Path):
+    # If __pycache__ existed before and there are no changes, there should be no
+    # patches.
+    top_pycache_path = custom_model_truss_dir / "__pycache__"
+    top_pycache_path.mkdir()
+    (top_pycache_path / "bla.pyc").touch()
+    model_pycache_path = custom_model_truss_dir / "model" / "__pycache__"
+    model_pycache_path.mkdir()
+    (model_pycache_path / "foo.pyo").touch()
+    sign = calc_truss_signature(custom_model_truss_dir)
+    patches = calc_truss_patch(
+        custom_model_truss_dir,
+        sign,
+    )
+    assert len(patches) == 0
+
+
 def test_calc_truss_ignore_changes_outside_patch_relevant_dirs(
     custom_model_truss_dir: Path,
 ):
     prev_sign = calc_truss_signature(custom_model_truss_dir)
     top_pycache_path = custom_model_truss_dir / "__pycache__"
     top_pycache_path.mkdir()
     (top_pycache_path / "README.md").touch()
```

### Comparing `truss-0.4.4.dev3/truss/tests/patch/test_hash.py` & `truss-0.4.5/truss/tests/patch/test_hash.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/samples.py` & `truss-0.4.5/truss/tests/samples.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/templates/control/control/helpers/test_patch_applier.py` & `truss-0.4.5/truss/tests/templates/control/control/helpers/test_patch_applier.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/templates/control/control/test_server.py` & `truss-0.4.5/truss/tests/templates/control/control/test_server.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/templates/core/server/common/test_util.py` & `truss-0.4.5/truss/tests/templates/core/server/common/test_util.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/templates/core/server/test_secrets_resolver.py` & `truss-0.4.5/truss/tests/templates/core/server/test_secrets_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/templates/server/common/test_external_resolver.py` & `truss-0.4.5/truss/tests/templates/server/common/test_external_resolver.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_backward.py` & `truss-0.4.5/truss/tests/test_backward.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_build.py` & `truss-0.4.5/truss/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_config.py` & `truss-0.4.5/truss/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_context_builder_image.py` & `truss-0.4.5/truss/tests/test_context_builder_image.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_docker.py` & `truss-0.4.5/truss/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_model_inference.py` & `truss-0.4.5/truss/tests/test_model_inference.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_notebooks.py` & `truss-0.4.5/truss/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_testing_utilities_for_other_tests.py` & `truss-0.4.5/truss/tests/test_testing_utilities_for_other_tests.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_truss_gatherer.py` & `truss-0.4.5/truss/tests/test_truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/tests/test_truss_handle.py` & `truss-0.4.5/truss/tests/test_truss_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,47 @@
     th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
     tag = "test-build-image-tag:0.0.1"
     image = th.build_serving_docker_image(tag=tag)
     assert image.repo_tags[0] == tag
 
 
 @pytest.mark.integration
+@pytest.mark.parametrize(
+    "base_image, expected_fail",
+    [
+        ("baseten/truss-server-base:3.9-v0.4.3", False),
+        ("baseten/truss-training-base:3.9-v0.4.3", False),
+        ("python:3.8.3", False),
+        ("alpine", True),
+        ("python:2.7-slim", True),
+        ("python:3.5-slim", True),
+    ],
+)
+def test_build_docker_image_from_user_base_image(
+    custom_model_truss_dir, base_image, expected_fail
+):
+    th = TrussHandle(custom_model_truss_dir)
+    th.set_base_image(base_image)
+    try:
+        th.build_serving_docker_image(cache=False)
+    except DockerException as exc:
+        assert expected_fail is True
+        assert "It returned with code 1" in str(exc)
+
+
+@pytest.mark.integration
+def test_docker_predict_custom_base_image(custom_model_truss_dir_with_pre_and_post):
+    th = TrussHandle(custom_model_truss_dir_with_pre_and_post)
+    th.set_base_image("baseten/truss-server-base:3.9-v0.4.3")
+    with ensure_kill_all():
+        result = th.docker_predict([1, 2])
+        assert result == {"predictions": [4, 5]}
+
+
+@pytest.mark.integration
 def test_build_docker_image_gpu(custom_model_truss_dir_for_gpu, tmp_path):
     th = TrussHandle(custom_model_truss_dir_for_gpu)
     tag = "test-build-image-gpu-tag:0.0.1"
     build_dir = tmp_path / "scaffold_build_dir"
     image = th.build_serving_docker_image(tag=tag, build_dir=build_dir)
     assert image.repo_tags[0] == tag
```

### Comparing `truss-0.4.4.dev3/truss/tests/test_validation.py` & `truss-0.4.5/truss/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/truss_config.py` & `truss-0.4.5/truss/truss_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,14 +240,15 @@
     description: Optional[str] = None
     bundled_packages_dir: str = DEFAULT_BUNDLED_PACKAGES_DIR
     external_package_dirs: List[str] = field(default_factory=list)
     live_reload: bool = False
     # spec_version is a version string
     spec_version: str = DEFAULT_SPEC_VERSION
     train: Train = field(default_factory=Train)
+    base_image: Optional[str] = None
 
     @property
     def canonical_python_version(self) -> str:
         return {
             "py39": "3.9",
             "py38": "3.8",
             "py37": "3.7",
@@ -286,14 +287,15 @@
             ),
             external_package_dirs=d.get("external_package_dirs", []),
             live_reload=d.get("live_reload", False),
             train=Train.from_dict(d.get("train", {})),
             external_data=transform_optional(
                 d.get("external_data"), ExternalData.from_list
             ),
+            base_image=d.get("base_image", None),
         )
         config.validate()
         return config
 
     @staticmethod
     def from_yaml(yaml_path: Path):
         with yaml_path.open() as yaml_file:
@@ -323,14 +325,15 @@
             "secrets": self.secrets,
             "description": self.description,
             "bundled_packages_dir": self.bundled_packages_dir,
             "external_package_dirs": self.external_package_dirs,
             "live_reload": self.live_reload,
             "spec_version": self.spec_version,
             "train": self.train.to_dict(),
+            "base_image": self.base_image,
         }
         if self.external_data is not None:
             d["external_data"] = transform_optional(
                 self.external_data, lambda data: data.to_list()
             )
         return d
```

### Comparing `truss-0.4.4.dev3/truss/truss_gatherer.py` & `truss-0.4.5/truss/truss_gatherer.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/truss_handle.py` & `truss-0.4.5/truss/truss_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,21 +127,25 @@
 
     def build_docker_image(self, *args, **kwargs):
         """[Deprected] Please use build_serving_docker_image."""
         return self.build_serving_docker_image(*args, **kwargs)
 
     @proxy_to_shadow_if_scattered
     def build_serving_docker_image(
-        self, build_dir: Optional[Path] = None, tag: Optional[str] = None
+        self,
+        build_dir: Optional[Path] = None,
+        tag: Optional[str] = None,
+        cache: bool = True,
     ):
         image = self._build_image(
             builder_context=ServingImageBuilderContext,
             labels=self._get_serving_lookup_labels(),
             build_dir=build_dir,
             tag=tag,
+            cache=cache,
         )
         self._store_signature()
         return image
 
     @proxy_to_shadow_if_scattered
     def build_training_docker_image(
         self, build_dir: Optional[Path] = None, tag: Optional[str] = None
@@ -685,14 +689,18 @@
 
         def enable_gpu_fn(conf: TrussConfig):
             new_resources = replace(conf.resources, use_gpu=True)
             return replace(conf, resources=new_resources)
 
         self._update_config(enable_gpu_fn)
 
+    def set_base_image(self, base_image: str):
+        """Set the base image for a given truss"""
+        self._update_config(lambda conf: replace(conf, base_image=base_image))
+
     @proxy_to_shadow_if_scattered
     def patch_container(self, patch_request: Dict):
         """Patch changes onto the container running this Truss.
 
         Useful for local incremental development.
         TODO(pankaj): Turn patch_request into a dataclass
         """
@@ -916,25 +924,24 @@
 
     def _build_image(
         self,
         builder_context,
         labels: Dict[str, str],
         build_dir: Optional[Path] = None,
         tag: Optional[str] = None,
+        cache: bool = True,
     ):
         image = _docker_image_from_labels(labels=labels)
         if image is not None:
             return image
 
         build_dir_path = Path(build_dir) if build_dir is not None else None
         image_builder = builder_context.run(self._truss_dir)
         build_image_result = image_builder.build_image(
-            build_dir_path,
-            tag,
-            labels=labels,
+            build_dir_path, tag, labels=labels, cache=cache
         )
         return build_image_result
 
     def _update_config(self, update_config_fn: Callable[[TrussConfig], TrussConfig]):
         config = update_config_fn(self._spec.config)
         config.write_to_yaml_file(self._spec.config_path)
         # reload spec
```

### Comparing `truss-0.4.4.dev3/truss/truss_spec.py` & `truss-0.4.5/truss/truss_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,10 +180,14 @@
     def description(self) -> str:
         return self._config.description
 
     @property
     def live_reload(self) -> bool:
         return self._config.live_reload
 
+    @property
+    def base_image(self) -> Optional[str]:
+        return self._config.base_image
+
 
 def _join_lines(lines: List[str]) -> str:
     return "\n".join(lines) + "\n"
```

### Comparing `truss-0.4.4.dev3/truss/types.py` & `truss-0.4.5/truss/types.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/util/gpu.py` & `truss-0.4.5/truss/util/gpu.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/util/path.py` & `truss-0.4.5/truss/util/path.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/truss/validation.py` & `truss-0.4.5/truss/validation.py`

 * *Files identical despite different names*

### Comparing `truss-0.4.4.dev3/PKG-INFO` & `truss-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: truss
-Version: 0.4.4.dev3
+Version: 0.4.5
 Summary: A seamless bridge from model development to model delivery
 Home-page: https://github.com/basetenlabs/truss
 License: MIT
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Pankaj Gupta
 Author-email: pankaj@baseten.co
 Requires-Python: >=3.8,<3.11
```

