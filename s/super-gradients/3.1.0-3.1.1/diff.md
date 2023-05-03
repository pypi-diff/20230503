# Comparing `tmp/super_gradients-3.1.0-py3-none-any.whl.zip` & `tmp/super_gradients-3.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,560 +1,559 @@
-Zip file size: 965424 bytes, number of entries: 558
--rw-r--r--  2.0 unx      711 b- defN 23-May-02 15:39 super_gradients/__init__.py
--rw-r--r--  2.0 unx     1657 b- defN 23-May-02 15:39 super_gradients/evaluate_checkpoint.py
--rw-r--r--  2.0 unx     1807 b- defN 23-May-02 15:39 super_gradients/evaluate_from_recipe.py
--rw-r--r--  2.0 unx      702 b- defN 23-May-02 15:39 super_gradients/qat_from_recipe.py
--rwxr-xr-x  2.0 unx       44 b- defN 23-May-02 15:39 super_gradients/requirements.pro.txt
--rwxr-xr-x  2.0 unx      729 b- defN 23-May-02 15:39 super_gradients/requirements.txt
--rw-r--r--  2.0 unx      537 b- defN 23-May-02 15:39 super_gradients/resume_experiment.py
--rw-r--r--  2.0 unx      693 b- defN 23-May-02 15:39 super_gradients/train_from_kd_recipe.py
--rw-r--r--  2.0 unx      650 b- defN 23-May-02 15:39 super_gradients/train_from_recipe.py
--rw-r--r--  2.0 unx     1098 b- defN 23-May-02 15:39 super_gradients/common/__init__.py
--rw-r--r--  2.0 unx    15372 b- defN 23-May-02 15:39 super_gradients/common/object_names.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/abstractions/__init__.py
--rw-r--r--  2.0 unx      879 b- defN 23-May-02 15:39 super_gradients/common/abstractions/abstract_logger.py
--rw-r--r--  2.0 unx     3129 b- defN 23-May-02 15:39 super_gradients/common/abstractions/mute_processes.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/auto_logging/__init__.py
--rw-r--r--  2.0 unx     4687 b- defN 23-May-02 15:39 super_gradients/common/auto_logging/auto_logger.py
--rw-r--r--  2.0 unx     6625 b- defN 23-May-02 15:39 super_gradients/common/auto_logging/console_logging.py
--rw-r--r--  2.0 unx      142 b- defN 23-May-02 15:39 super_gradients/common/aws_connection/__init__.py
--rw-r--r--  2.0 unx     4182 b- defN 23-May-02 15:39 super_gradients/common/aws_connection/aws_connector.py
--rw-r--r--  2.0 unx     7198 b- defN 23-May-02 15:39 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
--rw-r--r--  2.0 unx      119 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/__init__.py
--rw-r--r--  2.0 unx      669 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/crash_handler.py
--rw-r--r--  2.0 unx    11775 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/crash_tips.py
--rw-r--r--  2.0 unx      886 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/crash_tips_setup.py
--rw-r--r--  2.0 unx     1740 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/exception.py
--rw-r--r--  2.0 unx     2357 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/exception_monitoring_setup.py
--rw-r--r--  2.0 unx      789 b- defN 23-May-02 15:39 super_gradients/common/crash_handler/utils.py
--rw-r--r--  2.0 unx      140 b- defN 23-May-02 15:39 super_gradients/common/data_connection/__init__.py
--rw-r--r--  2.0 unx    17959 b- defN 23-May-02 15:39 super_gradients/common/data_connection/s3_connector.py
--rw-r--r--  2.0 unx      325 b- defN 23-May-02 15:39 super_gradients/common/data_interface/__init__.py
--rw-r--r--  2.0 unx     9699 b- defN 23-May-02 15:39 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
--rw-r--r--  2.0 unx     2050 b- defN 23-May-02 15:39 super_gradients/common/data_interface/dataset_data_interface.py
--rw-r--r--  2.0 unx      220 b- defN 23-May-02 15:39 super_gradients/common/data_types/__init__.py
--rw-r--r--  2.0 unx      597 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/__init__.py
--rw-r--r--  2.0 unx      309 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/deep_learning_task.py
--rw-r--r--  2.0 unx      108 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/downsample_mode.py
--rw-r--r--  2.0 unx      317 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/evaluation_type.py
--rw-r--r--  2.0 unx     1025 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/multi_gpu_mode.py
--rw-r--r--  2.0 unx     1200 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/strict_load.py
--rw-r--r--  2.0 unx      202 b- defN 23-May-02 15:39 super_gradients/common/data_types/enum/upsample_mode.py
--rw-r--r--  2.0 unx      257 b- defN 23-May-02 15:39 super_gradients/common/decorators/__init__.py
--rw-r--r--  2.0 unx     1567 b- defN 23-May-02 15:39 super_gradients/common/decorators/code_save_decorator.py
--rw-r--r--  2.0 unx     3663 b- defN 23-May-02 15:39 super_gradients/common/decorators/deci_logger.py
--rw-r--r--  2.0 unx     2921 b- defN 23-May-02 15:39 super_gradients/common/decorators/explicit_params_validator.py
--rw-r--r--  2.0 unx     1315 b- defN 23-May-02 15:39 super_gradients/common/decorators/factory_decorator.py
--rw-r--r--  2.0 unx     1132 b- defN 23-May-02 15:39 super_gradients/common/decorators/singleton.py
--rw-r--r--  2.0 unx      202 b- defN 23-May-02 15:39 super_gradients/common/environment/__init__.py
--rw-r--r--  2.0 unx      993 b- defN 23-May-02 15:39 super_gradients/common/environment/argparse_utils.py
--rw-r--r--  2.0 unx     9170 b- defN 23-May-02 15:39 super_gradients/common/environment/cfg_utils.py
--rw-r--r--  2.0 unx     4218 b- defN 23-May-02 15:39 super_gradients/common/environment/checkpoints_dir_utils.py
--rw-r--r--  2.0 unx     2682 b- defN 23-May-02 15:39 super_gradients/common/environment/ddp_utils.py
--rw-r--r--  2.0 unx      752 b- defN 23-May-02 15:39 super_gradients/common/environment/device_utils.py
--rw-r--r--  2.0 unx     1147 b- defN 23-May-02 15:39 super_gradients/common/environment/env_variables.py
--rw-r--r--  2.0 unx     4047 b- defN 23-May-02 15:39 super_gradients/common/environment/omegaconf_utils.py
--rw-r--r--  2.0 unx      459 b- defN 23-May-02 15:39 super_gradients/common/environment/path_utils.py
--rw-r--r--  2.0 unx      112 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/__init__.py
--rw-r--r--  2.0 unx      153 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/cpu.py
--rw-r--r--  2.0 unx     2517 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/data_models.py
--rw-r--r--  2.0 unx     1025 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/disk.py
--rw-r--r--  2.0 unx     5427 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/monitoring.py
--rw-r--r--  2.0 unx      948 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/network.py
--rw-r--r--  2.0 unx      629 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/utils.py
--rw-r--r--  2.0 unx      145 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/virtual_memory.py
--rw-r--r--  2.0 unx      681 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/gpu/__init__.py
--rw-r--r--  2.0 unx     2270 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/gpu/gpu.py
--rw-r--r--  2.0 unx   121647 b- defN 23-May-02 15:39 super_gradients/common/environment/monitoring/gpu/pynvml.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/exceptions/__init__.py
--rw-r--r--  2.0 unx      926 b- defN 23-May-02 15:39 super_gradients/common/exceptions/factory_exceptions.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/factories/__init__.py
--rw-r--r--  2.0 unx     1715 b- defN 23-May-02 15:39 super_gradients/common/factories/activations_type_factory.py
--rw-r--r--  2.0 unx     2881 b- defN 23-May-02 15:39 super_gradients/common/factories/base_factory.py
--rw-r--r--  2.0 unx      258 b- defN 23-May-02 15:39 super_gradients/common/factories/bbox_format_factory.py
--rw-r--r--  2.0 unx      232 b- defN 23-May-02 15:39 super_gradients/common/factories/callbacks_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-May-02 15:39 super_gradients/common/factories/collate_functions_factory.py
--rw-r--r--  2.0 unx      292 b- defN 23-May-02 15:39 super_gradients/common/factories/context_modules_factory.py
--rw-r--r--  2.0 unx      321 b- defN 23-May-02 15:39 super_gradients/common/factories/data_formats_factory.py
--rw-r--r--  2.0 unx      237 b- defN 23-May-02 15:39 super_gradients/common/factories/datasets_factory.py
--rw-r--r--  2.0 unx     1014 b- defN 23-May-02 15:39 super_gradients/common/factories/detection_modules_factory.py
--rw-r--r--  2.0 unx      572 b- defN 23-May-02 15:39 super_gradients/common/factories/list_factory.py
--rw-r--r--  2.0 unx      223 b- defN 23-May-02 15:39 super_gradients/common/factories/losses_factory.py
--rw-r--r--  2.0 unx      226 b- defN 23-May-02 15:39 super_gradients/common/factories/metrics_factory.py
--rw-r--r--  2.0 unx      467 b- defN 23-May-02 15:39 super_gradients/common/factories/optimizers_type_factory.py
--rw-r--r--  2.0 unx      271 b- defN 23-May-02 15:39 super_gradients/common/factories/pre_launch_callbacks_factory.py
--rw-r--r--  2.0 unx      623 b- defN 23-May-02 15:39 super_gradients/common/factories/processing_factory.py
--rw-r--r--  2.0 unx      229 b- defN 23-May-02 15:39 super_gradients/common/factories/samplers_factory.py
--rw-r--r--  2.0 unx      263 b- defN 23-May-02 15:39 super_gradients/common/factories/target_generator_factory.py
--rw-r--r--  2.0 unx     1873 b- defN 23-May-02 15:39 super_gradients/common/factories/transforms_factory.py
--rw-r--r--  2.0 unx     2377 b- defN 23-May-02 15:39 super_gradients/common/factories/type_factory.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/plugins/__init__.py
--rw-r--r--  2.0 unx    10974 b- defN 23-May-02 15:39 super_gradients/common/plugins/deci_client.py
--rw-r--r--  2.0 unx      271 b- defN 23-May-02 15:39 super_gradients/common/registry/__init__.py
--rw-r--r--  2.0 unx     1231 b- defN 23-May-02 15:39 super_gradients/common/registry/albumentation.py
--rw-r--r--  2.0 unx     6006 b- defN 23-May-02 15:39 super_gradients/common/registry/registry.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/common/registry/registry_utils.py
--rw-r--r--  2.0 unx      508 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/__init__.py
--rw-r--r--  2.0 unx     7355 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/abstract_sg_logger.py
--rw-r--r--  2.0 unx    14980 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/base_sg_logger.py
--rw-r--r--  2.0 unx    10055 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/clearml_sg_logger.py
--rw-r--r--  2.0 unx    10103 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/dagshub_sg_logger.py
--rw-r--r--  2.0 unx     6618 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
--rw-r--r--  2.0 unx    13073 b- defN 23-May-02 15:39 super_gradients/common/sg_loggers/wandb_sg_logger.py
--rw-r--r--  2.0 unx    85509 b- defN 23-May-02 15:39 super_gradients/examples/SG_Walkthrough.ipynb
--rw-r--r--  2.0 unx    69618 b- defN 23-May-02 15:39 super_gradients/examples/SG_quickstart_classification.ipynb
--rw-r--r--  2.0 unx    54966 b- defN 23-May-02 15:39 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
--rw-r--r--  2.0 unx    65090 b- defN 23-May-02 15:39 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/cifar10_training_torch_objects/__init__.py
--rw-r--r--  2.0 unx     2526 b- defN 23-May-02 15:39 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/convert_recipe_example/__init__.py
--rw-r--r--  2.0 unx      870 b- defN 23-May-02 15:39 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/ddrnet_imagenet/__init__.py
--rw-r--r--  2.0 unx     3114 b- defN 23-May-02 15:39 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/deci_lab_export_example/__init__.py
--rw-r--r--  2.0 unx     3562 b- defN 23-May-02 15:39 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/early_stop/__init__.py
--rw-r--r--  2.0 unx     1596 b- defN 23-May-02 15:39 super_gradients/examples/early_stop/early_stop_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/evaluate_checkpoint_example/__init__.py
--rw-r--r--  2.0 unx      289 b- defN 23-May-02 15:39 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/evaluate_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      292 b- defN 23-May-02 15:39 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/loggers_examples/__init__.py
--rw-r--r--  2.0 unx     1206 b- defN 23-May-02 15:39 super_gradients/examples/loggers_examples/clearml_logger_example.py
--rw-r--r--  2.0 unx     1088 b- defN 23-May-02 15:39 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/qat_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      277 b- defN 23-May-02 15:39 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/quantization/__init__.py
--rw-r--r--  2.0 unx     1104 b- defN 23-May-02 15:39 super_gradients/examples/quantization/non_default_calibrators_example.py
--rw-r--r--  2.0 unx     2310 b- defN 23-May-02 15:39 super_gradients/examples/quantization/ptq_e2e_example.py
--rw-r--r--  2.0 unx     1850 b- defN 23-May-02 15:39 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
--rw-r--r--  2.0 unx     4732 b- defN 23-May-02 15:39 super_gradients/examples/quantization/resnet_qat_example.py
--rw-r--r--  2.0 unx     1163 b- defN 23-May-02 15:39 super_gradients/examples/quantization/skipping_quantization_example.py
--rw-r--r--  2.0 unx      832 b- defN 23-May-02 15:39 super_gradients/examples/quantization/vanilla_quantize_all_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/regseg_transfer_learning_example/__init__.py
--rw-r--r--  2.0 unx     2379 b- defN 23-May-02 15:39 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/resume_experiment_example/__init__.py
--rw-r--r--  2.0 unx      283 b- defN 23-May-02 15:39 super_gradients/examples/resume_experiment_example/resume_experiment.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/train_from_kd_recipe_example/__init__.py
--rw-r--r--  2.0 unx      292 b- defN 23-May-02 15:39 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_example/__init__.py
--rw-r--r--  2.0 unx      283 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
--rw-r--r--  2.0 unx     1334 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
--rw-r--r--  2.0 unx     1643 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
--rw-r--r--  2.0 unx     1326 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_user_objects/train.py
--rw-r--r--  2.0 unx     2548 b- defN 23-May-02 15:39 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
--rw-r--r--  2.0 unx      174 b- defN 23-May-02 15:39 super_gradients/module_interfaces/__init__.py
--rw-r--r--  2.0 unx     2043 b- defN 23-May-02 15:39 super_gradients/module_interfaces/module_interfaces.py
--rw-r--r--  2.0 unx     3366 b- defN 23-May-02 15:39 super_gradients/modules/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/modules/all_detection_modules.py
--rw-r--r--  2.0 unx      617 b- defN 23-May-02 15:39 super_gradients/modules/anti_alias.py
--rw-r--r--  2.0 unx      776 b- defN 23-May-02 15:39 super_gradients/modules/base_modules.py
--rw-r--r--  2.0 unx     3054 b- defN 23-May-02 15:39 super_gradients/modules/conv_bn_act_block.py
--rw-r--r--  2.0 unx     1976 b- defN 23-May-02 15:39 super_gradients/modules/conv_bn_relu_block.py
--rw-r--r--  2.0 unx    14805 b- defN 23-May-02 15:39 super_gradients/modules/detection_modules.py
--rw-r--r--  2.0 unx     2143 b- defN 23-May-02 15:39 super_gradients/modules/head_replacement_utils.py
--rw-r--r--  2.0 unx     4362 b- defN 23-May-02 15:39 super_gradients/modules/multi_output_modules.py
--rw-r--r--  2.0 unx      860 b- defN 23-May-02 15:39 super_gradients/modules/pixel_shuffle.py
--rw-r--r--  2.0 unx     3953 b- defN 23-May-02 15:39 super_gradients/modules/pose_estimation_modules.py
--rw-r--r--  2.0 unx    11642 b- defN 23-May-02 15:39 super_gradients/modules/qarepvgg_block.py
--rw-r--r--  2.0 unx     8544 b- defN 23-May-02 15:39 super_gradients/modules/repvgg_block.py
--rw-r--r--  2.0 unx     2138 b- defN 23-May-02 15:39 super_gradients/modules/sampling.py
--rw-r--r--  2.0 unx     1459 b- defN 23-May-02 15:39 super_gradients/modules/se_blocks.py
--rw-r--r--  2.0 unx     1403 b- defN 23-May-02 15:39 super_gradients/modules/skip_connections.py
--rw-r--r--  2.0 unx     2968 b- defN 23-May-02 15:39 super_gradients/modules/utils.py
--rw-r--r--  2.0 unx      716 b- defN 23-May-02 15:39 super_gradients/modules/quantization/__init__.py
--rw-r--r--  2.0 unx     2649 b- defN 23-May-02 15:39 super_gradients/modules/quantization/quantized_skip_connections.py
--rw-r--r--  2.0 unx     4604 b- defN 23-May-02 15:39 super_gradients/modules/quantization/quantized_stdc_blocks.py
--rw-r--r--  2.0 unx     1281 b- defN 23-May-02 15:39 super_gradients/modules/quantization/resnet_bottleneck.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/recipes/__init__.py
--rw-r--r--  2.0 unx     1136 b- defN 23-May-02 15:39 super_gradients/recipes/cifar10_resnet.yaml
--rw-r--r--  2.0 unx     3502 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_ddrnet.yaml
--rw-r--r--  2.0 unx     3754 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_kd_base.yaml
--rw-r--r--  2.0 unx     3354 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_pplite_seg50.yaml
--rw-r--r--  2.0 unx     3253 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_pplite_seg75.yaml
--rw-r--r--  2.0 unx     2498 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_regseg48.yaml
--rw-r--r--  2.0 unx     4020 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_segformer.yaml
--rw-r--r--  2.0 unx      618 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_stdc_base.yaml
--rw-r--r--  2.0 unx     2862 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_stdc_seg50.yaml
--rw-r--r--  2.0 unx     3055 b- defN 23-May-02 15:39 super_gradients/recipes/cityscapes_stdc_seg75.yaml
--rw-r--r--  2.0 unx     1830 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_pose_ddrnet39.yaml
--rw-r--r--  2.0 unx     3549 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
--rw-r--r--  2.0 unx     1998 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_pose_pppose_l.yaml
--rw-r--r--  2.0 unx     1996 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ppyoloe_l.yaml
--rw-r--r--  2.0 unx     1996 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ppyoloe_m.yaml
--rw-r--r--  2.0 unx     1882 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ppyoloe_s.yaml
--rw-r--r--  2.0 unx     1975 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ppyoloe_x.yaml
--rw-r--r--  2.0 unx     1889 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
--rw-r--r--  2.0 unx     1385 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_yolo_nas_s.yaml
--rw-r--r--  2.0 unx     2583 b- defN 23-May-02 15:39 super_gradients/recipes/coco2017_yolox.yaml
--rw-r--r--  2.0 unx     1376 b- defN 23-May-02 15:39 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
--rw-r--r--  2.0 unx     1145 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_efficientnet.yaml
--rw-r--r--  2.0 unx     1129 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_mobilenetv2.yaml
--rw-r--r--  2.0 unx      507 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
--rw-r--r--  2.0 unx      719 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
--rw-r--r--  2.0 unx      719 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
--rw-r--r--  2.0 unx     1997 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_regnetY.yaml
--rw-r--r--  2.0 unx     1246 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_repvgg.yaml
--rw-r--r--  2.0 unx     1169 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_resnet50.yaml
--rw-r--r--  2.0 unx     2722 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_resnet50_kd.yaml
--rw-r--r--  2.0 unx     1136 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_vit_base.yaml
--rw-r--r--  2.0 unx     1010 b- defN 23-May-02 15:39 super_gradients/recipes/imagenet_vit_large.yaml
--rw-r--r--  2.0 unx     2007 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_ppyoloe.yaml
--rw-r--r--  2.0 unx     2347 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_yolo_nas_m.yaml
--rw-r--r--  2.0 unx     2347 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_yolo_nas_s.yaml
--rw-r--r--  2.0 unx      473 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
--rw-r--r--  2.0 unx     1915 b- defN 23-May-02 15:39 super_gradients/recipes/roboflow_yolox.yaml
--rw-r--r--  2.0 unx     1246 b- defN 23-May-02 15:39 super_gradients/recipes/supervisely_unet.yaml
--rw-r--r--  2.0 unx     1672 b- defN 23-May-02 15:39 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
--rw-r--r--  2.0 unx     2133 b- defN 23-May-02 15:39 super_gradients/recipes/user_recipe_mnist_example.yaml
--rw-r--r--  2.0 unx     2000 b- defN 23-May-02 15:39 super_gradients/recipes/variable_setup.yaml
--rw-r--r--  2.0 unx     2222 b- defN 23-May-02 15:39 super_gradients/recipes/anchors/ssd_anchors.yaml
--rw-r--r--  2.0 unx      563 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
--rw-r--r--  2.0 unx      104 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
--rw-r--r--  2.0 unx      103 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
--rw-r--r--  2.0 unx      194 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
--rw-r--r--  2.0 unx      156 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
--rw-r--r--  2.0 unx      409 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
--rw-r--r--  2.0 unx      356 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
--rw-r--r--  2.0 unx      281 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml
--rw-r--r--  2.0 unx     1245 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
--rw-r--r--  2.0 unx      985 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
--rw-r--r--  2.0 unx     1112 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
--rw-r--r--  2.0 unx      196 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
--rw-r--r--  2.0 unx      198 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
--rw-r--r--  2.0 unx      204 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
--rw-r--r--  2.0 unx      352 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
--rw-r--r--  2.0 unx       98 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
--rw-r--r--  2.0 unx       89 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
--rw-r--r--  2.0 unx       95 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
--rw-r--r--  2.0 unx       88 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
--rw-r--r--  2.0 unx       86 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
--rw-r--r--  2.0 unx       15 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
--rw-r--r--  2.0 unx       17 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
--rw-r--r--  2.0 unx       32 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
--rw-r--r--  2.0 unx      655 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
--rw-r--r--  2.0 unx      605 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
--rw-r--r--  2.0 unx     1369 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/unet_arch_params.yaml
--rw-r--r--  2.0 unx     3031 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
--rw-r--r--  2.0 unx       63 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
--rw-r--r--  2.0 unx     2393 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolo_arch_params.yaml
--rw-r--r--  2.0 unx     2337 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml
--rw-r--r--  2.0 unx     2346 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml
--rw-r--r--  2.0 unx     2341 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml
--rw-r--r--  2.0 unx      235 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
--rw-r--r--  2.0 unx      237 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
--rw-r--r--  2.0 unx      229 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
--rw-r--r--  2.0 unx      228 b- defN 23-May-02 15:39 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
--rw-r--r--  2.0 unx      611 b- defN 23-May-02 15:39 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
--rw-r--r--  2.0 unx       72 b- defN 23-May-02 15:39 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/recipes/conversion_params/__init__.py
--rw-r--r--  2.0 unx     1807 b- defN 23-May-02 15:39 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
--rw-r--r--  2.0 unx     2040 b- defN 23-May-02 15:39 super_gradients/recipes/conversion_params/default_conversion_params.yaml
--rw-r--r--  2.0 unx      869 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
--rw-r--r--  2.0 unx     1530 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
--rw-r--r--  2.0 unx     1056 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
--rw-r--r--  2.0 unx      615 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
--rw-r--r--  2.0 unx      525 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
--rw-r--r--  2.0 unx      706 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx      644 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
--rw-r--r--  2.0 unx      721 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
--rw-r--r--  2.0 unx      709 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
--rw-r--r--  2.0 unx      708 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
--rw-r--r--  2.0 unx     3946 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     4202 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
--rw-r--r--  2.0 unx     3590 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
--rw-r--r--  2.0 unx     5568 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml
--rw-r--r--  2.0 unx     3646 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml
--rw-r--r--  2.0 unx     2461 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
--rw-r--r--  2.0 unx      405 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
--rw-r--r--  2.0 unx     1466 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx      931 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx      732 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
--rw-r--r--  2.0 unx      142 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
--rw-r--r--  2.0 unx      734 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
--rw-r--r--  2.0 unx     1059 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
--rw-r--r--  2.0 unx     1093 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
--rw-r--r--  2.0 unx      845 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
--rw-r--r--  2.0 unx     1762 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
--rw-r--r--  2.0 unx      149 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     1571 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
--rw-r--r--  2.0 unx     1414 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
--rw-r--r--  2.0 unx     4112 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
--rw-r--r--  2.0 unx      961 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
--rw-r--r--  2.0 unx      559 b- defN 23-May-02 15:39 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
--rw-r--r--  2.0 unx     1155 b- defN 23-May-02 15:39 super_gradients/recipes/quantization_params/default_quantization_params.yaml
--rw-r--r--  2.0 unx      591 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
--rw-r--r--  2.0 unx      700 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
--rw-r--r--  2.0 unx      877 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
--rw-r--r--  2.0 unx     1302 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
--rw-r--r--  2.0 unx      723 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
--rw-r--r--  2.0 unx     1121 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
--rw-r--r--  2.0 unx      956 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
--rw-r--r--  2.0 unx      461 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
--rw-r--r--  2.0 unx     5459 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/default_train_params.yaml
--rw-r--r--  2.0 unx      794 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
--rw-r--r--  2.0 unx      742 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
--rw-r--r--  2.0 unx      549 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
--rw-r--r--  2.0 unx      795 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
--rw-r--r--  2.0 unx      476 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
--rw-r--r--  2.0 unx      484 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
--rw-r--r--  2.0 unx      522 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
--rw-r--r--  2.0 unx      602 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
--rw-r--r--  2.0 unx      519 b- defN 23-May-02 15:39 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
--rw-r--r--  2.0 unx      107 b- defN 23-May-02 15:39 super_gradients/sanity_check/__init__.py
--rw-r--r--  2.0 unx     5262 b- defN 23-May-02 15:39 super_gradients/sanity_check/env_sanity_check.py
--rw-r--r--  2.0 unx      666 b- defN 23-May-02 15:39 super_gradients/training/__init__.py
--rw-r--r--  2.0 unx     4155 b- defN 23-May-02 15:39 super_gradients/training/params.py
--rw-r--r--  2.0 unx     4301 b- defN 23-May-02 15:39 super_gradients/training/pretrained_models.py
--rw-r--r--  2.0 unx     3224 b- defN 23-May-02 15:39 super_gradients/training/dataloaders/__init__.py
--rw-r--r--  2.0 unx    32361 b- defN 23-May-02 15:39 super_gradients/training/dataloaders/dataloaders.py
--rw-r--r--  2.0 unx     1811 b- defN 23-May-02 15:39 super_gradients/training/datasets/__init__.py
--rw-r--r--  2.0 unx    14162 b- defN 23-May-02 15:39 super_gradients/training/datasets/auto_augment.py
--rw-r--r--  2.0 unx     3705 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_augmentation.py
--rw-r--r--  2.0 unx     3484 b- defN 23-May-02 15:39 super_gradients/training/datasets/datasets_conf.py
--rw-r--r--  2.0 unx    30279 b- defN 23-May-02 15:39 super_gradients/training/datasets/datasets_utils.py
--rw-r--r--  2.0 unx    14663 b- defN 23-May-02 15:39 super_gradients/training/datasets/mixup.py
--rw-r--r--  2.0 unx    11746 b- defN 23-May-02 15:39 super_gradients/training/datasets/sg_dataset.py
--rw-r--r--  2.0 unx      252 b- defN 23-May-02 15:39 super_gradients/training/datasets/classification_datasets/__init__.py
--rw-r--r--  2.0 unx     3096 b- defN 23-May-02 15:39 super_gradients/training/datasets/classification_datasets/cifar.py
--rw-r--r--  2.0 unx     1706 b- defN 23-May-02 15:39 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
--rw-r--r--  2.0 unx      862 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/__init__.py
--rw-r--r--  2.0 unx     3927 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/default_formats.py
--rw-r--r--  2.0 unx     3071 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/format_converter.py
--rw-r--r--  2.0 unx     7928 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/formats.py
--rw-r--r--  2.0 unx     1044 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
--rw-r--r--  2.0 unx     2674 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
--rw-r--r--  2.0 unx     5094 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
--rw-r--r--  2.0 unx     2089 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
--rw-r--r--  2.0 unx     2043 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
--rw-r--r--  2.0 unx     5043 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
--rw-r--r--  2.0 unx     2948 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
--rw-r--r--  2.0 unx      575 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
--rw-r--r--  2.0 unx     1792 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
--rw-r--r--  2.0 unx     8373 b- defN 23-May-02 15:39 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
--rw-r--r--  2.0 unx      683 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/__init__.py
--rw-r--r--  2.0 unx     2505 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/coco_detection.py
--rw-r--r--  2.0 unx     9258 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
--rw-r--r--  2.0 unx    26159 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/detection_dataset.py
--rw-r--r--  2.0 unx    11353 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
--rw-r--r--  2.0 unx    11120 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
--rw-r--r--  2.0 unx      328 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
--rw-r--r--  2.0 unx    18882 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
--rw-r--r--  2.0 unx     3504 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
--rw-r--r--  2.0 unx     1997 b- defN 23-May-02 15:39 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
--rw-r--r--  2.0 unx      502 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
--rw-r--r--  2.0 unx     4910 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
--rw-r--r--  2.0 unx     9066 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
--rw-r--r--  2.0 unx     5929 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
--rw-r--r--  2.0 unx    10167 b- defN 23-May-02 15:39 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
--rw-r--r--  2.0 unx      385 b- defN 23-May-02 15:39 super_gradients/training/datasets/samplers/__init__.py
--rw-r--r--  2.0 unx     2516 b- defN 23-May-02 15:39 super_gradients/training/datasets/samplers/infinite_sampler.py
--rw-r--r--  2.0 unx     4809 b- defN 23-May-02 15:39 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
--rw-r--r--  2.0 unx     1037 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/__init__.py
--rw-r--r--  2.0 unx     6714 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
--rw-r--r--  2.0 unx     7717 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
--rw-r--r--  2.0 unx     5518 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
--rw-r--r--  2.0 unx    11146 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
--rw-r--r--  2.0 unx     8470 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
--rw-r--r--  2.0 unx     3062 b- defN 23-May-02 15:39 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/exceptions/__init__.py
--rw-r--r--  2.0 unx     1761 b- defN 23-May-02 15:39 super_gradients/training/exceptions/dataset_exceptions.py
--rw-r--r--  2.0 unx     2826 b- defN 23-May-02 15:39 super_gradients/training/exceptions/kd_trainer_exceptions.py
--rw-r--r--  2.0 unx      946 b- defN 23-May-02 15:39 super_gradients/training/exceptions/loss_exceptions.py
--rw-r--r--  2.0 unx     1268 b- defN 23-May-02 15:39 super_gradients/training/exceptions/sg_trainer_exceptions.py
--rw-r--r--  2.0 unx      132 b- defN 23-May-02 15:39 super_gradients/training/kd_trainer/__init__.py
--rw-r--r--  2.0 unx    16582 b- defN 23-May-02 15:39 super_gradients/training/kd_trainer/kd_trainer.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/legacy/__init__.py
--rw-r--r--  2.0 unx     4198 b- defN 23-May-02 15:39 super_gradients/training/legacy/utils.py
--rw-r--r--  2.0 unx     1476 b- defN 23-May-02 15:39 super_gradients/training/losses/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/losses/all_losses.py
--rw-r--r--  2.0 unx     1219 b- defN 23-May-02 15:39 super_gradients/training/losses/bce_dice_loss.py
--rw-r--r--  2.0 unx      419 b- defN 23-May-02 15:39 super_gradients/training/losses/bce_loss.py
--rw-r--r--  2.0 unx     2374 b- defN 23-May-02 15:39 super_gradients/training/losses/cwd_loss.py
--rw-r--r--  2.0 unx     2525 b- defN 23-May-02 15:39 super_gradients/training/losses/ddrnet_loss.py
--rw-r--r--  2.0 unx     3377 b- defN 23-May-02 15:39 super_gradients/training/losses/dekr_loss.py
--rw-r--r--  2.0 unx     5618 b- defN 23-May-02 15:39 super_gradients/training/losses/dice_ce_edge_loss.py
--rw-r--r--  2.0 unx     5208 b- defN 23-May-02 15:39 super_gradients/training/losses/dice_loss.py
--rw-r--r--  2.0 unx     1214 b- defN 23-May-02 15:39 super_gradients/training/losses/focal_loss.py
--rw-r--r--  2.0 unx     5051 b- defN 23-May-02 15:39 super_gradients/training/losses/iou_loss.py
--rw-r--r--  2.0 unx     2176 b- defN 23-May-02 15:39 super_gradients/training/losses/kd_losses.py
--rw-r--r--  2.0 unx     4177 b- defN 23-May-02 15:39 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
--rw-r--r--  2.0 unx      550 b- defN 23-May-02 15:39 super_gradients/training/losses/loss_utils.py
--rw-r--r--  2.0 unx     3854 b- defN 23-May-02 15:39 super_gradients/training/losses/mask_loss.py
--rw-r--r--  2.0 unx     4129 b- defN 23-May-02 15:39 super_gradients/training/losses/ohem_ce_loss.py
--rw-r--r--  2.0 unx    41319 b- defN 23-May-02 15:39 super_gradients/training/losses/ppyolo_loss.py
--rw-r--r--  2.0 unx     1010 b- defN 23-May-02 15:39 super_gradients/training/losses/r_squared_loss.py
--rw-r--r--  2.0 unx     3453 b- defN 23-May-02 15:39 super_gradients/training/losses/seg_kd_loss.py
--rw-r--r--  2.0 unx     1650 b- defN 23-May-02 15:39 super_gradients/training/losses/shelfnet_ohem_loss.py
--rw-r--r--  2.0 unx     1949 b- defN 23-May-02 15:39 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
--rw-r--r--  2.0 unx     8794 b- defN 23-May-02 15:39 super_gradients/training/losses/ssd_loss.py
--rw-r--r--  2.0 unx     9721 b- defN 23-May-02 15:39 super_gradients/training/losses/stdc_loss.py
--rw-r--r--  2.0 unx     5771 b- defN 23-May-02 15:39 super_gradients/training/losses/structure_loss.py
--rw-r--r--  2.0 unx    50149 b- defN 23-May-02 15:39 super_gradients/training/losses/yolox_loss.py
--rw-r--r--  2.0 unx     1052 b- defN 23-May-02 15:39 super_gradients/training/metrics/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/metrics/all_metrics.py
--rw-r--r--  2.0 unx     3262 b- defN 23-May-02 15:39 super_gradients/training/metrics/classification_metrics.py
--rw-r--r--  2.0 unx    10741 b- defN 23-May-02 15:39 super_gradients/training/metrics/detection_metrics.py
--rw-r--r--  2.0 unx     3973 b- defN 23-May-02 15:39 super_gradients/training/metrics/metric_utils.py
--rw-r--r--  2.0 unx    15346 b- defN 23-May-02 15:39 super_gradients/training/metrics/pose_estimation_metrics.py
--rw-r--r--  2.0 unx    11454 b- defN 23-May-02 15:39 super_gradients/training/metrics/pose_estimation_utils.py
--rw-r--r--  2.0 unx    11935 b- defN 23-May-02 15:39 super_gradients/training/metrics/segmentation_metrics.py
--rw-r--r--  2.0 unx     8617 b- defN 23-May-02 15:39 super_gradients/training/models/__init__.py
--rw-r--r--  2.0 unx     1226 b- defN 23-May-02 15:39 super_gradients/training/models/arch_params_factory.py
--rw-r--r--  2.0 unx     7060 b- defN 23-May-02 15:39 super_gradients/training/models/conversion.py
--rw-r--r--  2.0 unx    11875 b- defN 23-May-02 15:39 super_gradients/training/models/model_factory.py
--rw-r--r--  2.0 unx    10986 b- defN 23-May-02 15:39 super_gradients/training/models/prediction_results.py
--rw-r--r--  2.0 unx     2054 b- defN 23-May-02 15:39 super_gradients/training/models/predictions.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/results.py
--rw-r--r--  2.0 unx     2998 b- defN 23-May-02 15:39 super_gradients/training/models/sg_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/__init__.py
--rw-r--r--  2.0 unx    20025 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/beit.py
--rw-r--r--  2.0 unx     7472 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/densenet.py
--rw-r--r--  2.0 unx     3707 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/dpn.py
--rw-r--r--  2.0 unx    36745 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/efficientnet.py
--rw-r--r--  2.0 unx     8862 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/googlenet.py
--rw-r--r--  2.0 unx      798 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/lenet.py
--rw-r--r--  2.0 unx     2407 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/mobilenet.py
--rw-r--r--  2.0 unx     9472 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/mobilenetv2.py
--rw-r--r--  2.0 unx     8696 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/mobilenetv3.py
--rw-r--r--  2.0 unx     4339 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/pnasnet.py
--rw-r--r--  2.0 unx     4209 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/preact_resnet.py
--rw-r--r--  2.0 unx    13599 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/regnet.py
--rw-r--r--  2.0 unx     7924 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/repvgg.py
--rw-r--r--  2.0 unx    15025 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/resnet.py
--rw-r--r--  2.0 unx     6294 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/resnext.py
--rw-r--r--  2.0 unx     4134 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/senet.py
--rw-r--r--  2.0 unx     3660 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/shufflenet.py
--rw-r--r--  2.0 unx     9768 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/shufflenetv2.py
--rw-r--r--  2.0 unx     1538 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/vgg.py
--rw-r--r--  2.0 unx     9210 b- defN 23-May-02 15:39 super_gradients/training/models/classification_models/vit.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/__init__.py
--rw-r--r--  2.0 unx     9130 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/csp_darknet53.py
--rw-r--r--  2.0 unx     9814 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/csp_resnet.py
--rw-r--r--  2.0 unx     9120 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/customizable_detector.py
--rw-r--r--  2.0 unx     4746 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/darknet53.py
--rw-r--r--  2.0 unx     2315 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/ssd.py
--rw-r--r--  2.0 unx    29459 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_base.py
--rw-r--r--  2.0 unx     2459 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolox.py
--rw-r--r--  2.0 unx      251 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
--rw-r--r--  2.0 unx     7000 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
--rw-r--r--  2.0 unx     3487 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
--rw-r--r--  2.0 unx     8243 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
--rw-r--r--  2.0 unx    12397 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
--rw-r--r--  2.0 unx      756 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/__init__.py
--rw-r--r--  2.0 unx    12084 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py
--rw-r--r--  2.0 unx     2646 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/panneck.py
--rw-r--r--  2.0 unx     4124 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py
--rw-r--r--  2.0 unx    13329 b- defN 23-May-02 15:39 super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/kd_modules/__init__.py
--rw-r--r--  2.0 unx     3553 b- defN 23-May-02 15:39 super_gradients/training/models/kd_modules/kd_module.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/pose_estimation_models/__init__.py
--rw-r--r--  2.0 unx    21231 b- defN 23-May-02 15:39 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
--rw-r--r--  2.0 unx     1294 b- defN 23-May-02 15:39 super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py
--rw-r--r--  2.0 unx     1335 b- defN 23-May-02 15:39 super_gradients/training/models/pose_estimation_models/pose_ppyolo.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/__init__.py
--rw-r--r--  2.0 unx      964 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/common.py
--rw-r--r--  2.0 unx     5139 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/context_modules.py
--rw-r--r--  2.0 unx    27896 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/ddrnet.py
--rw-r--r--  2.0 unx     2439 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
--rw-r--r--  2.0 unx    21760 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/laddernet.py
--rw-r--r--  2.0 unx    15648 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/ppliteseg.py
--rw-r--r--  2.0 unx    14424 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/regseg.py
--rw-r--r--  2.0 unx    20334 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/segformer.py
--rw-r--r--  2.0 unx     2256 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/segmentation_module.py
--rw-r--r--  2.0 unx    24833 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/shelfnet.py
--rw-r--r--  2.0 unx    29005 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/stdc.py
--rw-r--r--  2.0 unx      260 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/unet/__init__.py
--rw-r--r--  2.0 unx    12324 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/unet/unet.py
--rw-r--r--  2.0 unx    10718 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
--rw-r--r--  2.0 unx    13292 b- defN 23-May-02 15:39 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
--rw-r--r--  2.0 unx      119 b- defN 23-May-02 15:39 super_gradients/training/models/user_models/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/pipelines/__init__.py
--rw-r--r--  2.0 unx    14562 b- defN 23-May-02 15:39 super_gradients/training/pipelines/pipelines.py
--rw-r--r--  2.0 unx      393 b- defN 23-May-02 15:39 super_gradients/training/pre_launch_callbacks/__init__.py
--rw-r--r--  2.0 unx    13955 b- defN 23-May-02 15:39 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
--rw-r--r--  2.0 unx      517 b- defN 23-May-02 15:39 super_gradients/training/processing/__init__.py
--rw-r--r--  2.0 unx    13177 b- defN 23-May-02 15:39 super_gradients/training/processing/processing.py
--rw-r--r--  2.0 unx       98 b- defN 23-May-02 15:39 super_gradients/training/qat_trainer/__init__.py
--rw-r--r--  2.0 unx     9701 b- defN 23-May-02 15:39 super_gradients/training/qat_trainer/qat_trainer.py
--rw-r--r--  2.0 unx      184 b- defN 23-May-02 15:39 super_gradients/training/sg_trainer/__init__.py
--rw-r--r--  2.0 unx    97356 b- defN 23-May-02 15:39 super_gradients/training/sg_trainer/sg_trainer.py
--rw-r--r--  2.0 unx     1685 b- defN 23-May-02 15:39 super_gradients/training/training_hyperparams/__init__.py
--rw-r--r--  2.0 unx     3774 b- defN 23-May-02 15:39 super_gradients/training/training_hyperparams/training_hyperparams.py
--rw-r--r--  2.0 unx     1024 b- defN 23-May-02 15:39 super_gradients/training/transforms/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/transforms/all_transforms.py
--rw-r--r--  2.0 unx    16193 b- defN 23-May-02 15:39 super_gradients/training/transforms/keypoint_transforms.py
--rw-r--r--  2.0 unx     1134 b- defN 23-May-02 15:39 super_gradients/training/transforms/pipeline_adaptors.py
--rw-r--r--  2.0 unx    55089 b- defN 23-May-02 15:39 super_gradients/training/transforms/transforms.py
--rw-r--r--  2.0 unx     6048 b- defN 23-May-02 15:39 super_gradients/training/transforms/utils.py
--rw-r--r--  2.0 unx     1104 b- defN 23-May-02 15:39 super_gradients/training/utils/__init__.py
--rw-r--r--  2.0 unx     1673 b- defN 23-May-02 15:39 super_gradients/training/utils/activations_utils.py
--rw-r--r--  2.0 unx     1111 b- defN 23-May-02 15:39 super_gradients/training/utils/bbox_utils.py
--rw-r--r--  2.0 unx    15315 b- defN 23-May-02 15:39 super_gradients/training/utils/checkpoint_utils.py
--rw-r--r--  2.0 unx     9794 b- defN 23-May-02 15:39 super_gradients/training/utils/config_utils.py
--rw-r--r--  2.0 unx     1132 b- defN 23-May-02 15:39 super_gradients/training/utils/deprecated_utils.py
--rw-r--r--  2.0 unx    53278 b- defN 23-May-02 15:39 super_gradients/training/utils/detection_utils.py
--rw-r--r--  2.0 unx    16195 b- defN 23-May-02 15:39 super_gradients/training/utils/distributed_training_utils.py
--rw-r--r--  2.0 unx     6352 b- defN 23-May-02 15:39 super_gradients/training/utils/early_stopping.py
--rw-r--r--  2.0 unx     9322 b- defN 23-May-02 15:39 super_gradients/training/utils/ema.py
--rw-r--r--  2.0 unx     2610 b- defN 23-May-02 15:39 super_gradients/training/utils/ema_decay_schedules.py
--rw-r--r--  2.0 unx     1072 b- defN 23-May-02 15:39 super_gradients/training/utils/export_utils.py
--rw-r--r--  2.0 unx     7508 b- defN 23-May-02 15:39 super_gradients/training/utils/get_model_stats.py
--rw-r--r--  2.0 unx      771 b- defN 23-May-02 15:39 super_gradients/training/utils/kd_trainer_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/utils/load_image.py
--rw-r--r--  2.0 unx     5827 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizer_utils.py
--rw-r--r--  2.0 unx      839 b- defN 23-May-02 15:39 super_gradients/training/utils/regularization_utils.py
--rw-r--r--  2.0 unx    10388 b- defN 23-May-02 15:39 super_gradients/training/utils/segmentation_utils.py
--rw-r--r--  2.0 unx    19625 b- defN 23-May-02 15:39 super_gradients/training/utils/sg_trainer_utils.py
--rw-r--r--  2.0 unx     6272 b- defN 23-May-02 15:39 super_gradients/training/utils/ssd_utils.py
--rw-r--r--  2.0 unx    18273 b- defN 23-May-02 15:39 super_gradients/training/utils/utils.py
--rw-r--r--  2.0 unx      303 b- defN 23-May-02 15:39 super_gradients/training/utils/version_utils.py
--rw-r--r--  2.0 unx     6209 b- defN 23-May-02 15:39 super_gradients/training/utils/weight_averaging_utils.py
--rw-r--r--  2.0 unx     2030 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/all_callbacks.py
--rw-r--r--  2.0 unx    20126 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/base_callbacks.py
--rw-r--r--  2.0 unx    32630 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/callbacks.py
--rw-r--r--  2.0 unx     1169 b- defN 23-May-02 15:39 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/utils/media/__init__.py
--rw-r--r--  2.0 unx     5880 b- defN 23-May-02 15:39 super_gradients/training/utils/media/image.py
--rw-r--r--  2.0 unx     4046 b- defN 23-May-02 15:39 super_gradients/training/utils/media/stream.py
--rw-r--r--  2.0 unx     6926 b- defN 23-May-02 15:39 super_gradients/training/utils/media/video.py
--rw-r--r--  2.0 unx      396 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizers/__init__.py
--rw-r--r--  2.0 unx     9760 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizers/lamb.py
--rw-r--r--  2.0 unx     3008 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizers/lion.py
--rw-r--r--  2.0 unx     6834 b- defN 23-May-02 15:39 super_gradients/training/utils/optimizers/rmsprop_tf.py
--rw-r--r--  2.0 unx      213 b- defN 23-May-02 15:39 super_gradients/training/utils/pose_estimation/__init__.py
--rw-r--r--  2.0 unx    11167 b- defN 23-May-02 15:39 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
--rw-r--r--  2.0 unx     7140 b- defN 23-May-02 15:39 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
--rw-r--r--  2.0 unx      387 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/__init__.py
--rw-r--r--  2.0 unx     6271 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/calibrator.py
--rw-r--r--  2.0 unx     8417 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/core.py
--rw-r--r--  2.0 unx     2196 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/export.py
--rw-r--r--  2.0 unx    17062 b- defN 23-May-02 15:39 super_gradients/training/utils/quantization/selective_quantization_utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-02 15:39 super_gradients/training/utils/visualization/__init__.py
--rw-r--r--  2.0 unx     1698 b- defN 23-May-02 15:39 super_gradients/training/utils/visualization/detection.py
--rw-r--r--  2.0 unx     2847 b- defN 23-May-02 15:39 super_gradients/training/utils/visualization/utils.py
--rw-r--r--  2.0 unx     2218 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/LICENSE.YOLONAS.md
--rw-r--r--  2.0 unx    11341 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx    36159 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    64352 b- defN 23-May-02 15:40 super_gradients-3.1.0.dist-info/RECORD
-558 files, 2818306 bytes uncompressed, 857306 bytes compressed:  69.6%
+Zip file size: 964207 bytes, number of entries: 557
+-rw-r--r--  2.0 unx      711 b- defN 23-May-03 19:50 super_gradients/__init__.py
+-rw-r--r--  2.0 unx     1657 b- defN 23-May-03 19:50 super_gradients/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-May-03 19:50 super_gradients/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx      702 b- defN 23-May-03 19:50 super_gradients/qat_from_recipe.py
+-rwxr-xr-x  2.0 unx       44 b- defN 23-May-03 19:50 super_gradients/requirements.pro.txt
+-rwxr-xr-x  2.0 unx      729 b- defN 23-May-03 19:50 super_gradients/requirements.txt
+-rw-r--r--  2.0 unx      537 b- defN 23-May-03 19:50 super_gradients/resume_experiment.py
+-rw-r--r--  2.0 unx      693 b- defN 23-May-03 19:50 super_gradients/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx      650 b- defN 23-May-03 19:50 super_gradients/train_from_recipe.py
+-rw-r--r--  2.0 unx     1098 b- defN 23-May-03 19:50 super_gradients/common/__init__.py
+-rw-r--r--  2.0 unx    15339 b- defN 23-May-03 19:50 super_gradients/common/object_names.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/abstractions/__init__.py
+-rw-r--r--  2.0 unx      879 b- defN 23-May-03 19:50 super_gradients/common/abstractions/abstract_logger.py
+-rw-r--r--  2.0 unx     3129 b- defN 23-May-03 19:50 super_gradients/common/abstractions/mute_processes.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/auto_logging/__init__.py
+-rw-r--r--  2.0 unx     4846 b- defN 23-May-03 19:50 super_gradients/common/auto_logging/auto_logger.py
+-rw-r--r--  2.0 unx     6625 b- defN 23-May-03 19:50 super_gradients/common/auto_logging/console_logging.py
+-rw-r--r--  2.0 unx      142 b- defN 23-May-03 19:50 super_gradients/common/aws_connection/__init__.py
+-rw-r--r--  2.0 unx     4182 b- defN 23-May-03 19:50 super_gradients/common/aws_connection/aws_connector.py
+-rw-r--r--  2.0 unx     7198 b- defN 23-May-03 19:50 super_gradients/common/aws_connection/aws_secrets_manager_connector.py
+-rw-r--r--  2.0 unx      119 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/__init__.py
+-rw-r--r--  2.0 unx      669 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/crash_handler.py
+-rw-r--r--  2.0 unx    11775 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/crash_tips.py
+-rw-r--r--  2.0 unx      886 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/crash_tips_setup.py
+-rw-r--r--  2.0 unx     1740 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/exception.py
+-rw-r--r--  2.0 unx     2357 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/exception_monitoring_setup.py
+-rw-r--r--  2.0 unx      789 b- defN 23-May-03 19:50 super_gradients/common/crash_handler/utils.py
+-rw-r--r--  2.0 unx      140 b- defN 23-May-03 19:50 super_gradients/common/data_connection/__init__.py
+-rw-r--r--  2.0 unx    17959 b- defN 23-May-03 19:50 super_gradients/common/data_connection/s3_connector.py
+-rw-r--r--  2.0 unx      325 b- defN 23-May-03 19:50 super_gradients/common/data_interface/__init__.py
+-rw-r--r--  2.0 unx     9699 b- defN 23-May-03 19:50 super_gradients/common/data_interface/adnn_model_repository_data_interface.py
+-rw-r--r--  2.0 unx     2050 b- defN 23-May-03 19:50 super_gradients/common/data_interface/dataset_data_interface.py
+-rw-r--r--  2.0 unx      220 b- defN 23-May-03 19:50 super_gradients/common/data_types/__init__.py
+-rw-r--r--  2.0 unx      597 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/__init__.py
+-rw-r--r--  2.0 unx      309 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/deep_learning_task.py
+-rw-r--r--  2.0 unx      108 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/downsample_mode.py
+-rw-r--r--  2.0 unx      317 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/evaluation_type.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/multi_gpu_mode.py
+-rw-r--r--  2.0 unx     1200 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/strict_load.py
+-rw-r--r--  2.0 unx      202 b- defN 23-May-03 19:50 super_gradients/common/data_types/enum/upsample_mode.py
+-rw-r--r--  2.0 unx      257 b- defN 23-May-03 19:50 super_gradients/common/decorators/__init__.py
+-rw-r--r--  2.0 unx     1567 b- defN 23-May-03 19:50 super_gradients/common/decorators/code_save_decorator.py
+-rw-r--r--  2.0 unx     3663 b- defN 23-May-03 19:50 super_gradients/common/decorators/deci_logger.py
+-rw-r--r--  2.0 unx     2921 b- defN 23-May-03 19:50 super_gradients/common/decorators/explicit_params_validator.py
+-rw-r--r--  2.0 unx     1315 b- defN 23-May-03 19:50 super_gradients/common/decorators/factory_decorator.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-May-03 19:50 super_gradients/common/decorators/singleton.py
+-rw-r--r--  2.0 unx      202 b- defN 23-May-03 19:50 super_gradients/common/environment/__init__.py
+-rw-r--r--  2.0 unx      993 b- defN 23-May-03 19:50 super_gradients/common/environment/argparse_utils.py
+-rw-r--r--  2.0 unx     9170 b- defN 23-May-03 19:50 super_gradients/common/environment/cfg_utils.py
+-rw-r--r--  2.0 unx     4218 b- defN 23-May-03 19:50 super_gradients/common/environment/checkpoints_dir_utils.py
+-rw-r--r--  2.0 unx     2682 b- defN 23-May-03 19:50 super_gradients/common/environment/ddp_utils.py
+-rw-r--r--  2.0 unx      752 b- defN 23-May-03 19:50 super_gradients/common/environment/device_utils.py
+-rw-r--r--  2.0 unx     1147 b- defN 23-May-03 19:50 super_gradients/common/environment/env_variables.py
+-rw-r--r--  2.0 unx     4047 b- defN 23-May-03 19:50 super_gradients/common/environment/omegaconf_utils.py
+-rw-r--r--  2.0 unx      459 b- defN 23-May-03 19:50 super_gradients/common/environment/path_utils.py
+-rw-r--r--  2.0 unx      112 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/__init__.py
+-rw-r--r--  2.0 unx      153 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/cpu.py
+-rw-r--r--  2.0 unx     2517 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/data_models.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/disk.py
+-rw-r--r--  2.0 unx     5427 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/monitoring.py
+-rw-r--r--  2.0 unx      948 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/network.py
+-rw-r--r--  2.0 unx      629 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/utils.py
+-rw-r--r--  2.0 unx      145 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/virtual_memory.py
+-rw-r--r--  2.0 unx      681 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/gpu/__init__.py
+-rw-r--r--  2.0 unx     2270 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/gpu/gpu.py
+-rw-r--r--  2.0 unx   121647 b- defN 23-May-03 19:50 super_gradients/common/environment/monitoring/gpu/pynvml.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/exceptions/__init__.py
+-rw-r--r--  2.0 unx      926 b- defN 23-May-03 19:50 super_gradients/common/exceptions/factory_exceptions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/factories/__init__.py
+-rw-r--r--  2.0 unx     1715 b- defN 23-May-03 19:50 super_gradients/common/factories/activations_type_factory.py
+-rw-r--r--  2.0 unx     2881 b- defN 23-May-03 19:50 super_gradients/common/factories/base_factory.py
+-rw-r--r--  2.0 unx      258 b- defN 23-May-03 19:50 super_gradients/common/factories/bbox_format_factory.py
+-rw-r--r--  2.0 unx      232 b- defN 23-May-03 19:50 super_gradients/common/factories/callbacks_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-May-03 19:50 super_gradients/common/factories/collate_functions_factory.py
+-rw-r--r--  2.0 unx      292 b- defN 23-May-03 19:50 super_gradients/common/factories/context_modules_factory.py
+-rw-r--r--  2.0 unx      321 b- defN 23-May-03 19:50 super_gradients/common/factories/data_formats_factory.py
+-rw-r--r--  2.0 unx      237 b- defN 23-May-03 19:50 super_gradients/common/factories/datasets_factory.py
+-rw-r--r--  2.0 unx     1014 b- defN 23-May-03 19:50 super_gradients/common/factories/detection_modules_factory.py
+-rw-r--r--  2.0 unx      572 b- defN 23-May-03 19:50 super_gradients/common/factories/list_factory.py
+-rw-r--r--  2.0 unx      223 b- defN 23-May-03 19:50 super_gradients/common/factories/losses_factory.py
+-rw-r--r--  2.0 unx      226 b- defN 23-May-03 19:50 super_gradients/common/factories/metrics_factory.py
+-rw-r--r--  2.0 unx      467 b- defN 23-May-03 19:50 super_gradients/common/factories/optimizers_type_factory.py
+-rw-r--r--  2.0 unx      271 b- defN 23-May-03 19:50 super_gradients/common/factories/pre_launch_callbacks_factory.py
+-rw-r--r--  2.0 unx      623 b- defN 23-May-03 19:50 super_gradients/common/factories/processing_factory.py
+-rw-r--r--  2.0 unx      229 b- defN 23-May-03 19:50 super_gradients/common/factories/samplers_factory.py
+-rw-r--r--  2.0 unx      263 b- defN 23-May-03 19:50 super_gradients/common/factories/target_generator_factory.py
+-rw-r--r--  2.0 unx     1873 b- defN 23-May-03 19:50 super_gradients/common/factories/transforms_factory.py
+-rw-r--r--  2.0 unx     2377 b- defN 23-May-03 19:50 super_gradients/common/factories/type_factory.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/plugins/__init__.py
+-rw-r--r--  2.0 unx    10974 b- defN 23-May-03 19:50 super_gradients/common/plugins/deci_client.py
+-rw-r--r--  2.0 unx      271 b- defN 23-May-03 19:50 super_gradients/common/registry/__init__.py
+-rw-r--r--  2.0 unx     1231 b- defN 23-May-03 19:50 super_gradients/common/registry/albumentation.py
+-rw-r--r--  2.0 unx     6006 b- defN 23-May-03 19:50 super_gradients/common/registry/registry.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/common/registry/registry_utils.py
+-rw-r--r--  2.0 unx      508 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/__init__.py
+-rw-r--r--  2.0 unx     7355 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/abstract_sg_logger.py
+-rw-r--r--  2.0 unx    14980 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/base_sg_logger.py
+-rw-r--r--  2.0 unx    10055 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/clearml_sg_logger.py
+-rw-r--r--  2.0 unx    10103 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/dagshub_sg_logger.py
+-rw-r--r--  2.0 unx     6618 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/deci_platform_sg_logger.py
+-rw-r--r--  2.0 unx    13073 b- defN 23-May-03 19:50 super_gradients/common/sg_loggers/wandb_sg_logger.py
+-rw-r--r--  2.0 unx    85509 b- defN 23-May-03 19:50 super_gradients/examples/SG_Walkthrough.ipynb
+-rw-r--r--  2.0 unx    69618 b- defN 23-May-03 19:50 super_gradients/examples/SG_quickstart_classification.ipynb
+-rw-r--r--  2.0 unx    54966 b- defN 23-May-03 19:50 super_gradients/examples/SG_quickstart_model_upload_deci_lab.ipynb
+-rw-r--r--  2.0 unx    65090 b- defN 23-May-03 19:50 super_gradients/examples/SG_quickstart_tensorboard_logger.ipynb
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/cifar10_training_torch_objects/__init__.py
+-rw-r--r--  2.0 unx     2526 b- defN 23-May-03 19:50 super_gradients/examples/cifar10_training_torch_objects/cifar10_training_torch_objects_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/convert_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      870 b- defN 23-May-03 19:50 super_gradients/examples/convert_recipe_example/convert_recipe_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/ddrnet_imagenet/__init__.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-May-03 19:50 super_gradients/examples/ddrnet_imagenet/ddrnet_classification_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/deci_lab_export_example/__init__.py
+-rw-r--r--  2.0 unx     3562 b- defN 23-May-03 19:50 super_gradients/examples/deci_lab_export_example/deci_lab_export_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/early_stop/__init__.py
+-rw-r--r--  2.0 unx     1596 b- defN 23-May-03 19:50 super_gradients/examples/early_stop/early_stop_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/evaluate_checkpoint_example/__init__.py
+-rw-r--r--  2.0 unx      289 b- defN 23-May-03 19:50 super_gradients/examples/evaluate_checkpoint_example/evaluate_checkpoint.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/evaluate_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-May-03 19:50 super_gradients/examples/evaluate_from_recipe_example/evaluate_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/loggers_examples/__init__.py
+-rw-r--r--  2.0 unx     1206 b- defN 23-May-03 19:50 super_gradients/examples/loggers_examples/clearml_logger_example.py
+-rw-r--r--  2.0 unx     1088 b- defN 23-May-03 19:50 super_gradients/examples/loggers_examples/deci_platform_logger_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/qat_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      277 b- defN 23-May-03 19:50 super_gradients/examples/qat_from_recipe_example/qat_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/quantization/__init__.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-May-03 19:50 super_gradients/examples/quantization/non_default_calibrators_example.py
+-rw-r--r--  2.0 unx     2310 b- defN 23-May-03 19:50 super_gradients/examples/quantization/ptq_e2e_example.py
+-rw-r--r--  2.0 unx     1850 b- defN 23-May-03 19:50 super_gradients/examples/quantization/register_quantization_mapping_with_decorator_example.py
+-rw-r--r--  2.0 unx     4732 b- defN 23-May-03 19:50 super_gradients/examples/quantization/resnet_qat_example.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-May-03 19:50 super_gradients/examples/quantization/skipping_quantization_example.py
+-rw-r--r--  2.0 unx      832 b- defN 23-May-03 19:50 super_gradients/examples/quantization/vanilla_quantize_all_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/regseg_transfer_learning_example/__init__.py
+-rw-r--r--  2.0 unx     2379 b- defN 23-May-03 19:50 super_gradients/examples/regseg_transfer_learning_example/regseg_transfer_learning_example.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/resume_experiment_example/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-May-03 19:50 super_gradients/examples/resume_experiment_example/resume_experiment.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/train_from_kd_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      292 b- defN 23-May-03 19:50 super_gradients/examples/train_from_kd_recipe_example/train_from_kd_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_example/__init__.py
+-rw-r--r--  2.0 unx      283 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_example/train_from_recipe.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_dataset_registry/__init__.py
+-rw-r--r--  2.0 unx     1334 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_dataset_registry/train.py
+-rw-r--r--  2.0 unx     1643 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_dataset_registry/user_dataset.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_user_objects/__init__.py
+-rw-r--r--  2.0 unx     1326 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_user_objects/train.py
+-rw-r--r--  2.0 unx     2548 b- defN 23-May-03 19:50 super_gradients/examples/train_from_recipe_with_user_objects/user_dataset.py
+-rw-r--r--  2.0 unx      174 b- defN 23-May-03 19:50 super_gradients/module_interfaces/__init__.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-May-03 19:50 super_gradients/module_interfaces/module_interfaces.py
+-rw-r--r--  2.0 unx     3366 b- defN 23-May-03 19:50 super_gradients/modules/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/modules/all_detection_modules.py
+-rw-r--r--  2.0 unx      617 b- defN 23-May-03 19:50 super_gradients/modules/anti_alias.py
+-rw-r--r--  2.0 unx      776 b- defN 23-May-03 19:50 super_gradients/modules/base_modules.py
+-rw-r--r--  2.0 unx     3054 b- defN 23-May-03 19:50 super_gradients/modules/conv_bn_act_block.py
+-rw-r--r--  2.0 unx     1976 b- defN 23-May-03 19:50 super_gradients/modules/conv_bn_relu_block.py
+-rw-r--r--  2.0 unx    14805 b- defN 23-May-03 19:50 super_gradients/modules/detection_modules.py
+-rw-r--r--  2.0 unx     2143 b- defN 23-May-03 19:50 super_gradients/modules/head_replacement_utils.py
+-rw-r--r--  2.0 unx     4362 b- defN 23-May-03 19:50 super_gradients/modules/multi_output_modules.py
+-rw-r--r--  2.0 unx      860 b- defN 23-May-03 19:50 super_gradients/modules/pixel_shuffle.py
+-rw-r--r--  2.0 unx     3953 b- defN 23-May-03 19:50 super_gradients/modules/pose_estimation_modules.py
+-rw-r--r--  2.0 unx    11773 b- defN 23-May-03 19:50 super_gradients/modules/qarepvgg_block.py
+-rw-r--r--  2.0 unx     8699 b- defN 23-May-03 19:50 super_gradients/modules/repvgg_block.py
+-rw-r--r--  2.0 unx     2138 b- defN 23-May-03 19:50 super_gradients/modules/sampling.py
+-rw-r--r--  2.0 unx     1459 b- defN 23-May-03 19:50 super_gradients/modules/se_blocks.py
+-rw-r--r--  2.0 unx     1403 b- defN 23-May-03 19:50 super_gradients/modules/skip_connections.py
+-rw-r--r--  2.0 unx     2968 b- defN 23-May-03 19:50 super_gradients/modules/utils.py
+-rw-r--r--  2.0 unx      716 b- defN 23-May-03 19:50 super_gradients/modules/quantization/__init__.py
+-rw-r--r--  2.0 unx     2649 b- defN 23-May-03 19:50 super_gradients/modules/quantization/quantized_skip_connections.py
+-rw-r--r--  2.0 unx     4604 b- defN 23-May-03 19:50 super_gradients/modules/quantization/quantized_stdc_blocks.py
+-rw-r--r--  2.0 unx     1281 b- defN 23-May-03 19:50 super_gradients/modules/quantization/resnet_bottleneck.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/recipes/__init__.py
+-rw-r--r--  2.0 unx     1136 b- defN 23-May-03 19:50 super_gradients/recipes/cifar10_resnet.yaml
+-rw-r--r--  2.0 unx     3502 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_ddrnet.yaml
+-rw-r--r--  2.0 unx     3754 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_kd_base.yaml
+-rw-r--r--  2.0 unx     3354 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_pplite_seg50.yaml
+-rw-r--r--  2.0 unx     3253 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_pplite_seg75.yaml
+-rw-r--r--  2.0 unx     2498 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_regseg48.yaml
+-rw-r--r--  2.0 unx     4020 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_segformer.yaml
+-rw-r--r--  2.0 unx      618 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_stdc_base.yaml
+-rw-r--r--  2.0 unx     2862 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_stdc_seg50.yaml
+-rw-r--r--  2.0 unx     3055 b- defN 23-May-03 19:50 super_gradients/recipes/cityscapes_stdc_seg75.yaml
+-rw-r--r--  2.0 unx     1830 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_pose_ddrnet39.yaml
+-rw-r--r--  2.0 unx     3549 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_pose_dekr_w32_no_dc.yaml
+-rw-r--r--  2.0 unx     1998 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_pose_pppose_l.yaml
+-rw-r--r--  2.0 unx     1996 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ppyoloe_l.yaml
+-rw-r--r--  2.0 unx     1996 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ppyoloe_m.yaml
+-rw-r--r--  2.0 unx     1882 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ppyoloe_s.yaml
+-rw-r--r--  2.0 unx     1975 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ppyoloe_x.yaml
+-rw-r--r--  2.0 unx     1889 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_ssd_lite_mobilenet_v2.yaml
+-rw-r--r--  2.0 unx     1385 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_yolo_nas_s.yaml
+-rw-r--r--  2.0 unx     2583 b- defN 23-May-03 19:50 super_gradients/recipes/coco2017_yolox.yaml
+-rw-r--r--  2.0 unx     1376 b- defN 23-May-03 19:50 super_gradients/recipes/coco_segmentation_shelfnet_lw.yaml
+-rw-r--r--  2.0 unx     1145 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_efficientnet.yaml
+-rw-r--r--  2.0 unx     1129 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_mobilenetv2.yaml
+-rw-r--r--  2.0 unx      507 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_mobilenetv3_base.yaml
+-rw-r--r--  2.0 unx      719 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_mobilenetv3_large.yaml
+-rw-r--r--  2.0 unx      719 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_mobilenetv3_small.yaml
+-rw-r--r--  2.0 unx     1997 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_regnetY.yaml
+-rw-r--r--  2.0 unx     1246 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_repvgg.yaml
+-rw-r--r--  2.0 unx     1169 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_resnet50.yaml
+-rw-r--r--  2.0 unx     2722 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_resnet50_kd.yaml
+-rw-r--r--  2.0 unx     1136 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_vit_base.yaml
+-rw-r--r--  2.0 unx     1010 b- defN 23-May-03 19:50 super_gradients/recipes/imagenet_vit_large.yaml
+-rw-r--r--  2.0 unx     2007 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_ppyoloe.yaml
+-rw-r--r--  2.0 unx     2347 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_yolo_nas_m.yaml
+-rw-r--r--  2.0 unx     2347 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_yolo_nas_s.yaml
+-rw-r--r--  2.0 unx      473 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_yolo_nas_s_qat.yaml
+-rw-r--r--  2.0 unx     1915 b- defN 23-May-03 19:50 super_gradients/recipes/roboflow_yolox.yaml
+-rw-r--r--  2.0 unx     1246 b- defN 23-May-03 19:50 super_gradients/recipes/supervisely_unet.yaml
+-rw-r--r--  2.0 unx     1672 b- defN 23-May-03 19:50 super_gradients/recipes/user_recipe_mnist_as_external_dataset_example.yaml
+-rw-r--r--  2.0 unx     2133 b- defN 23-May-03 19:50 super_gradients/recipes/user_recipe_mnist_example.yaml
+-rw-r--r--  2.0 unx     2000 b- defN 23-May-03 19:50 super_gradients/recipes/variable_setup.yaml
+-rw-r--r--  2.0 unx     2222 b- defN 23-May-03 19:50 super_gradients/recipes/anchors/ssd_anchors.yaml
+-rw-r--r--  2.0 unx      563 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_arch_params.yaml
+-rw-r--r--  2.0 unx      104 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b0_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b1_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b2_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b3_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b4_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b5_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b6_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b7_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_b8_arch_params.yaml
+-rw-r--r--  2.0 unx      103 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/efficientnet_l2_arch_params.yaml
+-rw-r--r--  2.0 unx      194 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/mobilenet_v2_arch_params.yaml
+-rw-r--r--  2.0 unx      156 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/mobilenet_v3_arch_params.yaml
+-rw-r--r--  2.0 unx      409 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/mobilenet_v3_large_arch_params.yaml
+-rw-r--r--  2.0 unx      356 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/mobilenet_v3_small_arch_params.yaml
+-rw-r--r--  2.0 unx      281 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/pose_ddrnet39_arch_params.yaml
+-rw-r--r--  2.0 unx     1245 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/pose_dekr_w32_no_dc_arch_params.yaml
+-rw-r--r--  2.0 unx      985 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/pose_pppose_l_arch_params.yaml
+-rw-r--r--  2.0 unx     1112 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_arch_params.yaml
+-rw-r--r--  2.0 unx      196 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_l_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_m_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_s_arch_params.yaml
+-rw-r--r--  2.0 unx      198 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ppyoloe_x_arch_params.yaml
+-rw-r--r--  2.0 unx      204 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/regnetY_arch_params.yaml
+-rw-r--r--  2.0 unx      352 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvgg_arch_params.yaml
+-rw-r--r--  2.0 unx       98 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvgga0_arch_params.yaml
+-rw-r--r--  2.0 unx       89 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvgga1_arch_params.yaml
+-rw-r--r--  2.0 unx       95 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvgga2_arch_params.yaml
+-rw-r--r--  2.0 unx       88 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvggb0_arch_params.yaml
+-rw-r--r--  2.0 unx       86 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvggb1_arch_params.yaml
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/repvggb2_arch_params.yaml
+-rw-r--r--  2.0 unx       15 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/resnet18_cifar_arch_params.yaml
+-rw-r--r--  2.0 unx       17 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/resnet50_arch_params.yaml
+-rw-r--r--  2.0 unx       32 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/shelfnet34_lw_arch_params.yaml
+-rw-r--r--  2.0 unx      655 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ssd_lite_mobilenetv2_arch_params.yaml
+-rw-r--r--  2.0 unx      605 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/ssd_mobilenetv1_arch_params.yaml
+-rw-r--r--  2.0 unx     1369 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/unet_arch_params.yaml
+-rw-r--r--  2.0 unx     3031 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/unet_default_arch_params.yaml
+-rw-r--r--  2.0 unx       63 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/vit_base_arch_params.yaml
+-rw-r--r--  2.0 unx     2393 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolo_arch_params.yaml
+-rw-r--r--  2.0 unx     2337 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolo_nas_l_arch_params.yaml
+-rw-r--r--  2.0 unx     2346 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolo_nas_m_arch_params.yaml
+-rw-r--r--  2.0 unx     2341 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolo_nas_s_arch_params.yaml
+-rw-r--r--  2.0 unx      235 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_l_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_m_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_nano_arch_params.yaml
+-rw-r--r--  2.0 unx      237 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_s_arch_params.yaml
+-rw-r--r--  2.0 unx      229 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_tiny_arch_params.yaml
+-rw-r--r--  2.0 unx      228 b- defN 23-May-03 19:50 super_gradients/recipes/arch_params/yolox_x_arch_params.yaml
+-rw-r--r--  2.0 unx      611 b- defN 23-May-03 19:50 super_gradients/recipes/checkpoint_params/default_checkpoint_params.yaml
+-rw-r--r--  2.0 unx       72 b- defN 23-May-03 19:50 super_gradients/recipes/checkpoint_params/vit_base_imagenet_checkpoint_params.yaml
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/recipes/conversion_params/__init__.py
+-rw-r--r--  2.0 unx     1807 b- defN 23-May-03 19:50 super_gradients/recipes/conversion_params/cifar10_conversion_params.yaml
+-rw-r--r--  2.0 unx     2040 b- defN 23-May-03 19:50 super_gradients/recipes/conversion_params/default_conversion_params.yaml
+-rw-r--r--  2.0 unx      869 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cifar100_dataset_params.yaml
+-rw-r--r--  2.0 unx     1530 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cifar10_albumentations_dataset_params.yaml
+-rw-r--r--  2.0 unx     1056 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cifar10_dataset_params.yaml
+-rw-r--r--  2.0 unx      615 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_dataset_params.yaml
+-rw-r--r--  2.0 unx      525 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_ddrnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      706 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_ppliteseg_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx      644 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_regseg48_dataset_params.yaml
+-rw-r--r--  2.0 unx      721 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_segformer_dataset_params.yaml
+-rw-r--r--  2.0 unx      709 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_stdc_seg50_dataset_params.yaml
+-rw-r--r--  2.0 unx      708 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/cityscapes_stdc_seg75_dataset_params.yaml
+-rw-r--r--  2.0 unx     3946 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     4202 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_ppyoloe_dataset_params.yaml
+-rw-r--r--  2.0 unx     3590 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_ssd_lite_mobilenet_v2_dataset_params.yaml
+-rw-r--r--  2.0 unx     5568 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_yolo_format_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     3646 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_detection_yolo_nas_dataset_params.yaml
+-rw-r--r--  2.0 unx     2461 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_pose_estimation_dataset_params.yaml
+-rw-r--r--  2.0 unx      405 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_pose_estimation_dekr_dataset_params.yaml
+-rw-r--r--  2.0 unx     1466 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/coco_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx      931 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx      732 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_efficientnet_dataset_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_mobilenetv2_dataset_params.yaml
+-rw-r--r--  2.0 unx      142 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_mobilenetv3_dataset_params.yaml
+-rw-r--r--  2.0 unx      734 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_regnetY_dataset_params.yaml
+-rw-r--r--  2.0 unx     1059 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_resnet50_dataset_params.yaml
+-rw-r--r--  2.0 unx     1093 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_resnet50_kd_dataset_params.yaml
+-rw-r--r--  2.0 unx      845 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/imagenet_vit_base_dataset_params.yaml
+-rw-r--r--  2.0 unx     1762 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/mapillary_dataset_params.yaml
+-rw-r--r--  2.0 unx      149 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/pascal_aug_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     1571 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/pascal_voc_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx     1414 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/pascal_voc_segmentation_dataset_params.yaml
+-rw-r--r--  2.0 unx     4112 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/roboflow_detection_dataset_params.yaml
+-rw-r--r--  2.0 unx      961 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/supervisely_persons_dataset_params.yaml
+-rw-r--r--  2.0 unx      559 b- defN 23-May-03 19:50 super_gradients/recipes/dataset_params/tiny_imagenet_dataset_params.yaml
+-rw-r--r--  2.0 unx     1155 b- defN 23-May-03 19:50 super_gradients/recipes/quantization_params/default_quantization_params.yaml
+-rw-r--r--  2.0 unx      591 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/cifar10_resnet_train_params.yaml
+-rw-r--r--  2.0 unx      700 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/cityscapes_default_train_params.yaml
+-rw-r--r--  2.0 unx      877 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_dekr_pose_train_params.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_ppyoloe_train_params.yaml
+-rw-r--r--  2.0 unx      723 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_ssd_lite_mobilenet_v2_train_params.yaml
+-rw-r--r--  2.0 unx     1121 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_yolo_nas_train_params.yaml
+-rw-r--r--  2.0 unx      956 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco2017_yolox_train_params.yaml
+-rw-r--r--  2.0 unx      461 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/coco_segmentation_shelfnet_lw_train_params.yaml
+-rw-r--r--  2.0 unx     5459 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/default_train_params.yaml
+-rw-r--r--  2.0 unx      794 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_efficientnet_train_params.yaml
+-rw-r--r--  2.0 unx      742 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv2_train_params.yaml
+-rw-r--r--  2.0 unx      549 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_mobilenetv3_train_params.yaml
+-rw-r--r--  2.0 unx      795 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_regnetY_train_params.yaml
+-rw-r--r--  2.0 unx      476 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_repvgg_train_params.yaml
+-rw-r--r--  2.0 unx      484 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_resnet50_kd_train_params.yaml
+-rw-r--r--  2.0 unx      522 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_resnet50_train_params.yaml
+-rw-r--r--  2.0 unx      602 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/imagenet_vit_train_params.yaml
+-rw-r--r--  2.0 unx      519 b- defN 23-May-03 19:50 super_gradients/recipes/training_hyperparams/supervisely_default_train_params.yaml
+-rw-r--r--  2.0 unx      107 b- defN 23-May-03 19:50 super_gradients/sanity_check/__init__.py
+-rw-r--r--  2.0 unx     5262 b- defN 23-May-03 19:50 super_gradients/sanity_check/env_sanity_check.py
+-rw-r--r--  2.0 unx      666 b- defN 23-May-03 19:50 super_gradients/training/__init__.py
+-rw-r--r--  2.0 unx     4155 b- defN 23-May-03 19:50 super_gradients/training/params.py
+-rw-r--r--  2.0 unx     4301 b- defN 23-May-03 19:50 super_gradients/training/pretrained_models.py
+-rw-r--r--  2.0 unx     3224 b- defN 23-May-03 19:50 super_gradients/training/dataloaders/__init__.py
+-rw-r--r--  2.0 unx    32361 b- defN 23-May-03 19:50 super_gradients/training/dataloaders/dataloaders.py
+-rw-r--r--  2.0 unx     1811 b- defN 23-May-03 19:50 super_gradients/training/datasets/__init__.py
+-rw-r--r--  2.0 unx    14162 b- defN 23-May-03 19:50 super_gradients/training/datasets/auto_augment.py
+-rw-r--r--  2.0 unx     3705 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_augmentation.py
+-rw-r--r--  2.0 unx     3484 b- defN 23-May-03 19:50 super_gradients/training/datasets/datasets_conf.py
+-rw-r--r--  2.0 unx    30279 b- defN 23-May-03 19:50 super_gradients/training/datasets/datasets_utils.py
+-rw-r--r--  2.0 unx    14663 b- defN 23-May-03 19:50 super_gradients/training/datasets/mixup.py
+-rw-r--r--  2.0 unx    11746 b- defN 23-May-03 19:50 super_gradients/training/datasets/sg_dataset.py
+-rw-r--r--  2.0 unx      252 b- defN 23-May-03 19:50 super_gradients/training/datasets/classification_datasets/__init__.py
+-rw-r--r--  2.0 unx     3096 b- defN 23-May-03 19:50 super_gradients/training/datasets/classification_datasets/cifar.py
+-rw-r--r--  2.0 unx     1706 b- defN 23-May-03 19:50 super_gradients/training/datasets/classification_datasets/imagenet_dataset.py
+-rw-r--r--  2.0 unx      862 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/__init__.py
+-rw-r--r--  2.0 unx     3927 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/default_formats.py
+-rw-r--r--  2.0 unx     3071 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/format_converter.py
+-rw-r--r--  2.0 unx     7928 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/formats.py
+-rw-r--r--  2.0 unx     1044 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/__init__.py
+-rw-r--r--  2.0 unx     2674 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/bbox_format.py
+-rw-r--r--  2.0 unx     5094 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/cxcywh.py
+-rw-r--r--  2.0 unx     2089 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/normalized_cxcywh.py
+-rw-r--r--  2.0 unx     2043 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xywh.py
+-rw-r--r--  2.0 unx     5043 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/normalized_xyxy.py
+-rw-r--r--  2.0 unx     2948 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/xywh.py
+-rw-r--r--  2.0 unx      575 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/xyxy.py
+-rw-r--r--  2.0 unx     1792 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/bbox_formats/yxyx.py
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/output_adapters/__init__.py
+-rw-r--r--  2.0 unx     8373 b- defN 23-May-03 19:50 super_gradients/training/datasets/data_formats/output_adapters/detection_adapter.py
+-rw-r--r--  2.0 unx      683 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/__init__.py
+-rw-r--r--  2.0 unx     2505 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/coco_detection.py
+-rw-r--r--  2.0 unx     9258 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/coco_format_detection.py
+-rw-r--r--  2.0 unx    26159 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/detection_dataset.py
+-rw-r--r--  2.0 unx    11353 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/pascal_voc_detection.py
+-rw-r--r--  2.0 unx    11120 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/yolo_format_detection.py
+-rw-r--r--  2.0 unx      328 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/roboflow/__init__.py
+-rw-r--r--  2.0 unx    18882 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/roboflow/metadata.py
+-rw-r--r--  2.0 unx     3504 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py
+-rw-r--r--  2.0 unx     1997 b- defN 23-May-03 19:50 super_gradients/training/datasets/detection_datasets/roboflow/utils.py
+-rw-r--r--  2.0 unx      502 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/__init__.py
+-rw-r--r--  2.0 unx     4910 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py
+-rw-r--r--  2.0 unx     9066 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py
+-rw-r--r--  2.0 unx     5929 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py
+-rw-r--r--  2.0 unx    10167 b- defN 23-May-03 19:50 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
+-rw-r--r--  2.0 unx      278 b- defN 23-May-03 19:50 super_gradients/training/datasets/samplers/__init__.py
+-rw-r--r--  2.0 unx     4809 b- defN 23-May-03 19:50 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
+-rw-r--r--  2.0 unx     1037 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/__init__.py
+-rw-r--r--  2.0 unx     6714 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
+-rw-r--r--  2.0 unx     7717 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py
+-rw-r--r--  2.0 unx     5518 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py
+-rw-r--r--  2.0 unx    11146 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py
+-rw-r--r--  2.0 unx     8470 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py
+-rw-r--r--  2.0 unx     3062 b- defN 23-May-03 19:50 super_gradients/training/datasets/segmentation_datasets/supervisely_persons_segmentation.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/exceptions/__init__.py
+-rw-r--r--  2.0 unx     1761 b- defN 23-May-03 19:50 super_gradients/training/exceptions/dataset_exceptions.py
+-rw-r--r--  2.0 unx     2826 b- defN 23-May-03 19:50 super_gradients/training/exceptions/kd_trainer_exceptions.py
+-rw-r--r--  2.0 unx      946 b- defN 23-May-03 19:50 super_gradients/training/exceptions/loss_exceptions.py
+-rw-r--r--  2.0 unx     1268 b- defN 23-May-03 19:50 super_gradients/training/exceptions/sg_trainer_exceptions.py
+-rw-r--r--  2.0 unx      132 b- defN 23-May-03 19:50 super_gradients/training/kd_trainer/__init__.py
+-rw-r--r--  2.0 unx    16582 b- defN 23-May-03 19:50 super_gradients/training/kd_trainer/kd_trainer.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/legacy/__init__.py
+-rw-r--r--  2.0 unx     4198 b- defN 23-May-03 19:50 super_gradients/training/legacy/utils.py
+-rw-r--r--  2.0 unx     1476 b- defN 23-May-03 19:50 super_gradients/training/losses/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/losses/all_losses.py
+-rw-r--r--  2.0 unx     1219 b- defN 23-May-03 19:50 super_gradients/training/losses/bce_dice_loss.py
+-rw-r--r--  2.0 unx      419 b- defN 23-May-03 19:50 super_gradients/training/losses/bce_loss.py
+-rw-r--r--  2.0 unx     2374 b- defN 23-May-03 19:50 super_gradients/training/losses/cwd_loss.py
+-rw-r--r--  2.0 unx     2525 b- defN 23-May-03 19:50 super_gradients/training/losses/ddrnet_loss.py
+-rw-r--r--  2.0 unx     3377 b- defN 23-May-03 19:50 super_gradients/training/losses/dekr_loss.py
+-rw-r--r--  2.0 unx     5618 b- defN 23-May-03 19:50 super_gradients/training/losses/dice_ce_edge_loss.py
+-rw-r--r--  2.0 unx     5208 b- defN 23-May-03 19:50 super_gradients/training/losses/dice_loss.py
+-rw-r--r--  2.0 unx     1214 b- defN 23-May-03 19:50 super_gradients/training/losses/focal_loss.py
+-rw-r--r--  2.0 unx     5051 b- defN 23-May-03 19:50 super_gradients/training/losses/iou_loss.py
+-rw-r--r--  2.0 unx     2176 b- defN 23-May-03 19:50 super_gradients/training/losses/kd_losses.py
+-rw-r--r--  2.0 unx     4177 b- defN 23-May-03 19:50 super_gradients/training/losses/label_smoothing_cross_entropy_loss.py
+-rw-r--r--  2.0 unx      550 b- defN 23-May-03 19:50 super_gradients/training/losses/loss_utils.py
+-rw-r--r--  2.0 unx     3854 b- defN 23-May-03 19:50 super_gradients/training/losses/mask_loss.py
+-rw-r--r--  2.0 unx     4129 b- defN 23-May-03 19:50 super_gradients/training/losses/ohem_ce_loss.py
+-rw-r--r--  2.0 unx    41319 b- defN 23-May-03 19:50 super_gradients/training/losses/ppyolo_loss.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-May-03 19:50 super_gradients/training/losses/r_squared_loss.py
+-rw-r--r--  2.0 unx     3453 b- defN 23-May-03 19:50 super_gradients/training/losses/seg_kd_loss.py
+-rw-r--r--  2.0 unx     1650 b- defN 23-May-03 19:50 super_gradients/training/losses/shelfnet_ohem_loss.py
+-rw-r--r--  2.0 unx     1949 b- defN 23-May-03 19:50 super_gradients/training/losses/shelfnet_semantic_encoding_loss.py
+-rw-r--r--  2.0 unx     8794 b- defN 23-May-03 19:50 super_gradients/training/losses/ssd_loss.py
+-rw-r--r--  2.0 unx     9721 b- defN 23-May-03 19:50 super_gradients/training/losses/stdc_loss.py
+-rw-r--r--  2.0 unx     5771 b- defN 23-May-03 19:50 super_gradients/training/losses/structure_loss.py
+-rw-r--r--  2.0 unx    50149 b- defN 23-May-03 19:50 super_gradients/training/losses/yolox_loss.py
+-rw-r--r--  2.0 unx     1052 b- defN 23-May-03 19:50 super_gradients/training/metrics/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/metrics/all_metrics.py
+-rw-r--r--  2.0 unx     3262 b- defN 23-May-03 19:50 super_gradients/training/metrics/classification_metrics.py
+-rw-r--r--  2.0 unx    10741 b- defN 23-May-03 19:50 super_gradients/training/metrics/detection_metrics.py
+-rw-r--r--  2.0 unx     3973 b- defN 23-May-03 19:50 super_gradients/training/metrics/metric_utils.py
+-rw-r--r--  2.0 unx    15346 b- defN 23-May-03 19:50 super_gradients/training/metrics/pose_estimation_metrics.py
+-rw-r--r--  2.0 unx    11454 b- defN 23-May-03 19:50 super_gradients/training/metrics/pose_estimation_utils.py
+-rw-r--r--  2.0 unx    11935 b- defN 23-May-03 19:50 super_gradients/training/metrics/segmentation_metrics.py
+-rw-r--r--  2.0 unx     8617 b- defN 23-May-03 19:50 super_gradients/training/models/__init__.py
+-rw-r--r--  2.0 unx     1226 b- defN 23-May-03 19:50 super_gradients/training/models/arch_params_factory.py
+-rw-r--r--  2.0 unx     7060 b- defN 23-May-03 19:50 super_gradients/training/models/conversion.py
+-rw-r--r--  2.0 unx    11875 b- defN 23-May-03 19:50 super_gradients/training/models/model_factory.py
+-rw-r--r--  2.0 unx    10986 b- defN 23-May-03 19:50 super_gradients/training/models/prediction_results.py
+-rw-r--r--  2.0 unx     2054 b- defN 23-May-03 19:50 super_gradients/training/models/predictions.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/results.py
+-rw-r--r--  2.0 unx     2998 b- defN 23-May-03 19:50 super_gradients/training/models/sg_module.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/__init__.py
+-rw-r--r--  2.0 unx    20025 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/beit.py
+-rw-r--r--  2.0 unx     7472 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/densenet.py
+-rw-r--r--  2.0 unx     3707 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/dpn.py
+-rw-r--r--  2.0 unx    36745 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/efficientnet.py
+-rw-r--r--  2.0 unx     8862 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/googlenet.py
+-rw-r--r--  2.0 unx      798 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/lenet.py
+-rw-r--r--  2.0 unx     2407 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/mobilenet.py
+-rw-r--r--  2.0 unx     9472 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/mobilenetv2.py
+-rw-r--r--  2.0 unx     8696 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/mobilenetv3.py
+-rw-r--r--  2.0 unx     4339 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/pnasnet.py
+-rw-r--r--  2.0 unx     4209 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/preact_resnet.py
+-rw-r--r--  2.0 unx    13599 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/regnet.py
+-rw-r--r--  2.0 unx     7924 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/repvgg.py
+-rw-r--r--  2.0 unx    15025 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/resnet.py
+-rw-r--r--  2.0 unx     6294 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/resnext.py
+-rw-r--r--  2.0 unx     4134 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/senet.py
+-rw-r--r--  2.0 unx     3660 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/shufflenet.py
+-rw-r--r--  2.0 unx     9768 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/shufflenetv2.py
+-rw-r--r--  2.0 unx     1538 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/vgg.py
+-rw-r--r--  2.0 unx     9210 b- defN 23-May-03 19:50 super_gradients/training/models/classification_models/vit.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/__init__.py
+-rw-r--r--  2.0 unx     9130 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/csp_darknet53.py
+-rw-r--r--  2.0 unx     9814 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/csp_resnet.py
+-rw-r--r--  2.0 unx     9120 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/customizable_detector.py
+-rw-r--r--  2.0 unx     4746 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/darknet53.py
+-rw-r--r--  2.0 unx     2315 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/ssd.py
+-rw-r--r--  2.0 unx    29459 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_base.py
+-rw-r--r--  2.0 unx     2459 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolox.py
+-rw-r--r--  2.0 unx      251 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/__init__.py
+-rw-r--r--  2.0 unx     7000 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/pan.py
+-rw-r--r--  2.0 unx     3487 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/post_prediction_callback.py
+-rw-r--r--  2.0 unx     8243 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_e.py
+-rw-r--r--  2.0 unx    12397 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/pp_yolo_e/pp_yolo_head.py
+-rw-r--r--  2.0 unx      756 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/__init__.py
+-rw-r--r--  2.0 unx    12084 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/dfl_heads.py
+-rw-r--r--  2.0 unx     2646 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/panneck.py
+-rw-r--r--  2.0 unx     4124 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/yolo_nas_variants.py
+-rw-r--r--  2.0 unx    13329 b- defN 23-May-03 19:50 super_gradients/training/models/detection_models/yolo_nas/yolo_stages.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/kd_modules/__init__.py
+-rw-r--r--  2.0 unx     3553 b- defN 23-May-03 19:50 super_gradients/training/models/kd_modules/kd_module.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/pose_estimation_models/__init__.py
+-rw-r--r--  2.0 unx    21231 b- defN 23-May-03 19:50 super_gradients/training/models/pose_estimation_models/dekr_hrnet.py
+-rw-r--r--  2.0 unx     1294 b- defN 23-May-03 19:50 super_gradients/training/models/pose_estimation_models/pose_ddrnet39.py
+-rw-r--r--  2.0 unx     1335 b- defN 23-May-03 19:50 super_gradients/training/models/pose_estimation_models/pose_ppyolo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/__init__.py
+-rw-r--r--  2.0 unx      964 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/common.py
+-rw-r--r--  2.0 unx     5139 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/context_modules.py
+-rw-r--r--  2.0 unx    27896 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/ddrnet.py
+-rw-r--r--  2.0 unx     2439 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/ddrnet_backbones.py
+-rw-r--r--  2.0 unx    21760 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/laddernet.py
+-rw-r--r--  2.0 unx    15648 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/ppliteseg.py
+-rw-r--r--  2.0 unx    14424 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/regseg.py
+-rw-r--r--  2.0 unx    20334 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/segformer.py
+-rw-r--r--  2.0 unx     2256 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/segmentation_module.py
+-rw-r--r--  2.0 unx    24833 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/shelfnet.py
+-rw-r--r--  2.0 unx    29005 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/stdc.py
+-rw-r--r--  2.0 unx      260 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/unet/__init__.py
+-rw-r--r--  2.0 unx    12324 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/unet/unet.py
+-rw-r--r--  2.0 unx    10718 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/unet/unet_decoder.py
+-rw-r--r--  2.0 unx    13292 b- defN 23-May-03 19:50 super_gradients/training/models/segmentation_models/unet/unet_encoder.py
+-rw-r--r--  2.0 unx      119 b- defN 23-May-03 19:50 super_gradients/training/models/user_models/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/pipelines/__init__.py
+-rw-r--r--  2.0 unx    14562 b- defN 23-May-03 19:50 super_gradients/training/pipelines/pipelines.py
+-rw-r--r--  2.0 unx      393 b- defN 23-May-03 19:50 super_gradients/training/pre_launch_callbacks/__init__.py
+-rw-r--r--  2.0 unx    13955 b- defN 23-May-03 19:50 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py
+-rw-r--r--  2.0 unx      517 b- defN 23-May-03 19:50 super_gradients/training/processing/__init__.py
+-rw-r--r--  2.0 unx    13177 b- defN 23-May-03 19:50 super_gradients/training/processing/processing.py
+-rw-r--r--  2.0 unx       98 b- defN 23-May-03 19:50 super_gradients/training/qat_trainer/__init__.py
+-rw-r--r--  2.0 unx     9701 b- defN 23-May-03 19:50 super_gradients/training/qat_trainer/qat_trainer.py
+-rw-r--r--  2.0 unx      184 b- defN 23-May-03 19:50 super_gradients/training/sg_trainer/__init__.py
+-rw-r--r--  2.0 unx    96749 b- defN 23-May-03 19:50 super_gradients/training/sg_trainer/sg_trainer.py
+-rw-r--r--  2.0 unx     1685 b- defN 23-May-03 19:50 super_gradients/training/training_hyperparams/__init__.py
+-rw-r--r--  2.0 unx     3774 b- defN 23-May-03 19:50 super_gradients/training/training_hyperparams/training_hyperparams.py
+-rw-r--r--  2.0 unx     1024 b- defN 23-May-03 19:50 super_gradients/training/transforms/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/transforms/all_transforms.py
+-rw-r--r--  2.0 unx    16193 b- defN 23-May-03 19:50 super_gradients/training/transforms/keypoint_transforms.py
+-rw-r--r--  2.0 unx     1134 b- defN 23-May-03 19:50 super_gradients/training/transforms/pipeline_adaptors.py
+-rw-r--r--  2.0 unx    55089 b- defN 23-May-03 19:50 super_gradients/training/transforms/transforms.py
+-rw-r--r--  2.0 unx     6048 b- defN 23-May-03 19:50 super_gradients/training/transforms/utils.py
+-rw-r--r--  2.0 unx     1104 b- defN 23-May-03 19:50 super_gradients/training/utils/__init__.py
+-rw-r--r--  2.0 unx     1673 b- defN 23-May-03 19:50 super_gradients/training/utils/activations_utils.py
+-rw-r--r--  2.0 unx     1111 b- defN 23-May-03 19:50 super_gradients/training/utils/bbox_utils.py
+-rw-r--r--  2.0 unx    15315 b- defN 23-May-03 19:50 super_gradients/training/utils/checkpoint_utils.py
+-rw-r--r--  2.0 unx     9794 b- defN 23-May-03 19:50 super_gradients/training/utils/config_utils.py
+-rw-r--r--  2.0 unx     1132 b- defN 23-May-03 19:50 super_gradients/training/utils/deprecated_utils.py
+-rw-r--r--  2.0 unx    53278 b- defN 23-May-03 19:50 super_gradients/training/utils/detection_utils.py
+-rw-r--r--  2.0 unx    16195 b- defN 23-May-03 19:50 super_gradients/training/utils/distributed_training_utils.py
+-rw-r--r--  2.0 unx     6352 b- defN 23-May-03 19:50 super_gradients/training/utils/early_stopping.py
+-rw-r--r--  2.0 unx     9322 b- defN 23-May-03 19:50 super_gradients/training/utils/ema.py
+-rw-r--r--  2.0 unx     2610 b- defN 23-May-03 19:50 super_gradients/training/utils/ema_decay_schedules.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-May-03 19:50 super_gradients/training/utils/export_utils.py
+-rw-r--r--  2.0 unx     7508 b- defN 23-May-03 19:50 super_gradients/training/utils/get_model_stats.py
+-rw-r--r--  2.0 unx      771 b- defN 23-May-03 19:50 super_gradients/training/utils/kd_trainer_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/utils/load_image.py
+-rw-r--r--  2.0 unx     5827 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizer_utils.py
+-rw-r--r--  2.0 unx      839 b- defN 23-May-03 19:50 super_gradients/training/utils/regularization_utils.py
+-rw-r--r--  2.0 unx    10388 b- defN 23-May-03 19:50 super_gradients/training/utils/segmentation_utils.py
+-rw-r--r--  2.0 unx    19625 b- defN 23-May-03 19:50 super_gradients/training/utils/sg_trainer_utils.py
+-rw-r--r--  2.0 unx     6272 b- defN 23-May-03 19:50 super_gradients/training/utils/ssd_utils.py
+-rw-r--r--  2.0 unx    18273 b- defN 23-May-03 19:50 super_gradients/training/utils/utils.py
+-rw-r--r--  2.0 unx      303 b- defN 23-May-03 19:50 super_gradients/training/utils/version_utils.py
+-rw-r--r--  2.0 unx     6209 b- defN 23-May-03 19:50 super_gradients/training/utils/weight_averaging_utils.py
+-rw-r--r--  2.0 unx     2030 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/all_callbacks.py
+-rw-r--r--  2.0 unx    20126 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/base_callbacks.py
+-rw-r--r--  2.0 unx    32630 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/callbacks.py
+-rw-r--r--  2.0 unx     1169 b- defN 23-May-03 19:50 super_gradients/training/utils/callbacks/ppyoloe_switch_callback.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/utils/media/__init__.py
+-rw-r--r--  2.0 unx     5880 b- defN 23-May-03 19:50 super_gradients/training/utils/media/image.py
+-rw-r--r--  2.0 unx     4046 b- defN 23-May-03 19:50 super_gradients/training/utils/media/stream.py
+-rw-r--r--  2.0 unx     6926 b- defN 23-May-03 19:50 super_gradients/training/utils/media/video.py
+-rw-r--r--  2.0 unx      396 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizers/__init__.py
+-rw-r--r--  2.0 unx     9760 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizers/lamb.py
+-rw-r--r--  2.0 unx     3008 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizers/lion.py
+-rw-r--r--  2.0 unx     6834 b- defN 23-May-03 19:50 super_gradients/training/utils/optimizers/rmsprop_tf.py
+-rw-r--r--  2.0 unx      213 b- defN 23-May-03 19:50 super_gradients/training/utils/pose_estimation/__init__.py
+-rw-r--r--  2.0 unx    11167 b- defN 23-May-03 19:50 super_gradients/training/utils/pose_estimation/dekr_decode_callbacks.py
+-rw-r--r--  2.0 unx     7140 b- defN 23-May-03 19:50 super_gradients/training/utils/pose_estimation/dekr_visualization_callbacks.py
+-rw-r--r--  2.0 unx      387 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/__init__.py
+-rw-r--r--  2.0 unx     6271 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/calibrator.py
+-rw-r--r--  2.0 unx     8417 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/core.py
+-rw-r--r--  2.0 unx     2196 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/export.py
+-rw-r--r--  2.0 unx    17062 b- defN 23-May-03 19:50 super_gradients/training/utils/quantization/selective_quantization_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-03 19:50 super_gradients/training/utils/visualization/__init__.py
+-rw-r--r--  2.0 unx     1698 b- defN 23-May-03 19:50 super_gradients/training/utils/visualization/detection.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-May-03 19:50 super_gradients/training/utils/visualization/utils.py
+-rw-r--r--  2.0 unx     2218 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/LICENSE.YOLONAS.md
+-rw-r--r--  2.0 unx    11341 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx    36095 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    64233 b- defN 23-May-03 19:50 super_gradients-3.1.1.dist-info/RECORD
+557 files, 2815305 bytes uncompressed, 856289 bytes compressed:  69.6%
```

## zipnote {}

```diff
@@ -1092,17 +1092,14 @@
 
 Filename: super_gradients/training/datasets/pose_estimation_datasets/target_generators.py
 Comment: 
 
 Filename: super_gradients/training/datasets/samplers/__init__.py
 Comment: 
 
