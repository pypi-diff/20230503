# Comparing `tmp/ml-starter-0.0.25.tar.gz` & `tmp/ml-starter-0.0.26.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.25.tar", last modified: Tue May  2 21:28:22 2023, max compression
+gzip compressed data, was "ml-starter-0.0.26.tar", last modified: Wed May  3 03:42:13 2023, max compression
```

## Comparing `ml-starter-0.0.25.tar` & `ml-starter-0.0.26.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-02 21:28:05.000000 ml-starter-0.0.25/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-02 21:28:05.000000 ml-starter-0.0.25/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-02 21:28:22.834049 ml-starter-0.0.25/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-02 21:28:05.000000 ml-starter-0.0.25/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.818049 ml-starter-0.0.25/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    23447 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/launchers/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/launchers/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.822049 ml-starter-0.0.25/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.830049 ml-starter-0.0.25/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.830049 ml-starter-0.0.25/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.830049 ml-starter-0.0.25/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.830049 ml-starter-0.0.25/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20288 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-02 21:28:05.000000 ml-starter-0.0.25/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 21:28:22.834049 ml-starter-0.0.25/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-02 21:28:22.000000 ml-starter-0.0.25/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-02 21:28:05.000000 ml-starter-0.0.25/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 21:28:05.000000 ml-starter-0.0.25/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-02 21:28:05.000000 ml-starter-0.0.25/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 21:28:05.000000 ml-starter-0.0.25/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 21:28:22.834049 ml-starter-0.0.25/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-02 21:28:05.000000 ml-starter-0.0.25/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.129641 ml-starter-0.0.26/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-03 03:42:00.000000 ml-starter-0.0.26/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 03:42:00.000000 ml-starter-0.0.26/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 03:42:13.129641 ml-starter-0.0.26/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-03 03:42:00.000000 ml-starter-0.0.26/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.113641 ml-starter-0.0.26/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.117641 ml-starter-0.0.26/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23447 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.117641 ml-starter-0.0.26/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/launchers/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9906 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/launchers/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.117641 ml-starter-0.0.26/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32984 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12321 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.117641 ml-starter-0.0.26/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.117641 ml-starter-0.0.26/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.117641 ml-starter-0.0.26/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.117641 ml-starter-0.0.26/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.121641 ml-starter-0.0.26/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/scripts/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.121641 ml-starter-0.0.26/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17920 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.121641 ml-starter-0.0.26/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.121641 ml-starter-0.0.26/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13280 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.121641 ml-starter-0.0.26/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.121641 ml-starter-0.0.26/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.121641 ml-starter-0.0.26/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.125641 ml-starter-0.0.26/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20360 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.125641 ml-starter-0.0.26/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8898 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.125641 ml-starter-0.0.26/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.129641 ml-starter-0.0.26/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-03 03:42:00.000000 ml-starter-0.0.26/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 03:42:13.129641 ml-starter-0.0.26/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 03:42:13.000000 ml-starter-0.0.26/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-03 03:42:13.000000 ml-starter-0.0.26/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 03:42:13.000000 ml-starter-0.0.26/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-03 03:42:13.000000 ml-starter-0.0.26/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-03 03:42:13.000000 ml-starter-0.0.26/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-03 03:42:00.000000 ml-starter-0.0.26/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 03:42:00.000000 ml-starter-0.0.26/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-03 03:42:00.000000 ml-starter-0.0.26/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-03 03:42:00.000000 ml-starter-0.0.26/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-03 03:42:13.129641 ml-starter-0.0.26/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-03 03:42:00.000000 ml-starter-0.0.26/setup.py
```

### Comparing `ml-starter-0.0.25/LICENSE` & `ml-starter-0.0.26/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/PKG-INFO` & `ml-starter-0.0.26/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.25
+Version: 0.0.26
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.25/README.md` & `ml-starter-0.0.26/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/api.py` & `ml-starter-0.0.26/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/core/config.py` & `ml-starter-0.0.26/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/core/env.py` & `ml-starter-0.0.26/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/core/registry.py` & `ml-starter-0.0.26/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/core/state.py` & `ml-starter-0.0.26/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/launchers/base.py` & `ml-starter-0.0.26/ml/launchers/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 from dataclasses import dataclass
 from typing import Generic, TypeVar
 
 from ml.core.config import BaseConfig, BaseObjectWithPointers
 from ml.trainers.base import BaseTrainer
 
+T = TypeVar("T", bound="BaseLauncher")
+
 
 @dataclass
 class BaseLauncherConfig(BaseConfig):
     pass
 
 
 LauncherConfigT = TypeVar("LauncherConfigT", bound=BaseLauncherConfig)
