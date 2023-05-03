# Comparing `tmp/rl_algo_impls-0.0.5.tar.gz` & `tmp/rl_algo_impls-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rl_algo_impls-0.0.5.tar", last modified: Sat Mar 18 04:37:06 2023, max compression
+gzip compressed data, was "rl_algo_impls-0.0.8.tar", last modified: Mon Apr  3 16:46:30 2023, max compression
```

## Comparing `rl_algo_impls-0.0.5.tar` & `rl_algo_impls-0.0.8.tar`

### file list

```diff
@@ -1,108 +1,134 @@
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.808269 rl_algo_impls-0.0.5/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2011 2023-02-01 01:37:55.000000 rl_algo_impls-0.0.5/.gitignore
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1073 2023-01-12 22:15:55.000000 rl_algo_impls-0.0.5/LICENSE
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     8275 2023-03-18 04:37:06.808014 rl_algo_impls-0.0.5/PKG-INFO
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     6400 2023-03-16 21:41:41.000000 rl_algo_impls-0.0.5/README.md
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      114 2023-03-16 16:20:34.000000 rl_algo_impls-0.0.5/benchmark_publish.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.797916 rl_algo_impls-0.0.5/colab/
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      205 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.5/colab/colab_atari1.sh
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      211 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.5/colab/colab_atari2.sh
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      242 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.5/colab/colab_basic.sh
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     5362 2023-03-16 17:21:31.000000 rl_algo_impls-0.0.5/colab/colab_benchmark.ipynb
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      176 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.5/colab/colab_carracing.sh
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     4692 2023-03-16 17:21:31.000000 rl_algo_impls-0.0.5/colab/colab_enjoy.ipynb
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      243 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.5/colab/colab_pybullet.sh
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     4721 2023-03-16 17:21:31.000000 rl_algo_impls-0.0.5/colab/colab_train.ipynb
--rw-r--r--   0 sgoodfriend   (501) staff       (20)       99 2023-03-16 16:20:05.000000 rl_algo_impls-0.0.5/compare_runs.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1062 2023-03-02 18:13:38.000000 rl_algo_impls-0.0.5/enjoy.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      171 2023-03-15 22:55:00.000000 rl_algo_impls-0.0.5/environment.yml
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      120 2023-03-16 16:30:54.000000 rl_algo_impls-0.0.5/huggingface_publish.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)       87 2023-03-16 16:31:46.000000 rl_algo_impls-0.0.5/optimize.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1458 2023-03-18 04:35:13.000000 rl_algo_impls-0.0.5/pyproject.toml
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.798563 rl_algo_impls-0.0.5/rl_algo_impls/
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.799421 rl_algo_impls-0.0.5/rl_algo_impls/a2c/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     7586 2023-03-16 00:57:44.000000 rl_algo_impls-0.0.5/rl_algo_impls/a2c/a2c.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2900 2023-03-16 00:51:09.000000 rl_algo_impls-0.0.5/rl_algo_impls/a2c/optimize.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     3365 2023-03-16 16:20:24.000000 rl_algo_impls-0.0.5/rl_algo_impls/benchmark_publish.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     6165 2023-03-16 16:20:13.000000 rl_algo_impls-0.0.5/rl_algo_impls/compare_runs.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.799855 rl_algo_impls-0.0.5/rl_algo_impls/dqn/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     6275 2023-03-16 18:23:23.000000 rl_algo_impls-0.0.5/rl_algo_impls/dqn/dqn.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1674 2023-03-16 18:22:45.000000 rl_algo_impls-0.0.5/rl_algo_impls/dqn/policy.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1382 2023-03-16 00:52:03.000000 rl_algo_impls-0.0.5/rl_algo_impls/dqn/q_net.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     6292 2023-03-16 16:19:56.000000 rl_algo_impls-0.0.5/rl_algo_impls/huggingface_publish.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.800854 rl_algo_impls-0.0.5/rl_algo_impls/hyperparams/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2911 2023-03-16 22:05:21.000000 rl_algo_impls-0.0.5/rl_algo_impls/hyperparams/a2c.yml
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2989 2023-03-02 18:11:44.000000 rl_algo_impls-0.0.5/rl_algo_impls/hyperparams/dqn.yml
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     8909 2023-03-17 21:09:15.000000 rl_algo_impls-0.0.5/rl_algo_impls/hyperparams/ppo.yml
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     4006 2023-03-02 18:11:44.000000 rl_algo_impls-0.0.5/rl_algo_impls/hyperparams/vpg.yml
--rw-r--r--   0 sgoodfriend   (501) staff       (20)    14509 2023-03-18 01:22:13.000000 rl_algo_impls-0.0.5/rl_algo_impls/optimize.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.801092 rl_algo_impls-0.0.5/rl_algo_impls/ppo/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)    12487 2023-03-16 00:52:15.000000 rl_algo_impls-0.0.5/rl_algo_impls/ppo/ppo.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.801210 rl_algo_impls-0.0.5/rl_algo_impls/publish/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     7039 2023-03-16 21:41:55.000000 rl_algo_impls-0.0.5/rl_algo_impls/publish/markdown_format.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.801804 rl_algo_impls-0.0.5/rl_algo_impls/runner/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     5798 2023-03-18 04:34:08.000000 rl_algo_impls-0.0.5/rl_algo_impls/runner/config.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)    10735 2023-03-18 04:34:08.000000 rl_algo_impls-0.0.5/rl_algo_impls/runner/env.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2915 2023-03-16 00:53:14.000000 rl_algo_impls-0.0.5/rl_algo_impls/runner/evaluate.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     5833 2023-03-16 18:00:33.000000 rl_algo_impls-0.0.5/rl_algo_impls/runner/running_utils.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     4619 2023-03-16 00:53:32.000000 rl_algo_impls-0.0.5/rl_algo_impls/runner/train.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.802384 rl_algo_impls-0.0.5/rl_algo_impls/shared/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1011 2023-03-16 00:50:09.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/algorithm.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.802908 rl_algo_impls-0.0.5/rl_algo_impls/shared/callbacks/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      269 2023-03-16 00:53:43.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/callbacks/callback.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     6793 2023-03-16 00:53:51.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/callbacks/eval_callback.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     3371 2023-03-16 00:53:57.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/callbacks/optimize_callback.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2057 2023-03-16 00:54:53.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/gae.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.803195 rl_algo_impls-0.0.5/rl_algo_impls/shared/module/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     6868 2023-03-16 00:54:03.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/module/feature_extractor.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1109 2023-02-15 23:24:59.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/module/module.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.803836 rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)    10334 2023-03-16 00:54:19.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/actor.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      714 2023-03-16 00:54:27.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/critic.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     7500 2023-03-16 16:35:10.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/on_policy.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1069 2023-03-16 00:54:40.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/optimize_on_policy.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     4115 2023-03-16 00:54:45.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/policy.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      852 2023-03-02 18:11:44.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/schedule.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     4553 2023-03-02 18:11:44.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/stats.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2461 2023-03-16 00:55:00.000000 rl_algo_impls-0.0.5/rl_algo_impls/shared/trajectory.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2076 2023-03-18 01:22:13.000000 rl_algo_impls-0.0.5/rl_algo_impls/train.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.803981 rl_algo_impls-0.0.5/rl_algo_impls/tuning/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1351 2023-03-16 00:55:25.000000 rl_algo_impls-0.0.5/rl_algo_impls/tuning/optimize_env.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.804249 rl_algo_impls-0.0.5/rl_algo_impls/vpg/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     4200 2023-03-16 00:55:38.000000 rl_algo_impls-0.0.5/rl_algo_impls/vpg/policy.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     6135 2023-03-16 00:55:44.000000 rl_algo_impls-0.0.5/rl_algo_impls/vpg/vpg.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.806193 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     3048 2023-03-16 00:55:50.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/atari_wrappers.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2600 2023-03-16 00:55:54.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/episode_record_video.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2518 2023-03-16 00:55:59.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/episode_stats_writer.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      964 2023-03-16 00:56:04.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/initial_step_truncate_wrapper.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      322 2023-03-16 00:56:08.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/is_vector_env.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2024 2023-03-16 00:56:12.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/no_reward_timeout.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      326 2023-03-16 00:56:16.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/noop_env_seed.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     4058 2023-03-16 00:56:20.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/normalize.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1015 2023-03-16 00:56:24.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/sync_vector_env_render_compat.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1223 2023-02-15 23:24:59.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/transpose_image_observation.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1795 2023-03-16 00:56:32.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/vec_episode_recorder.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     1473 2023-03-17 21:44:18.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/vectorable_wrapper.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      461 2023-03-16 00:56:41.000000 rl_algo_impls-0.0.5/rl_algo_impls/wrappers/video_compat_wrapper.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.799171 rl_algo_impls-0.0.5/rl_algo_impls.egg-info/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     8275 2023-03-18 04:37:06.000000 rl_algo_impls-0.0.5/rl_algo_impls.egg-info/PKG-INFO
--rw-r--r--   0 sgoodfriend   (501) staff       (20)     2672 2023-03-18 04:37:06.000000 rl_algo_impls-0.0.5/rl_algo_impls.egg-info/SOURCES.txt
--rw-r--r--   0 sgoodfriend   (501) staff       (20)        1 2023-03-18 04:37:06.000000 rl_algo_impls-0.0.5/rl_algo_impls.egg-info/dependency_links.txt
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      426 2023-03-18 04:37:06.000000 rl_algo_impls-0.0.5/rl_algo_impls.egg-info/requires.txt
--rw-r--r--   0 sgoodfriend   (501) staff       (20)       14 2023-03-18 04:37:06.000000 rl_algo_impls-0.0.5/rl_algo_impls.egg-info/top_level.txt
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.807355 rl_algo_impls-0.0.5/scripts/
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)     1542 2023-03-18 04:34:04.000000 rl_algo_impls-0.0.5/scripts/benchmark.sh
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      266 2023-03-17 19:38:04.000000 rl_algo_impls-0.0.5/scripts/setup.sh
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)       63 2023-03-17 20:09:24.000000 rl_algo_impls-0.0.5/scripts/tags_benchmark.sh
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      543 2023-03-17 20:12:02.000000 rl_algo_impls-0.0.5/scripts/train_loop.sh
--rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      922 2023-03-14 18:58:37.000000 rl_algo_impls-0.0.5/scripts/tuning.sh
--rw-r--r--   0 sgoodfriend   (501) staff       (20)       38 2023-03-18 04:37:06.808310 rl_algo_impls-0.0.5/setup.cfg
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.807465 rl_algo_impls-0.0.5/tests/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)        0 2023-03-14 23:36:57.000000 rl_algo_impls-0.0.5/tests/__init__.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.807557 rl_algo_impls-0.0.5/tests/shared/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)        0 2023-03-14 23:36:51.000000 rl_algo_impls-0.0.5/tests/shared/__init__.py
-drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-03-18 04:37:06.807740 rl_algo_impls-0.0.5/tests/shared/policy/
--rw-r--r--   0 sgoodfriend   (501) staff       (20)        0 2023-03-14 23:36:12.000000 rl_algo_impls-0.0.5/tests/shared/policy/__init__.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)      652 2023-03-16 16:37:41.000000 rl_algo_impls-0.0.5/tests/shared/policy/test_on_policy.py
--rw-r--r--   0 sgoodfriend   (501) staff       (20)       78 2023-03-16 00:41:26.000000 rl_algo_impls-0.0.5/train.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.356845 rl_algo_impls-0.0.8/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2011 2023-02-01 01:37:55.000000 rl_algo_impls-0.0.8/.gitignore
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1073 2023-01-12 22:15:55.000000 rl_algo_impls-0.0.8/LICENSE
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     8912 2023-04-03 16:46:30.356649 rl_algo_impls-0.0.8/PKG-INFO
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     6939 2023-03-31 18:33:23.000000 rl_algo_impls-0.0.8/README.md
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      114 2023-03-16 16:20:34.000000 rl_algo_impls-0.0.8/benchmark_publish.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.343292 rl_algo_impls-0.0.8/colab/
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      205 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.8/colab/colab_atari1.sh
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      211 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.8/colab/colab_atari2.sh
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      242 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.8/colab/colab_basic.sh
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     5362 2023-03-16 17:21:31.000000 rl_algo_impls-0.0.8/colab/colab_benchmark.ipynb
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      176 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.8/colab/colab_carracing.sh
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     4692 2023-03-16 17:21:31.000000 rl_algo_impls-0.0.8/colab/colab_enjoy.ipynb
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      243 2023-03-16 17:19:59.000000 rl_algo_impls-0.0.8/colab/colab_pybullet.sh
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     4721 2023-03-16 17:21:31.000000 rl_algo_impls-0.0.8/colab/colab_train.ipynb
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)       99 2023-03-16 16:20:05.000000 rl_algo_impls-0.0.8/compare_runs.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)       78 2023-03-22 17:38:39.000000 rl_algo_impls-0.0.8/enjoy.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      171 2023-03-15 22:55:00.000000 rl_algo_impls-0.0.8/environment.yml
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      120 2023-03-16 16:30:54.000000 rl_algo_impls-0.0.8/huggingface_publish.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)       87 2023-03-16 16:31:46.000000 rl_algo_impls-0.0.8/optimize.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1874 2023-03-31 18:56:15.000000 rl_algo_impls-0.0.8/pyproject.toml
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.344107 rl_algo_impls-0.0.8/rl_algo_impls/
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.344915 rl_algo_impls-0.0.8/rl_algo_impls/a2c/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     7156 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/a2c/a2c.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2904 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/a2c/optimize.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3365 2023-03-22 17:44:05.000000 rl_algo_impls-0.0.8/rl_algo_impls/benchmark_publish.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     6167 2023-03-22 17:44:05.000000 rl_algo_impls-0.0.8/rl_algo_impls/compare_runs.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.345259 rl_algo_impls-0.0.8/rl_algo_impls/dqn/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     6275 2023-03-16 18:23:23.000000 rl_algo_impls-0.0.8/rl_algo_impls/dqn/dqn.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1880 2023-03-31 00:36:41.000000 rl_algo_impls-0.0.8/rl_algo_impls/dqn/policy.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1347 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/dqn/q_net.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1172 2023-03-22 17:38:39.000000 rl_algo_impls-0.0.8/rl_algo_impls/enjoy.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     6315 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/huggingface_publish.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.346235 rl_algo_impls-0.0.8/rl_algo_impls/hyperparams/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3108 2023-03-31 00:44:34.000000 rl_algo_impls-0.0.8/rl_algo_impls/hyperparams/a2c.yml
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2989 2023-03-31 00:36:41.000000 rl_algo_impls-0.0.8/rl_algo_impls/hyperparams/dqn.yml
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)    12424 2023-04-03 16:45:30.000000 rl_algo_impls-0.0.8/rl_algo_impls/hyperparams/ppo.yml
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     4006 2023-03-31 00:36:41.000000 rl_algo_impls-0.0.8/rl_algo_impls/hyperparams/vpg.yml
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)    14499 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/optimize.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.346537 rl_algo_impls-0.0.8/rl_algo_impls/ppo/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)    14703 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/ppo/ppo.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.346683 rl_algo_impls-0.0.8/rl_algo_impls/publish/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     7059 2023-03-22 17:38:51.000000 rl_algo_impls-0.0.8/rl_algo_impls/publish/markdown_format.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.347181 rl_algo_impls-0.0.8/rl_algo_impls/runner/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     6065 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/runner/config.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2912 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/runner/evaluate.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     6661 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/runner/running_utils.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     4678 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/runner/train.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.347854 rl_algo_impls-0.0.8/rl_algo_impls/shared/
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.349171 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      123 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/__init__.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1067 2023-03-31 00:36:41.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/actor.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1897 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/categorical.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1816 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/gaussian.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3811 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/gridnet.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2713 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/gridnet_decoder.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3674 2023-03-31 00:36:41.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/make_actor.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3444 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/multi_discrete.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     6782 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/actor/state_dependent_noise.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1011 2023-03-16 00:50:09.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/algorithm.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.349574 rl_algo_impls-0.0.8/rl_algo_impls/shared/callbacks/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      269 2023-03-16 00:53:43.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/callbacks/callback.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     7613 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/callbacks/eval_callback.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3371 2023-03-16 00:53:57.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/callbacks/optimize_callback.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.350439 rl_algo_impls-0.0.8/rl_algo_impls/shared/encoder/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      116 2023-03-31 00:36:41.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/encoder/__init__.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1919 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/encoder/cnn.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2837 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/encoder/encoder.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2075 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/encoder/gridnet_encoder.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2725 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/encoder/impala_cnn.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1265 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/encoder/microrts_cnn.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1562 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/encoder/nature_cnn.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3008 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/gae.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.350565 rl_algo_impls-0.0.8/rl_algo_impls/shared/module/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1208 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/module/module.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.351014 rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1129 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/critic.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     8215 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/on_policy.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1069 2023-03-16 00:54:40.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/optimize_on_policy.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     4197 2023-03-23 00:36:09.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/policy.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1651 2023-03-22 17:44:05.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/schedule.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     5401 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/stats.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2461 2023-03-16 00:55:00.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/trajectory.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.351825 rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)       74 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/__init__.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2064 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/make_env.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3103 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/microrts.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1743 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/microrts_compat.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2526 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/procgen.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      678 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/utils.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     7662 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/vec_env.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2114 2023-04-03 16:45:30.000000 rl_algo_impls-0.0.8/rl_algo_impls/train.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.351951 rl_algo_impls-0.0.8/rl_algo_impls/tuning/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1351 2023-03-16 00:55:25.000000 rl_algo_impls-0.0.8/rl_algo_impls/tuning/optimize_env.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.352182 rl_algo_impls-0.0.8/rl_algo_impls/vpg/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     4712 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/rl_algo_impls/vpg/policy.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     5838 2023-03-23 00:36:09.000000 rl_algo_impls-0.0.8/rl_algo_impls/vpg/vpg.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.354210 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1289 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/action_mask_wrapper.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3048 2023-03-16 00:55:50.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/atari_wrappers.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2600 2023-03-16 00:55:54.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/episode_record_video.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2825 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/episode_stats_writer.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1217 2023-03-22 17:44:05.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/hwc_to_chw_observation.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      964 2023-03-16 00:56:04.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/initial_step_truncate_wrapper.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      322 2023-03-27 19:45:55.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/is_vector_env.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1274 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/microrts_stats_recorder.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     2024 2023-03-16 00:56:12.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/no_reward_timeout.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      326 2023-03-16 00:56:16.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/noop_env_seed.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     4058 2023-03-16 00:56:20.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/normalize.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1015 2023-03-16 00:56:24.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/sync_vector_env_render_compat.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1795 2023-03-16 00:56:32.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/vec_episode_recorder.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     1473 2023-03-28 22:38:58.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/vectorable_wrapper.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      461 2023-03-16 00:56:41.000000 rl_algo_impls-0.0.8/rl_algo_impls/wrappers/video_compat_wrapper.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.344687 rl_algo_impls-0.0.8/rl_algo_impls.egg-info/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     8912 2023-04-03 16:46:30.000000 rl_algo_impls-0.0.8/rl_algo_impls.egg-info/PKG-INFO
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)     3635 2023-04-03 16:46:30.000000 rl_algo_impls-0.0.8/rl_algo_impls.egg-info/SOURCES.txt
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)        1 2023-04-03 16:46:30.000000 rl_algo_impls-0.0.8/rl_algo_impls.egg-info/dependency_links.txt
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      622 2023-04-03 16:46:30.000000 rl_algo_impls-0.0.8/rl_algo_impls.egg-info/requires.txt
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)       14 2023-04-03 16:46:30.000000 rl_algo_impls-0.0.8/rl_algo_impls.egg-info/top_level.txt
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.355851 rl_algo_impls-0.0.8/scripts/
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)     2492 2023-03-31 18:40:53.000000 rl_algo_impls-0.0.8/scripts/benchmark.sh
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      289 2023-03-31 18:56:23.000000 rl_algo_impls-0.0.8/scripts/setup.sh
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      239 2023-03-31 00:31:47.000000 rl_algo_impls-0.0.8/scripts/tags_benchmark.sh
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      543 2023-03-17 20:12:02.000000 rl_algo_impls-0.0.8/scripts/train_loop.sh
+-rwxr-xr-x   0 sgoodfriend   (501) staff       (20)      922 2023-03-14 18:58:37.000000 rl_algo_impls-0.0.8/scripts/tuning.sh
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)       38 2023-04-03 16:46:30.356881 rl_algo_impls-0.0.8/setup.cfg
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.356089 rl_algo_impls-0.0.8/tests/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)        0 2023-03-14 23:36:57.000000 rl_algo_impls-0.0.8/tests/__init__.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.356184 rl_algo_impls-0.0.8/tests/shared/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)        0 2023-03-14 23:36:51.000000 rl_algo_impls-0.0.8/tests/shared/__init__.py
+drwxr-xr-x   0 sgoodfriend   (501) staff       (20)        0 2023-04-03 16:46:30.356390 rl_algo_impls-0.0.8/tests/shared/policy/
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)        0 2023-03-14 23:36:12.000000 rl_algo_impls-0.0.8/tests/shared/policy/__init__.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)      652 2023-04-03 16:45:31.000000 rl_algo_impls-0.0.8/tests/shared/policy/test_on_policy.py
+-rw-r--r--   0 sgoodfriend   (501) staff       (20)       78 2023-03-31 00:50:27.000000 rl_algo_impls-0.0.8/train.py
```

### Comparing `rl_algo_impls-0.0.5/.gitignore` & `rl_algo_impls-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/LICENSE` & `rl_algo_impls-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/PKG-INFO` & `rl_algo_impls-0.0.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl_algo_impls
-Version: 0.0.5
+Version: 0.0.8
 Summary: Implementations of reinforcement learning algorithms
 Author-email: Scott Goodfriend <goodfriend.scott@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Scott Goodfriend
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,21 +31,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: procgen
+Provides-Extra: microrts-old
+Provides-Extra: microrts
+Provides-Extra: jupyter
+Provides-Extra: all
 License-File: LICENSE
 
 # rl-algo-impls
 
 Implementations of reinforcement learning algorithms.
 