-Filename: super_gradients/training/datasets/samplers/infinite_sampler.py
-Comment: 
-
 Filename: super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py
 Comment: 
 
 Filename: super_gradients/training/datasets/segmentation_datasets/__init__.py
 Comment: 
 
 Filename: super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py
@@ -1650,26 +1647,26 @@
 
 Filename: super_gradients/training/utils/visualization/detection.py
 Comment: 
 
 Filename: super_gradients/training/utils/visualization/utils.py
 Comment: 
 
-Filename: super_gradients-3.1.0.dist-info/LICENSE.YOLONAS.md
+Filename: super_gradients-3.1.1.dist-info/LICENSE.YOLONAS.md
 Comment: 
 
-Filename: super_gradients-3.1.0.dist-info/LICENSE.md
+Filename: super_gradients-3.1.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: super_gradients-3.1.0.dist-info/METADATA
+Filename: super_gradients-3.1.1.dist-info/METADATA
 Comment: 
 
-Filename: super_gradients-3.1.0.dist-info/WHEEL
+Filename: super_gradients-3.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: super_gradients-3.1.0.dist-info/top_level.txt
+Filename: super_gradients-3.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: super_gradients-3.1.0.dist-info/RECORD
+Filename: super_gradients-3.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## super_gradients/__init__.py