-TrainerT = TypeVar("TrainerT", bound=BaseTrainer)
 
 
 class BaseLauncher(BaseObjectWithPointers[LauncherConfigT], Generic[LauncherConfigT]):
-    def launch(self) -> None:
+    def launch(self, trainer: BaseTrainer) -> None:
         """Launches the training process.
 
+        Args:
+            trainer: The trainer being launched
+
         Raises:
             NotImplementedError: If the subclass does not implement this method
         """
 
         raise NotImplementedError
```

### Comparing `ml-starter-0.0.25/ml/launchers/ddp.py` & `ml-starter-0.0.26/ml/launchers/ddp.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import torch
 import torch.multiprocessing as mp
 from omegaconf import DictConfig
 
 from ml.core.registry import Objects, register_launcher
 from ml.launchers.base import BaseLauncher, BaseLauncherConfig
 from ml.scripts.train import train_main
-from ml.trainers.base import MultiprocessConfig
+from ml.trainers.base import BaseTrainer, MultiprocessConfig
 from ml.utils.distributed import (
     set_init_method,
     set_master_addr,
     set_master_port,
     set_rank,
     set_world_size,
 )
@@ -70,15 +70,15 @@
 @dataclass
 class DDPLauncherConfig(BaseLauncherConfig):
     pass
 
 
 @register_launcher("ddp", DDPLauncherConfig)
 class DDPLauncher(BaseLauncher[DDPLauncherConfig]):
