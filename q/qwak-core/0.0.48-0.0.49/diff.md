# Comparing `tmp/qwak_core-0.0.48.tar.gz` & `tmp/qwak_core-0.0.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.48.tar", max compression
+gzip compressed data, was "qwak_core-0.0.49.tar", max compression
```

## Comparing `qwak_core-0.0.48.tar` & `qwak_core-0.0.49.tar`

### file list

```diff
@@ -1,567 +1,567 @@
--rw-r--r--   0        0        0      264 2023-05-03 14:26:34.233126 qwak_core-0.0.48/README.md
--rw-r--r--   0        0        0        0 2023-05-03 14:28:17.702354 qwak_core-0.0.48/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-03 14:28:17.726354 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-03 14:27:57.862119 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.726354 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-03 14:28:17.722354 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-03 14:27:57.490115 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.722354 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-03 14:28:17.722354 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-03 14:27:57.670117 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.722354 qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-03 14:28:17.714354 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-03 14:27:56.938108 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-03 14:28:17.714354 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-03 14:28:17.718354 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-03 14:27:57.122110 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.718354 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-03 14:28:17.718354 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-03 14:27:57.306112 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.718354 qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-03 14:28:17.702354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-03 14:27:56.746106 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-03 14:28:17.702354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-03 14:28:17.702354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-03 14:27:58.050121 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.706354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-03 14:28:17.710354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-03 14:27:58.418125 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.710354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-03 14:28:17.710354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-03 14:27:58.606128 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-03 14:28:17.710354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-03 14:28:17.706354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-03 14:27:58.234123 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.706354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-03 14:28:17.714354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-03 14:27:58.790130 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.714354 qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-03 14:28:17.790355 qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-03 14:28:01.322160 qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.794355 qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-03 14:28:17.794355 qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-03 14:28:01.502162 qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-03 14:28:17.794355 qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-03 14:28:17.858355 qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-03 14:28:06.518221 qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.858355 qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-03 14:28:17.858355 qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-03 14:28:06.702224 qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-03 14:28:17.862356 qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-03 14:28:17.862356 qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-03 14:28:07.610234 qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-03 14:28:17.866356 qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-03 14:28:17.862356 qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-03 14:28:07.426232 qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.862356 qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-03 14:28:17.866356 qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-03 14:28:07.814237 qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.866356 qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-03 14:28:17.870356 qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-03 14:28:07.994239 qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-03 14:28:17.874356 qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-05-03 14:28:17.930356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-05-03 14:28:13.194300 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.930356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-03 14:28:17.926356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-03 14:28:12.834296 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.926356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-03 14:28:17.930356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-03 14:28:13.010298 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.930356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-03 14:28:17.922356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-03 14:28:12.478292 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-03 14:28:17.922356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-03 14:28:17.926356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-03 14:28:12.658294 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.926356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-03 14:28:17.938356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-03 14:28:13.722307 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.938356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-03 14:28:17.934356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-03 14:28:13.546305 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.934356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-03 14:28:17.934356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-03 14:28:13.370303 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.934356 qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-03 14:28:17.974357 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-03 14:28:17.082346 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.974357 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-03 14:28:17.970357 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-03 14:28:16.698342 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.970357 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-05-03 14:28:17.970357 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-05-03 14:28:16.894344 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-03 14:28:17.974357 qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-03 14:28:17.898356 qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-03 14:28:09.878261 qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-03 14:28:17.898356 qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-03 14:28:17.894356 qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-03 14:28:09.690259 qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.898356 qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-03 14:28:17.886356 qwak_core-0.0.48/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-03 14:28:09.314255 qwak_core-0.0.48/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.886356 qwak_core-0.0.48/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-03 14:28:17.890356 qwak_core-0.0.48/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-03 14:28:09.498257 qwak_core-0.0.48/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.890356 qwak_core-0.0.48/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-03 14:28:17.890356 qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-03 14:28:10.066264 qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-03 14:28:17.894356 qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-03 14:28:17.894356 qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-03 14:28:10.466268 qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-03 14:28:17.894356 qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-03 14:28:17.902356 qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-03 14:28:10.846273 qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.906356 qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-03 14:28:17.906356 qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-03 14:28:11.030275 qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-03 14:28:17.906356 qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-03 14:28:17.882356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-03 14:28:08.762248 qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.882356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-03 14:28:17.882356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-03 14:28:08.946250 qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-03 14:28:17.882356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-03 14:28:17.878356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-03 14:28:08.382243 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.878356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-05-03 14:28:17.874356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-05-03 14:28:08.194241 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.874356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-03 14:28:17.878356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-03 14:28:08.578246 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-03 14:28:17.878356 qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-03 14:28:17.782354 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-03 14:28:00.430149 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.782354 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-03 14:28:17.782354 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-03 14:28:00.610152 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.782354 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-03 14:28:17.786355 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-03 14:28:00.790154 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-03 14:28:17.786355 qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-03 14:28:17.838355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-03 14:28:05.422209 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.842355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-03 14:28:17.838355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-03 14:28:05.238206 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-03 14:28:17.838355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-03 14:28:17.822355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-03 14:28:03.738189 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.822355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-03 14:28:17.818355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-03 14:28:03.554186 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.818355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-03 14:28:17.810355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-03 14:28:02.982180 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.814355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-03 14:28:17.818355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-03 14:28:03.370184 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-03 14:28:17.818355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-03 14:28:17.822355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-03 14:28:03.926191 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.822355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-03 14:28:17.826355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-03 14:28:04.110193 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-03 14:28:17.826355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-05-03 14:28:17.814355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-05-03 14:28:03.174182 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.814355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-03 14:28:17.826355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-03 14:28:04.294195 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.826355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-03 14:28:17.842355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-03 14:28:17.262349 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.842355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-03 14:28:17.842355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-03 14:28:17.450351 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-03 14:28:17.846355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-03 14:28:17.846355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-03 14:28:05.966215 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.846355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-03 14:28:17.846355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-03 14:28:06.154217 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-03 14:28:17.850355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-03 14:28:17.850355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-03 14:28:06.334219 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.850355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-03 14:28:17.854355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-03 14:28:07.066228 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.854355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-03 14:28:17.850355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-03 14:28:06.882226 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-03 14:28:17.854355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-03 14:28:17.854355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-03 14:28:07.242230 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.858355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-03 14:28:17.830355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-03 14:28:04.490198 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.830355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-03 14:28:17.830355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-03 14:28:04.678200 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.830355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-03 14:28:17.834355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-03 14:28:04.866202 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-03 14:28:17.834355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-03 14:28:17.834355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-03 14:28:05.054204 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.834355 qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-03 14:28:17.938356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-03 14:28:13.902309 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.938356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-03 14:28:17.942356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-03 14:28:14.082311 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-03 14:28:17.942356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-03 14:28:17.942356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-03 14:28:14.266313 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.942356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-03 14:28:17.946356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-03 14:28:14.454315 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-03 14:28:17.946356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-03 14:28:17.946356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-03 14:28:14.646318 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-03 14:28:17.946356 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-03 14:28:17.950357 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-03 14:28:14.834320 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.950357 qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-03 14:28:17.906356 qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-03 14:28:11.218277 qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.910356 qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-03 14:28:17.910356 qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-03 14:28:11.394279 qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-03 14:28:17.910356 qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-03 14:28:17.798355 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-03 14:28:02.242171 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.798355 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-03 14:28:17.802355 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-03 14:28:02.422173 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.802355 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-03 14:28:17.806355 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-03 14:28:02.606175 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-03 14:28:17.806355 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-03 14:28:17.806355 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-03 14:28:02.790177 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.810355 qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-03 14:28:17.886356 qwak_core-0.0.48/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-03 14:28:09.126252 qwak_core-0.0.48/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-03 14:28:17.886356 qwak_core-0.0.48/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-03 14:28:17.950357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-03 14:28:15.018322 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.950357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-03 14:28:17.954357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-03 14:28:15.194324 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.954357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-03 14:28:17.954357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-03 14:28:15.382326 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.954357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-03 14:28:17.958357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-03 14:28:15.570328 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.958357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-03 14:28:17.958357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-03 14:28:15.758331 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.958357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-03 14:28:17.962357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-03 14:28:15.962333 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-03 14:28:17.962357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-03 14:28:17.962357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-03 14:28:16.146335 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.966357 qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-03 14:28:17.914356 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-03 14:28:11.750283 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.914356 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-03 14:28:17.918356 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-03 14:28:12.290290 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.922356 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-03 14:28:17.914356 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-03 14:28:11.930286 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-03 14:28:17.918356 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-03 14:28:17.918356 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-03 14:28:12.114288 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.918356 qwak_core-0.0.48/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-03 14:28:17.902356 qwak_core-0.0.48/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-03 14:28:10.662270 qwak_core-0.0.48/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-03 14:28:17.902356 qwak_core-0.0.48/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-03 14:28:17.778355 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-03 14:28:01.870167 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-03 14:28:17.778355 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-03 14:28:17.774355 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-03 14:28:01.686164 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.774355 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-03 14:28:17.778355 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-03 14:28:02.054169 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-03 14:28:17.778355 qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-03 14:28:17.898356 qwak_core-0.0.48/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-03 14:28:10.262266 qwak_core-0.0.48/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-03 14:28:17.902356 qwak_core-0.0.48/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-03 14:28:17.910356 qwak_core-0.0.48/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-03 14:28:11.570281 qwak_core-0.0.48/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-03 14:28:17.914356 qwak_core-0.0.48/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-03 14:28:17.774355 qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-03 14:27:59.698141 qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.774355 qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-03 14:28:17.770354 qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-03 14:27:59.518139 qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-03 14:28:17.770354 qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-03 14:28:17.726354 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-03 14:27:58.974132 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.726354 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-03 14:28:17.730354 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-03 14:27:59.154134 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.730354 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-03 14:28:17.730354 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-03 14:27:59.334137 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-03 14:28:17.730354 qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-03 14:28:17.966357 qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-03 14:28:16.514340 qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-03 14:28:17.970357 qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-03 14:28:17.966357 qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-03 14:28:16.330337 qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.966357 qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-05-03 14:28:17.786355 qwak_core-0.0.48/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-05-03 14:28:00.966156 qwak_core-0.0.48/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.790355 qwak_core-0.0.48/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-03 14:28:17.790355 qwak_core-0.0.48/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-03 14:28:01.142158 qwak_core-0.0.48/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-03 14:28:17.790355 qwak_core-0.0.48/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-03 14:28:19.082370 qwak_core-0.0.48/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-03 14:28:19.082370 qwak_core-0.0.48/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-03 14:26:34.233126 qwak_core-0.0.48/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-03 14:26:34.233126 qwak_core-0.0.48/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0      211 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1263 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     1941 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2987 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1717 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9480 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-03 14:26:34.237126 qwak_core-0.0.48/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      829 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/testing/fixtures.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/tools/__init__.py
--rw-r--r--   0        0        0      107 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/tools/logger/__init__.py
--rw-r--r--   0        0        0     9600 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/tools/logger/logger.py
--rw-r--r--   0        0        0     1941 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak/tools/logger/logging.yml
--rw-r--r--   0        0        0       46 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-03 14:26:34.241126 qwak_core-0.0.48/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.48/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.48/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-03 15:12:45.918559 qwak_core-0.0.49/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 15:14:24.711266 qwak_core-0.0.49/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-03 15:14:24.735266 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-03 15:14:04.387122 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.735266 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-03 15:14:24.731266 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-03 15:14:04.015120 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.731266 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-03 15:14:24.731266 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-03 15:14:04.195121 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.731266 qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-03 15:14:24.723266 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-03 15:14:03.459116 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-03 15:14:24.723266 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-03 15:14:24.727266 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-03 15:14:03.643117 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.727266 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-03 15:14:24.727266 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-03 15:14:03.827118 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.727266 qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-03 15:14:24.711266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-03 15:14:03.275114 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-03 15:14:24.711266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-03 15:14:24.711266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-03 15:14:04.571123 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.715266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-03 15:14:24.715266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-03 15:14:04.939126 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.719266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-03 15:14:24.719266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-03 15:14:05.123128 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-03 15:14:24.719266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-03 15:14:24.715266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-03 15:14:04.755125 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.715266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-03 15:14:24.723266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-03 15:14:05.307129 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.723266 qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-03 15:14:24.763266 qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-03 15:14:07.899147 qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.767266 qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-03 15:14:24.767266 qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-03 15:14:08.087149 qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-03 15:14:24.767266 qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-03 15:14:24.911267 qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-03 15:14:13.223185 qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.915267 qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-03 15:14:24.915267 qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-03 15:14:13.407186 qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-03 15:14:24.915267 qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-03 15:14:24.919268 qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-03 15:14:14.335193 qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-03 15:14:24.919268 qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-03 15:14:24.915267 qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-03 15:14:14.155192 qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.919268 qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-03 15:14:24.923267 qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-03 15:14:14.519194 qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.923267 qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-03 15:14:24.923267 qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-03 15:14:14.703195 qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-03 15:14:24.923267 qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-05-03 15:14:24.987268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-05-03 15:14:19.971233 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.987268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-03 15:14:24.983268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-03 15:14:19.603230 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.983268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-03 15:14:24.983268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-03 15:14:19.787231 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.983268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-03 15:14:24.975268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-03 15:14:19.235227 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-03 15:14:24.979268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-03 15:14:24.979268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-03 15:14:19.419229 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.979268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-03 15:14:24.991268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-03 15:14:20.523236 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.995268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-03 15:14:24.991268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-03 15:14:20.339235 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.991268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-03 15:14:24.987268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-03 15:14:20.155234 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.987268 qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-03 15:14:25.031268 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-03 15:14:23.927260 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.035268 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-03 15:14:25.027268 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-03 15:14:23.547258 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.027268 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-05-03 15:14:25.031268 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-05-03 15:14:23.743259 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-03 15:14:25.031268 qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-03 15:14:24.951268 qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-03 15:14:16.587209 qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-03 15:14:24.951268 qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-03 15:14:24.947268 qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-03 15:14:16.395207 qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.951268 qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-03 15:14:24.939267 qwak_core-0.0.49/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-03 15:14:16.023205 qwak_core-0.0.49/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.939267 qwak_core-0.0.49/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-03 15:14:24.943268 qwak_core-0.0.49/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-03 15:14:16.207206 qwak_core-0.0.49/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.943268 qwak_core-0.0.49/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-03 15:14:24.943268 qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-03 15:14:16.775210 qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-03 15:14:24.943268 qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-03 15:14:24.947268 qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-03 15:14:17.179213 qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-03 15:14:24.947268 qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-03 15:14:24.959268 qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-03 15:14:17.563216 qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.959268 qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-03 15:14:24.959268 qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-03 15:14:17.751217 qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-03 15:14:24.959268 qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-03 15:14:24.931268 qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-03 15:14:15.463201 qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.935268 qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-03 15:14:24.935268 qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-03 15:14:15.647202 qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-03 15:14:24.935268 qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-03 15:14:24.927267 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-03 15:14:15.083198 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.927267 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-05-03 15:14:24.927267 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-05-03 15:14:14.899197 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.927267 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-03 15:14:24.931268 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-03 15:14:15.279199 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-03 15:14:24.931268 qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-03 15:14:24.755266 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-03 15:14:06.971141 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.755266 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-03 15:14:24.755266 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-03 15:14:07.155142 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.755266 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-03 15:14:24.759266 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-03 15:14:07.343143 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-03 15:14:24.759266 qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-03 15:14:24.895267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-03 15:14:12.111177 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.895267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-03 15:14:24.891267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-03 15:14:11.923176 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-03 15:14:24.891267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-03 15:14:24.875267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-03 15:14:10.331164 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.875267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-03 15:14:24.871267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-03 15:14:10.151163 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.871267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-03 15:14:24.863267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-03 15:14:09.575159 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.867267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-03 15:14:24.867267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-03 15:14:09.963162 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-03 15:14:24.871267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-03 15:14:24.875267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-03 15:14:10.519166 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.875267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-03 15:14:24.879267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-03 15:14:10.703167 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-03 15:14:24.879267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-05-03 15:14:24.867267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-05-03 15:14:09.771160 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.867267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-03 15:14:24.879267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-03 15:14:10.883168 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.883267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-03 15:14:24.895267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-03 15:14:24.135262 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.895267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-03 15:14:24.899267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-03 15:14:24.355264 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-03 15:14:24.899267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-03 15:14:24.899267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-03 15:14:12.671181 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.899267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-03 15:14:24.903267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-03 15:14:12.855182 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-03 15:14:24.903267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-03 15:14:24.903267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-03 15:14:13.039183 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.903267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-03 15:14:24.907267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-03 15:14:13.783189 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.911267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-03 15:14:24.907267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-03 15:14:13.595188 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-03 15:14:24.907267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-03 15:14:24.911267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-03 15:14:13.967190 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.911267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-03 15:14:24.883267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-03 15:14:11.075170 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.883267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-03 15:14:24.883267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-03 15:14:11.323171 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.887267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-03 15:14:24.887267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-03 15:14:11.551173 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-03 15:14:24.887267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-03 15:14:24.887267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-03 15:14:11.739174 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.891267 qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-03 15:14:24.995268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-03 15:14:20.707238 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.995268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-03 15:14:24.995268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-03 15:14:20.899239 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-03 15:14:24.999268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-03 15:14:24.999268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-03 15:14:21.091241 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.999268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-03 15:14:25.003268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-03 15:14:21.283242 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-03 15:14:25.003268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-03 15:14:25.003268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-03 15:14:21.475243 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-03 15:14:25.003268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-03 15:14:25.007268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-03 15:14:21.659244 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.007268 qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-03 15:14:24.963268 qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-03 15:14:17.935218 qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.963268 qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-03 15:14:24.963268 qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-03 15:14:18.123220 qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-03 15:14:24.963268 qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-03 15:14:24.787267 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-03 15:14:08.839154 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.799267 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-03 15:14:24.811267 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-03 15:14:09.023155 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.823267 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-03 15:14:24.835267 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-03 15:14:09.207157 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-03 15:14:24.843267 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-03 15:14:24.855267 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-03 15:14:09.387158 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.863267 qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-03 15:14:24.935268 qwak_core-0.0.49/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-03 15:14:15.831203 qwak_core-0.0.49/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-03 15:14:24.939267 qwak_core-0.0.49/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-03 15:14:25.007268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-03 15:14:21.843246 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.007268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-03 15:14:25.011268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-03 15:14:22.027247 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.011268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-03 15:14:25.011268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-03 15:14:22.219248 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.015268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-03 15:14:25.015268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-03 15:14:22.407250 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.015268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-03 15:14:25.015268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-03 15:14:22.603251 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.019268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-03 15:14:25.019268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-03 15:14:22.807253 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-03 15:14:25.019268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-03 15:14:25.023268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-03 15:14:22.991254 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.023268 qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-03 15:14:24.967268 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-03 15:14:18.495222 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.971268 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-03 15:14:24.975268 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-03 15:14:19.047226 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.975268 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-03 15:14:24.971268 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-03 15:14:18.679223 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-03 15:14:24.971268 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-03 15:14:24.971268 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-03 15:14:18.867225 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.975268 qwak_core-0.0.49/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-03 15:14:24.955268 qwak_core-0.0.49/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-03 15:14:17.379214 qwak_core-0.0.49/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-03 15:14:24.955268 qwak_core-0.0.49/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-03 15:14:24.751266 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-03 15:14:08.467151 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-03 15:14:24.751266 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-03 15:14:24.747266 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-03 15:14:08.279150 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.747266 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-03 15:14:24.751266 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-03 15:14:08.655152 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-03 15:14:24.751266 qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-03 15:14:24.951268 qwak_core-0.0.49/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-03 15:14:16.971211 qwak_core-0.0.49/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-03 15:14:24.955268 qwak_core-0.0.49/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-03 15:14:24.967268 qwak_core-0.0.49/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-03 15:14:18.307221 qwak_core-0.0.49/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-03 15:14:24.967268 qwak_core-0.0.49/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-03 15:14:24.743266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-03 15:14:06.231135 qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.747266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-03 15:14:24.743266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-03 15:14:06.043134 qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-03 15:14:24.743266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-03 15:14:24.735266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-03 15:14:05.487130 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.739266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-03 15:14:24.739266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-03 15:14:05.671131 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.739266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-03 15:14:24.739266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-03 15:14:05.855133 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-03 15:14:24.743266 qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-03 15:14:25.027268 qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-03 15:14:23.363257 qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-03 15:14:25.027268 qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-03 15:14:25.023268 qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-03 15:14:23.179255 qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:25.023268 qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-05-03 15:14:24.759266 qwak_core-0.0.49/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-05-03 15:14:07.527145 qwak_core-0.0.49/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.763266 qwak_core-0.0.49/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-03 15:14:24.763266 qwak_core-0.0.49/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-03 15:14:07.711146 qwak_core-0.0.49/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 15:14:24.763266 qwak_core-0.0.49/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-03 15:14:26.619279 qwak_core-0.0.49/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-03 15:14:26.623279 qwak_core-0.0.49/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0      211 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-03 15:12:45.922559 qwak_core-0.0.49/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9480 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      829 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/tools/__init__.py
+-rw-r--r--   0        0        0      107 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/tools/logger/__init__.py
+-rw-r--r--   0        0        0     9598 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/tools/logger/logger.py
+-rw-r--r--   0        0        0     1941 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak/tools/logger/logging.yml
+-rw-r--r--   0        0        0       46 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-03 15:12:45.926559 qwak_core-0.0.49/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-03 15:12:45.930559 qwak_core-0.0.49/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4910 1970-01-01 00:00:00.000000 qwak_core-0.0.49/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.49/PKG-INFO
```

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.49/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.49/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/pyproject.toml` & `qwak_core-0.0.49/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.48"
+version = "0.0.49"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.48/qwak/automations/__init__.py` & `qwak_core-0.0.49/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/automations/automation_executions.py` & `qwak_core-0.0.49/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/automations/automations.py` & `qwak_core-0.0.49/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.49/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.49/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.49/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.49/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.49/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/alert_management/client.py` & `qwak_core-0.0.49/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/analytics/client.py` & `qwak_core-0.0.49/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/audience/client.py` & `qwak_core-0.0.49/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/automation_management/client.py` & `qwak_core-0.0.49/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.49/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.49/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.49/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.49/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/build_management/client.py` & `qwak_core-0.0.49/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.49/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.49/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/deployment/client.py` & `qwak_core-0.0.49/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.49/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.49/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.49/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.49/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.49/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/logging_client/client.py` & `qwak_core-0.0.49/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/model_management/client.py` & `qwak_core-0.0.49/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/project/client.py` & `qwak_core-0.0.49/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/secret_service/client.py` & `qwak_core-0.0.49/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.49/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.49/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.49/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.49/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.49/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/parquet.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/postgres.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.49/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.49/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.49/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.49/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.49/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.49/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.49/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.49/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.49/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.49/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/offline/client.py` & `qwak_core-0.0.49/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/feature_store/online/client.py` & `qwak_core-0.0.49/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/const.py` & `qwak_core-0.0.49/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.49/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.49/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.49/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.49/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/singleton_meta.py` & `qwak_core-0.0.49/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/tool/auth.py` & `qwak_core-0.0.49/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.49/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.49/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.49/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.49/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/adapters/__init__.py` & `qwak_core-0.0.49/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.49/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.49/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.49/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.49/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.49/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/base.py` & `qwak_core-0.0.49/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/decorators/api.py` & `qwak_core-0.0.49/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.49/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/experiment_tracking.py` & `qwak_core-0.0.49/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/schema.py` & `qwak_core-0.0.49/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/schema_entities.py` & `qwak_core-0.0.49/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.49/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.49/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.49/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.49/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.49/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.49/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.49/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.49/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/qwak_client/client.py` & `qwak_core-0.0.49/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.49/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/qwak_client/models/model.py` & `qwak_core-0.0.49/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.49/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.49/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak/tools/logger/logger.py` & `qwak_core-0.0.49/qwak/tools/logger/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,16 @@
                 )
             else:
                 existing_handlers = existing_logger.handlers
             existing_logger.handlers = existing_handlers + requested_logger_handlers
 
 
 def get_qwak_logger(
-    logger_name: Optional[str] = None, fallback_logger_name: Optional[str] = None
+    logger_name: Optional[str] = None,
+    fallback_logger_name: Optional[str] = DEFAULT_LOGGER_NAME,
 ) -> logging.Logger:
     """Get qwak logger (Singleton)
     :param logger_name: logger name to get
     :param fallback_logger_name: fallback logger name to get if logger_name is not defined
 
     Returns:
         logging.Logger: Qwak logger.
@@ -183,15 +184,15 @@
 
     if (logger_name not in DEFINED_LOGGER_NAMES) and not non_qwak_logger_enabled():
         print(LOGGER_NOT_FOUND_MESSAGE.format(logger_name=logger_name))
 
     return logging.getLogger(logger_name)
 
 
-def get_qwak_logger_name(fallback_logger_name: str = DEFAULT_LOGGER_NAME) -> str:
+def get_qwak_logger_name(fallback_logger_name: str) -> str:
     return os.getenv(ENVIRON_LOGGER_TYPE, fallback_logger_name)
 
 
 def non_qwak_logger_enabled() -> bool:
     return os.getenv(AIRFLOW_ENV_FLAG) is not None
```

### Comparing `qwak_core-0.0.48/qwak/tools/logger/logging.yml` & `qwak_core-0.0.49/qwak/tools/logger/logging.yml`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.49/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/qwak_services_mock/services_mock.py` & `qwak_core-0.0.49/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.48/setup.py` & `qwak_core-0.0.49/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.48',
+    'version': '0.0.49',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.48/PKG-INFO` & `qwak_core-0.0.49/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.48
+Version: 0.0.49
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