```diff
@@ -16,10 +16,10 @@
     "object_names",
     "init_trainer",
     "is_distributed",
     "env_sanity_check",
     "setup_device",
 ]
 
-__version__ = "3.1.0"
+__version__ = "3.1.1"
 
 env_sanity_check()
```

## super_gradients/common/object_names.py

```diff
@@ -163,15 +163,14 @@
     LINEAR_EPOCH_STEP = "linear_epoch_step"
     LINEAR_BATCH_STEP = "linear_batch_step"
 
 
 class Samplers:
     """Static class to hold all the supported Samplers names"""
 
-    INFINITE = "InfiniteSampler"
     REPEAT_AUG = "RepeatAugSampler"
     DISTRIBUTED = "DistributedSampler"
     SEQUENTIAL = "SequentialSampler"
     SUBSET_RANDOM = "SubsetRandomSampler"
     RANDOM = "RandomSampler"
     WEIGHTED_RANDOM = "WeightedRandomSampler"
```

## super_gradients/common/auto_logging/auto_logger.py

```diff
@@ -66,14 +66,19 @@
         extra_kwargs = {}
         if cur_version >= python_38:
             extra_kwargs = dict(
                 force=True,
             )
         else:
             # If the logging does not support force=True, we should manually delete handlers
+            for h in manager.root.handlers:
+                try:
+                    h.close()
+                except AttributeError:
+                    pass
             del manager.root.handlers[:]
 
         if cur_version >= python_39:
             extra_kwargs["encoding"] = "utf-8"
 
         logging.basicConfig(
             filename=filename,
```

