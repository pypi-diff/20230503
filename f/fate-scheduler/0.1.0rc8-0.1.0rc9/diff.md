# Comparing `tmp/fate-scheduler-0.1.0rc8.tar.gz` & `tmp/fate_scheduler-0.1.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fate-scheduler-0.1.0rc8.tar", max compression
+gzip compressed data, was "fate_scheduler-0.1.0rc9.tar", max compression
```

## Comparing `fate-scheduler-0.1.0rc8.tar` & `fate_scheduler-0.1.0rc9.tar`

### file list

```diff
@@ -1,72 +1,77 @@
--rw-r--r--   0        0        0     1051 2023-04-05 17:18:21.570433 fate-scheduler-0.1.0rc8/pyproject.toml
--rw-r--r--   0        0        0       51 2022-12-14 18:48:24.597216 fate-scheduler-0.1.0rc8/src/fate/__init__.py
--rw-r--r--   0        0        0       59 2022-07-14 16:56:20.397684 fate-scheduler-0.1.0rc8/src/fate/__main__.py
--rw-r--r--   0        0        0      113 2023-02-15 20:13:13.830171 fate-scheduler-0.1.0rc8/src/fate/cli/__init__.py
--rw-r--r--   0        0        0       59 2022-07-14 16:56:20.397684 fate-scheduler-0.1.0rc8/src/fate/cli/__main__.py
--rw-r--r--   0        0        0      144 2023-02-15 20:13:13.830171 fate-scheduler-0.1.0rc8/src/fate/cli/base/__init__.py
--rw-r--r--   0        0        0     3325 2023-02-15 20:13:13.830171 fate-scheduler-0.1.0rc8/src/fate/cli/base/common.py
--rw-r--r--   0        0        0     5924 2023-03-14 22:17:01.873103 fate-scheduler-0.1.0rc8/src/fate/cli/base/execution.py
--rw-r--r--   0        0        0      502 2023-02-15 20:13:13.830171 fate-scheduler-0.1.0rc8/src/fate/cli/base/main.py
--rw-r--r--   0        0        0        0 2022-07-14 16:56:20.397684 fate-scheduler-0.1.0rc8/src/fate/cli/command/__init__.py
--rw-r--r--   0        0        0    13976 2023-04-05 17:08:36.658186 fate-scheduler-0.1.0rc8/src/fate/cli/command/control.py
--rw-r--r--   0        0        0     3277 2023-03-14 21:42:34.614329 fate-scheduler-0.1.0rc8/src/fate/cli/command/debug.py
--rw-r--r--   0        0        0    11526 2023-02-15 20:13:13.834171 fate-scheduler-0.1.0rc8/src/fate/cli/command/init.py
--rw-r--r--   0        0        0      610 2022-12-14 18:48:24.597216 fate-scheduler-0.1.0rc8/src/fate/cli/include/banner/broadway
--rw-r--r--   0        0        0      232 2022-12-14 18:48:24.597216 fate-scheduler-0.1.0rc8/src/fate/cli/include/banner/fire-font-k
--rw-r--r--   0        0        0      237 2022-12-14 18:48:24.597216 fate-scheduler-0.1.0rc8/src/fate/cli/include/banner/larry-3d
--rw-r--r--   0        0        0      897 2023-02-15 20:13:13.834171 fate-scheduler-0.1.0rc8/src/fate/cli/root.py
--rw-r--r--   0        0        0      422 2023-04-05 17:08:36.658186 fate-scheduler-0.1.0rc8/src/fate/conf/__init__.py
--rw-r--r--   0        0        0       96 2022-12-14 18:48:24.597216 fate-scheduler-0.1.0rc8/src/fate/conf/base/__init__.py
--rw-r--r--   0        0        0     3640 2023-02-15 20:13:13.834171 fate-scheduler-0.1.0rc8/src/fate/conf/base/conf.py
--rw-r--r--   0        0        0     3198 2023-02-15 20:13:13.834171 fate-scheduler-0.1.0rc8/src/fate/conf/base/conf_group.py
--rw-r--r--   0        0        0     1379 2023-04-05 17:08:36.658186 fate-scheduler-0.1.0rc8/src/fate/conf/error.py
--rw-r--r--   0        0        0        0 2023-01-24 23:15:24.844720 fate-scheduler-0.1.0rc8/src/fate/conf/include/defaults.toml
--rw-r--r--   0        0        0        0 2023-01-24 23:15:24.844720 fate-scheduler-0.1.0rc8/src/fate/conf/include/defaults.yaml
--rw-r--r--   0        0        0        0 2023-01-24 23:14:51.868976 fate-scheduler-0.1.0rc8/src/fate/conf/include/tasks.toml
--rw-r--r--   0        0        0        0 2023-01-24 23:14:51.868976 fate-scheduler-0.1.0rc8/src/fate/conf/include/tasks.yaml
--rw-r--r--   0        0        0     6461 2023-02-15 20:13:13.834171 fate-scheduler-0.1.0rc8/src/fate/conf/path.py
--rw-r--r--   0        0        0      568 2023-02-28 17:02:51.486625 fate-scheduler-0.1.0rc8/src/fate/conf/schema.py
--rw-r--r--   0        0        0      945 2023-01-04 18:39:38.837686 fate-scheduler-0.1.0rc8/src/fate/conf/template.py
--rw-r--r--   0        0        0      179 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/conf/types/__init__.py
--rw-r--r--   0        0        0      794 2023-01-25 17:58:26.686756 fate-scheduler-0.1.0rc8/src/fate/conf/types/base.py
--rw-r--r--   0        0        0     4254 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/conf/types/default.py
--rw-r--r--   0        0        0    13962 2023-04-05 17:08:36.658186 fate-scheduler-0.1.0rc8/src/fate/conf/types/task.py
--rw-r--r--   0        0        0       65 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/sched/__init__.py
--rw-r--r--   0        0        0      102 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/sched/base/__init__.py
--rw-r--r--   0        0        0     3724 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/sched/base/pool.py
--rw-r--r--   0        0        0     3896 2023-04-05 17:08:36.658186 fate-scheduler-0.1.0rc8/src/fate/sched/base/scheduled_task.py
--rw-r--r--   0        0        0     5165 2023-04-05 17:09:25.117862 fate-scheduler-0.1.0rc8/src/fate/sched/base/scheduler.py
--rw-r--r--   0        0        0        0 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/sched/base/util/__init__.py
--rw-r--r--   0        0        0     2003 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/sched/base/util/reset.py
--rw-r--r--   0        0        0     9648 2023-04-05 17:09:25.117862 fate-scheduler-0.1.0rc8/src/fate/sched/tiered_tenancy.py
--rw-r--r--   0        0        0       64 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/task/__init__.py
--rw-r--r--   0        0        0     4844 2023-01-18 02:36:37.145857 fate-scheduler-0.1.0rc8/src/fate/task/log.py
--rw-r--r--   0        0        0     2314 2023-03-14 22:17:01.873103 fate-scheduler-0.1.0rc8/src/fate/task/param.py
--rw-r--r--   0        0        0      805 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/task/result.py
--rw-r--r--   0        0        0        0 2022-08-16 21:13:09.191404 fate-scheduler-0.1.0rc8/src/fate/util/__init__.py
--rw-r--r--   0        0        0       75 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/abstract.py
--rw-r--r--   0        0        0     3636 2023-02-15 20:13:13.834171 fate-scheduler-0.1.0rc8/src/fate/util/argument.py
--rw-r--r--   0        0        0        0 2022-08-16 21:13:21.110276 fate-scheduler-0.1.0rc8/src/fate/util/compat/__init__.py
--rw-r--r--   0        0        0     1845 2023-02-15 20:13:13.834171 fate-scheduler-0.1.0rc8/src/fate/util/compat/argument.py
--rw-r--r--   0        0        0      589 2023-02-01 23:34:42.365271 fate-scheduler-0.1.0rc8/src/fate/util/compat/os.py
--rw-r--r--   0        0        0      454 2022-08-16 21:16:55.972841 fate-scheduler-0.1.0rc8/src/fate/util/compat/path.py
--rw-r--r--   0        0        0      556 2023-04-05 17:12:33.164628 fate-scheduler-0.1.0rc8/src/fate/util/compat/resources.py
--rw-r--r--   0        0        0       82 2023-01-18 00:20:20.228735 fate-scheduler-0.1.0rc8/src/fate/util/compat/types.py
--rw-r--r--   0        0        0      507 2023-02-01 21:20:36.452543 fate-scheduler-0.1.0rc8/src/fate/util/datastructure/__init__.py
--rw-r--r--   0        0        0     1987 2023-02-01 21:20:36.452543 fate-scheduler-0.1.0rc8/src/fate/util/datastructure/access.py
--rw-r--r--   0        0        0     1937 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/datastructure/collection.py
--rw-r--r--   0        0        0     2519 2023-01-04 21:15:09.039677 fate-scheduler-0.1.0rc8/src/fate/util/datastructure/enum.py
--rw-r--r--   0        0        0     1759 2023-02-01 21:20:36.452543 fate-scheduler-0.1.0rc8/src/fate/util/datastructure/lazy.py
--rw-r--r--   0        0        0     7096 2023-01-04 18:39:38.837686 fate-scheduler-0.1.0rc8/src/fate/util/datastructure/nesting.py
--rw-r--r--   0        0        0     1965 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/event.py
--rw-r--r--   0        0        0     5845 2023-02-28 17:40:11.827893 fate-scheduler-0.1.0rc8/src/fate/util/format.py
--rw-r--r--   0        0        0     1608 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/iteration.py
--rw-r--r--   0        0        0     7170 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/lazy.py
--rw-r--r--   0        0        0       47 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/log/__init__.py
--rw-r--r--   0        0        0     3489 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/log/encoder.py
--rw-r--r--   0        0        0     7517 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/log/logger.py
--rw-r--r--   0        0        0      732 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/os.py
--rw-r--r--   0        0        0      148 2022-12-14 18:48:24.601216 fate-scheduler-0.1.0rc8/src/fate/util/sentinel.py
--rw-r--r--   0        0        0      497 2023-02-15 20:13:13.834171 fate-scheduler-0.1.0rc8/src/fate/util/term.py
--rw-r--r--   0        0        0     1593 2023-04-05 17:18:42.169369 fate-scheduler-0.1.0rc8/setup.py
--rw-r--r--   0        0        0     1034 2023-04-05 17:18:42.169606 fate-scheduler-0.1.0rc8/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-04-12 16:57:14.691447 fate_scheduler-0.1.0rc9/pyproject.toml
+-rw-r--r--   0        0        0       51 2022-12-14 18:48:24.597216 fate_scheduler-0.1.0rc9/src/fate/__init__.py
+-rw-r--r--   0        0        0       59 2022-07-14 16:56:20.397684 fate_scheduler-0.1.0rc9/src/fate/__main__.py
+-rw-r--r--   0        0        0      113 2023-02-15 20:13:13.830171 fate_scheduler-0.1.0rc9/src/fate/cli/__init__.py
+-rw-r--r--   0        0        0       59 2022-07-14 16:56:20.397684 fate_scheduler-0.1.0rc9/src/fate/cli/__main__.py
+-rw-r--r--   0        0        0      144 2023-02-15 20:13:13.830171 fate_scheduler-0.1.0rc9/src/fate/cli/base/__init__.py
+-rw-r--r--   0        0        0     3325 2023-02-15 20:13:13.830171 fate_scheduler-0.1.0rc9/src/fate/cli/base/common.py
+-rw-r--r--   0        0        0     5924 2023-03-14 22:17:01.873103 fate_scheduler-0.1.0rc9/src/fate/cli/base/execution.py
+-rw-r--r--   0        0        0      502 2023-02-15 20:13:13.830171 fate_scheduler-0.1.0rc9/src/fate/cli/base/main.py
+-rw-r--r--   0        0        0        0 2022-07-14 16:56:20.397684 fate_scheduler-0.1.0rc9/src/fate/cli/command/__init__.py
+-rw-r--r--   0        0        0    14135 2023-04-12 16:56:12.791877 fate_scheduler-0.1.0rc9/src/fate/cli/command/control.py
+-rw-r--r--   0        0        0     3277 2023-03-14 21:42:34.614329 fate_scheduler-0.1.0rc9/src/fate/cli/command/debug.py
+-rw-r--r--   0        0        0    11526 2023-02-15 20:13:13.834171 fate_scheduler-0.1.0rc9/src/fate/cli/command/init.py
+-rw-r--r--   0        0        0      610 2022-12-14 18:48:24.597216 fate_scheduler-0.1.0rc9/src/fate/cli/include/banner/broadway
+-rw-r--r--   0        0        0      232 2022-12-14 18:48:24.597216 fate_scheduler-0.1.0rc9/src/fate/cli/include/banner/fire-font-k
+-rw-r--r--   0        0        0      237 2022-12-14 18:48:24.597216 fate_scheduler-0.1.0rc9/src/fate/cli/include/banner/larry-3d
+-rw-r--r--   0        0        0      897 2023-02-15 20:13:13.834171 fate_scheduler-0.1.0rc9/src/fate/cli/root.py
+-rw-r--r--   0        0        0      446 2023-04-12 16:56:12.791877 fate_scheduler-0.1.0rc9/src/fate/conf/__init__.py
+-rw-r--r--   0        0        0       96 2022-12-14 18:48:24.597216 fate_scheduler-0.1.0rc9/src/fate/conf/base/__init__.py
+-rw-r--r--   0        0        0     3640 2023-02-15 20:13:13.834171 fate_scheduler-0.1.0rc9/src/fate/conf/base/conf.py
+-rw-r--r--   0        0        0     3198 2023-02-15 20:13:13.834171 fate_scheduler-0.1.0rc9/src/fate/conf/base/conf_group.py
+-rw-r--r--   0        0        0     1569 2023-04-12 16:56:12.791877 fate_scheduler-0.1.0rc9/src/fate/conf/error.py
+-rw-r--r--   0        0        0        0 2023-01-24 23:15:24.844720 fate_scheduler-0.1.0rc9/src/fate/conf/include/defaults.toml
+-rw-r--r--   0        0        0        0 2023-01-24 23:15:24.844720 fate_scheduler-0.1.0rc9/src/fate/conf/include/defaults.yaml
+-rw-r--r--   0        0        0        0 2023-01-24 23:14:51.868976 fate_scheduler-0.1.0rc9/src/fate/conf/include/tasks.toml
+-rw-r--r--   0        0        0        0 2023-01-24 23:14:51.868976 fate_scheduler-0.1.0rc9/src/fate/conf/include/tasks.yaml
+-rw-r--r--   0        0        0     6461 2023-02-15 20:13:13.834171 fate_scheduler-0.1.0rc9/src/fate/conf/path.py
+-rw-r--r--   0        0        0      568 2023-02-28 17:02:51.486625 fate_scheduler-0.1.0rc9/src/fate/conf/schema.py
+-rw-r--r--   0        0        0      945 2023-01-04 18:39:38.837686 fate_scheduler-0.1.0rc9/src/fate/conf/template.py
+-rw-r--r--   0        0        0      179 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/conf/types/__init__.py
+-rw-r--r--   0        0        0      794 2023-01-25 17:58:26.686756 fate_scheduler-0.1.0rc9/src/fate/conf/types/base.py
+-rw-r--r--   0        0        0     4254 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/conf/types/default.py
+-rw-r--r--   0        0        0    13985 2023-04-12 16:56:12.791877 fate_scheduler-0.1.0rc9/src/fate/conf/types/task.py
+-rw-r--r--   0        0        0       65 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/sched/__init__.py
+-rw-r--r--   0        0        0      102 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/sched/base/__init__.py
+-rw-r--r--   0        0        0     3724 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/sched/base/pool.py
+-rw-r--r--   0        0        0     7440 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/sched/base/scheduled_task.py
+-rw-r--r--   0        0        0     7096 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/sched/base/scheduler.py
+-rw-r--r--   0        0        0     4106 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/sched/base/state.py
+-rw-r--r--   0        0        0     1933 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/sched/base/timing.py
+-rw-r--r--   0        0        0        0 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/sched/base/util/__init__.py
+-rw-r--r--   0        0        0     2003 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/sched/base/util/reset.py
+-rw-r--r--   0        0        0     9655 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/sched/tiered_tenancy.py
+-rw-r--r--   0        0        0       75 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/task/__init__.py
+-rw-r--r--   0        0        0     4844 2023-01-18 02:36:37.145857 fate_scheduler-0.1.0rc9/src/fate/task/log.py
+-rw-r--r--   0        0        0     2314 2023-03-14 22:17:01.873103 fate_scheduler-0.1.0rc9/src/fate/task/param.py
+-rw-r--r--   0        0        0      805 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/task/result.py
+-rw-r--r--   0        0        0       53 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/task/state/__init__.py
+-rw-r--r--   0        0        0     2384 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/task/state/self.py
+-rw-r--r--   0        0        0        0 2022-08-16 21:13:09.191404 fate_scheduler-0.1.0rc9/src/fate/util/__init__.py
+-rw-r--r--   0        0        0       75 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/abstract.py
+-rw-r--r--   0        0        0      303 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/util/animals.py
+-rw-r--r--   0        0        0     3636 2023-02-15 20:13:13.834171 fate_scheduler-0.1.0rc9/src/fate/util/argument.py
+-rw-r--r--   0        0        0        0 2022-08-16 21:13:21.110276 fate_scheduler-0.1.0rc9/src/fate/util/compat/__init__.py
+-rw-r--r--   0        0        0     1845 2023-02-15 20:13:13.834171 fate_scheduler-0.1.0rc9/src/fate/util/compat/argument.py
+-rw-r--r--   0        0        0      589 2023-02-01 23:34:42.365271 fate_scheduler-0.1.0rc9/src/fate/util/compat/os.py
+-rw-r--r--   0        0        0      454 2022-08-16 21:16:55.972841 fate_scheduler-0.1.0rc9/src/fate/util/compat/path.py
+-rw-r--r--   0        0        0      556 2023-04-05 17:32:56.261141 fate_scheduler-0.1.0rc9/src/fate/util/compat/resources.py
+-rw-r--r--   0        0        0       82 2023-01-18 00:20:20.228735 fate_scheduler-0.1.0rc9/src/fate/util/compat/types.py
+-rw-r--r--   0        0        0      522 2023-04-12 16:56:12.795877 fate_scheduler-0.1.0rc9/src/fate/util/datastructure/__init__.py
+-rw-r--r--   0        0        0     1987 2023-02-01 21:20:36.452543 fate_scheduler-0.1.0rc9/src/fate/util/datastructure/access.py
+-rw-r--r--   0        0        0     1937 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/datastructure/collection.py
+-rw-r--r--   0        0        0     2519 2023-01-04 21:15:09.039677 fate_scheduler-0.1.0rc9/src/fate/util/datastructure/enum.py
+-rw-r--r--   0        0        0     1759 2023-02-01 21:20:36.452543 fate_scheduler-0.1.0rc9/src/fate/util/datastructure/lazy.py
+-rw-r--r--   0        0        0     7096 2023-01-04 18:39:38.837686 fate_scheduler-0.1.0rc9/src/fate/util/datastructure/nesting.py
+-rw-r--r--   0        0        0     1965 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/event.py
+-rw-r--r--   0        0        0     5845 2023-02-28 17:40:11.827893 fate_scheduler-0.1.0rc9/src/fate/util/format.py
+-rw-r--r--   0        0        0     1608 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/iteration.py
+-rw-r--r--   0        0        0     7170 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/lazy.py
+-rw-r--r--   0        0        0       47 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/log/__init__.py
+-rw-r--r--   0        0        0     3489 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/log/encoder.py
+-rw-r--r--   0        0        0     7517 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/log/logger.py
+-rw-r--r--   0        0        0      732 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/os.py
+-rw-r--r--   0        0        0      148 2022-12-14 18:48:24.601216 fate_scheduler-0.1.0rc9/src/fate/util/sentinel.py
+-rw-r--r--   0        0        0      497 2023-02-15 20:13:13.834171 fate_scheduler-0.1.0rc9/src/fate/util/term.py
+-rw-r--r--   0        0        0     1224 2023-04-05 17:33:19.768998 fate_scheduler-0.1.0rc9/src/fate/util/timing.py
+-rw-r--r--   0        0        0     1162 1970-01-01 00:00:00.000000 fate_scheduler-0.1.0rc9/PKG-INFO
```

### Comparing `fate-scheduler-0.1.0rc8/pyproject.toml` & `fate_scheduler-0.1.0rc9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 [tool.poetry]
 name = "fate-scheduler"