-Latest WandB report: https://api.wandb.ai/links/sgoodfriend/6p2sjqtn
+- [WandB benchmark reports](https://wandb.ai/sgoodfriend/rl-algo-impls-benchmarks/reportlist)
+  - [Basic, PyBullet, and Atari games
+    (v0.0.4)](https://api.wandb.ai/links/sgoodfriend/09frjfcs)
+  - [procgen
+    (starpilot, hard)](https://api.wandb.ai/links/sgoodfriend/v1p4976e) and [procgen (easy)](https://api.wandb.ai/links/sgoodfriend/f3w1hwyb)
+  - [Gridnet MicroRTS](https://api.wandb.ai/links/sgoodfriend/zdee7ovm)
+- [Huggingface models](https://huggingface.co/models?other=rl-algo-impls)
 
 ## Prerequisites: Weights & Biases (WandB)
 
 Training and benchmarking assumes you have a Weights & Biases project to upload runs to.
 By default training goes to a rl-algo-impls project while benchmarks go to
 rl-algo-impls-benchmarks. During training and benchmarking runs, videos of the best
 models and the model weights are uploaded to WandB.
@@ -201,7 +211,15 @@
 pip install -e .
 python -c "from procgen import ProcgenGym3Env; ProcgenGym3Env(num=1, env_name='coinrun')"
 python -m procgen.interactive
 ```
 
 amd64 Linux machines (e.g., Lambda Labs and Google Colab) should install procgen with
 `python -m pip install '.[procgen]'`
+
+## gym-microrts Setup
+
+```
+python -m pip install -e '.[microrts]'
+```
+
+Requires Java SDK to also be installed.
```

### Comparing `rl_algo_impls-0.0.5/README.md` & `rl_algo_impls-0.0.8/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # rl-algo-impls
 
 Implementations of reinforcement learning algorithms.
 
-Latest WandB report: https://api.wandb.ai/links/sgoodfriend/6p2sjqtn
+- [WandB benchmark reports](https://wandb.ai/sgoodfriend/rl-algo-impls-benchmarks/reportlist)
+  - [Basic, PyBullet, and Atari games
+    (v0.0.4)](https://api.wandb.ai/links/sgoodfriend/09frjfcs)
+  - [procgen
+    (starpilot, hard)](https://api.wandb.ai/links/sgoodfriend/v1p4976e) and [procgen (easy)](https://api.wandb.ai/links/sgoodfriend/f3w1hwyb)
+  - [Gridnet MicroRTS](https://api.wandb.ai/links/sgoodfriend/zdee7ovm)
+- [Huggingface models](https://huggingface.co/models?other=rl-algo-impls)
 
 ## Prerequisites: Weights & Biases (WandB)
 
 Training and benchmarking assumes you have a Weights & Biases project to upload runs to.
 By default training goes to a rl-algo-impls project while benchmarks go to
 rl-algo-impls-benchmarks. During training and benchmarking runs, videos of the best
 models and the model weights are uploaded to WandB.
@@ -162,7 +168,15 @@
 pip install -e .
 python -c "from procgen import ProcgenGym3Env; ProcgenGym3Env(num=1, env_name='coinrun')"
 python -m procgen.interactive
 ```
 
 amd64 Linux machines (e.g., Lambda Labs and Google Colab) should install procgen with
 `python -m pip install '.[procgen]'`
+
+## gym-microrts Setup
+
+```
+python -m pip install -e '.[microrts]'
+```
+
+Requires Java SDK to also be installed.
```

### Comparing `rl_algo_impls-0.0.5/colab/colab_benchmark.ipynb` & `rl_algo_impls-0.0.8/colab/colab_benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/colab/colab_enjoy.ipynb` & `rl_algo_impls-0.0.8/colab/colab_enjoy.ipynb`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/colab/colab_train.ipynb` & `rl_algo_impls-0.0.8/colab/colab_train.ipynb`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/enjoy.py` & `rl_algo_impls-0.0.8/rl_algo_impls/enjoy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 # Support for PyTorch mps mode (https://pytorch.org/docs/stable/notes/mps.html)
 import os
 
 os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 
-from runner.evaluate import EvalArgs, evaluate_model
-from runner.running_utils import base_parser
+from rl_algo_impls.runner.evaluate import EvalArgs, evaluate_model
+from rl_algo_impls.runner.running_utils import base_parser
 
 
-if __name__ == "__main__":
+def enjoy() -> None:
     parser = base_parser(multiple=False)
     parser.add_argument("--render", default=True, type=bool)
     parser.add_argument("--best", default=True, type=bool)
     parser.add_argument("--n_envs", default=1, type=int)
     parser.add_argument("--n_episodes", default=3, type=int)
     parser.add_argument("--deterministic-eval", default=None, type=bool)
     parser.add_argument(
         "--no-print-returns", action="store_true", help="Limit printing"
     )
     # wandb-run-path overrides base RunArgs
     parser.add_argument("--wandb-run-path", default=None, type=str)
     parser.set_defaults(
         algo=["ppo"],
+        wandb_run_path="sgoodfriend/rl-algo-impls/m5c1t7g5",
     )
     args = parser.parse_args()
     args.algo = args.algo[0]
     args.env = args.env[0]
     args = EvalArgs(**vars(args))
 
-    evaluate_model(args, os.path.dirname(__file__))
+    evaluate_model(args, os.getcwd())
+
+
+if __name__ == "__main__":
+    enjoy()
```

### Comparing `rl_algo_impls-0.0.5/pyproject.toml` & `rl_algo_impls-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rl_algo_impls"
-version = "0.0.5"
+version = "0.0.8"
 description = "Implementations of reinforcement learning algorithms"
 authors = [
     {name = "Scott Goodfriend", email = "goodfriend.scott@gmail.com"},
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">= 3.8"
@@ -52,14 +52,34 @@
 ]
 procgen = [
     "numexpr >= 2.8.4",
     "gym3",
     "glfw >= 1.12.0, < 1.13",
     "procgen; platform_machine=='x86_64'",
 ]
+microrts-old = [
+    "numpy < 1.24.0", # Support for gym-microrts < 0.6.0
+    "gym-microrts == 0.2.0", # Match ppo-implementation-details
+]
+microrts = [
+    "numpy < 1.24.0", # Support for gym-microrts < 0.6.0
+    "gym-microrts == 0.3.2",
+]
+jupyter = [
+    "jupyter",
+    "notebook"
+]
+all = [
+    "rl-algo-impls[test]",
+    "rl-algo-impls[procgen]",
+    "rl-algo-impls[microrts]",
+]
 
 [project.urls]
 "Homepage" = "https://github.com/sgoodfriend/rl-algo-impls"
 
 [build-system]
 requires = ["setuptools==65.5.0", "setuptools-scm"]
-build-backend = "setuptools.build_meta"
+build-backend = "setuptools.build_meta"
+
+[tool.isort]
+profile = "black"
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/a2c/a2c.py` & `rl_algo_impls-0.0.8/rl_algo_impls/a2c/a2c.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from time import perf_counter
 from torch.utils.tensorboard.writer import SummaryWriter
 from typing import Optional, TypeVar
 
 from rl_algo_impls.shared.algorithm import Algorithm
 from rl_algo_impls.shared.callbacks.callback import Callback
+from rl_algo_impls.shared.gae import compute_advantages
 from rl_algo_impls.shared.policy.on_policy import ActorCritic
 from rl_algo_impls.shared.schedule import schedule, update_learning_rate
 from rl_algo_impls.shared.stats import log_scalars
 from rl_algo_impls.wrappers.vectorable_wrapper import (
     VecEnv,
     single_observation_space,
     single_action_space,
@@ -80,20 +81,20 @@
         step_dim = (self.env.num_envs,)
         obs_space = single_observation_space(self.env)
         act_space = single_action_space(self.env)
 
         obs = np.zeros(epoch_dim + obs_space.shape, dtype=obs_space.dtype)
         actions = np.zeros(epoch_dim + act_space.shape, dtype=act_space.dtype)
         rewards = np.zeros(epoch_dim, dtype=np.float32)
-        episode_starts = np.zeros(epoch_dim, dtype=np.byte)
+        episode_starts = np.zeros(epoch_dim, dtype=np.bool8)
         values = np.zeros(epoch_dim, dtype=np.float32)
         logprobs = np.zeros(epoch_dim, dtype=np.float32)
 
         next_obs = self.env.reset()
-        next_episode_starts = np.ones(step_dim, dtype=np.byte)
+        next_episode_starts = np.full(step_dim, True, dtype=np.bool8)
 
         timesteps_elapsed = start_timesteps
         while timesteps_elapsed < start_timesteps + train_timesteps:
             start_time = perf_counter()
 
             progress = timesteps_elapsed / total_timesteps
             ent_coef = self.ent_coef_schedule(progress)
@@ -122,31 +123,24 @@
                 actions[s], values[s], logprobs[s], clamped_action = self.policy.step(
                     next_obs
                 )
                 next_obs, rewards[s], next_episode_starts, _ = self.env.step(
                     clamped_action
                 )
 
-            advantages = np.zeros(epoch_dim, dtype=np.float32)
-            last_gae_lam = 0
-            for t in reversed(range(self.n_steps)):
-                if t == self.n_steps - 1:
-                    next_nonterminal = 1.0 - next_episode_starts
-                    next_value = self.policy.value(next_obs)
-                else:
-                    next_nonterminal = 1.0 - episode_starts[t + 1]
-                    next_value = values[t + 1]
-                delta = (
-                    rewards[t] + self.gamma * next_value * next_nonterminal - values[t]
-                )
-                last_gae_lam = (
-                    delta
-                    + self.gamma * self.gae_lambda * next_nonterminal * last_gae_lam
-                )
-                advantages[t] = last_gae_lam
+            advantages = compute_advantages(
+                rewards,
+                values,
+                episode_starts,
+                next_episode_starts,
+                next_obs,
+                self.policy,
+                self.gamma,
+                self.gae_lambda,
+            )
             returns = advantages + values
 
             b_obs = torch.tensor(obs.reshape((-1,) + obs_space.shape)).to(self.device)
             b_actions = torch.tensor(actions.reshape((-1,) + act_space.shape)).to(
                 self.device
             )
             b_advantages = torch.tensor(advantages.reshape(-1)).to(self.device)
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/a2c/optimize.py` & `rl_algo_impls-0.0.8/rl_algo_impls/a2c/optimize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import optuna
 
 from copy import deepcopy
 
 from rl_algo_impls.runner.config import Config, Hyperparams, EnvHyperparams
-from rl_algo_impls.runner.env import make_eval_env
+from rl_algo_impls.shared.vec_env import make_eval_env
 from rl_algo_impls.shared.policy.optimize_on_policy import sample_on_policy_hyperparams
 from rl_algo_impls.tuning.optimize_env import sample_env_hyperparams
 
 
 def sample_params(
     trial: optuna.Trial,
     base_hyperparams: Hyperparams,
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/benchmark_publish.py` & `rl_algo_impls-0.0.8/rl_algo_impls/benchmark_publish.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/compare_runs.py` & `rl_algo_impls-0.0.8/rl_algo_impls/compare_runs.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,9 +190,10 @@
             )
         runs_by_run_group[rg].add_run(r)
     df = RunGroupRuns.data_frame(runs_by_run_group.values()).round(decimals=2)
     print(f"**Total Score: {sum(df.score)}**")
     df.loc["mean"] = df.mean(numeric_only=True)
     print(df.to_markdown())
 
+
 if __name__ == "__main__":
-    compare_runs()
+    compare_runs()
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/dqn/dqn.py` & `rl_algo_impls-0.0.8/rl_algo_impls/dqn/dqn.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/dqn/policy.py` & `rl_algo_impls-0.0.8/rl_algo_impls/dqn/policy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,58 @@
-import numpy as np
 import os
-import torch
-
 from typing import Optional, Sequence, TypeVar
 
+import numpy as np
+import torch
+
 from rl_algo_impls.dqn.q_net import QNetwork
 from rl_algo_impls.shared.policy.policy import Policy
 from rl_algo_impls.wrappers.vectorable_wrapper import (
     VecEnv,
     VecEnvObs,
-    single_observation_space,
     single_action_space,
+    single_observation_space,
 )
 
 DQNPolicySelf = TypeVar("DQNPolicySelf", bound="DQNPolicy")
 
 
 class DQNPolicy(Policy):
     def __init__(
         self,
         env: VecEnv,
         hidden_sizes: Sequence[int] = [],
-        cnn_feature_dim: int = 512,
+        cnn_flatten_dim: int = 512,
         cnn_style: str = "nature",
         cnn_layers_init_orthogonal: Optional[bool] = None,
         impala_channels: Sequence[int] = (16, 32, 32),
         **kwargs,
     ) -> None:
         super().__init__(env, **kwargs)
         self.q_net = QNetwork(
             single_observation_space(env),
             single_action_space(env),
             hidden_sizes,
-            cnn_feature_dim=cnn_feature_dim,
+            cnn_flatten_dim=cnn_flatten_dim,
             cnn_style=cnn_style,
             cnn_layers_init_orthogonal=cnn_layers_init_orthogonal,
             impala_channels=impala_channels,
         )
 
     def act(
-        self, obs: VecEnvObs, eps: float = 0, deterministic: bool = True
+        self,
+        obs: VecEnvObs,
+        eps: float = 0,
+        deterministic: bool = True,
+        action_masks: Optional[np.ndarray] = None,
     ) -> np.ndarray:
         assert eps == 0 if deterministic else eps >= 0
+        assert (
+            action_masks is None
+        ), f"action_masks not currently supported in {self.__class__.__name__}"
         if not deterministic and np.random.random() < eps:
             return np.array(
                 [
                     single_action_space(self.env).sample()
                     for _ in range(self.env.num_envs)
                 ]
             )
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/huggingface_publish.py` & `rl_algo_impls-0.0.8/rl_algo_impls/huggingface_publish.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from huggingface_hub.hf_api import HfApi, upload_folder
 from huggingface_hub.repocard import metadata_save
 from pyvirtualdisplay.display import Display
 
 from rl_algo_impls.publish.markdown_format import EvalTableData, model_card_text
 from rl_algo_impls.runner.config import EnvHyperparams
 from rl_algo_impls.runner.evaluate import EvalArgs, evaluate_model
-from rl_algo_impls.runner.env import make_eval_env
+from rl_algo_impls.shared.vec_env import make_eval_env
 from rl_algo_impls.shared.callbacks.eval_callback import evaluate
 from rl_algo_impls.wrappers.vec_episode_recorder import VecEpisodeRecorder
 
 
 def publish(
     wandb_run_paths: List[str],
     wandb_report_url: str,
@@ -48,15 +48,15 @@
                 render=False,
                 best=True,
                 n_envs=None,
                 n_episodes=10,
                 no_print_returns=True,
                 wandb_run_path="/".join(r.path),
             ),
-            os.path.dirname(__file__),
+            os.getcwd(),
         )
         for r in runs
     ]
     run_metadata = requests.get(runs[0].file("wandb-metadata.json").url).json()
     table_data = list(EvalTableData(r, e) for r, e in zip(runs, evaluations))
     best_eval = sorted(
         table_data, key=lambda d: d.evaluation.stats.score, reverse=True
@@ -158,14 +158,15 @@
         )
         repo_url = upload_folder(
             repo_id=huggingface_repo,
             folder_path=repo_dir_path,
             path_in_repo="",
             commit_message=f"{algo.upper()} playing {env_id} from {github_url}/tree/{commit_hash}",
             token=huggingface_token,
+            delete_patterns="*",
         )
         print(f"Pushed model to the hub: {repo_url}")
 
 
 def huggingface_publish():
     parser = argparse.ArgumentParser()
     parser.add_argument(
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/hyperparams/a2c.yml` & `rl_algo_impls-0.0.8/rl_algo_impls/hyperparams/a2c.yml`

 * *Files 4% similar despite different names*

```diff
@@ -93,39 +93,43 @@
 
 Walker2DBulletEnv-v0:
   <<: *pybullet-defaults
 
 HopperBulletEnv-v0:
   <<: *pybullet-defaults
 
+# Tuned
 CarRacing-v0:
   n_timesteps: !!float 4e6
   env_hyperparams:
-    n_envs: 8
+    n_envs: 16
     frame_stack: 4
     normalize: true
     normalize_kwargs:
       norm_obs: false
       norm_reward: true
   policy_hyperparams:
-    use_sde: true
-    log_std_init: -2
-    init_layers_orthogonal: false
-    activation_fn: relu
+    use_sde: false
+    log_std_init: -1.3502584927786276
+    init_layers_orthogonal: true
+    activation_fn: tanh
     share_features_extractor: false
-    cnn_feature_dim: 256
+    cnn_flatten_dim: 256
     hidden_sizes: [256]
   algo_hyperparams:
-    n_steps: 512
-    learning_rate: !!float 1.62e-5
-    gamma: 0.997
-    gae_lambda: 0.975
-    ent_coef: 0
-    sde_sample_freq: 128
-    vf_coef: 0.64
+    n_steps: 16
+    learning_rate: 0.000025630993245026736
+    learning_rate_decay: linear
+    gamma: 0.99957617037542
+    gae_lambda: 0.949455676599436
+    ent_coef: !!float 1.707983205298309e-7
+    vf_coef: 0.10428178193833336
+    max_grad_norm: 0.5406643389792273
+    normalize_advantage: true
+    use_rms_prop: false
 
 _atari: &atari-defaults
   n_timesteps: !!float 1e7
   env_hyperparams: &atari-env-defaults
     n_envs: 16
     frame_stack: 4
     no_reward_timeout_steps: 1000
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/hyperparams/dqn.yml` & `rl_algo_impls-0.0.8/rl_algo_impls/hyperparams/dqn.yml`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
   <<: *atari-defaults
   n_timesteps: !!float 2.5e6
 
 _impala-atari: &impala-atari-defaults
   <<: *atari-defaults
   policy_hyperparams:
     cnn_style: impala
-    cnn_feature_dim: 256
+    cnn_flatten_dim: 256
     init_layers_orthogonal: true
     cnn_layers_init_orthogonal: false
 
 impala-PongNoFrameskip-v4:
   <<: *impala-atari-defaults
   env_id: PongNoFrameskip-v4
   n_timesteps: !!float 2.5e6
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/hyperparams/vpg.yml` & `rl_algo_impls-0.0.8/rl_algo_impls/hyperparams/vpg.yml`

 * *Files 4% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     n_envs: 4
     vec_env_class: sync
   policy_hyperparams:
     use_sde: true
     log_std_init: -2
     init_layers_orthogonal: false
     activation_fn: relu
-    cnn_feature_dim: 256
+    cnn_flatten_dim: 256
     hidden_sizes: [256]
   algo_hyperparams:
     n_steps: 1000
     pi_lr: !!float 5e-5
     gamma: 0.99
     gae_lambda: 0.95
     val_lr: !!float 1e-4
@@ -171,25 +171,25 @@
     max_grad_norm: 0.5
   eval_params:
     step_freq: !!float 5e4
     n_episodes: 10
     save_best: true
 
 _atari: &atari-defaults
-  n_timesteps: !!float 25e6
+  n_timesteps: !!float 10e6
   env_hyperparams:
-    n_envs: 4
+    n_envs: 2
     frame_stack: 4
     no_reward_timeout_steps: 1000
     no_reward_fire_steps: 500
     vec_env_class: async
   policy_hyperparams:
     activation_fn: relu
   algo_hyperparams:
-    n_steps: 2048
+    n_steps: 3072
     pi_lr: !!float 5e-5
     gamma: 0.99
     gae_lambda: 0.95
     val_lr: !!float 1e-4
     train_v_iters: 80
     max_grad_norm: 0.5
     ent_coef: 0.01
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/optimize.py` & `rl_algo_impls-0.0.8/rl_algo_impls/optimize.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from optuna.samplers import TPESampler
 from optuna.visualization import plot_optimization_history, plot_param_importances
 from torch.utils.tensorboard.writer import SummaryWriter
 from typing import Callable, List, NamedTuple, Optional, Sequence, Union
 
 from rl_algo_impls.a2c.optimize import sample_params as a2c_sample_params
 from rl_algo_impls.runner.config import Config, EnvHyperparams, RunArgs
-from rl_algo_impls.runner.env import make_env, make_eval_env
+from rl_algo_impls.shared.vec_env import make_env, make_eval_env
 from rl_algo_impls.runner.running_utils import (
     base_parser,
     load_hyperparams,
     set_seeds,
     get_device,
     make_policy,
     ALGOS,
@@ -190,15 +190,15 @@
 
     tb_writer = SummaryWriter(config.tensorboard_summary_path)
     set_seeds(args.seed, args.use_deterministic_algorithms)
 
     env = make_env(
         config, EnvHyperparams(**config.env_hyperparams), tb_writer=tb_writer
     )
-    device = get_device(config.device, env)
+    device = get_device(config, env)
     policy = make_policy(args.algo, env, device, **config.policy_hyperparams)
     algo = ALGOS[args.algo](policy, env, device, tb_writer, **config.algo_hyperparams)
 
     eval_env = make_eval_env(
         config,
         EnvHyperparams(**config.env_hyperparams),
         override_n_envs=study_args.n_eval_envs,
@@ -294,15 +294,15 @@
 
             env = make_env(
                 config,
                 EnvHyperparams(**config.env_hyperparams),
                 normalize_load_path=config.model_dir_path() if i > 0 else None,
                 tb_writer=tb_writer,
             )
-            device = get_device(config.device, env)
+            device = get_device(config, env)
             policy = make_policy(arg.algo, env, device, **config.policy_hyperparams)
             if i > 0:
                 policy.load(config.model_dir_path())
             algo = ALGOS[arg.algo](
                 policy, env, device, tb_writer, **config.algo_hyperparams
             )
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/publish/markdown_format.py` & `rl_algo_impls-0.0.8/rl_algo_impls/publish/markdown_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 This and other models from {report_url} were generated by running a script on a Lambda
 Labs instance. In a Lambda Labs instance terminal:
 ```
 git clone git@github.com:sgoodfriend/rl-algo-impls.git
 cd rl-algo-impls
 bash ./lambda_labs/setup.sh
 wandb login
-bash ./lambda_labs/benchmark.sh [-a {"ppo"}] [-e ENVS] [-j {6}] [-p {rl-algo-impls-benchmarks}] [-s {"1 2 3"}]
+bash ./lambda_labs/benchmark.sh [-a {{"ppo a2c dqn vpg"}}] [-e ENVS] [-j {{6}}] [-p {{rl-algo-impls-benchmarks}}] [-s {{"1 2 3"}}]
 ```
 
 ### Alternative: Google Colab Pro+
 As an alternative,
 [colab_benchmark.ipynb](https://github.com/sgoodfriend/rl-algo-impls/tree/main/benchmarks#:~:text=colab_benchmark.ipynb),
 can be used. However, this requires a Google Colab Pro+ subscription and running across
 4 separate instances because otherwise running all jobs will exceed the 24-hour limit.
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/runner/config.py` & `rl_algo_impls-0.0.8/rl_algo_impls/runner/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import dataclasses
 import inspect
 import itertools
 import os
-
-from datetime import datetime
 from dataclasses import dataclass
+from datetime import datetime
 from typing import Any, Dict, List, Optional, Type, TypeVar, Union
 
-
 RunArgsSelf = TypeVar("RunArgsSelf", bound="RunArgs")
 
 
 @dataclass
 class RunArgs:
     algo: str
     env: str
@@ -32,43 +30,46 @@
             _d.update({"algo": algo, "env": env, "seed": seed})
             args.append(cls(**_d))
         return args
 
 
 @dataclass
 class EnvHyperparams:
-    env_type: str = "sb3vec"
+    env_type: str = "gymvec"
     n_envs: int = 1
     frame_stack: int = 1
     make_kwargs: Optional[Dict[str, Any]] = None
     no_reward_timeout_steps: Optional[int] = None
     no_reward_fire_steps: Optional[int] = None
     vec_env_class: str = "sync"
     normalize: bool = False
     normalize_kwargs: Optional[Dict[str, Any]] = None
     rolling_length: int = 100
     train_record_video: bool = False
     video_step_interval: Union[int, float] = 1_000_000
     initial_steps_to_truncate: Optional[int] = None
     clip_atari_rewards: bool = True
-    normalize_type: Optional[str] = "gymlike"
+    normalize_type: Optional[str] = None
+    mask_actions: bool = False
+    bots: Optional[Dict[str, int]] = None
 
 
 HyperparamsSelf = TypeVar("HyperparamsSelf", bound="Hyperparams")
 
 
 @dataclass
 class Hyperparams:
     device: str = "auto"
     n_timesteps: Union[int, float] = 100_000
     env_hyperparams: Dict[str, Any] = dataclasses.field(default_factory=dict)
     policy_hyperparams: Dict[str, Any] = dataclasses.field(default_factory=dict)
     algo_hyperparams: Dict[str, Any] = dataclasses.field(default_factory=dict)
     eval_params: Dict[str, Any] = dataclasses.field(default_factory=dict)
     env_id: Optional[str] = None
+    additional_keys_to_log: List[str] = dataclasses.field(default_factory=list)
 
     @classmethod
     def from_dict_with_extra_fields(
         cls: Type[HyperparamsSelf], d: Dict[str, Any]
     ) -> HyperparamsSelf:
         return cls(
             **{k: v for k, v in d.items() if k in inspect.signature(cls).parameters}
@@ -116,14 +117,18 @@
     def algo(self) -> str:
         return self.args.algo
 
     @property
     def env_id(self) -> str:
         return self.hyperparams.env_id or self.args.env
 
+    @property
+    def additional_keys_to_log(self) -> List[str]:
+        return self.hyperparams.additional_keys_to_log
+
     def model_name(self, include_seed: bool = True) -> str:
         # Use arg env name instead of environment name
         parts = [self.algo, self.args.env]
         if include_seed and self.args.seed is not None:
             parts.append(f"S{self.args.seed}")
 
         # Assume that the custom arg name already has the necessary information
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/runner/env.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/vec_env/vec_env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,57 @@
-import gym
-import numpy as np
 import os
+from dataclasses import astuple
+from typing import Callable, Optional
 
-from dataclasses import asdict, astuple
+import gym
 from gym.vector.async_vector_env import AsyncVectorEnv
 from gym.vector.sync_vector_env import SyncVectorEnv
-from gym.wrappers.resize_observation import ResizeObservation
-from gym.wrappers.gray_scale_observation import GrayScaleObservation
 from gym.wrappers.frame_stack import FrameStack
-from stable_baselines3.common.atari_wrappers import (
-    MaxAndSkipEnv,
-    NoopResetEnv,
-)
+from gym.wrappers.gray_scale_observation import GrayScaleObservation
+from gym.wrappers.resize_observation import ResizeObservation
+from stable_baselines3.common.atari_wrappers import MaxAndSkipEnv, NoopResetEnv
 from stable_baselines3.common.vec_env.dummy_vec_env import DummyVecEnv
 from stable_baselines3.common.vec_env.subproc_vec_env import SubprocVecEnv
 from stable_baselines3.common.vec_env.vec_normalize import VecNormalize
 from torch.utils.tensorboard.writer import SummaryWriter
-from typing import Callable, Optional
 
 from rl_algo_impls.runner.config import Config, EnvHyperparams
 from rl_algo_impls.shared.policy.policy import VEC_NORMALIZE_FILENAME
+from rl_algo_impls.shared.vec_env.utils import (
+    import_for_env_id,
+    is_atari,
+    is_bullet_env,
+    is_car_racing,
+    is_gym_procgen,
+    is_microrts,
+)
+from rl_algo_impls.wrappers.action_mask_wrapper import SingleActionMaskWrapper
 from rl_algo_impls.wrappers.atari_wrappers import (
+    ClipRewardEnv,
     EpisodicLifeEnv,
     FireOnLifeStarttEnv,
-    ClipRewardEnv,
 )
 from rl_algo_impls.wrappers.episode_record_video import EpisodeRecordVideo
 from rl_algo_impls.wrappers.episode_stats_writer import EpisodeStatsWriter
+from rl_algo_impls.wrappers.hwc_to_chw_observation import HwcToChwObservation
 from rl_algo_impls.wrappers.initial_step_truncate_wrapper import (
     InitialStepTruncateWrapper,
 )
 from rl_algo_impls.wrappers.is_vector_env import IsVectorEnv
 from rl_algo_impls.wrappers.no_reward_timeout import NoRewardTimeout
 from rl_algo_impls.wrappers.noop_env_seed import NoopEnvSeed
 from rl_algo_impls.wrappers.normalize import NormalizeObservation, NormalizeReward
 from rl_algo_impls.wrappers.sync_vector_env_render_compat import (
     SyncVectorEnvRenderCompat,
 )
-from rl_algo_impls.wrappers.transpose_image_observation import TransposeImageObservation
 from rl_algo_impls.wrappers.vectorable_wrapper import VecEnv
 from rl_algo_impls.wrappers.video_compat_wrapper import VideoCompatWrapper
 
 
-def make_env(
-    config: Config,
-    hparams: EnvHyperparams,
-    training: bool = True,
-    render: bool = False,
-    normalize_load_path: Optional[str] = None,
-    tb_writer: Optional[SummaryWriter] = None,
-) -> VecEnv:
-    if hparams.env_type == "procgen":
-        return _make_procgen_env(
-            config,
-            hparams,
-            training=training,
-            render=render,
-            normalize_load_path=normalize_load_path,
-            tb_writer=tb_writer,
-        )
-    elif hparams.env_type in {"sb3vec", "gymvec"}:
-        return _make_vec_env(
-            config,
-            hparams,
-            training=training,
-            render=render,
-            normalize_load_path=normalize_load_path,
-            tb_writer=tb_writer,
-        )
-    else:
-        raise ValueError(f"env_type {hparams.env_type} not supported")
-
-
-def make_eval_env(
-    config: Config,
-    hparams: EnvHyperparams,
-    override_n_envs: Optional[int] = None,
-    **kwargs,
-) -> VecEnv:
-    kwargs = kwargs.copy()
-    kwargs["training"] = False
-    if override_n_envs is not None:
-        hparams_kwargs = asdict(hparams)
-        hparams_kwargs["n_envs"] = override_n_envs
-        if override_n_envs == 1:
-            hparams_kwargs["vec_env_class"] = "sync"
-        hparams = EnvHyperparams(**hparams_kwargs)
-    return make_env(config, hparams, **kwargs)
-
-
-def _make_vec_env(
+def make_vec_env(
     config: Config,
     hparams: EnvHyperparams,
     training: bool = True,
     render: bool = False,
     normalize_load_path: Optional[str] = None,
     tb_writer: Optional[SummaryWriter] = None,
 ) -> VecEnv:
@@ -109,30 +67,29 @@
         normalize_kwargs,
         rolling_length,
         train_record_video,
         video_step_interval,
         initial_steps_to_truncate,
         clip_atari_rewards,
         normalize_type,
+        mask_actions,
+        _,  # bots
     ) = astuple(hparams)
 
-    if "BulletEnv" in config.env_id:
-        import pybullet_envs
+    import_for_env_id(config.env_id)
 
-    spec = gym.spec(config.env_id)
     seed = config.seed(training=training)
 
     make_kwargs = make_kwargs.copy() if make_kwargs is not None else {}
-    if "BulletEnv" in config.env_id and render:
+    if is_bullet_env(config) and render:
         make_kwargs["render"] = True
-    if "CarRacing" in config.env_id:
+    if is_car_racing(config):
         make_kwargs["verbose"] = 0
-    if "procgen" in config.env_id:
-        if not render:
-            make_kwargs["render_mode"] = "rgb_array"
+    if is_gym_procgen(config) and not render:
+        make_kwargs["render_mode"] = "rgb_array"
 
     def make(idx: int) -> Callable[[], gym.Env]:
         def _make() -> gym.Env:
             env = gym.make(config.env_id, **make_kwargs)
             env = gym.wrappers.RecordEpisodeStatistics(env)
             env = VideoCompatWrapper(env)
             if training and train_record_video and idx == 0:
@@ -142,36 +99,38 @@
                     step_increment=n_envs,
                     video_step_interval=int(video_step_interval),
                 )
             if training and initial_steps_to_truncate:
                 env = InitialStepTruncateWrapper(
                     env, idx * initial_steps_to_truncate // n_envs
                 )
-            if "AtariEnv" in spec.entry_point:  # type: ignore
+            if is_atari(config):  # type: ignore
                 env = NoopResetEnv(env, noop_max=30)
                 env = MaxAndSkipEnv(env, skip=4)
                 env = EpisodicLifeEnv(env, training=training)
                 action_meanings = env.unwrapped.get_action_meanings()
                 if "FIRE" in action_meanings:  # type: ignore
                     env = FireOnLifeStarttEnv(env, action_meanings.index("FIRE"))
                 if clip_atari_rewards:
                     env = ClipRewardEnv(env, training=training)
                 env = ResizeObservation(env, (84, 84))
                 env = GrayScaleObservation(env, keep_dim=False)
                 env = FrameStack(env, frame_stack)
-            elif "CarRacing" in config.env_id:
+            elif is_car_racing(config):
                 env = ResizeObservation(env, (64, 64))
                 env = GrayScaleObservation(env, keep_dim=False)
                 env = FrameStack(env, frame_stack)
-            elif "procgen" in config.env_id:
+            elif is_gym_procgen(config):
                 # env = GrayScaleObservation(env, keep_dim=False)
                 env = NoopEnvSeed(env)
-                env = TransposeImageObservation(env)
+                env = HwcToChwObservation(env)
                 if frame_stack > 1:
                     env = FrameStack(env, frame_stack)
+            elif is_microrts(config):
+                env = HwcToChwObservation(env)
 
             if no_reward_timeout_steps:
                 env = NoRewardTimeout(
                     env, no_reward_timeout_steps, n_fire_steps=no_reward_fire_steps
                 )
 
             if seed is not None:
@@ -190,14 +149,16 @@
     else:
         raise ValueError(f"env_type {env_type} unsupported")
     envs = VecEnvClass([make(i) for i in range(n_envs)])
     if env_type == "gymvec" and vec_env_class == "sync":
         envs = SyncVectorEnvRenderCompat(envs)
     if env_type == "sb3vec":
         envs = IsVectorEnv(envs)
+    if mask_actions:
+        envs = SingleActionMaskWrapper(envs)
     if training:
         assert tb_writer
         envs = EpisodeStatsWriter(
             envs, tb_writer, training=training, rolling_length=rolling_length
         )
     if normalize:
         if normalize_type is None:
@@ -229,73 +190,7 @@
                     clip=normalize_kwargs.get("clip_reward", 10.0),
                 )
         else:
             raise ValueError(
                 f"normalize_type {normalize_type} not supported (sb3 or gymlike)"
             )
     return envs
-
-
-def _make_procgen_env(
-    config: Config,
-    hparams: EnvHyperparams,
-    training: bool = True,
-    render: bool = False,
-    normalize_load_path: Optional[str] = None,
-    tb_writer: Optional[SummaryWriter] = None,
-) -> VecEnv:
-    from gym3 import ViewerWrapper, ExtractDictObWrapper
-    from procgen.env import ProcgenGym3Env, ToBaselinesVecEnv
-
-    (
-        _,  # env_type
-        n_envs,
-        _,  # frame_stack
-        make_kwargs,
-        _,  # no_reward_timeout_steps
-        _,  # no_reward_fire_steps
-        _,  # vec_env_class
-        normalize,
-        normalize_kwargs,
-        rolling_length,
-        _,  # train_record_video
-        _,  # video_step_interval
-        _,  # initial_steps_to_truncate
-        _,  # clip_atari_rewards
-    ) = astuple(hparams)
-
-    seed = config.seed(training=training)
-
-    make_kwargs = make_kwargs or {}
-    make_kwargs["render_mode"] = "rgb_array"
-    if seed is not None:
-        make_kwargs["rand_seed"] = seed
-
-    envs = ProcgenGym3Env(n_envs, config.env_id, **make_kwargs)
-    envs = ExtractDictObWrapper(envs, key="rgb")
-    if render:
-        envs = ViewerWrapper(envs, info_key="rgb")
-    envs = ToBaselinesVecEnv(envs)
-    envs = IsVectorEnv(envs)
-    # TODO: Handle Grayscale and/or FrameStack
-    envs = TransposeImageObservation(envs)
-
-    envs = gym.wrappers.RecordEpisodeStatistics(envs)
-
-    if seed is not None:
-        envs.action_space.seed(seed)
-        envs.observation_space.seed(seed)
-
-    if training:
-        assert tb_writer
-        envs = EpisodeStatsWriter(
-            envs, tb_writer, training=training, rolling_length=rolling_length
-        )
-    if normalize and training:
-        normalize_kwargs = normalize_kwargs or {}
-        envs = gym.wrappers.NormalizeReward(envs)
-        clip_obs = normalize_kwargs.get("clip_reward", 10.0)
-        envs = gym.wrappers.TransformReward(
-            envs, lambda r: np.clip(r, -clip_obs, clip_obs)
-        )
-
-    return envs  # type: ignore
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/runner/evaluate.py` & `rl_algo_impls-0.0.8/rl_algo_impls/runner/evaluate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 
 from dataclasses import dataclass
 from typing import NamedTuple, Optional
 
-from rl_algo_impls.runner.env import make_eval_env
+from rl_algo_impls.shared.vec_env import make_eval_env
 from rl_algo_impls.runner.config import Config, EnvHyperparams, Hyperparams, RunArgs
 from rl_algo_impls.runner.running_utils import (
     load_hyperparams,
     set_seeds,
     get_device,
     make_policy,
 )
@@ -71,15 +71,15 @@
     env = make_eval_env(
         config,
         EnvHyperparams(**config.env_hyperparams),
         override_n_envs=args.n_envs,
         render=args.render,
         normalize_load_path=model_path,
     )
-    device = get_device(config.device, env)
+    device = get_device(config, env)
     policy = make_policy(
         args.algo,
         env,
         device,
         load_path=model_path,
         **config.policy_hyperparams,
     ).eval()
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/runner/running_utils.py` & `rl_algo_impls-0.0.8/rl_algo_impls/runner/running_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import argparse
-import gym
 import json
-import matplotlib.pyplot as plt
-import numpy as np
 import os
 import random
+from dataclasses import asdict
+from pathlib import Path
+from typing import Dict, Optional, Type, Union
+
+import gym
+import matplotlib.pyplot as plt
+import numpy as np
 import torch
 import torch.backends.cudnn
 import yaml
-
-from dataclasses import asdict
 from gym.spaces import Box, Discrete
-from pathlib import Path
 from torch.utils.tensorboard.writer import SummaryWriter
-from typing import Dict, Optional, Type, Union
-
-from rl_algo_impls.runner.config import Hyperparams
-from rl_algo_impls.shared.algorithm import Algorithm
-from rl_algo_impls.shared.callbacks.eval_callback import EvalCallback
-from rl_algo_impls.shared.policy.on_policy import ActorCritic
-from rl_algo_impls.shared.policy.policy import Policy
 
 from rl_algo_impls.a2c.a2c import A2C
 from rl_algo_impls.dqn.dqn import DQN
 from rl_algo_impls.dqn.policy import DQNPolicy
 from rl_algo_impls.ppo.ppo import PPO
-from rl_algo_impls.vpg.vpg import VanillaPolicyGradient
+from rl_algo_impls.runner.config import Config, Hyperparams
+from rl_algo_impls.shared.algorithm import Algorithm
+from rl_algo_impls.shared.callbacks.eval_callback import EvalCallback
+from rl_algo_impls.shared.policy.on_policy import ActorCritic
+from rl_algo_impls.shared.policy.policy import Policy
+from rl_algo_impls.shared.vec_env.utils import import_for_env_id, is_microrts
 from rl_algo_impls.vpg.policy import VPGActorCritic
+from rl_algo_impls.vpg.vpg import VanillaPolicyGradient
 from rl_algo_impls.wrappers.vectorable_wrapper import VecEnv, single_observation_space
 
 ALGOS: Dict[str, Type[Algorithm]] = {
     "dqn": DQN,
     "vpg": VanillaPolicyGradient,
     "ppo": PPO,
     "a2c": A2C,
@@ -77,24 +77,27 @@
     hyperparams_path = os.path.join(root_path, HYPERPARAMS_PATH, f"{algo}.yml")
     with open(hyperparams_path, "r") as f:
         hyperparams_dict = yaml.safe_load(f)
 
     if env_id in hyperparams_dict:
         return Hyperparams(**hyperparams_dict[env_id])
 
-    if "BulletEnv" in env_id:
-        import pybullet_envs
+    import_for_env_id(env_id)
     spec = gym.spec(env_id)
-    if "AtariEnv" in str(spec.entry_point) and "_atari" in hyperparams_dict:
+    entry_point_name = str(spec.entry_point)  # type: ignore
+    if "AtariEnv" in entry_point_name and "_atari" in hyperparams_dict:
         return Hyperparams(**hyperparams_dict["_atari"])
+    elif "gym_microrts" in entry_point_name and "_microrts" in hyperparams_dict:
+        return Hyperparams(**hyperparams_dict["_microrts"])
     else:
         raise ValueError(f"{env_id} not specified in {algo} hyperparameters file")
 
 
-def get_device(device: str, env: VecEnv) -> torch.device:
+def get_device(config: Config, env: VecEnv) -> torch.device:
+    device = config.device
     # cuda by default
     if device == "auto":
         device = "cuda"
     # Apple MPS is a second choice (sometimes)
     if device == "cuda" and not torch.cuda.is_available():
         device = "mps"
     # If no MPS, fallback to cpu
@@ -104,14 +107,24 @@
     # served with the CPU.
     if device == "mps":
         obs_space = single_observation_space(env)
         if isinstance(obs_space, Discrete):
             device = "cpu"
         elif isinstance(obs_space, Box) and len(obs_space.shape) == 1:
             device = "cpu"
+        if is_microrts(config):
+            try:
+                from gym_microrts.envs.vec_env import MicroRTSGridModeVecEnv
+
+                # Models that move more than one unit at a time should use mps
+                if not isinstance(env.unwrapped, MicroRTSGridModeVecEnv):
+                    device = "cpu"
+            except ModuleNotFoundError:
+                # Likely on gym_microrts v0.0.2 to match ppo-implementation-details
+                device = "cpu"
     print(f"Device: {device}")
     return torch.device(device)
 
 
 def set_seeds(seed: Optional[int], use_deterministic_algorithms: bool) -> None:
     if seed is None:
         return
@@ -183,10 +196,12 @@
         if isinstance(v, dict):
             for sk, sv in v.items():
                 key = f"{k}/{sk}"
                 if isinstance(sv, dict) or isinstance(sv, list):
                     flattened[key] = str(sv)
                 else:
                     flattened[key] = sv
+        elif isinstance(v, list):
+            flattened[k] = json.dumps(v)
         else:
             flattened[k] = v  # type: ignore
     return flattened  # type: ignore
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/runner/train.py` & `rl_algo_impls-0.0.8/rl_algo_impls/runner/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # Support for PyTorch mps mode (https://pytorch.org/docs/stable/notes/mps.html)
 import os
 
 os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 
 import dataclasses
 import shutil
-import wandb
-import yaml
-
 from dataclasses import asdict, dataclass
-from torch.utils.tensorboard.writer import SummaryWriter
 from typing import Any, Dict, Optional, Sequence
 
-from rl_algo_impls.shared.callbacks.eval_callback import EvalCallback
+import yaml
+from torch.utils.tensorboard.writer import SummaryWriter
+
+import wandb
 from rl_algo_impls.runner.config import Config, EnvHyperparams, RunArgs
-from rl_algo_impls.runner.env import make_env, make_eval_env
 from rl_algo_impls.runner.running_utils import (
     ALGOS,
-    load_hyperparams,
-    set_seeds,
     get_device,
+    hparam_dict,
+    load_hyperparams,
     make_policy,
     plot_eval_callback,
-    hparam_dict,
+    set_seeds,
 )
+from rl_algo_impls.shared.callbacks.eval_callback import EvalCallback
 from rl_algo_impls.shared.stats import EpisodesStats
+from rl_algo_impls.shared.vec_env import make_env, make_eval_env
 
 
 @dataclass
 class TrainArgs(RunArgs):
     wandb_project_name: Optional[str] = None
     wandb_entity: Optional[str] = None
     wandb_tags: Sequence[str] = dataclasses.field(default_factory=list)
@@ -61,15 +61,15 @@
     tb_writer = SummaryWriter(config.tensorboard_summary_path)
 
     set_seeds(args.seed, args.use_deterministic_algorithms)
 
     env = make_env(
         config, EnvHyperparams(**config.env_hyperparams), tb_writer=tb_writer
     )
-    device = get_device(config.device, env)
+    device = get_device(config, env)
     policy = make_policy(args.algo, env, device, **config.policy_hyperparams)
     algo = ALGOS[args.algo](policy, env, device, tb_writer, **config.algo_hyperparams)
 
     num_parameters = policy.num_parameters()
     num_trainable_parameters = policy.num_trainable_parameters()
     if wandb_enabled:
         wandb.run.summary["num_parameters"] = num_parameters
@@ -90,14 +90,15 @@
         **config.eval_params,
         video_env=make_eval_env(
             config, EnvHyperparams(**config.env_hyperparams), override_n_envs=1
         )
         if record_best_videos
         else None,
         best_video_dir=config.best_videos_dir,
+        additional_keys_to_log=config.additional_keys_to_log,
     )
     algo.learn(config.n_timesteps, callback=callback)
 
     policy.save(config.model_dir_path(best=False))
 
     eval_stats = callback.evaluate(n_episodes=10, print_returns=True)
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/algorithm.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/algorithm.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/callbacks/eval_callback.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/callbacks/eval_callback.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 import itertools
-import numpy as np
 import os
-
 from time import perf_counter
+from typing import Dict, List, Optional, Union
+
+import numpy as np
 from torch.utils.tensorboard.writer import SummaryWriter
-from typing import List, Optional, Union
 
 from rl_algo_impls.shared.callbacks.callback import Callback
 from rl_algo_impls.shared.policy.policy import Policy
 from rl_algo_impls.shared.stats import Episode, EpisodeAccumulator, EpisodesStats
+from rl_algo_impls.wrappers.action_mask_wrapper import find_action_masker
 from rl_algo_impls.wrappers.vec_episode_recorder import VecEpisodeRecorder
 from rl_algo_impls.wrappers.vectorable_wrapper import VecEnv
 
 
 class EvaluateAccumulator(EpisodeAccumulator):
     def __init__(
         self,
         num_envs: int,
         goal_episodes: int,
         print_returns: bool = True,
         ignore_first_episode: bool = False,
+        additional_keys_to_log: Optional[List[str]] = None,
     ):
         super().__init__(num_envs)
         self.completed_episodes_by_env_idx = [[] for _ in range(num_envs)]
         self.goal_episodes_per_env = int(np.ceil(goal_episodes / num_envs))
         self.print_returns = print_returns
         if ignore_first_episode:
             first_done = set()
@@ -32,16 +34,19 @@
                 has_done_first_episode = idx in first_done
                 first_done.add(idx)
                 return has_done_first_episode
 
             self.should_record_done = should_record_done
         else:
             self.should_record_done = lambda idx: True
+        self.additional_keys_to_log = additional_keys_to_log
 
-    def on_done(self, ep_idx: int, episode: Episode) -> None:
+    def on_done(self, ep_idx: int, episode: Episode, info: Dict) -> None:
+        if self.additional_keys_to_log:
+            episode.info = {k: info[k] for k in self.additional_keys_to_log}
         if (
             self.should_record_done(ep_idx)
             and len(self.completed_episodes_by_env_idx[ep_idx])
             >= self.goal_episodes_per_env
         ):
             return
         self.completed_episodes_by_env_idx[ep_idx].append(episode)
@@ -70,27 +75,37 @@
     env: VecEnv,
     policy: Policy,
     n_episodes: int,
     render: bool = False,
     deterministic: bool = True,
     print_returns: bool = True,
     ignore_first_episode: bool = False,
+    additional_keys_to_log: Optional[List[str]] = None,
 ) -> EpisodesStats:
     policy.sync_normalization(env)
     policy.eval()
 
     episodes = EvaluateAccumulator(
-        env.num_envs, n_episodes, print_returns, ignore_first_episode
+        env.num_envs,
+        n_episodes,
+        print_returns,
+        ignore_first_episode,
+        additional_keys_to_log=additional_keys_to_log,
     )
 
     obs = env.reset()
+    action_masker = find_action_masker(env)
     while not episodes.is_done():
-        act = policy.act(obs, deterministic=deterministic)
-        obs, rew, done, _ = env.step(act)
-        episodes.step(rew, done)
+        act = policy.act(
+            obs,
+            deterministic=deterministic,
+            action_masks=action_masker.action_masks() if action_masker else None,
+        )
+        obs, rew, done, info = env.step(act)
+        episodes.step(rew, done, info)
         if render:
             env.render()
     stats = EpisodesStats(episodes.episodes)
     if print_returns:
         print(stats)
     return stats
 
@@ -107,14 +122,15 @@
         save_best: bool = True,
         deterministic: bool = True,
         record_best_videos: bool = True,
         video_env: Optional[VecEnv] = None,
         best_video_dir: Optional[str] = None,
         max_video_length: int = 3600,
         ignore_first_episode: bool = False,
+        additional_keys_to_log: Optional[List[str]] = None,
     ) -> None:
         super().__init__()
         self.policy = policy
         self.env = env
         self.tb_writer = tb_writer
         self.best_model_path = best_model_path
         self.step_freq = int(step_freq)
@@ -129,16 +145,16 @@
         self.video_env = video_env
         assert best_video_dir or not record_best_videos
         self.best_video_dir = best_video_dir
         if best_video_dir:
             os.makedirs(best_video_dir, exist_ok=True)
         self.max_video_length = max_video_length
         self.best_video_base_path = None
-
         self.ignore_first_episode = ignore_first_episode
+        self.additional_keys_to_log = additional_keys_to_log
 
     def on_step(self, timesteps_elapsed: int = 1) -> bool:
         super().on_step(timesteps_elapsed)
         if self.timesteps_elapsed // self.step_freq >= len(self.stats):
             self.evaluate()
         return True
 
@@ -149,14 +165,15 @@
         eval_stat = evaluate(
             self.env,
             self.policy,
             n_episodes or self.n_episodes,
             deterministic=self.deterministic,
             print_returns=print_returns or False,
             ignore_first_episode=self.ignore_first_episode,
+            additional_keys_to_log=self.additional_keys_to_log,
         )
         end_time = perf_counter()
         self.tb_writer.add_scalar(
             "eval/steps_per_second",
             eval_stat.length.sum() / (end_time - start_time),
             self.timesteps_elapsed,
         )
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/callbacks/optimize_callback.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/callbacks/optimize_callback.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/actor.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/on_policy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,310 +1,249 @@
+from abc import abstractmethod
+from typing import NamedTuple, Optional, Sequence, Tuple, TypeVar
+
 import gym
+import numpy as np
 import torch
-import torch.nn as nn
+from gym.spaces import Box, Discrete, Space
 
-from abc import ABC, abstractmethod
-from gym.spaces import Box, Discrete
-from torch.distributions import Categorical, Distribution, Normal
-from typing import NamedTuple, Optional, Sequence, Type, TypeVar, Union
+from rl_algo_impls.shared.actor import PiForward, actor_head
+from rl_algo_impls.shared.encoder import Encoder
+from rl_algo_impls.shared.policy.critic import CriticHead
+from rl_algo_impls.shared.policy.policy import ACTIVATION, Policy
+from rl_algo_impls.wrappers.vectorable_wrapper import (
+    VecEnv,
+    VecEnvObs,
+    single_action_space,
+    single_observation_space,
+)
 
-from rl_algo_impls.shared.module.module import mlp
 
+class Step(NamedTuple):
+    a: np.ndarray
+    v: np.ndarray
+    logp_a: np.ndarray
+    clamped_a: np.ndarray
+
+
+class ACForward(NamedTuple):
+    logp_a: torch.Tensor
+    entropy: torch.Tensor
+    v: torch.Tensor
+
+
+FEAT_EXT_FILE_NAME = "feat_ext.pt"
+V_FEAT_EXT_FILE_NAME = "v_feat_ext.pt"
+PI_FILE_NAME = "pi.pt"
+V_FILE_NAME = "v.pt"
+ActorCriticSelf = TypeVar("ActorCriticSelf", bound="ActorCritic")
+
+
+def clamp_actions(
+    actions: np.ndarray, action_space: gym.Space, squash_output: bool
+) -> np.ndarray:
+    if isinstance(action_space, Box):
+        low, high = action_space.low, action_space.high  # type: ignore
+        if squash_output:
+            # Squashed output is already between -1 and 1. Rescale if the actual
+            # output needs to something other than -1 and 1
+            return low + 0.5 * (actions + 1) * (high - low)
+        else:
+            return np.clip(actions, low, high)
+    return actions
 
-class PiForward(NamedTuple):
-    pi: Distribution
-    logp_a: Optional[torch.Tensor]
-    entropy: Optional[torch.Tensor]
+
+def default_hidden_sizes(obs_space: Space) -> Sequence[int]:
+    if isinstance(obs_space, Box):
+        if len(obs_space.shape) == 3:
+            # By default feature extractor to output has no hidden layers
+            return []
+        elif len(obs_space.shape) == 1:
+            return [64, 64]
+        else:
+            raise ValueError(f"Unsupported observation space: {obs_space}")
+    elif isinstance(obs_space, Discrete):
+        return [64]
+    else:
+        raise ValueError(f"Unsupported observation space: {obs_space}")
 
 
-class Actor(nn.Module, ABC):
+class OnPolicy(Policy):
     @abstractmethod
-    def forward(self, obs: torch.Tensor, a: Optional[torch.Tensor] = None) -> PiForward:
+    def value(self, obs: VecEnvObs) -> np.ndarray:
         ...
 
+    @abstractmethod
+    def step(self, obs: VecEnvObs, action_masks: Optional[np.ndarray] = None) -> Step:
+        ...
 
-class CategoricalActorHead(Actor):
-    def __init__(
-        self,
-        act_dim: int,
-        hidden_sizes: Sequence[int] = (32,),
-        activation: Type[nn.Module] = nn.Tanh,
-        init_layers_orthogonal: bool = True,
-    ) -> None:
-        super().__init__()
-        layer_sizes = tuple(hidden_sizes) + (act_dim,)
-        self._fc = mlp(
-            layer_sizes,
-            activation,
-            init_layers_orthogonal=init_layers_orthogonal,
-            final_layer_gain=0.01,
-        )
-
-    def forward(self, obs: torch.Tensor, a: Optional[torch.Tensor] = None) -> PiForward:
-        logits = self._fc(obs)
-        pi = Categorical(logits=logits)
-        logp_a = None
-        entropy = None
-        if a is not None:
-            logp_a = pi.log_prob(a)
-            entropy = pi.entropy()
-        return PiForward(pi, logp_a, entropy)
-
-
-class GaussianDistribution(Normal):
-    def log_prob(self, a: torch.Tensor) -> torch.Tensor:
-        return super().log_prob(a).sum(axis=-1)
-
-    def sample(self) -> torch.Tensor:
-        return self.rsample()
+    @property
+    @abstractmethod
+    def action_shape(self) -> Tuple[int, ...]:
+        ...
 
 
-class GaussianActorHead(Actor):
+class ActorCritic(OnPolicy):
     def __init__(
         self,
-        act_dim: int,
-        hidden_sizes: Sequence[int] = (32,),
-        activation: Type[nn.Module] = nn.Tanh,
+        env: VecEnv,
+        pi_hidden_sizes: Optional[Sequence[int]] = None,
+        v_hidden_sizes: Optional[Sequence[int]] = None,
         init_layers_orthogonal: bool = True,
+        activation_fn: str = "tanh",
         log_std_init: float = -0.5,
+        use_sde: bool = False,
+        full_std: bool = True,
+        squash_output: bool = False,
+        share_features_extractor: bool = True,
+        cnn_flatten_dim: int = 512,
+        cnn_style: str = "nature",
+        cnn_layers_init_orthogonal: Optional[bool] = None,
+        impala_channels: Sequence[int] = (16, 32, 32),
+        actor_head_style: str = "single",
+        **kwargs,
     ) -> None:
-        super().__init__()
-        layer_sizes = tuple(hidden_sizes) + (act_dim,)
-        self.mu_net = mlp(
-            layer_sizes,
+        super().__init__(env, **kwargs)
+
+        observation_space = single_observation_space(env)
+        action_space = single_action_space(env)
+
+        pi_hidden_sizes = (
+            pi_hidden_sizes
+            if pi_hidden_sizes is not None
+            else default_hidden_sizes(observation_space)
+        )
+        v_hidden_sizes = (
+            v_hidden_sizes
+            if v_hidden_sizes is not None
+            else default_hidden_sizes(observation_space)
+        )
+
+        activation = ACTIVATION[activation_fn]
+        self.action_space = action_space
+        self.squash_output = squash_output
+        self.share_features_extractor = share_features_extractor
+        self._feature_extractor = Encoder(
+            observation_space,
             activation,
             init_layers_orthogonal=init_layers_orthogonal,
-            final_layer_gain=0.01,
-        )
-        self.log_std = nn.Parameter(
-            torch.ones(act_dim, dtype=torch.float32) * log_std_init
+            cnn_flatten_dim=cnn_flatten_dim,
+            cnn_style=cnn_style,
+            cnn_layers_init_orthogonal=cnn_layers_init_orthogonal,
+            impala_channels=impala_channels,
+        )
+        self._pi = actor_head(
+            self.action_space,
+            self._feature_extractor.out_dim,
+            tuple(pi_hidden_sizes),
+            init_layers_orthogonal,
+            activation,
+            log_std_init=log_std_init,
+            use_sde=use_sde,
+            full_std=full_std,
+            squash_output=squash_output,
+            actor_head_style=actor_head_style,
         )
 
-    def _distribution(self, obs: torch.Tensor) -> Distribution:
-        mu = self.mu_net(obs)
-        std = torch.exp(self.log_std)
-        return GaussianDistribution(mu, std)
-
-    def forward(self, obs: torch.Tensor, a: Optional[torch.Tensor] = None) -> PiForward:
-        pi = self._distribution(obs)
-        logp_a = None
-        entropy = None
-        if a is not None:
-            logp_a = pi.log_prob(a)
-            entropy = pi.entropy()
-        return PiForward(pi, logp_a, entropy)
-
-
-class TanhBijector:
-    def __init__(self, epsilon: float = 1e-6) -> None:
-        self.epsilon = epsilon
-
-    @staticmethod
-    def forward(x: torch.Tensor) -> torch.Tensor:
-        return torch.tanh(x)
-
-    @staticmethod
-    def inverse(y: torch.Tensor) -> torch.Tensor:
-        eps = torch.finfo(y.dtype).eps
-        clamped_y = y.clamp(min=-1.0 + eps, max=1.0 - eps)
-        return torch.atanh(clamped_y)
-
-    def log_prob_correction(self, x: torch.Tensor) -> torch.Tensor:
-        return torch.log(1.0 - torch.tanh(x) ** 2 + self.epsilon)
-
-
-def sum_independent_dims(tensor: torch.Tensor) -> torch.Tensor:
-    if len(tensor.shape) > 1:
-        return tensor.sum(dim=1)
-    return tensor.sum()
-
-
-class StateDependentNoiseDistribution(Normal):
-    def __init__(
-        self,
-        loc,
-        scale,
-        latent_sde: torch.Tensor,
-        exploration_mat: torch.Tensor,
-        exploration_matrices: torch.Tensor,
-        bijector: Optional[TanhBijector] = None,
-        validate_args=None,
-    ):
-        super().__init__(loc, scale, validate_args)
-        self.latent_sde = latent_sde
-        self.exploration_mat = exploration_mat
-        self.exploration_matrices = exploration_matrices
-        self.bijector = bijector
-
-    def log_prob(self, a: torch.Tensor) -> torch.Tensor:
-        gaussian_a = self.bijector.inverse(a) if self.bijector else a
-        log_prob = sum_independent_dims(super().log_prob(gaussian_a))
-        if self.bijector:
-            log_prob -= torch.sum(self.bijector.log_prob_correction(gaussian_a), dim=1)
-        return log_prob
-
-    def sample(self) -> torch.Tensor:
-        noise = self._get_noise()
-        actions = self.mean + noise
-        return self.bijector.forward(actions) if self.bijector else actions
-
-    def _get_noise(self) -> torch.Tensor:
-        if len(self.latent_sde) == 1 or len(self.latent_sde) != len(
-            self.exploration_matrices
-        ):
-            return torch.mm(self.latent_sde, self.exploration_mat)
-        # (batch_size, n_features) -> (batch_size, 1, n_features)
-        latent_sde = self.latent_sde.unsqueeze(dim=1)
-        # (batch_size, 1, n_actions)
-        noise = torch.bmm(latent_sde, self.exploration_matrices)
-        return noise.squeeze(dim=1)
-
-    @property
-    def mode(self) -> torch.Tensor:
-        mean = super().mode
-        return self.bijector.forward(mean) if self.bijector else mean
-
-
-StateDependentNoiseActorHeadSelf = TypeVar(
-    "StateDependentNoiseActorHeadSelf", bound="StateDependentNoiseActorHead"
-)
-
-
-class StateDependentNoiseActorHead(Actor):
-    def __init__(
-        self,
-        act_dim: int,
-        hidden_sizes: Sequence[int] = (32,),
-        activation: Type[nn.Module] = nn.Tanh,
-        init_layers_orthogonal: bool = True,
-        log_std_init: float = -0.5,
-        full_std: bool = True,
-        squash_output: bool = False,
-        learn_std: bool = False,
-    ) -> None:
-        super().__init__()
-        self.act_dim = act_dim
-        layer_sizes = tuple(hidden_sizes) + (self.act_dim,)
-        if len(layer_sizes) == 2:
-            self.latent_net = nn.Identity()
-        elif len(layer_sizes) > 2:
-            self.latent_net = mlp(
-                layer_sizes[:-1],
+        if not share_features_extractor:
+            self._v_feature_extractor = Encoder(
+                observation_space,
                 activation,
-                output_activation=activation,
                 init_layers_orthogonal=init_layers_orthogonal,
+                cnn_flatten_dim=cnn_flatten_dim,
+                cnn_style=cnn_style,
+                cnn_layers_init_orthogonal=cnn_layers_init_orthogonal,
             )
+            critic_in_dim = self._v_feature_extractor.out_dim
         else:
-            raise ValueError("hidden_sizes must be of at least length 1")
-        self.mu_net = mlp(
-            layer_sizes[-2:],
-            activation,
+            self._v_feature_extractor = None
+            critic_in_dim = self._feature_extractor.out_dim
+        self._v = CriticHead(
+            in_dim=critic_in_dim,
+            hidden_sizes=v_hidden_sizes,
+            activation=activation,
             init_layers_orthogonal=init_layers_orthogonal,
-            final_layer_gain=0.01,
-        )
-        self.full_std = full_std
-        std_dim = (hidden_sizes[-1], act_dim if self.full_std else 1)
-        self.log_std = nn.Parameter(
-            torch.ones(std_dim, dtype=torch.float32) * log_std_init
-        )
-        self.bijector = TanhBijector() if squash_output else None
-        self.learn_std = learn_std
-        self.device = None
-
-        self.exploration_mat = None
-        self.exploration_matrices = None
-        self.sample_weights()
-
-    def to(
-        self: StateDependentNoiseActorHeadSelf,
-        device: Optional[torch.device] = None,
-        dtype: Optional[Union[torch.dtype, str]] = None,
-        non_blocking: bool = False,
-    ) -> StateDependentNoiseActorHeadSelf:
-        super().to(device, dtype, non_blocking)
-        self.device = device
-        return self
-
-    def _distribution(self, obs: torch.Tensor) -> Distribution:
-        latent = self.latent_net(obs)
-        mu = self.mu_net(latent)
-        latent_sde = latent if self.learn_std else latent.detach()
-        variance = torch.mm(latent_sde**2, self._get_std() ** 2)
-        assert self.exploration_mat is not None
-        assert self.exploration_matrices is not None
-        return StateDependentNoiseDistribution(
-            mu,
-            torch.sqrt(variance + 1e-6),
-            latent_sde,
-            self.exploration_mat,
-            self.exploration_matrices,
-            self.bijector,
         )
 
-    def _get_std(self) -> torch.Tensor:
-        std = torch.exp(self.log_std)
-        if self.full_std:
-            return std
-        ones = torch.ones(self.log_std.shape[0], self.act_dim)
-        if self.device:
-            ones = ones.to(self.device)
-        return ones * std
-
-    def forward(self, obs: torch.Tensor, a: Optional[torch.Tensor] = None) -> PiForward:
-        pi = self._distribution(obs)
-        logp_a = None
-        entropy = None
-        if a is not None:
-            logp_a = pi.log_prob(a)
-            entropy = -logp_a if self.bijector else sum_independent_dims(pi.entropy())
-        return PiForward(pi, logp_a, entropy)
+    def _pi_forward(
+        self,
+        obs: torch.Tensor,
+        action_masks: Optional[torch.Tensor],
+        action: Optional[torch.Tensor] = None,
+    ) -> Tuple[PiForward, torch.Tensor]:
+        p_fe = self._feature_extractor(obs)
+        pi_forward = self._pi(p_fe, actions=action, action_masks=action_masks)
+
+        return pi_forward, p_fe
+
+    def _v_forward(self, obs: torch.Tensor, p_fc: torch.Tensor) -> torch.Tensor:
+        v_fe = self._v_feature_extractor(obs) if self._v_feature_extractor else p_fc
+        return self._v(v_fe)
 
-    def sample_weights(self, batch_size: int = 1) -> None:
-        std = self._get_std()
-        weights_dist = Normal(torch.zeros_like(std), std)
-        # Reparametrization trick to pass gradients
-        self.exploration_mat = weights_dist.rsample()
-        self.exploration_matrices = weights_dist.rsample(torch.Size((batch_size,)))
-
-
-def actor_head(
-    action_space: gym.Space,
-    hidden_sizes: Sequence[int],
-    init_layers_orthogonal: bool,
-    activation: Type[nn.Module],
-    log_std_init: float = -0.5,
-    use_sde: bool = False,
-    full_std: bool = True,
-    squash_output: bool = False,
-) -> Actor:
-    assert not use_sde or isinstance(
-        action_space, Box
-    ), "use_sde only valid if Box action_space"
-    assert not squash_output or use_sde, "squash_output only valid if use_sde"
-    if isinstance(action_space, Discrete):
-        return CategoricalActorHead(
-            action_space.n,
-            hidden_sizes=hidden_sizes,
-            activation=activation,
-            init_layers_orthogonal=init_layers_orthogonal,
-        )
-    elif isinstance(action_space, Box):
-        if use_sde:
-            return StateDependentNoiseActorHead(
-                action_space.shape[0],
-                hidden_sizes=hidden_sizes,
-                activation=activation,
-                init_layers_orthogonal=init_layers_orthogonal,
-                log_std_init=log_std_init,
-                full_std=full_std,
-                squash_output=squash_output,
+    def forward(
+        self,
+        obs: torch.Tensor,
+        action: torch.Tensor,
+        action_masks: Optional[torch.Tensor] = None,
+    ) -> ACForward:
+        (_, logp_a, entropy), p_fc = self._pi_forward(obs, action_masks, action=action)
+        v = self._v_forward(obs, p_fc)
+
+        assert logp_a is not None
+        assert entropy is not None
+        return ACForward(logp_a, entropy, v)
+
+    def value(self, obs: VecEnvObs) -> np.ndarray:
+        o = self._as_tensor(obs)
+        with torch.no_grad():
+            fe = (
+                self._v_feature_extractor(o)
+                if self._v_feature_extractor
+                else self._feature_extractor(o)
             )
+            v = self._v(fe)
+        return v.cpu().numpy()
+
+    def step(self, obs: VecEnvObs, action_masks: Optional[np.ndarray] = None) -> Step:
+        o = self._as_tensor(obs)
+        a_masks = self._as_tensor(action_masks) if action_masks is not None else None
+        with torch.no_grad():
+            (pi, _, _), p_fc = self._pi_forward(o, action_masks=a_masks)
+            a = pi.sample()
+            logp_a = pi.log_prob(a)
+
+            v = self._v_forward(o, p_fc)
+
+        a_np = a.cpu().numpy()
+        clamped_a_np = clamp_actions(a_np, self.action_space, self.squash_output)
+        return Step(a_np, v.cpu().numpy(), logp_a.cpu().numpy(), clamped_a_np)
+
+    def act(
+        self,
+        obs: np.ndarray,
+        deterministic: bool = True,
+        action_masks: Optional[np.ndarray] = None,
+    ) -> np.ndarray:
+        if not deterministic:
+            return self.step(obs, action_masks=action_masks).clamped_a
         else:
-            return GaussianActorHead(
-                action_space.shape[0],
-                hidden_sizes=hidden_sizes,
-                activation=activation,
-                init_layers_orthogonal=init_layers_orthogonal,
-                log_std_init=log_std_init,
+            o = self._as_tensor(obs)
+            a_masks = (
+                self._as_tensor(action_masks) if action_masks is not None else None
             )
-    else:
-        raise ValueError(f"Unsupported action space: {action_space}")
+            with torch.no_grad():
+                (pi, _, _), _ = self._pi_forward(o, action_masks=a_masks)
+                a = pi.mode
+            return clamp_actions(a.cpu().numpy(), self.action_space, self.squash_output)
+
+    def load(self, path: str) -> None:
+        super().load(path)
+        self.reset_noise()
+
+    def reset_noise(self, batch_size: Optional[int] = None) -> None:
+        self._pi.sample_weights(
+            batch_size=batch_size if batch_size else self.env.num_envs
+        )
+
+    @property
+    def action_shape(self) -> Tuple[int, ...]:
+        return self._pi.action_shape
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/critic.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/critic.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,40 @@
-import gym
+from typing import Sequence, Type
+
+import numpy as np
 import torch
 import torch.nn as nn
 
-from typing import Sequence, Type
-
+from rl_algo_impls.shared.encoder import EncoderOutDim
 from rl_algo_impls.shared.module.module import mlp
 
 
 class CriticHead(nn.Module):
     def __init__(
         self,
-        hidden_sizes: Sequence[int] = (32,),
+        in_dim: EncoderOutDim,
+        hidden_sizes: Sequence[int] = (),
         activation: Type[nn.Module] = nn.Tanh,
         init_layers_orthogonal: bool = True,
     ) -> None:
         super().__init__()
-        layer_sizes = tuple(hidden_sizes) + (1,)
-        self._fc = mlp(
-            layer_sizes,
-            activation,
-            init_layers_orthogonal=init_layers_orthogonal,
-            final_layer_gain=1.0,
+        seq = []
+        if isinstance(in_dim, tuple):
+            seq.append(nn.Flatten())
+            in_channels = int(np.prod(in_dim))
+        else:
+            in_channels = in_dim
+        layer_sizes = (in_channels,) + tuple(hidden_sizes) + (1,)
+        seq.append(
+            mlp(
+                layer_sizes,
+                activation,
+                init_layers_orthogonal=init_layers_orthogonal,
+                final_layer_gain=1.0,
+                hidden_layer_gain=1.0,
+            )
         )
+        self._fc = nn.Sequential(*seq)
 
     def forward(self, obs: torch.Tensor) -> torch.Tensor:
         v = self._fc(obs)
         return v.squeeze(-1)
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/optimize_on_policy.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/optimize_on_policy.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/policy/policy.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/policy/policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,20 @@
         non_blocking: bool = False,
     ) -> PolicySelf:
         super().to(device, dtype, non_blocking)
         self.device = device
         return self
 
     @abstractmethod
-    def act(self, obs: VecEnvObs, deterministic: bool = True) -> np.ndarray:
+    def act(
+        self,
+        obs: VecEnvObs,
+        deterministic: bool = True,
+        action_masks: Optional[np.ndarray] = None,
+    ) -> np.ndarray:
         ...
 
     def save(self, path: str) -> None:
         os.makedirs(path, exist_ok=True)
 
         if self.vec_normalize:
             self.vec_normalize.save(os.path.join(path, VEC_NORMALIZE_FILENAME))
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/stats.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/stats.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-import numpy as np
-
+import dataclasses
+from collections import defaultdict
 from dataclasses import dataclass
+from typing import Any, Dict, List, Optional, Sequence, TypeVar, Union
+
+import numpy as np
 from torch.utils.tensorboard.writer import SummaryWriter
-from typing import Dict, List, Optional, Sequence, Union, TypeVar
 
 
 @dataclass
 class Episode:
     score: float = 0
     length: int = 0
+    info: Dict[str, Dict[str, Any]] = dataclasses.field(default_factory=dict)
 
 
 StatisticSelf = TypeVar("StatisticSelf", bound="Statistic")
 
 
 @dataclass
 class Statistic:
@@ -71,20 +74,33 @@
 
 
 class EpisodesStats:
     episodes: Sequence[Episode]
     simple: bool
     score: Statistic
     length: Statistic
+    additional_stats: Dict[str, Statistic]
 
     def __init__(self, episodes: Sequence[Episode], simple: bool = False) -> None:
         self.episodes = episodes
         self.simple = simple
         self.score = Statistic(np.array([e.score for e in episodes]))
         self.length = Statistic(np.array([e.length for e in episodes]), round_digits=0)
+        additional_values = defaultdict(list)
+        for e in self.episodes:
+            if e.info:
+                for k, v in e.info.items():
+                    if isinstance(v, dict):
+                        for k2, v2 in v.items():
+                            additional_values[f"{k}_{k2}"].append(v2)
+                    else:
+                        additional_values[k].append(v)
+        self.additional_stats = {
+            k: Statistic(np.array(values)) for k, values in additional_values.items()
+        }
 
     def __gt__(self: EpisodesStatsSelf, o: EpisodesStatsSelf) -> bool:
         return self.score > o.score
 
     def __ge__(self: EpisodesStatsSelf, o: EpisodesStatsSelf) -> bool:
         return self.score >= o.score
 
@@ -114,40 +130,42 @@
                     "min": self.score.min,
                     "max": self.score.max,
                     "result": self.score.mean - self.score.std,
                     "n_episodes": len(self.episodes),
                     "length": self.length.mean,
                 }
             )
+            for k, addl_stats in self.additional_stats.items():
+                stats[k] = addl_stats.mean
         for name, value in stats.items():
             tb_writer.add_scalar(f"{main_tag}/{name}", value, global_step=global_step)
 
 
 class EpisodeAccumulator:
     def __init__(self, num_envs: int):
         self._episodes = []
         self.current_episodes = [Episode() for _ in range(num_envs)]
 
     @property
     def episodes(self) -> List[Episode]:
         return self._episodes
 
-    def step(self, reward: np.ndarray, done: np.ndarray) -> None:
+    def step(self, reward: np.ndarray, done: np.ndarray, info: List[Dict]) -> None:
         for idx, current in enumerate(self.current_episodes):
             current.score += reward[idx]
             current.length += 1
             if done[idx]:
                 self._episodes.append(current)
                 self.current_episodes[idx] = Episode()
-                self.on_done(idx, current)
+                self.on_done(idx, current, info[idx])
 
     def __len__(self) -> int:
         return len(self.episodes)
 
-    def on_done(self, ep_idx: int, episode: Episode) -> None:
+    def on_done(self, ep_idx: int, episode: Episode, info: Dict) -> None:
         pass
 
     def stats(self) -> EpisodesStats:
         return EpisodesStats(self.episodes)
 
 
 def log_scalars(
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/shared/trajectory.py` & `rl_algo_impls-0.0.8/rl_algo_impls/shared/trajectory.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/train.py` & `rl_algo_impls-0.0.8/rl_algo_impls/train.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os
 
 os.environ["PYTORCH_ENABLE_MPS_FALLBACK"] = "1"
 
 from multiprocessing import Pool
 
 from rl_algo_impls.runner.running_utils import base_parser
-from rl_algo_impls.runner.train import train as runner_train, TrainArgs
+from rl_algo_impls.runner.train import TrainArgs
+from rl_algo_impls.runner.train import train as runner_train
 
 
 def train() -> None:
     parser = base_parser()
     parser.add_argument(
         "--wandb-project-name",
         type=str,
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/tuning/optimize_env.py` & `rl_algo_impls-0.0.8/rl_algo_impls/tuning/optimize_env.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/vpg/policy.py` & `rl_algo_impls-0.0.8/rl_algo_impls/vpg/policy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,51 @@
+from typing import Optional, Sequence, Tuple
+
 import numpy as np
 import torch
 import torch.nn as nn
 
-from typing import Optional, Sequence
-
-from rl_algo_impls.shared.module.feature_extractor import FeatureExtractor
-from rl_algo_impls.shared.policy.actor import (
-    PiForward,
-    Actor,
-    StateDependentNoiseActorHead,
-    actor_head,
-)
+from rl_algo_impls.shared.actor import Actor, PiForward, actor_head
+from rl_algo_impls.shared.encoder import Encoder
 from rl_algo_impls.shared.policy.critic import CriticHead
 from rl_algo_impls.shared.policy.on_policy import (
-    Step,
-    ACForward,
     OnPolicy,
+    Step,
     clamp_actions,
     default_hidden_sizes,
 )
 from rl_algo_impls.shared.policy.policy import ACTIVATION
 from rl_algo_impls.wrappers.vectorable_wrapper import (
     VecEnv,
     VecEnvObs,
-    single_observation_space,
     single_action_space,
+    single_observation_space,
 )
 
 PI_FILE_NAME = "pi.pt"
 V_FILE_NAME = "v.pt"
 
 
 class VPGActor(Actor):
-    def __init__(self, feature_extractor: FeatureExtractor, head: Actor) -> None:
+    def __init__(self, feature_extractor: Encoder, head: Actor) -> None:
         super().__init__()
         self.feature_extractor = feature_extractor
         self.head = head
 
     def forward(self, obs: torch.Tensor, a: Optional[torch.Tensor] = None) -> PiForward:
         fe = self.feature_extractor(obs)
         return self.head(fe, a)
 
+    def sample_weights(self, batch_size: int = 1) -> None:
+        self.head.sample_weights(batch_size=batch_size)
+
+    @property
+    def action_shape(self) -> Tuple[int, ...]:
+        return self.head.action_shape
+
 
 class VPGActorCritic(OnPolicy):
     def __init__(
         self,
         env: VecEnv,
         hidden_sizes: Optional[Sequence[int]] = None,
         init_layers_orthogonal: bool = True,
@@ -64,70 +65,86 @@
 
         hidden_sizes = (
             hidden_sizes
             if hidden_sizes is not None
             else default_hidden_sizes(obs_space)
         )
 
-        pi_feature_extractor = FeatureExtractor(
+        pi_feature_extractor = Encoder(
             obs_space, activation, init_layers_orthogonal=init_layers_orthogonal
         )
         pi_head = actor_head(
             self.action_space,
-            (pi_feature_extractor.out_dim,) + tuple(hidden_sizes),
+            pi_feature_extractor.out_dim,
+            tuple(hidden_sizes),
             init_layers_orthogonal,
             activation,
             log_std_init=log_std_init,
             use_sde=use_sde,
             full_std=full_std,
             squash_output=squash_output,
         )
         self.pi = VPGActor(pi_feature_extractor, pi_head)
 
-        v_feature_extractor = FeatureExtractor(
+        v_feature_extractor = Encoder(
             obs_space, activation, init_layers_orthogonal=init_layers_orthogonal
         )
         v_head = CriticHead(
-            (v_feature_extractor.out_dim,) + tuple(hidden_sizes),
+            v_feature_extractor.out_dim,
+            tuple(hidden_sizes),
             activation=activation,
             init_layers_orthogonal=init_layers_orthogonal,
         )
         self.v = nn.Sequential(v_feature_extractor, v_head)
 
     def value(self, obs: VecEnvObs) -> np.ndarray:
         o = self._as_tensor(obs)
         with torch.no_grad():
             v = self.v(o)
         return v.cpu().numpy()
 
-    def step(self, obs: VecEnvObs) -> Step:
+    def step(self, obs: VecEnvObs, action_masks: Optional[np.ndarray] = None) -> Step:
+        assert (
+            action_masks is None
+        ), f"action_masks not currently supported in {self.__class__.__name__}"
         o = self._as_tensor(obs)
         with torch.no_grad():
             pi, _, _ = self.pi(o)
             a = pi.sample()
             logp_a = pi.log_prob(a)
 
             v = self.v(o)
 
         a_np = a.cpu().numpy()
         clamped_a_np = clamp_actions(a_np, self.action_space, self.squash_output)
         return Step(a_np, v.cpu().numpy(), logp_a.cpu().numpy(), clamped_a_np)
 
-    def act(self, obs: np.ndarray, deterministic: bool = True) -> np.ndarray:
+    def act(
+        self,
+        obs: np.ndarray,
+        deterministic: bool = True,
+        action_masks: Optional[np.ndarray] = None,
+    ) -> np.ndarray:
+        assert (
+            action_masks is None
+        ), f"action_masks not currently supported in {self.__class__.__name__}"
         if not deterministic:
             return self.step(obs).clamped_a
         else:
             o = self._as_tensor(obs)
             with torch.no_grad():
                 pi, _, _ = self.pi(o)
                 a = pi.mode
             return clamp_actions(a.cpu().numpy(), self.action_space, self.squash_output)
 
     def load(self, path: str) -> None:
         super().load(path)
         self.reset_noise()
 
     def reset_noise(self, batch_size: Optional[int] = None) -> None:
-        if isinstance(self.pi.head, StateDependentNoiseActorHead):
-            self.pi.head.sample_weights(
-                batch_size=batch_size if batch_size else self.env.num_envs
-            )
+        self.pi.sample_weights(
+            batch_size=batch_size if batch_size else self.env.num_envs
+        )
+
+    @property
+    def action_shape(self) -> Tuple[int, ...]:
+        return self.pi.action_shape
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/vpg/vpg.py` & `rl_algo_impls-0.0.8/rl_algo_impls/vpg/vpg.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from dataclasses import dataclass, asdict
 from torch.optim import Adam
 from torch.utils.tensorboard.writer import SummaryWriter
 from typing import Optional, Sequence, TypeVar
 
 from rl_algo_impls.shared.algorithm import Algorithm
 from rl_algo_impls.shared.callbacks.callback import Callback
-from rl_algo_impls.shared.gae import compute_rtg_and_advantage, compute_advantage
+from rl_algo_impls.shared.gae import compute_rtg_and_advantage_from_trajectories
 from rl_algo_impls.shared.trajectory import Trajectory, TrajectoryAccumulator
 from rl_algo_impls.vpg.policy import VPGActorCritic
 from rl_algo_impls.wrappers.vectorable_wrapper import VecEnv
 
 
 @dataclass
 class TrainEpochStats:
@@ -54,30 +54,28 @@
         pi_lr: float = 3e-4,
         val_lr: float = 1e-3,
         train_v_iters: int = 80,
         gae_lambda: float = 0.97,
         max_grad_norm: float = 10.0,
         n_steps: int = 4_000,
         sde_sample_freq: int = -1,
-        update_rtg_between_v_iters: bool = False,
         ent_coef: float = 0.0,
     ) -> None:
         super().__init__(policy, env, device, tb_writer)
         self.policy = policy
 
         self.gamma = gamma
         self.gae_lambda = gae_lambda
         self.pi_optim = Adam(self.policy.pi.parameters(), lr=pi_lr)
         self.val_optim = Adam(self.policy.v.parameters(), lr=val_lr)
         self.max_grad_norm = max_grad_norm
 
         self.n_steps = n_steps
         self.train_v_iters = train_v_iters
         self.sde_sample_freq = sde_sample_freq
-        self.update_rtg_between_v_iters = update_rtg_between_v_iters
 
         self.ent_coef = ent_coef
 
     def learn(
         self: VanillaPolicyGradientSelf,
         total_timesteps: int,
         callback: Optional[Callback] = None,
@@ -114,15 +112,15 @@
         self.policy.train()
         obs = torch.as_tensor(
             np.concatenate([np.array(t.obs) for t in trajectories]), device=self.device
         )
         act = torch.as_tensor(
             np.concatenate([np.array(t.act) for t in trajectories]), device=self.device
         )
-        rtg, adv = compute_rtg_and_advantage(
+        rtg, adv = compute_rtg_and_advantage_from_trajectories(
             trajectories, self.policy, self.gamma, self.gae_lambda, self.device
         )
 
         _, logp, entropy = self.policy.pi(obs, act)
         pi_loss = -(logp * adv).mean()
         entropy_loss = entropy.mean()
 
@@ -131,18 +129,14 @@
         self.pi_optim.zero_grad()
         actor_loss.backward()
         nn.utils.clip_grad_norm_(self.policy.pi.parameters(), self.max_grad_norm)
         self.pi_optim.step()
 
         v_loss = 0
         for _ in range(self.train_v_iters):
-            if self.update_rtg_between_v_iters:
-                rtg = compute_advantage(
-                    trajectories, self.policy, self.gamma, self.gae_lambda, self.device
-                )
             v = self.policy.v(obs)
             v_loss = ((v - rtg) ** 2).mean()
 
             self.val_optim.zero_grad()
             v_loss.backward()
             nn.utils.clip_grad_norm_(self.policy.v.parameters(), self.max_grad_norm)
             self.val_optim.step()
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/atari_wrappers.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/atari_wrappers.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/episode_record_video.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/episode_record_video.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/episode_stats_writer.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/episode_stats_writer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,41 @@
-import numpy as np
-
 from collections import deque
+from typing import Any, Dict, List, Optional
+
+import numpy as np
 from torch.utils.tensorboard.writer import SummaryWriter
-from typing import Any, Dict, List
 
 from rl_algo_impls.shared.stats import Episode, EpisodesStats
 from rl_algo_impls.wrappers.vectorable_wrapper import (
-    VecotarableWrapper,
-    VecEnvStepReturn,
     VecEnvObs,
+    VecEnvStepReturn,
+    VecotarableWrapper,
 )
 
 
 class EpisodeStatsWriter(VecotarableWrapper):
     def __init__(
         self,
         env,
         tb_writer: SummaryWriter,
         training: bool = True,
         rolling_length=100,
+        additional_keys_to_log: Optional[List[str]] = None,
     ):
         super().__init__(env)
         self.training = training
         self.tb_writer = tb_writer
         self.rolling_length = rolling_length
         self.episodes = deque(maxlen=rolling_length)
         self.total_steps = 0
         self.episode_cnt = 0
         self.last_episode_cnt_print = 0
+        self.additional_keys_to_log = (
+            additional_keys_to_log if additional_keys_to_log is not None else []
+        )
 
     def step(self, actions: np.ndarray) -> VecEnvStepReturn:
         obs, rews, dones, infos = self.env.step(actions)
         self._record_stats(infos)
         return obs, rews, dones, infos
 
     # Support for stable_baselines3.common.vec_env.VecEnvWrapper
@@ -42,15 +46,16 @@
 
     def _record_stats(self, infos: List[Dict[str, Any]]) -> None:
         self.total_steps += getattr(self.env, "num_envs", 1)
         step_episodes = []
         for info in infos:
             ep_info = info.get("episode")
             if ep_info:
-                episode = Episode(ep_info["r"], ep_info["l"])
+                additional_info = {k: info[k] for k in self.additional_keys_to_log}
+                episode = Episode(ep_info["r"], ep_info["l"], info=additional_info)
                 step_episodes.append(episode)
                 self.episodes.append(episode)
         if step_episodes:
             tag = "train" if self.training else "eval"
             step_stats = EpisodesStats(step_episodes, simple=True)
             step_stats.write_to_tensorboard(self.tb_writer, tag, self.total_steps)
             rolling_stats = EpisodesStats(self.episodes)
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/initial_step_truncate_wrapper.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/initial_step_truncate_wrapper.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/no_reward_timeout.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/no_reward_timeout.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/normalize.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/normalize.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/sync_vector_env_render_compat.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/sync_vector_env_render_compat.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/transpose_image_observation.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/hwc_to_chw_observation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import gym
 import numpy as np
 
 from gym import ObservationWrapper
 from gym.spaces import Box
 
 
-class TransposeImageObservation(ObservationWrapper):
+class HwcToChwObservation(ObservationWrapper):
     def __init__(self, env: gym.Env) -> None:
         super().__init__(env)
 
         assert isinstance(env.observation_space, Box)
 
         obs_space = env.observation_space
         axes = tuple(i for i in range(len(obs_space.shape)))
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/vec_episode_recorder.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/vec_episode_recorder.py`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls/wrappers/vectorable_wrapper.py` & `rl_algo_impls-0.0.8/rl_algo_impls/wrappers/vectorable_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from typing import Dict, List, Optional, Tuple, Type, TypeVar, Union
+
 import numpy as np
 from gym import Env, Space, Wrapper
-
 from stable_baselines3.common.vec_env import VecEnv as SB3VecEnv
-from typing import Dict, List, Optional, Type, TypeVar, Tuple, Union
 
 VecEnvObs = Union[np.ndarray, Dict[str, np.ndarray], Tuple[np.ndarray, ...]]
 VecEnvStepReturn = Tuple[VecEnvObs, np.ndarray, np.ndarray, List[Dict]]
 
 
 class VecotarableWrapper(Wrapper):
     def __init__(self, env: Env) -> None:
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls.egg-info/PKG-INFO` & `rl_algo_impls-0.0.8/rl_algo_impls.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rl-algo-impls
-Version: 0.0.5
+Version: 0.0.8
 Summary: Implementations of reinforcement learning algorithms
 Author-email: Scott Goodfriend <goodfriend.scott@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Scott Goodfriend
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -31,21 +31,31 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: procgen
+Provides-Extra: microrts-old
+Provides-Extra: microrts
+Provides-Extra: jupyter
+Provides-Extra: all
 License-File: LICENSE
 
 # rl-algo-impls
 
 Implementations of reinforcement learning algorithms.
 
-Latest WandB report: https://api.wandb.ai/links/sgoodfriend/6p2sjqtn
+- [WandB benchmark reports](https://wandb.ai/sgoodfriend/rl-algo-impls-benchmarks/reportlist)
+  - [Basic, PyBullet, and Atari games
+    (v0.0.4)](https://api.wandb.ai/links/sgoodfriend/09frjfcs)
+  - [procgen
+    (starpilot, hard)](https://api.wandb.ai/links/sgoodfriend/v1p4976e) and [procgen (easy)](https://api.wandb.ai/links/sgoodfriend/f3w1hwyb)
+  - [Gridnet MicroRTS](https://api.wandb.ai/links/sgoodfriend/zdee7ovm)
+- [Huggingface models](https://huggingface.co/models?other=rl-algo-impls)
 
 ## Prerequisites: Weights & Biases (WandB)
 
 Training and benchmarking assumes you have a Weights & Biases project to upload runs to.
 By default training goes to a rl-algo-impls project while benchmarks go to
 rl-algo-impls-benchmarks. During training and benchmarking runs, videos of the best
 models and the model weights are uploaded to WandB.
@@ -201,7 +211,15 @@
 pip install -e .
 python -c "from procgen import ProcgenGym3Env; ProcgenGym3Env(num=1, env_name='coinrun')"
 python -m procgen.interactive
 ```
 
 amd64 Linux machines (e.g., Lambda Labs and Google Colab) should install procgen with
 `python -m pip install '.[procgen]'`
+
+## gym-microrts Setup
+
+```
+python -m pip install -e '.[microrts]'
+```
+
+Requires Java SDK to also be installed.
```

### Comparing `rl_algo_impls-0.0.5/rl_algo_impls.egg-info/SOURCES.txt` & `rl_algo_impls-0.0.8/rl_algo_impls.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 colab/colab_benchmark.ipynb
 colab/colab_carracing.sh
 colab/colab_enjoy.ipynb
 colab/colab_pybullet.sh
 colab/colab_train.ipynb
 rl_algo_impls/benchmark_publish.py
 rl_algo_impls/compare_runs.py
+rl_algo_impls/enjoy.py
 rl_algo_impls/huggingface_publish.py
 rl_algo_impls/optimize.py
 rl_algo_impls/train.py
 rl_algo_impls.egg-info/PKG-INFO
 rl_algo_impls.egg-info/SOURCES.txt
 rl_algo_impls.egg-info/dependency_links.txt
 rl_algo_impls.egg-info/requires.txt
@@ -35,46 +36,68 @@
 rl_algo_impls/hyperparams/a2c.yml
 rl_algo_impls/hyperparams/dqn.yml
 rl_algo_impls/hyperparams/ppo.yml
 rl_algo_impls/hyperparams/vpg.yml
 rl_algo_impls/ppo/ppo.py
 rl_algo_impls/publish/markdown_format.py
 rl_algo_impls/runner/config.py
-rl_algo_impls/runner/env.py
 rl_algo_impls/runner/evaluate.py
 rl_algo_impls/runner/running_utils.py
 rl_algo_impls/runner/train.py
 rl_algo_impls/shared/algorithm.py
 rl_algo_impls/shared/gae.py
 rl_algo_impls/shared/schedule.py
 rl_algo_impls/shared/stats.py
 rl_algo_impls/shared/trajectory.py
+rl_algo_impls/shared/actor/__init__.py
+rl_algo_impls/shared/actor/actor.py
+rl_algo_impls/shared/actor/categorical.py
+rl_algo_impls/shared/actor/gaussian.py
+rl_algo_impls/shared/actor/gridnet.py
+rl_algo_impls/shared/actor/gridnet_decoder.py
+rl_algo_impls/shared/actor/make_actor.py
+rl_algo_impls/shared/actor/multi_discrete.py
+rl_algo_impls/shared/actor/state_dependent_noise.py
 rl_algo_impls/shared/callbacks/callback.py
 rl_algo_impls/shared/callbacks/eval_callback.py
 rl_algo_impls/shared/callbacks/optimize_callback.py
-rl_algo_impls/shared/module/feature_extractor.py
+rl_algo_impls/shared/encoder/__init__.py
+rl_algo_impls/shared/encoder/cnn.py
+rl_algo_impls/shared/encoder/encoder.py
+rl_algo_impls/shared/encoder/gridnet_encoder.py
+rl_algo_impls/shared/encoder/impala_cnn.py
+rl_algo_impls/shared/encoder/microrts_cnn.py
+rl_algo_impls/shared/encoder/nature_cnn.py
 rl_algo_impls/shared/module/module.py
-rl_algo_impls/shared/policy/actor.py
 rl_algo_impls/shared/policy/critic.py
 rl_algo_impls/shared/policy/on_policy.py
 rl_algo_impls/shared/policy/optimize_on_policy.py
 rl_algo_impls/shared/policy/policy.py
+rl_algo_impls/shared/vec_env/__init__.py
+rl_algo_impls/shared/vec_env/make_env.py
+rl_algo_impls/shared/vec_env/microrts.py
+rl_algo_impls/shared/vec_env/microrts_compat.py
+rl_algo_impls/shared/vec_env/procgen.py
+rl_algo_impls/shared/vec_env/utils.py
+rl_algo_impls/shared/vec_env/vec_env.py
 rl_algo_impls/tuning/optimize_env.py
 rl_algo_impls/vpg/policy.py
 rl_algo_impls/vpg/vpg.py
+rl_algo_impls/wrappers/action_mask_wrapper.py
 rl_algo_impls/wrappers/atari_wrappers.py
 rl_algo_impls/wrappers/episode_record_video.py
 rl_algo_impls/wrappers/episode_stats_writer.py
+rl_algo_impls/wrappers/hwc_to_chw_observation.py
 rl_algo_impls/wrappers/initial_step_truncate_wrapper.py
 rl_algo_impls/wrappers/is_vector_env.py
+rl_algo_impls/wrappers/microrts_stats_recorder.py
 rl_algo_impls/wrappers/no_reward_timeout.py
 rl_algo_impls/wrappers/noop_env_seed.py
 rl_algo_impls/wrappers/normalize.py
 rl_algo_impls/wrappers/sync_vector_env_render_compat.py
-rl_algo_impls/wrappers/transpose_image_observation.py
 rl_algo_impls/wrappers/vec_episode_recorder.py
 rl_algo_impls/wrappers/vectorable_wrapper.py
 rl_algo_impls/wrappers/video_compat_wrapper.py
 scripts/benchmark.sh
 scripts/setup.sh
 scripts/tags_benchmark.sh
 scripts/train_loop.sh
```

### Comparing `rl_algo_impls-0.0.5/scripts/train_loop.sh` & `rl_algo_impls-0.0.8/scripts/train_loop.sh`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/scripts/tuning.sh` & `rl_algo_impls-0.0.8/scripts/tuning.sh`

 * *Files identical despite different names*

### Comparing `rl_algo_impls-0.0.5/tests/shared/policy/test_on_policy.py` & `rl_algo_impls-0.0.8/tests/shared/policy/test_on_policy.py`

 * *Files identical despite different names*