## super_gradients/modules/qarepvgg_block.py

```diff
@@ -311,7 +311,10 @@
         # inference frameworks will take care of resulting conv-bn-act-se
         # no need to fuse post_bn prematurely if it is there
         # call self.full_fusion() if you need it
         self.partial_fusion()
 
     def from_repvgg(self, src: RepVGGBlock):
         raise NotImplementedError
+
+    def prep_model_for_conversion(self, input_size: Optional[Union[tuple, list]] = None, **kwargs):
+        self.partial_fusion()
```

## super_gradients/modules/repvgg_block.py

```diff
@@ -1,8 +1,8 @@
-from typing import Type, Union, Mapping, Any
+from typing import Type, Union, Mapping, Any, Optional
 
 import numpy as np
 import torch
 from torch import nn
 
 
 class RepVGGBlock(nn.Module):
@@ -199,14 +199,17 @@
                 bias=False,
                 dilation=dilation,
             ),
         )
         result.add_module("bn", nn.BatchNorm2d(num_features=out_channels))
         return result
 
+    def prep_model_for_conversion(self, input_size: Optional[Union[tuple, list]] = None, **kwargs):
+        self.fuse_block_residual_branches()
+
 
 def fuse_repvgg_blocks_residual_branches(model: nn.Module):
     """
     Call fuse_block_residual_branches for all repvgg blocks in the model
     :param model: torch.nn.Module with repvgg blocks. Doesn't have to be entirely consists of repvgg.
     :type model: torch.nn.Module
     """
```