-version = "0.1.0-rc.8"
+version = "0.1.0-rc.9"
 description = "The operating system-level command scheduler and manager."
 license = "MIT"
 repository = "https://github.com/chicago-cdac/fate"
 authors = [
   "Jesse London <jesselondon@gmail.com>",
   "Kyle MacMillan <macmillan@uchicago.edu>",
 ]
 packages = [{include = "fate", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-argcmdr = "^1.0.0"
+argcmdr = "^1.0.1"
 argcomplete = "^2.0"
 croniter = "^1.3.5"
+Dickens = "^2.1"
 Jinja2 = "^3.1.2"
+lmdb-dict-full = ">=1.0.2"
 loguru = "^0.6.0"
 pyyaml = "^6.0"
 schema = "^0.7.5"
 toml = "^0.10.2"
 wcwidth = "^0.2.5"
 importlib-resources = {version = "5.0", python = ">= 3.8, < 3.10"}
 
 [tool.poetry.dev-dependencies]
 # Note: poetry, et al, currently feature no facility to *do* anything
 # with this optional, dev requirement. rather, this is listed purely as
 # metadata record or note.
-ipdb = {version = "^0.13.9", optional = true}
+ipdb = {version = "^0.13.13", optional = true}
 
 [tool.poetry.scripts]
 fate = "fate:main"
 fates = "fate:serve"
 fated = "fate:daemon"
 
 [build-system]
```

### Comparing `fate-scheduler-0.1.0rc8/src/fate/cli/base/common.py` & `fate_scheduler-0.1.0rc9/src/fate/cli/base/common.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/cli/base/execution.py` & `fate_scheduler-0.1.0rc9/src/fate/cli/base/execution.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/cli/command/control.py` & `fate_scheduler-0.1.0rc9/src/fate/cli/command/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,21 @@
 from fate.util.lazy import lazy_id
 from fate.util.log import StructLogger
 from fate.util.os import pid_exists
 
 from .. import Main
 
 
+def snip(text, length=36, ellipsis=' ...'):
+    if len(text) <= length:
+        return text
+
+    return text[:length - len(ellipsis)] + ellipsis
+
+
 class ControlCommand(Main):
     """Base command class for concrete implementations of the task
     controller command.
 
     """
     # default package resource path at which to look up command banner files
     banner_path = 'fate.cli.include.banner'
@@ -244,15 +251,15 @@
 
         status_record = {
             'status': str(status),
             'exitcode': task.returncode,
         }
 
         if status is self.CommandStatus.Error:
-            logger.error(status_record, stdout=task.stdout, stderr=task.stderr)
+            logger.error(status_record, stdout=snip(task.stdout), stderr=snip(task.stderr))
         else:
             logger.info(status_record)
 
         if status is self.CommandStatus.OK:
             # Write task result (subprocess stdout)
             try:
                 result_path = task.path_.result_()
```

### Comparing `fate-scheduler-0.1.0rc8/src/fate/cli/command/debug.py` & `fate_scheduler-0.1.0rc9/src/fate/cli/command/debug.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/cli/command/init.py` & `fate_scheduler-0.1.0rc9/src/fate/cli/command/init.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/cli/include/banner/broadway` & `fate_scheduler-0.1.0rc9/src/fate/cli/include/banner/broadway`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/cli/root.py` & `fate_scheduler-0.1.0rc9/src/fate/cli/root.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/base/conf.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/base/conf.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/base/conf_group.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/base/conf_group.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/error.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,22 @@
     def __init__(self, format_, errors, identifier):
         super().__init__(format_, errors, identifier)
         self.format = format_
         self.errors = errors
         self.identifier = identifier
 
 
+class StateEncodingError(ValueError, ConfError):
+
+    def __init__(self, format_, error):
+        super().__init__(format_, error)
+        self.format = format_
+        self.error = error
+
+
 class ConfBracketError(ValueError, ConfError):
 
     message = ('expression SHOULD NOT be enclosed by brackets '
                'outside of interpolation context')
 
     def __init__(self, path, evaluation):
         super().__init__(path, evaluation)
```

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/path.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/path.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/schema.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/schema.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/template.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/template.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/types/base.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/types/base.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/types/default.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/types/default.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/conf/types/task.py` & `fate_scheduler-0.1.0rc9/src/fate/conf/types/task.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     _LogDecodingStatus = collections.namedtuple('LogDecodingStatus', ('format', 'errors'))
 
     class _DefaultFormat(StrEnum):
 
         param = 'json'
         log = 'auto'
         result = 'auto'
+        state = 'auto'
 
     class _DefaultScheduling(IntEnum):
 
         tenancy = (2 * cpu_count() - 1)
 
     class _ShellExecutable(StrEnum):
```

### Comparing `fate-scheduler-0.1.0rc8/src/fate/sched/base/pool.py` & `fate_scheduler-0.1.0rc9/src/fate/sched/base/pool.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/sched/base/scheduled_task.py` & `fate_scheduler-0.1.0rc9/src/fate/sched/base/state.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,137 +1,156 @@
-import plumbum
-from descriptors import classonlymethod
+"""Task-state connector"""
+from lmdb_dict import CachedLmdbDict
 
-from fate.conf.error import LogsDecodingError
-from fate.conf.types import TaskConfDict, TaskChainMap
-from fate.util.datastructure import at_depth, adopt
+from fate.conf import ConfValueError, StateEncodingError
 
 
-class ImmediateFailure:
-    """Dummy Future for tasks failing to initialize."""
+class BoundTaskStateManager:
+    """Interface to a `TaskStateManager` bound to a specified task.
 
-    returncode = None
-    stdout = None
-    stderr = None
+    All methods will return results serialized for consumption by the
+    bound task. Methods do not require specification of the requesting
+    task.
 
-    def __init__(self, exc):
-        self.exception = exc
+    """
+    def __init__(self, manager, task):
+        self.manager = manager
+        self.task = task
 
-    @staticmethod
-    def poll():
-        return True
-
-    ready = poll
+    def read(self):
+        return self.manager.read(self.task)
 
+    def write(self, output):
+        self.manager.write(self.task, output)
 
-class ScheduledTask(TaskConfDict):
-    """Task class extended for processing by the operating system."""
+    def read_all(self):
+        return self.manager.read_all(self.task)
 
-    @classonlymethod
-    def schedule(cls, task):
-        """Construct a ScheduledTask extending the specified Task."""
-        self = cls(task)
-        task.__parent__.__adopt__(task.__name__, self)
-        return self
 
-    def __adopt_parent__(self, name, mapping):
-        if mapping.__parent__ is None:
-            mapping.__parent__ = self
-            return
+class TaskStateManager:
+    """Task state input and output in the configured serialization
+    format of the requesting task.
 
-        # we've likely taken over for existing configuration via schedule().
-        # rather than insist that child is in our tree, merely check
-        # that its tree looks the same.
-        assert isinstance(mapping.__parent__, TaskConfDict)
-        assert mapping.__parent__.__path__ == self.__path__
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.__future__ = None
-        self.returncode = None
-        self.stdout = None
-        self.stderr = None
+    Values are cached in memory to avoid redundant serializations.
 
-    def __call__(self):
-        """Execute the task's program in a background process.
+    """
+    class _AutoEncodingError(Exception):
+        pass
 
-        A ScheduledTask may only be executed once -- subsequent
-        invocations are idempotent / no-op.
+    def __init__(self, state_path):
+        self.db = CachedLmdbDict(state_path)
 
-        Returns the execution-initiated ScheduledTask (self).
+        self._l_cache_ = {}
+        self._g_cache_ = {}
 
-        """
-        if self.__future__ is None:
-            try:
-                if isinstance(exec_ := self.exec_, str):
-                    cmd = plumbum.local[exec_]
-                else:
-                    (root, *arguments) = exec_
-                    cmd = plumbum.local[root][arguments]
-            except plumbum.CommandNotFound as exc:
-                future = ImmediateFailure(exc)
-            else:
-                bound = cmd << self.param_
-                future = bound.run_bg()
+    @staticmethod
+    def _format_dump(task):
+        format_ = task.format_['state']
 
-            self.__future__ = future
+        if format_ == 'auto':
+            return task.format_['param']
 
-        return self
+        return format_
 
-    def exception(self):
-        """The in-process exception, raised by Task program
-        initialization, if any.
+    @classmethod
+    def _dump_state(cls, task, data):
+        format_ = cls._format_dump(task)
+
+        try:
+            dumper = task._Dumper[format_]
+        except KeyError:
+            raise ConfValueError(
+                f'{task.__name__}: unsupported state serialization format: '
+                f"{format_!r} (select from: {task._Dumper.__names__})"
+            )
+        else:
+            return dumper(data)
+
+    @classmethod
+    def _load_state(cls, task, output):
+        format_ = task.format_['state']
+
+        try:
+            (data, loader) = task._Loader.autoload(output, format_)
+        except task._Loader.NonAutoError:
+            pass
+        else:
+            if loader is None:
+                raise cls._AutoEncodingError
+
+            return data
+
+        try:
+            loader = task._Loader[format_]
+        except KeyError:
+            raise ConfValueError(
+                task._serializer_error.format(
+                    conf_path=f'{task.__name__}.format.state',
+                    format_=format_,
+                )
+            )
+
+        try:
+            return loader(output)
+        except loader.raises as exc:
+            raise StateEncodingError(format_, exc)
 
-        """
-        return self.__future__.exception if isinstance(self.__future__, ImmediateFailure) else None
+    def bind(self, task):
+        return BoundTaskStateManager(self, task)
 
-    def poll(self):
-        """Return whether the Task program's process has exited.
+    def read(self, task):
+        """Retrieve task's state in its preferred serialization format.
 
-        Sets the ScheduledTask's `returncode`, `stdout` and `stderr`
-        when the process has exited.
+        Returns None if task has stored no state.
 
         """
-        if self.__future__ is None:
-            return False
+        if task.__name__ not in self._l_cache_:
+            data = self.db.get(task.__name__, '')
+
+            if isinstance(data, str):
+                serialization = data
+            else:
+                serialization = self._dump_state(task, data)
 
-        if ready := self.__future__.poll():
-            self.returncode = self.__future__.returncode
-            self.stdout = self.__future__.stdout
-            self.stderr = self.__future__.stderr
+            self._l_cache_[task.__name__] = serialization
 
-        return ready
+            return serialization
 
-    ready = poll
+        return self._l_cache_[task.__name__]
 
-    def logs(self):
-        """Parse LogRecords from `stderr`.
+    def write(self, task, output):
+        """Persist task's written output state.
 
-        Raises LogsDecodingError to indicate decoding errors when the
-        encoding of a task's stderr log output is configured explicitly.
-        Note, in this case, the parsed logs *may still* be retrieved
-        from the exception.
+        Does nothing if written output is empty or if it does not differ
+        from cached state.
 
         """
-        if self.stderr is None:
-            return None
+        if not output or output == self._l_cache_.get(task.__name__):
+            return
+
+        # update caches
+        self._g_cache_.clear()
+        self._l_cache_[task.__name__] = output
+
+        # deserialize output
+        try:
+            data = self._load_state(task, output)
+        except self._AutoEncodingError:
+            data = output
 
-        stream = self._iter_logs_(self.stderr)
-        logs = tuple(stream)
+        # update db
+        self.db[task.__name__] = data
 
-        if stream.status.errors:
-            raise LogsDecodingError(*stream.status, logs)
+    def read_all(self, task):
+        """Serialize all tasks' states in given task's preferred format.
 
-        return logs
+        """
+        format_ = self._format_dump(task)
 
-    @property
-    @adopt('path')
-    def path_(self):
-        default = super().path_
-        return ScheduledTaskChainMap(*default.maps)
+        if format_ not in self._g_cache_:
+            serialization = self._dump_state(task, self.db)
 
+            self._g_cache_[format_] = serialization
 
-class ScheduledTaskChainMap(TaskChainMap):
+            return serialization
 
-    @at_depth('*.path')
-    def result_(self, *args, **kwargs):
-        return self._result_(self.__parent__.stdout, *args, **kwargs)
+        return self._g_cache_[format_]
```

### Comparing `fate-scheduler-0.1.0rc8/src/fate/sched/base/util/reset.py` & `fate_scheduler-0.1.0rc9/src/fate/sched/base/util/reset.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/sched/tiered_tenancy.py` & `fate_scheduler-0.1.0rc9/src/fate/sched/tiered_tenancy.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             while pool.active:
                 min_tenancy = min(get_tenancy(task) for task in pool.iter_tasks())
 
                 if min_tenancy > pool.size:
                     pool.expand(queue.tenancy_tasks(min_tenancy), size=min_tenancy)
                     self.logger.debug(tenancy=pool.size, active=pool.count, msg='expanded pool')
 
-                if time.time() >= self.next_check:
+                if time.time() >= self.timing.next_check:
                     tasks_1 = self.collect_tasks(reset=True)
                     queue.append(tasks_1)
 
                     self.logger.debug(cohort=(len(queue) - 1), size=queue[-1].size,
                                       tenancies=queue[-1].infomap, msg='enqueued cohort')
 
                     count_fill = pool.fill(queue.tenancy_tasks(pool.size))
```

### Comparing `fate-scheduler-0.1.0rc8/src/fate/task/log.py` & `fate_scheduler-0.1.0rc9/src/fate/task/log.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/task/param.py` & `fate_scheduler-0.1.0rc9/src/fate/task/param.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/task/result.py` & `fate_scheduler-0.1.0rc9/src/fate/task/result.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/argument.py` & `fate_scheduler-0.1.0rc9/src/fate/util/argument.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/compat/argument.py` & `fate_scheduler-0.1.0rc9/src/fate/util/compat/argument.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/compat/os.py` & `fate_scheduler-0.1.0rc9/src/fate/util/compat/os.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/compat/resources.py` & `fate_scheduler-0.1.0rc9/src/fate/util/compat/resources.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/datastructure/access.py` & `fate_scheduler-0.1.0rc9/src/fate/util/datastructure/access.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/datastructure/collection.py` & `fate_scheduler-0.1.0rc9/src/fate/util/datastructure/collection.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/datastructure/enum.py` & `fate_scheduler-0.1.0rc9/src/fate/util/datastructure/enum.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/datastructure/lazy.py` & `fate_scheduler-0.1.0rc9/src/fate/util/datastructure/lazy.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/datastructure/nesting.py` & `fate_scheduler-0.1.0rc9/src/fate/util/datastructure/nesting.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/event.py` & `fate_scheduler-0.1.0rc9/src/fate/util/event.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/format.py` & `fate_scheduler-0.1.0rc9/src/fate/util/format.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/iteration.py` & `fate_scheduler-0.1.0rc9/src/fate/util/iteration.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/lazy.py` & `fate_scheduler-0.1.0rc9/src/fate/util/lazy.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/log/encoder.py` & `fate_scheduler-0.1.0rc9/src/fate/util/log/encoder.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/log/logger.py` & `fate_scheduler-0.1.0rc9/src/fate/util/log/logger.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/src/fate/util/os.py` & `fate_scheduler-0.1.0rc9/src/fate/util/os.py`

 * *Files identical despite different names*

### Comparing `fate-scheduler-0.1.0rc8/PKG-INFO` & `fate_scheduler-0.1.0rc9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: fate-scheduler
-Version: 0.1.0rc8
+Version: 0.1.0rc9
 Summary: The operating system-level command scheduler and manager.
 Home-page: https://github.com/chicago-cdac/fate
 License: MIT
 Author: Jesse London
 Author-email: jesselondon@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: Dickens (>=2.1,<3.0)
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: argcmdr (>=1.0.0,<2.0.0)
+Requires-Dist: argcmdr (>=1.0.1,<2.0.0)
 Requires-Dist: argcomplete (>=2.0,<3.0)
 Requires-Dist: croniter (>=1.3.5,<2.0.0)
-Requires-Dist: importlib-resources (==5.0); python_version >= "3.8" and python_version < "3.10"
+Requires-Dist: importlib-resources (==5.0) ; python_version >= "3.8" and python_version < "3.10"
+Requires-Dist: lmdb-dict-full (>=1.0.2)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: schema (>=0.7.5,<0.8.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: wcwidth (>=0.2.5,<0.3.0)
 Project-URL: Repository, https://github.com/chicago-cdac/fate
```