-    def launch(self) -> None:
+    def launch(self, trainer: BaseTrainer) -> None:
         if not torch.cuda.is_available():
             raise RuntimeError("DDPLauncher requires CUDA")
         device_count = torch.cuda.device_count()
 
         func = functools.partial(process_main, raw_config=self.raw_config)
 
         cfg = MultiprocessConfig(
```

### Comparing `ml-starter-0.0.25/ml/launchers/slurm.py` & `ml-starter-0.0.26/ml/launchers/slurm.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,22 +19,24 @@
 import re
 import signal
 import subprocess
 import sys
 from dataclasses import dataclass
 from pathlib import Path
 from types import FrameType
+from typing import TypeVar
 
 from omegaconf import II, MISSING, OmegaConf
 
 from ml.core.config import conf_field
 from ml.core.env import get_stage_dir
 from ml.core.registry import Objects, project_dirs, register_launcher
 from ml.launchers.base import BaseLauncher, BaseLauncherConfig
 from ml.scripts.train import train_main
+from ml.trainers.base import BaseTrainer
 from ml.utils.distributed import (
     get_master_addr,
     get_master_port,
     get_random_port,
     is_master,
     set_init_method,
     set_master_addr,
@@ -43,14 +45,16 @@
 )
 from ml.utils.logging import configure_logging
 from ml.utils.staging import stage_environment
 from ml.utils.torch_distributed import get_distributed_backend, init_process_group
 
 logger: logging.Logger = logging.getLogger(__name__)
 
+T = TypeVar("T", bound="SlurmLauncher")
+
 SBATCH_TEMPLATE: str = """
 #!/bin/bash
 #SBATCH --job-name={job_name}
 #SBATCH --partition={partition}
 #SBATCH --requeue
 #SBATCH --signal=USR1@90
 #SBATCH --time={time_limit}
@@ -142,15 +146,15 @@
 def ignore_signal(signum: int, _: FrameType | None) -> None:
     sig = signal.Signals(signum)
     logger.info("Ignoring signal %s", sig.name)
 
 
 @register_launcher("slurm", SlurmLauncherConfig)
 class SlurmLauncher(BaseLauncher[SlurmLauncherConfig]):
-    def launch(self) -> None:
+    def write_sbatch_file(self, trainer: BaseTrainer) -> Path:
         # Gets some configuration options.
         gpus_per_node = self.config.gpus_per_node
         gpu_type = self.config.gpu_type
         tasks_per_node = gpus_per_node
         cpus_per_task = self.config.cpus_per_gpu
 
         # GRES and GPU Bind SBatch options.
@@ -159,60 +163,65 @@
 
         # Gets extra SBatch options.
         sbatch_lines: list[str] = []
         if "EMAIL" in os.environ:
             sbatch_lines += [f"--mail-user={os.environ['EMAIL']}", "--mail-type=ALL"]
 
         # Writes all Slurm stuff (including logs) to this folder.
-        slurm_log_dir = self.exp_dir / "logs"
+        slurm_log_dir = trainer.exp_dir / "logs"
         slurm_log_dir.mkdir(exist_ok=True, parents=True)
-        sbatch_path = self.exp_dir / "sbatch.sh"
+        sbatch_path = trainer.exp_dir / "sbatch.sh"
 
         # Stages all files to a new directory.
         stage_dir = stage_environment(project_dirs.paths[1:], get_stage_dir())
 
         # Gets the python path with the new output directory.
         python_path_parts = [str(stage_dir)] + os.environ.get("PYTHONPATH", "").split(":")
         python_path = ":".join(p for p in python_path_parts if p)
 
         # Comment miscellaneous stuff here.
         comments: list[str] = []
         if self.config.comment is not None:
             comments += [self.config.comment]
-        comments += [f"Log directory: {self.exp_dir}"]
+        comments += [f"Log directory: {trainer.exp_dir}"]
         comments += [f"Code location: {stage_dir}"]
 
         # Saves the config that is used to launch the Slurm job.
-        self.save_config()
+        trainer.save_config()
 
         # Builds the SBatch file.
         sbatch_file = SBATCH_TEMPLATE.format(
-            job_name=self.config.exp_name,
+            job_name=trainer.exp_name,
             partition=self.config.partition,
             time_limit=self.config.time_limit,
             comment="; ".join(comments),
             num_nodes=self.config.num_nodes,
             tasks_per_node=tasks_per_node,
             cpus_per_task=cpus_per_task,
             gres=gres,
             gpu_bind=gpu_bind,
             output_path=slurm_log_dir / "slurm_out.txt",
             error_path=slurm_log_dir / "slurm_err.%j.txt",
             extra_sbatch_lines="\n".join(f"#SBATCH {line}" for line in sbatch_lines),
             stage_dir=stage_dir,
             pythonpath=python_path,
             master_port=self.config.master_port,
-            config_path=self.exp_dir / "config.yaml",
-            lock_file_path=self.exp_dir / ".lock_running",
+            config_path=trainer.exp_dir / "config.yaml",
+            lock_file_path=trainer.exp_dir / ".lock_running",
         )
 
         with open(sbatch_path, "w", encoding="utf-8") as f:
             f.write(sbatch_file)
         logger.info("Wrote sbatch file to %s", sbatch_path)
 
+        return sbatch_path
+
+    def launch(self, trainer: BaseTrainer) -> None:
+        sbatch_path = self.write_sbatch_file(trainer)
+
         # Call `sbatch` on the given file.
         all_run_ids: list[str] = []
         for _ in range(self.config.num_jobs):
             command = ["sbatch", str(sbatch_path)]
             if all_run_ids:
                 command += ["--dependency", all_run_ids[-1]]
             proc = subprocess.Popen(  # pylint: disable=consider-using-with
@@ -226,15 +235,15 @@
             run_ids = re.findall(r"Submitted batch job (\d+)", log_line)
             assert len(run_ids) == 1, f"Unexpected log line: {log_line}"
             all_run_ids += [run_ids[0]]
 
         run_ids_str = "".join(f"\n - {run_id}" for run_id in all_run_ids)
         logger.info("Launched %d job(s):%s", len(all_run_ids), run_ids_str)
 
-        self.add_lock_file("scheduled", exists_ok=False)
+        trainer.add_lock_file("scheduled", exists_ok=False)
 
 
 def slurm_main() -> None:
     args = sys.argv[1:]
     assert len(args) == 1, f"Unexpected arguments to `slurm_main`: {sys.argv}"
 
     # Adds the stage directories as project directories.
```

### Comparing `ml-starter-0.0.25/ml/loggers/base.py` & `ml-starter-0.0.26/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/loggers/meter.py` & `ml-starter-0.0.26/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/loggers/multi.py` & `ml-starter-0.0.26/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/loggers/stdout.py` & `ml-starter-0.0.26/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/loggers/tensorboard.py` & `ml-starter-0.0.26/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/lr_schedulers/base.py` & `ml-starter-0.0.26/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.26/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.26/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/lr_schedulers/linear.py` & `ml-starter-0.0.26/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.26/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.26/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/models/activations.py` & `ml-starter-0.0.26/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/models/base.py` & `ml-starter-0.0.26/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/models/embeddings.py` & `ml-starter-0.0.26/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/models/init.py` & `ml-starter-0.0.26/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/models/norms.py` & `ml-starter-0.0.26/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/optimizers/adam.py` & `ml-starter-0.0.26/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/optimizers/adamw.py` & `ml-starter-0.0.26/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/optimizers/adan.py` & `ml-starter-0.0.26/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/optimizers/base.py` & `ml-starter-0.0.26/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/optimizers/sgd.py` & `ml-starter-0.0.26/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/optimizers/shampoo.py` & `ml-starter-0.0.26/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/scripts/cli.py` & `ml-starter-0.0.26/ml/scripts/cli.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     if project_root is not None:
         add_project_dir(Path(project_root).resolve())
 
     set_random_seed()
 
     without_objects_scripts: dict[str, Callable[[DictConfig], None]] = {
         "compile": compiler.compile_main,
-        "launch": launch.launch_main,
         "stage": stage.stage_main,
         "resolve": resolve.resolve_main,
+        "launch": launch.launch_main,
     }
 
     with_objects_scripts: dict[str, Callable[[Objects], None]] = {
         "train": train.train_main,
     }
 
     scripts: dict[str, Callable[..., None]] = {**with_objects_scripts, **without_objects_scripts}
```

### Comparing `ml-starter-0.0.25/ml/scripts/compiler.py` & `ml-starter-0.0.26/ml/scripts/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/scripts/stage.py` & `ml-starter-0.0.26/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/scripts/train.py` & `ml-starter-0.0.26/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/base.py` & `ml-starter-0.0.26/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.26/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.26/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/collate.py` & `ml-starter-0.0.26/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.26/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.26/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.26/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.26/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.26/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/utils.py` & `ml-starter-0.0.26/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.26/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/environments/base.py` & `ml-starter-0.0.26/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/environments/utils.py` & `ml-starter-0.0.26/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/environments/worker.py` & `ml-starter-0.0.26/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/losses/reduce.py` & `ml-starter-0.0.26/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/rl/base.py` & `ml-starter-0.0.26/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/rl/replay.py` & `ml-starter-0.0.26/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/tasks/sl/base.py` & `ml-starter-0.0.26/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/base.py` & `ml-starter-0.0.26/ml/trainers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,17 @@
 
     logger: MultiLogger
     loggers: list[BaseLogger]
 
     def __init__(self, config: TrainerConfigT) -> None:
         super().__init__(config)
 
-        self.exp_dir = get_exp_dir(Path(config.base_run_dir), config.exp_name, config.run_id)
+        self.exp_name = config.exp_name
+        self.run_id = config.run_id
+        self.exp_dir = get_exp_dir(Path(config.base_run_dir), self.exp_name, self.run_id)
         self.log_dir = self.exp_dir / config.log_dir_name
         self.checkpoint_config = config.checkpoint
         self.loggers = []
         self.logger = MultiLogger(default_namespace="trainer")
         self.signal_handlers: dict[signal.Signals, list[Callable[[], None]]] = {}
 
         logger.info("Experiment directory: %s", self.exp_dir)
```

### Comparing `ml-starter-0.0.25/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.26/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.26/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.26/ml/trainers/mixins/grad_clipping.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.26/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.26/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.26/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.26/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.26/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/rl.py` & `ml-starter-0.0.26/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/sl.py` & `ml-starter-0.0.26/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/trainers/vanilla.py` & `ml-starter-0.0.26/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/argparse.py` & `ml-starter-0.0.26/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/atomic.py` & `ml-starter-0.0.26/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/augmentation.py` & `ml-starter-0.0.26/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/caching.py` & `ml-starter-0.0.26/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/call_train.py` & `ml-starter-0.0.26/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/cli.py` & `ml-starter-0.0.26/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/colors.py` & `ml-starter-0.0.26/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/compiler.py` & `ml-starter-0.0.26/ml/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/data.py` & `ml-starter-0.0.26/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/datetime.py` & `ml-starter-0.0.26/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/device/auto.py` & `ml-starter-0.0.26/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/device/base.py` & `ml-starter-0.0.26/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/device/cpu.py` & `ml-starter-0.0.26/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/device/gpu.py` & `ml-starter-0.0.26/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/device/metal.py` & `ml-starter-0.0.26/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/distributed.py` & `ml-starter-0.0.26/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/image.py` & `ml-starter-0.0.26/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/io.py` & `ml-starter-0.0.26/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/large_models.py` & `ml-starter-0.0.26/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/logging.py` & `ml-starter-0.0.26/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/meter.py` & `ml-starter-0.0.26/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/staging.py` & `ml-starter-0.0.26/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/timer.py` & `ml-starter-0.0.26/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/torch_distributed.py` & `ml-starter-0.0.26/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml/utils/video.py` & `ml-starter-0.0.26/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.26/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.25
+Version: 0.0.26
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.25/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.26/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/pyproject.toml` & `ml-starter-0.0.26/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.25/setup.py` & `ml-starter-0.0.26/setup.py`

 * *Files identical despite different names*