## super_gradients/training/datasets/samplers/__init__.py

```diff
@@ -1,7 +1,6 @@
-from super_gradients.training.datasets.samplers.infinite_sampler import InfiniteSampler
 from super_gradients.training.datasets.samplers.repeated_augmentation_sampler import RepeatAugSampler
 from super_gradients.common.object_names import Samplers
 from super_gradients.common.registry.registry import SAMPLERS
 
 
-__all__ = ["SAMPLERS", "Samplers", "InfiniteSampler", "RepeatAugSampler"]
+__all__ = ["SAMPLERS", "Samplers", "RepeatAugSampler"]
```

## super_gradients/training/sg_trainer/sg_trainer.py

```diff
@@ -28,15 +28,15 @@
 from super_gradients.common.decorators.factory_decorator import resolve_param
 from super_gradients.common.factories.callbacks_factory import CallbacksFactory
 from super_gradients.common.factories.list_factory import ListFactory
 from super_gradients.common.factories.losses_factory import LossesFactory
 from super_gradients.common.factories.metrics_factory import MetricsFactory
 
 from super_gradients.training import utils as core_utils, models, dataloaders
-from super_gradients.training.datasets.samplers import InfiniteSampler, RepeatAugSampler
+from super_gradients.training.datasets.samplers import RepeatAugSampler
 from super_gradients.training.exceptions.sg_trainer_exceptions import UnsupportedOptimizerFormat
 from super_gradients.training.metrics.metric_utils import (
     get_metrics_titles,
     get_metrics_results_tuple,
     get_logging_values,
     get_metrics_dict,
     get_train_loop_description_dict,
@@ -156,15 +156,14 @@
         self.average_model_checkpoint_filename = "average_model.pth"
         self.start_epoch = 0
         self.best_metric = np.inf
         self.external_checkpoint_path = None
         self.strict_load = StrictLoad.ON
         self.load_ema_as_net = False
         self.ckpt_best_name = "ckpt_best.pth"
-        self._infinite_train_loader = False
         self._first_backward = True
 
         # METRICS
         self.loss_logging_items_names = None
         self.train_metrics = None
         self.valid_metrics = None
         self.greater_metric_to_watch_is_better = None
@@ -457,19 +456,15 @@
             pbar_message_dict = get_train_loop_description_dict(
                 logging_values, self.train_metrics, self.loss_logging_items_names, gpu_mem=gpu_memory_utilization
             )
 
             progress_bar_train_loader.set_postfix(**pbar_message_dict)
             self.phase_callback_handler.on_train_batch_end(context)
 
-            # TODO: ITERATE BY MAX ITERS
-            # FOR INFINITE SAMPLERS WE MUST BREAK WHEN REACHING LEN ITERATIONS.
-            if (self._infinite_train_loader and batch_idx == len(self.train_loader) - 1) or (
-                self.max_train_batches is not None and self.max_train_batches - 1 <= batch_idx
-            ):
+            if self.max_train_batches is not None and self.max_train_batches - 1 <= batch_idx:
                 break
 
         self.train_monitored_values = sg_trainer_utils.update_monitored_values_dict(
             monitored_values_dict=self.train_monitored_values, new_values_dict=pbar_message_dict
         )
 
         return logging_values
@@ -1018,18 +1013,18 @@
             # Note: the dataloader uses sampler of the batch_sampler when it is not None.
             train_sampler = self.train_loader.batch_sampler.sampler if self.train_loader.batch_sampler is not None else self.train_loader.sampler
             if isinstance(train_sampler, SequentialSampler):
                 raise ValueError(
                     "You are using a SequentialSampler on you training dataloader, while working on DDP. "
                     "This cancels the DDP benefits since it makes each process iterate through the entire dataset"
                 )
-            if not isinstance(train_sampler, (DistributedSampler, InfiniteSampler, RepeatAugSampler)):
+            if not isinstance(train_sampler, (DistributedSampler, RepeatAugSampler)):
                 logger.warning(
                     "The training sampler you are using might not support DDP. "
-                    "If it doesnt, please use one of the following sampler: DistributedSampler, InfiniteSampler, RepeatAugSampler"
+                    "If it doesnt, please use one of the following sampler: DistributedSampler, RepeatAugSampler"
                 )
         self.training_params = TrainingParams()
         self.training_params.override(**training_params)
 
         self.net = model
         self._prep_net_for_train()
 
@@ -1160,18 +1155,14 @@
         if self.load_checkpoint and load_opt_params:
             self.optimizer.load_state_dict(self.checkpoint["optimizer_state_dict"])
 
         self.pre_prediction_callback = CallbacksFactory().get(self.training_params.pre_prediction_callback)
 
         self._initialize_mixed_precision(self.training_params.mixed_precision)
 
-        self._infinite_train_loader = (hasattr(self.train_loader, "sampler") and isinstance(self.train_loader.sampler, InfiniteSampler)) or (
-            hasattr(self.train_loader, "batch_sampler") and isinstance(self.train_loader.batch_sampler.sampler, InfiniteSampler)
-        )
-
         self.ckpt_best_name = self.training_params.ckpt_best_name
 
         if self.training_params.max_train_batches is not None:
             if self.training_params.max_train_batches > len(self.train_loader):
                 logger.warning("max_train_batches is greater than len(self.train_loader) and will have no effect.")
             elif self.training_params.max_train_batches <= 0:
                 raise ValueError("max_train_batches must be positive.")
```

## Comparing `super_gradients-3.1.0.dist-info/LICENSE.YOLONAS.md` & `super_gradients-3.1.1.dist-info/LICENSE.YOLONAS.md`

 * *Files identical despite different names*

## Comparing `super_gradients-3.1.0.dist-info/LICENSE.md` & `super_gradients-3.1.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `super_gradients-3.1.0.dist-info/METADATA` & `super_gradients-3.1.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: super-gradients
-Version: 3.1.0
+Version: 3.1.1
 Summary: SuperGradients
 Home-page: https://docs.deci.ai/super-gradients/documentation/source/welcome.html
 Author: Deci AI
 Author-email: rnd@deci.ai
 License: UNKNOWN
 Keywords: Deci,AI,Training,Deep Learning,Computer Vision,PyTorch,SOTA,Recipes,Pre Trained,Models
 Platform: UNKNOWN
@@ -167,34 +167,35 @@
 __________________________________________________________________________________________________________
 
 
 ```bash
 pip install super-gradients
 ```
 
-## What's New - Version 3.0.8
+## What's New - Version 3.1.1 (May 3rd)
 __________________________________________________________________________________________________________
-*  [QAT&PTQ](https://bit.ly/41hC8uI)
-* [Pose estimation](http://bit.ly/3o0xHq2)
-* [New documentation](http://bit.ly/3KYVCiJ)
-* [New semantic segmentation dataset - Mapillary Vistas Dataset](https://github.com/Deci-AI/super-gradients/blob/master/src/super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py)
-*  Lion optimizer
-* PP-YoloE pre-trained - new pre-trained [checkpoints](https://bit.ly/41dkt89) and [recipes](http://bit.ly/3gfLw07) for COCO2017 🎯
-* DDRNet pre-trained segmentation model - new pre-trained [checkpoints](https://bit.ly/41dkt89) and [recipes](http://bit.ly/3gfLw07) for Cityscapes and  [Knowledge distillation recipe for DDRNet](http://bit.ly/3GzZHHo)🎯
-
+* [YOLO-NAS](https://bit.ly/41WeNPZ)
+* New [predict function](https://bit.ly/3oZfaea) (predict on any image, video, url, path, stream)
+* [RoboFlow100](https://bit.ly/40YOJ5z) datasets integration 
+* A new [Documentation Hub](https://docs.deci.ai/super-gradients/documentation/source/welcome.html)
+* Integration with [DagsHub for experiment monitoring](https://bit.ly/3ALFUkQ)
+* Support [Darknet/Yolo format detection dataset](https://bit.ly/41VX6Qu) (used by Yolo v5, v6, v7, v8) 
+* [Segformer](https://bit.ly/3oYu6Jp) model and recipe 
+* Post Training Quantization and Quantization Aware Training - [notebooks](http://bit.ly/3KrN6an)
 
 Check out SG full [release notes](https://github.com/Deci-AI/super-gradients/releases).
 
 ## Coming soon
 __________________________________________________________________________________________________________
 - [ ] Pre-trained pose estimation model
-- [ ] New predict function on detection models
-- [ ] RoboFlow100 datasets integration 
-- [ ] A new documentation hub
+- [ ] Test Time Augmentations (TTA)
+- [ ] Recipe to train DEKR model(convertable to TRT) 
+- [ ] Key-points Rescoring for Pose estimation 
 - [ ] LR finder
+- [ ] Data analysis tools
 
 
 ## Table of Content
 __________________________________________________________________________________________________________
 <!-- toc -->
 
 - [Getting Started](#getting-started)
@@ -759,16 +760,16 @@
 If you are using SuperGradients library or benchmarks in your research, please cite SuperGradients deep learning training library.
 
 ## Community
 
 If you want to be a part of SuperGradients growing community, hear about all the exciting news and updates, need help, request for advanced features,
     or want to file a bug or issue report, we would love to welcome you aboard!
 
-* Slack is the place to be and ask questions about SuperGradients and get support. [Click here to join our Slack](
-  https://join.slack.com/t/supergradients-comm52/shared_invite/zt-10vz6o1ia-b_0W5jEPEnuHXm087K~t8Q)
+* Discord is the place to be and ask questions about SuperGradients and get support. [Click here to join our Discord Community](
+  https://discord.gg/2v6cEGMREN)
 
 * To report a bug, [file an issue](https://github.com/Deci-AI/super-gradients/issues) on GitHub.
 
 * Join the [SG Newsletter](https://www.supergradients.com/#Newsletter)
   for staying up to date with new features and models, important announcements, and upcoming events.
 
 * For a short meeting with us, use this [link](https://calendly.com/ofer-baratz-deci/15min) and choose your preferred time.
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: super-gradients Version: 3.1.0 Summary:
+Metadata-Version: 2.1 Name: super-gradients Version: 3.1.1 Summary:
 SuperGradients Home-page: https://docs.deci.ai/super-gradients/documentation/
 source/welcome.html Author: Deci AI Author-email: rnd@deci.ai License: UNKNOWN
 Keywords: Deci,AI,Training,Deep Learning,Computer
 Vision,PyTorch,SOTA,Recipes,Pre Trained,Models Platform: UNKNOWN Description-
 Content-Type: text/markdown Requires-Dist: torch (<1.14,>=1.9.0) Requires-Dist:
 tqdm (>=4.57.0) Requires-Dist: boto3 (>=1.17.15) Requires-Dist: jsonschema
 (>=3.2.0) Requires-Dist: Deprecated (>=1.2.11) Requires-Dist: opencv-python
@@ -83,31 +83,31 @@
 Input size is in format of [Batch x Channels x Width x Height] where 640 is the
 standard COCO dataset dimensions model.eval() model.prep_model_for_conversion
 (input_size=[1, 3, 640, 640]) # Create dummy_input # Convert model to onnx
 torch.onnx.export(model, dummy_input, "yolo_nas_m.onnx") ``` More information
 on how to take your model to production can be found in [Getting Started]
 (#getting-started) notebooks ## Quick Installation
 __________________________________________________________________________________________________________
-```bash pip install super-gradients ``` ## What's New - Version 3.0.8
+```bash pip install super-gradients ``` ## What's New - Version 3.1.1 (May 3rd)
 __________________________________________________________________________________________________________
-* [QAT&PTQ](https://bit.ly/41hC8uI) * [Pose estimation](http://bit.ly/3o0xHq2)
-* [New documentation](http://bit.ly/3KYVCiJ) * [New semantic segmentation
-dataset - Mapillary Vistas Dataset](https://github.com/Deci-AI/super-gradients/
-blob/master/src/super_gradients/training/datasets/segmentation_datasets/
-mapillary_dataset.py) * Lion optimizer * PP-YoloE pre-trained - new pre-trained
-[checkpoints](https://bit.ly/41dkt89) and [recipes](http://bit.ly/3gfLw07) for
-COCO2017 ð¯ * DDRNet pre-trained segmentation model - new pre-trained
-[checkpoints](https://bit.ly/41dkt89) and [recipes](http://bit.ly/3gfLw07) for
-Cityscapes and [Knowledge distillation recipe for DDRNet](http://bit.ly/
-3GzZHHo)ð¯ Check out SG full [release notes](https://github.com/Deci-AI/
-super-gradients/releases). ## Coming soon
-__________________________________________________________________________________________________________
-- [ ] Pre-trained pose estimation model - [ ] New predict function on detection
-models - [ ] RoboFlow100 datasets integration - [ ] A new documentation hub -
-[ ] LR finder ## Table of Content
+* [YOLO-NAS](https://bit.ly/41WeNPZ) * New [predict function](https://bit.ly/
+3oZfaea) (predict on any image, video, url, path, stream) * [RoboFlow100]
+(https://bit.ly/40YOJ5z) datasets integration * A new [Documentation Hub]
+(https://docs.deci.ai/super-gradients/documentation/source/welcome.html) *
+Integration with [DagsHub for experiment monitoring](https://bit.ly/3ALFUkQ) *
+Support [Darknet/Yolo format detection dataset](https://bit.ly/41VX6Qu) (used
+by Yolo v5, v6, v7, v8) * [Segformer](https://bit.ly/3oYu6Jp) model and recipe
+* Post Training Quantization and Quantization Aware Training - [notebooks]
+(http://bit.ly/3KrN6an) Check out SG full [release notes](https://github.com/
+Deci-AI/super-gradients/releases). ## Coming soon
+__________________________________________________________________________________________________________
+- [ ] Pre-trained pose estimation model - [ ] Test Time Augmentations (TTA) -
+[ ] Recipe to train DEKR model(convertable to TRT) - [ ] Key-points Rescoring
+for Pose estimation - [ ] LR finder - [ ] Data analysis tools ## Table of
+Content
 __________________________________________________________________________________________________________
 - [Getting Started](#getting-started) - [Advanced Features](#advanced-features)
 - [Installation Methods](#installation-methods) - [Prerequisites]
 (#prerequisites) - [Quick Installation](#quick-installation) - [Implemented
 Model Architectures](#implemented-model-architectures) - [Contributing]
 (#contributing) - [Citation](#citation) - [Community](#community) - [License]
 (#license) - [Deci Platform](#deci-platform)  ## Getting Started
@@ -375,32 +375,31 @@
 awesome contributors: [https://contrib.rocks/image?repo=Deci-AI/super-
 gradients]
 Made with [contrib.rocks](https://contrib.rocks). ## Citation If you are using
 SuperGradients library or benchmarks in your research, please cite
 SuperGradients deep learning training library. ## Community If you want to be a
 part of SuperGradients growing community, hear about all the exciting news and
 updates, need help, request for advanced features, or want to file a bug or
-issue report, we would love to welcome you aboard! * Slack is the place to be
+issue report, we would love to welcome you aboard! * Discord is the place to be
 and ask questions about SuperGradients and get support. [Click here to join our
-Slack]( https://join.slack.com/t/supergradients-comm52/shared_invite/zt-
-10vz6o1ia-b_0W5jEPEnuHXm087K~t8Q) * To report a bug, [file an issue](https://
-github.com/Deci-AI/super-gradients/issues) on GitHub. * Join the [SG
-Newsletter](https://www.supergradients.com/#Newsletter) for staying up to date
-with new features and models, important announcements, and upcoming events. *
-For a short meeting with us, use this [link](https://calendly.com/ofer-baratz-
-deci/15min) and choose your preferred time. ## License This project is released
-under the [Apache 2.0 license](LICENSE). ## Citing ### BibTeX ```bibtex @misc
-{supergradients, doi = {10.5281/ZENODO.7789328}, url = {https://zenodo.org/
-record/7789328}, author = {Aharon, Shay and {Louis-Dupont} and {Ofri Masad} and
-Yurkova, Kate and {Lotem Fridman} and {Lkdci} and Khvedchenya, Eugene and
-Rubin, Ran and Bagrov, Natan and Tymchenko, Borys and Keren, Tomer and Zhilko,
-Alexander and {Eran-Deci}}, title = {Super-Gradients}, publisher = {GitHub},
-journal = {GitHub repository}, year = {2021}, } ``` ### Latest DOI [![DOI]
-(https://zenodo.org/badge/DOI/10.5281/zenodo.7789328.svg)](https://doi.org/
-10.5281/zenodo.7789328)
+Discord Community]( https://discord.gg/2v6cEGMREN) * To report a bug, [file an
+issue](https://github.com/Deci-AI/super-gradients/issues) on GitHub. * Join the
+[SG Newsletter](https://www.supergradients.com/#Newsletter) for staying up to
+date with new features and models, important announcements, and upcoming
+events. * For a short meeting with us, use this [link](https://calendly.com/
+ofer-baratz-deci/15min) and choose your preferred time. ## License This project
+is released under the [Apache 2.0 license](LICENSE). ## Citing ### BibTeX
+```bibtex @misc{supergradients, doi = {10.5281/ZENODO.7789328}, url = {https://
+zenodo.org/record/7789328}, author = {Aharon, Shay and {Louis-Dupont} and {Ofri
+Masad} and Yurkova, Kate and {Lotem Fridman} and {Lkdci} and Khvedchenya,
+Eugene and Rubin, Ran and Bagrov, Natan and Tymchenko, Borys and Keren, Tomer
+and Zhilko, Alexander and {Eran-Deci}}, title = {Super-Gradients}, publisher =
+{GitHub}, journal = {GitHub repository}, year = {2021}, } ``` ### Latest DOI [!
+[DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7789328.svg)](https://
+doi.org/10.5281/zenodo.7789328)
 __________________________________________________________________________________________________________
 ## Deci Platform Deci Platform is our end to end platform for building,
 optimizing and deploying deep learning models to production. [Request free
 trial](https://bit.ly/3qO3icq) to enjoy immediate improvement in throughput,
 latency, memory footprint and model size. Features - Automatically compile and
 quantize your models with just a few clicks (TensorRT, OpenVINO). - Gain up to
 10X improvement in throughput, latency, memory and model size. - Easily
```

## Comparing `super_gradients-3.1.0.dist-info/RECORD` & `super_gradients-3.1.1.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-super_gradients/__init__.py,sha256=bwjT_UxykuA7BjB2FfWvbiWu6xtNB6YJXX5mqLPmp1I,711
+super_gradients/__init__.py,sha256=T2_OhgYgFhdmsAJSTvLMXKYOFL8asv3oPZANEq9w-7A,711
 super_gradients/evaluate_checkpoint.py,sha256=cAB8pjlpxrpyJ2RhDp9jtV90TRvih7Axl0D2HVbfFKA,1657
 super_gradients/evaluate_from_recipe.py,sha256=aEUFWz0ue8tI55ChEivtABxUe7lhLCqT9aOywoenYfM,1807
 super_gradients/qat_from_recipe.py,sha256=Jb355vmclhurcOYN8Qgr6DFRMnnoxRB6N1uI5RLT9cM,702
 super_gradients/requirements.pro.txt,sha256=N4SNm12LMYBhOwA5ShEQlihV_6nJoveWkbEo1037idI,44
 super_gradients/requirements.txt,sha256=-hJEsVtZGOENWHmv4jiAUp-doNLwlJ_Ld4uhVULJf-U,729
 super_gradients/resume_experiment.py,sha256=VSmGBGaFOdz6hOTRkHm7un0MHolUk4_CvXfu2jtjGZM,537
 super_gradients/train_from_kd_recipe.py,sha256=OpRZsmleqXWQyFeaLzcnIooa_YEYEHFhkHr63Cs_QU8,693
 super_gradients/train_from_recipe.py,sha256=ZdCUpUlLPiCejcKff2FTfg33_TjZF0CwvZ-eaQlVyrA,650
 super_gradients/common/__init__.py,sha256=1F7pRDWoGs7wMWpbBw3iaTPWpeegxOroNPqUO3nzEMw,1098
-super_gradients/common/object_names.py,sha256=si2UiliiCCsSULfT-6kBXNs98C6snrawOFlC0vPMsgU,15372
+super_gradients/common/object_names.py,sha256=XdIY0xm9zurs5xjZ_RPh0f6RCJxmtpKreDaEHt-dVJk,15339
 super_gradients/common/abstractions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/common/abstractions/abstract_logger.py,sha256=MpEjg7PihMZb_qLBKC-R58wWFqNJdPJMlOkxEU25hCU,879
 super_gradients/common/abstractions/mute_processes.py,sha256=JxC3ofVySoiL7U7x9QYhzWLVYArkgqKQB2Kp3HyPOyE,3129
 super_gradients/common/auto_logging/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-super_gradients/common/auto_logging/auto_logger.py,sha256=qH84FkmTe50L7Mg8kDjTKVHVxCsCi4DQTMV2V53jARU,4687
+super_gradients/common/auto_logging/auto_logger.py,sha256=WtlKaj5p8Ayx3gJ9XcRkuIG7oVicTs3K_X_gVeEfZOI,4846
 super_gradients/common/auto_logging/console_logging.py,sha256=PEPSfHQ8incS13dkM9gzlWBeRdwbodo9qVqRSk32s_E,6625
 super_gradients/common/aws_connection/__init__.py,sha256=cZCFSeQHk8E6TTZHTjnAhezGATF5iSKiFR2dBof8vqg,142
 super_gradients/common/aws_connection/aws_connector.py,sha256=2wHpTZubxc54tAqE5FaNIbC0LwtLFMkDS_rmx9x3XXg,4182
 super_gradients/common/aws_connection/aws_secrets_manager_connector.py,sha256=RUyDEx96sC4pGI3lH_z_Eo0dwP5QxZ0Qpy-ZFxQ6mz4,7198
 super_gradients/common/crash_handler/__init__.py,sha256=BWse71cn7bDfvpw52Rhpr0WtQyoxN9KmzEWX3w__ElE,119
 super_gradients/common/crash_handler/crash_handler.py,sha256=cZokQPUpTtlXJ6Y8QzviF4fpXulmHvEnVCl6pRKipVY,669
 super_gradients/common/crash_handler/crash_tips.py,sha256=sbBzMKnPMMvQv8ba7MV1w1tyOyaSS-p4bE7DV1yUHdw,11775
@@ -153,16 +153,16 @@
 super_gradients/modules/conv_bn_act_block.py,sha256=uJgtSZbW_km3zvlS9hh2PzxgmHjeiINtNEC9RlffD6Y,3054
 super_gradients/modules/conv_bn_relu_block.py,sha256=pZ0OazMsoP7PxjV6-ltgR8IytjsF6tsC71GH4kRgEgE,1976
 super_gradients/modules/detection_modules.py,sha256=srfbJXd4tWk4UL92Wu2Lq2l6qI3YvzSP_Khjtsn9fS0,14805
 super_gradients/modules/head_replacement_utils.py,sha256=sDXb1CiJN08-mpjrdzyY46s_FEG72yFx2YsF2Rl22Xw,2143
 super_gradients/modules/multi_output_modules.py,sha256=YLofR05Z56k4iHM460KRO-GQ4jMcP1MrrrgT-aOcew4,4362
 super_gradients/modules/pixel_shuffle.py,sha256=Rcka24mhF8fR5OuG3jgIGV1yUllaEOWZU4qFjKMheIg,860
 super_gradients/modules/pose_estimation_modules.py,sha256=PjYY28XkAz52KgREnCupoIbCCFM6TBYu1Shudmq7xxs,3953
-super_gradients/modules/qarepvgg_block.py,sha256=Ou0FbQGC4OfmGjRb7GN0fnhvg4Ib7bavlG4YhUTRjOM,11642
-super_gradients/modules/repvgg_block.py,sha256=uT107B_lO09aeqvg0z9uDeR3c-tmyvNqJEdVmWtV1cw,8544
+super_gradients/modules/qarepvgg_block.py,sha256=k5w_gvJyFfPiwPFEOJ909Rmq6x3IVS9qTM30o-Hg3iE,11773
+super_gradients/modules/repvgg_block.py,sha256=RIc3Iq7Ce1JwatM-acmpWCYV8gpMtu9AXV1lo5BkFEw,8699
 super_gradients/modules/sampling.py,sha256=xcGx0oIvQGyPjtZFGQko_vybYYtQk-mL2AFA0G4MULs,2138
 super_gradients/modules/se_blocks.py,sha256=itIUGGoqKNBYhAyj20aKcRKQlK_HdD0sqCsfK-a8yE4,1459
 super_gradients/modules/skip_connections.py,sha256=QR1V7AG9_4eK3xgywanDU4NpK5HMiv_jy2AMOgH0di4,1403
 super_gradients/modules/utils.py,sha256=B3h8_ABd15fS6yaozvG7xsAc0VfuDNmGBKm3ty-Yejg,2968
 super_gradients/modules/quantization/__init__.py,sha256=YNuNoitnDrNS30BBeadjiGZfqOTdZu_GPTbiHyLmPV4,716
 super_gradients/modules/quantization/quantized_skip_connections.py,sha256=0NaQ63tdFC9s7YL1VV9VLheUYaN4pb29kjw_etmzR_g,2649
 super_gradients/modules/quantization/quantized_stdc_blocks.py,sha256=aahisE-qutTEnfVH2rfRKhUYEKssuTJTPnuBIq7lYHY,4604
@@ -359,16 +359,15 @@
 super_gradients/training/datasets/detection_datasets/roboflow/roboflow100.py,sha256=9UEctKh8WxBLxdRP8wqfg3KDFq_KDYTr5AX4qD2Om7I,3504
 super_gradients/training/datasets/detection_datasets/roboflow/utils.py,sha256=_7mtuGnTHUVqfUqWlC9zpKGutBdaYJCGGj9pSbItfxI,1997
 super_gradients/training/datasets/pose_estimation_datasets/__init__.py,sha256=BeCVpXLn0FV9Oo_8iWtHz9n1GxdhXqTzymGT97_bdCA,502
 super_gradients/training/datasets/pose_estimation_datasets/base_keypoints.py,sha256=6xNszBrqqOOdIKgM2ZFOZ4Crwssfh096_AcLZL5R1q4,4910
 super_gradients/training/datasets/pose_estimation_datasets/coco_keypoints.py,sha256=aADh3OLNLBLCk-3_nxLHjrrHniqr-tfbIHjKzJf-REA,9066
 super_gradients/training/datasets/pose_estimation_datasets/coco_utils.py,sha256=uMq0vV22npZqz21L_preyhbyKSHiBqS14Mp2UuEb-_4,5929
 super_gradients/training/datasets/pose_estimation_datasets/target_generators.py,sha256=McVUG3sWR9Lxgk_ca8ECqvYieQwZApsFRfLNABES51Q,10167
-super_gradients/training/datasets/samplers/__init__.py,sha256=bsLNxxZ61qQx2DbmGzsfd_6jDo4UYPkYNswoTOQtjrE,385
-super_gradients/training/datasets/samplers/infinite_sampler.py,sha256=VPqUXdOAsPAwuozPQ19rweHkT-RYlq9BMLlNWt8Zofw,2516
+super_gradients/training/datasets/samplers/__init__.py,sha256=CfddXWvnsVLbQyYkUGyBwdl98U8wj7-MfNPbGjZjl8g,278
 super_gradients/training/datasets/samplers/repeated_augmentation_sampler.py,sha256=dnYh_2wWCFPlWVwnEhUEwhAaRpJGIGtoIbNiXSRAfq4,4809
 super_gradients/training/datasets/segmentation_datasets/__init__.py,sha256=5zkvFQ4Av5Ceydrnkq9jS19xp9axFBF7M-41K6DXBFU,1037
 super_gradients/training/datasets/segmentation_datasets/cityscape_segmentation.py,sha256=tRPCnl07gmducqFp9nm_ks5ZkRAZnIG5bQQTVKhweLs,6714
 super_gradients/training/datasets/segmentation_datasets/coco_segmentation.py,sha256=ehn6K8hMAItoGPA9NRa8T23z-oDeCQ-6jADRyBmu8i0,7717
 super_gradients/training/datasets/segmentation_datasets/mapillary_dataset.py,sha256=DcRz59FNdX3koBCth09AT1EEHn77xXoxBX-yaWa-fmo,5518
 super_gradients/training/datasets/segmentation_datasets/pascal_voc_segmentation.py,sha256=uQJyztsrnSHbxvzitYqixVeNeXN52UYZ66L__Pkcgbc,11146
 super_gradients/training/datasets/segmentation_datasets/segmentation_dataset.py,sha256=5uYUtLVaCj5J-Khw9xNazADAEAj6VvfZgRLOg1V9O6A,8470
@@ -490,15 +489,15 @@
 super_gradients/training/pre_launch_callbacks/__init__.py,sha256=SZtn0Kq5PJ_GIMfFT5bBb0Pck6r5mAnBAfgpDaX5Cdk,393
 super_gradients/training/pre_launch_callbacks/pre_launch_callbacks.py,sha256=E3UsNalAFR0-7pwga-OjFCTp4m7SuO9BEy04Lwt18kk,13955
 super_gradients/training/processing/__init__.py,sha256=L_S3KapcujiBTXjHcMZxQz5aCwJM9Xxurbhs08oy0_o,517
 super_gradients/training/processing/processing.py,sha256=xx6q2nO2VXC-FGX4rYVp9Otbipbv43gToYepKe0jQyk,13177
 super_gradients/training/qat_trainer/__init__.py,sha256=GZRdCf6P1Ximp-eoVw8kHv5Zb4AjBqxV0E2NwO1OmNo,98
 super_gradients/training/qat_trainer/qat_trainer.py,sha256=wrdK5ao9S1EJpufOtg_rJjI-qExzlHUa_ybsTNOVdTA,9701
 super_gradients/training/sg_trainer/__init__.py,sha256=dug-p1erLN2SzYFQytJzPWDLOCmfvE94kFtcFLOTqj0,184
-super_gradients/training/sg_trainer/sg_trainer.py,sha256=XXLM3D_c-XVQW4j-G7sJRAfjD7DgMuFJf75N85Gm8jY,97356
+super_gradients/training/sg_trainer/sg_trainer.py,sha256=22Pvj4ZKntAcC1oU-SKSJAyX7drtf06r1TX6qJ1B0OU,96749
 super_gradients/training/training_hyperparams/__init__.py,sha256=R5pvZNSQgDNxRp23qAlAAhGdPT7u_e78QiztqQDqosc,1685
 super_gradients/training/training_hyperparams/training_hyperparams.py,sha256=pZIOz9L6vf-tgCMUbvf2WLch1zCCfDevhfYPnL3QR7A,3774
 super_gradients/training/transforms/__init__.py,sha256=SMLfPEp8zqooiV6mB4byOzk5SprUUo77LIUNgTTB7A8,1024
 super_gradients/training/transforms/all_transforms.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/transforms/keypoint_transforms.py,sha256=-lTR8tHtWGmK6THZvyI52OpH5yhWXDGJeUJM_FwcZhE,16193
 super_gradients/training/transforms/pipeline_adaptors.py,sha256=ukVHjcx-XaCEGZ3I_afIb9Uj73vwYtkmgrLJw9jr7oU,1134
 super_gradients/training/transforms/transforms.py,sha256=uDbuGhNmEL0Mo_FvO4R9NhUf3nH9yQygGIxSgciqV60,55089
@@ -546,13 +545,13 @@
 super_gradients/training/utils/quantization/calibrator.py,sha256=vfXnyPxLdHjk5e5CF3-lBwofRDjX-ZCyDaRreuu6_h4,6271
 super_gradients/training/utils/quantization/core.py,sha256=CYykLasziH9YT0h_utxWj6WZ6tXi4KUSKaiBf1N2YZM,8417
 super_gradients/training/utils/quantization/export.py,sha256=GW22x2GMQJMEp1iZcJ63qcxev6Etay_FI6taKbJpmv8,2196
 super_gradients/training/utils/quantization/selective_quantization_utils.py,sha256=hQ8uZliyAK21pguj0aSybxINffXrj0R2YCHCWIRV7Z4,17062
 super_gradients/training/utils/visualization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 super_gradients/training/utils/visualization/detection.py,sha256=348rm6aggC_RLn9Zsnr9FC0AJu5zieHVhTzQGJs6sfk,1698
 super_gradients/training/utils/visualization/utils.py,sha256=LXh2fmdauApUJEn62a0yEXwKQ6G1ySlWvqkK9Ap8ybU,2847
-super_gradients-3.1.0.dist-info/LICENSE.YOLONAS.md,sha256=mPgPXAN-RoGSYLzisdBu2uJx2HyJHd8enqEUlpO5mmQ,2218
-super_gradients-3.1.0.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
-super_gradients-3.1.0.dist-info/METADATA,sha256=Zu_Yq27JlSrrBb214F99EmW_9UWoh0lxi52IJVsh7tk,36159
-super_gradients-3.1.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-super_gradients-3.1.0.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
-super_gradients-3.1.0.dist-info/RECORD,,
+super_gradients-3.1.1.dist-info/LICENSE.YOLONAS.md,sha256=mPgPXAN-RoGSYLzisdBu2uJx2HyJHd8enqEUlpO5mmQ,2218
+super_gradients-3.1.1.dist-info/LICENSE.md,sha256=jWCBQN-JmCX0hwvn3MqItDj18W3riP4zda31ncMkcfA,11341
+super_gradients-3.1.1.dist-info/METADATA,sha256=APFfugaXHwe_gu19_wXwrq5gFJ2kO015ihom34VXe9c,36095
+super_gradients-3.1.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+super_gradients-3.1.1.dist-info/top_level.txt,sha256=k8ZbuOXtbEm0O2O3MCG-rnUyDilV2FYLXMbeXUspUXI,16
+super_gradients-3.1.1.dist-info/RECORD,,
```

