# Comparing `tmp/qwak_core-0.0.42.tar.gz` & `tmp/qwak_core-0.0.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_core-0.0.42.tar", max compression
+gzip compressed data, was "qwak_core-0.0.43.tar", max compression
```

## Comparing `qwak_core-0.0.42.tar` & `qwak_core-0.0.43.tar`

### file list

```diff
@@ -1,563 +1,563 @@
--rw-r--r--   0        0        0      264 2023-05-02 20:09:52.767386 qwak_core-0.0.42/README.md
--rw-r--r--   0        0        0        0 2023-05-02 20:11:35.111852 qwak_core-0.0.42/_qwak_proto/__init__.py
--rw-r--r--   0        0        0     5378 2023-05-02 20:11:35.135852 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/account_pb2.py
--rw-r--r--   0        0        0     6623 2023-05-02 20:11:14.247757 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.135852 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
--rw-r--r--   0        0        0     2390 2023-05-02 20:11:35.131852 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
--rw-r--r--   0        0        0     1475 2023-05-02 20:11:13.863755 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.131852 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     2106 2023-05-02 20:11:35.131852 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
--rw-r--r--   0        0        0     1207 2023-05-02 20:11:14.055756 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.135852 qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
--rw-r--r--   0        0        0     6751 2023-05-02 20:11:35.123852 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
--rw-r--r--   0        0        0     4346 2023-05-02 20:11:13.279753 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
--rw-r--r--   0        0        0     7662 2023-05-02 20:11:35.127852 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-02 20:11:35.127852 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
--rw-r--r--   0        0        0     2650 2023-05-02 20:11:13.475753 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.127852 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
--rw-r--r--   0        0        0     4864 2023-05-02 20:11:35.127852 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
--rw-r--r--   0        0        0     5792 2023-05-02 20:11:13.667754 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.131852 qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
--rw-r--r--   0        0        0     4635 2023-05-02 20:11:35.111852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
--rw-r--r--   0        0        0     3664 2023-05-02 20:11:13.087752 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
--rw-r--r--   0        0        0     3167 2023-05-02 20:11:35.111852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
--rw-r--r--   0        0        0     5670 2023-05-02 20:11:35.115852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
--rw-r--r--   0        0        0     8035 2023-05-02 20:11:14.435758 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.115852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
--rw-r--r--   0        0        0     4512 2023-05-02 20:11:35.119852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
--rw-r--r--   0        0        0     5690 2023-05-02 20:11:14.819759 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.119852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
--rw-r--r--   0        0        0    16001 2023-05-02 20:11:35.119852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
--rw-r--r--   0        0        0    12387 2023-05-02 20:11:15.015761 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
--rw-r--r--   0        0        0    16458 2023-05-02 20:11:35.123852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2464 2023-05-02 20:11:35.115852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
--rw-r--r--   0        0        0     1347 2023-05-02 20:11:14.631759 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.115852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
--rw-r--r--   0        0        0     6425 2023-05-02 20:11:35.123852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/users/user_pb2.py
--rw-r--r--   0        0        0    10323 2023-05-02 20:11:15.211761 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.123852 qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
--rw-r--r--   0        0        0     9577 2023-05-02 20:11:35.167852 qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
--rw-r--r--   0        0        0    13624 2023-05-02 20:11:18.007774 qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.167852 qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
--rw-r--r--   0        0        0     9270 2023-05-02 20:11:35.167852 qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
--rw-r--r--   0        0        0     5571 2023-05-02 20:11:18.207775 qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
--rw-r--r--   0        0        0    10742 2023-05-02 20:11:35.167852 qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
--rw-r--r--   0        0        0     7365 2023-05-02 20:11:35.235853 qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_pb2.py
--rw-r--r--   0        0        0    11839 2023-05-02 20:11:23.431799 qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.239853 qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
--rw-r--r--   0        0        0     9396 2023-05-02 20:11:35.239853 qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_service_pb2.py
--rw-r--r--   0        0        0     7896 2023-05-02 20:11:23.623800 qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
--rw-r--r--   0        0        0    11917 2023-05-02 20:11:35.239853 qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
--rw-r--r--   0        0        0     9021 2023-05-02 20:11:35.243853 qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
--rw-r--r--   0        0        0     5865 2023-05-02 20:11:24.583804 qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
--rw-r--r--   0        0        0    11486 2023-05-02 20:11:35.243853 qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
--rw-r--r--   0        0        0     8807 2023-05-02 20:11:35.239853 qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_pb2.py
--rw-r--r--   0        0        0    13570 2023-05-02 20:11:24.395803 qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.243853 qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
--rw-r--r--   0        0        0     5497 2023-05-02 20:11:35.247853 qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7820 2023-05-02 20:11:24.779805 qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.247853 qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     2937 2023-05-02 20:11:35.247853 qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
--rw-r--r--   0        0        0     2014 2023-05-02 20:11:24.971806 qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
--rw-r--r--   0        0        0     2991 2023-05-02 20:11:35.247853 qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
--rw-r--r--   0        0        0    11441 2023-05-02 20:11:35.307853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/action_pb2.py
--rw-r--r--   0        0        0    17892 2023-05-02 20:11:30.363831 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.311853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
--rw-r--r--   0        0        0     5494 2023-05-02 20:11:35.303853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
--rw-r--r--   0        0        0     7776 2023-05-02 20:11:29.979829 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.307853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
--rw-r--r--   0        0        0     3373 2023-05-02 20:11:35.307853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
--rw-r--r--   0        0        0     4400 2023-05-02 20:11:30.171830 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.307853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
--rw-r--r--   0        0        0    17887 2023-05-02 20:11:35.299853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
--rw-r--r--   0        0        0    12310 2023-05-02 20:11:29.603827 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
--rw-r--r--   0        0        0    23338 2023-05-02 20:11:35.303853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
--rw-r--r--   0        0        0     3873 2023-05-02 20:11:35.303853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_pb2.py
--rw-r--r--   0        0        0     5291 2023-05-02 20:11:29.795828 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.303853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
--rw-r--r--   0        0        0     2383 2023-05-02 20:11:35.315853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/common_pb2.py
--rw-r--r--   0        0        0     2446 2023-05-02 20:11:30.935833 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/common_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.315853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
--rw-r--r--   0        0        0     5209 2023-05-02 20:11:35.315853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/notification_pb2.py
--rw-r--r--   0        0        0     5492 2023-05-02 20:11:30.743832 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.315853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
--rw-r--r--   0        0        0     4210 2023-05-02 20:11:35.311853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/trigger_pb2.py
--rw-r--r--   0        0        0     4746 2023-05-02 20:11:30.555832 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.311853 qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
--rw-r--r--   0        0        0    10275 2023-05-02 20:11:35.355853 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
--rw-r--r--   0        0        0    14803 2023-05-02 20:11:34.459849 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.355853 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
--rw-r--r--   0        0        0     2042 2023-05-02 20:11:35.351853 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
--rw-r--r--   0        0        0     1904 2023-05-02 20:11:34.071848 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.351853 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
--rw-r--r--   0        0        0    37419 2023-05-02 20:11:35.355853 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
--rw-r--r--   0        0        0    48027 2023-05-02 20:11:34.271849 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
--rw-r--r--   0        0        0    29918 2023-05-02 20:11:35.355853 qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
--rw-r--r--   0        0        0    18658 2023-05-02 20:11:35.275853 qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_api_pb2.py
--rw-r--r--   0        0        0    15525 2023-05-02 20:11:26.915815 qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
--rw-r--r--   0        0        0    18652 2023-05-02 20:11:35.275853 qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
--rw-r--r--   0        0        0    16953 2023-05-02 20:11:35.271853 qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_pb2.py
--rw-r--r--   0        0        0    25941 2023-05-02 20:11:26.719814 qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.271853 qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
--rw-r--r--   0        0        0    11034 2023-05-02 20:11:35.263853 qwak_core-0.0.42/_qwak_proto/qwak/builds/build_pb2.py
--rw-r--r--   0        0        0    18276 2023-05-02 20:11:26.339812 qwak_core-0.0.42/_qwak_proto/qwak/builds/build_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.263853 qwak_core-0.0.42/_qwak_proto/qwak/builds/build_pb2_grpc.py
--rw-r--r--   0        0        0     4777 2023-05-02 20:11:35.263853 qwak_core-0.0.42/_qwak_proto/qwak/builds/build_url_pb2.py
--rw-r--r--   0        0        0     5773 2023-05-02 20:11:26.527813 qwak_core-0.0.42/_qwak_proto/qwak/builds/build_url_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.267853 qwak_core-0.0.42/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
--rw-r--r--   0        0        0    12490 2023-05-02 20:11:35.267853 qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
--rw-r--r--   0        0        0     9351 2023-05-02 20:11:27.103816 qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
--rw-r--r--   0        0        0    14916 2023-05-02 20:11:35.267853 qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
--rw-r--r--   0        0        0    38245 2023-05-02 20:11:35.271853 qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_pb2.py
--rw-r--r--   0        0        0    52572 2023-05-02 20:11:27.511818 qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_pb2.pyi
--rw-r--r--   0        0        0    11572 2023-05-02 20:11:35.271853 qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_pb2_grpc.py
--rw-r--r--   0        0        0     1671 2023-05-02 20:11:35.279853 qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
--rw-r--r--   0        0        0     1689 2023-05-02 20:11:27.907819 qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.283853 qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4328 2023-05-02 20:11:35.283853 qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-02 20:11:28.095820 qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-02 20:11:35.283853 qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     7716 2023-05-02 20:11:35.255853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_pb2.py
--rw-r--r--   0        0        0    11197 2023-05-02 20:11:25.763810 qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.259853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
--rw-r--r--   0        0        0    11580 2023-05-02 20:11:35.259853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_service_pb2.py
--rw-r--r--   0        0        0     7373 2023-05-02 20:11:25.959811 qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
--rw-r--r--   0        0        0    12803 2023-05-02 20:11:35.259853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
--rw-r--r--   0        0        0     2162 2023-05-02 20:11:35.251853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
--rw-r--r--   0        0        0     2685 2023-05-02 20:11:25.371808 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.251853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
--rw-r--r--   0        0        0    42956 2023-05-02 20:11:35.251853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_pb2.py
--rw-r--r--   0        0        0    62847 2023-05-02 20:11:25.175807 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.251853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    38320 2023-05-02 20:11:35.255853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_service_pb2.py
--rw-r--r--   0        0        0    33325 2023-05-02 20:11:25.575809 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
--rw-r--r--   0        0        0    20242 2023-05-02 20:11:35.255853 qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
--rw-r--r--   0        0        0     2527 2023-05-02 20:11:35.155852 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
--rw-r--r--   0        0        0     2791 2023-05-02 20:11:16.943769 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.155852 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-02 20:11:35.155852 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
--rw-r--r--   0        0        0    12641 2023-05-02 20:11:17.135770 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.159853 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
--rw-r--r--   0        0        0    16366 2023-05-02 20:11:35.159853 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
--rw-r--r--   0        0        0    17148 2023-05-02 20:11:17.327771 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
--rw-r--r--   0        0        0    10706 2023-05-02 20:11:35.159853 qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
--rw-r--r--   0        0        0     4787 2023-05-02 20:11:35.215853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
--rw-r--r--   0        0        0     6713 2023-05-02 20:11:22.283794 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.219853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
--rw-r--r--   0        0        0     9721 2023-05-02 20:11:35.215853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
--rw-r--r--   0        0        0     7409 2023-05-02 20:11:22.095793 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
--rw-r--r--   0        0        0    12256 2023-05-02 20:11:35.215853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
--rw-r--r--   0        0        0     9535 2023-05-02 20:11:35.199853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
--rw-r--r--   0        0        0    10460 2023-05-02 20:11:20.563786 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.199853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
--rw-r--r--   0        0        0     5268 2023-05-02 20:11:35.195853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/execution_pb2.py
--rw-r--r--   0        0        0     8525 2023-05-02 20:11:20.371785 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.195853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
--rw-r--r--   0        0        0    10074 2023-05-02 20:11:35.187853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
--rw-r--r--   0        0        0    14303 2023-05-02 20:11:19.779782 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.191853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
--rw-r--r--   0        0        0    27847 2023-05-02 20:11:35.191853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
--rw-r--r--   0        0        0    20073 2023-05-02 20:11:20.183784 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
--rw-r--r--   0        0        0    33080 2023-05-02 20:11:35.195853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
--rw-r--r--   0        0        0    12638 2023-05-02 20:11:35.199853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
--rw-r--r--   0        0        0    14071 2023-05-02 20:11:20.759787 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.199853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
--rw-r--r--   0        0        0    10044 2023-05-02 20:11:35.203853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
--rw-r--r--   0        0        0     6846 2023-05-02 20:11:20.947788 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
--rw-r--r--   0        0        0    11647 2023-05-02 20:11:35.203853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
--rw-r--r--   0        0        0    24876 2023-05-02 20:11:35.191853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
--rw-r--r--   0        0        0    36861 2023-05-02 20:11:19.979783 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.191853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
--rw-r--r--   0        0        0     2872 2023-05-02 20:11:35.203853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
--rw-r--r--   0        0        0     2428 2023-05-02 20:11:21.135789 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.203853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
--rw-r--r--   0        0        0     4196 2023-05-02 20:11:35.219853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
--rw-r--r--   0        0        0     7323 2023-05-02 20:11:34.651850 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.219853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
--rw-r--r--   0        0        0     9895 2023-05-02 20:11:35.223853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
--rw-r--r--   0        0        0     9029 2023-05-02 20:11:34.843851 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
--rw-r--r--   0        0        0    12090 2023-05-02 20:11:35.223853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     3596 2023-05-02 20:11:35.223853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
--rw-r--r--   0        0        0     6664 2023-05-02 20:11:22.851796 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.223853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
--rw-r--r--   0        0        0    11930 2023-05-02 20:11:35.227853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
--rw-r--r--   0        0        0    11052 2023-05-02 20:11:23.043797 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
--rw-r--r--   0        0        0    14459 2023-05-02 20:11:35.227853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
--rw-r--r--   0        0        0     5158 2023-05-02 20:11:35.227853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/reports/report_pb2.py
--rw-r--r--   0        0        0     7436 2023-05-02 20:11:23.239798 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.227853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
--rw-r--r--   0        0        0     4549 2023-05-02 20:11:35.231853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
--rw-r--r--   0        0        0     6442 2023-05-02 20:11:24.011802 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.235853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
--rw-r--r--   0        0        0    16693 2023-05-02 20:11:35.231853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
--rw-r--r--   0        0        0    20355 2023-05-02 20:11:23.815801 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
--rw-r--r--   0        0        0     4809 2023-05-02 20:11:35.231853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
--rw-r--r--   0        0        0     2553 2023-05-02 20:11:35.235853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
--rw-r--r--   0        0        0     4000 2023-05-02 20:11:24.203802 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.235853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
--rw-r--r--   0        0        0    14046 2023-05-02 20:11:35.207853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
--rw-r--r--   0        0        0    23615 2023-05-02 20:11:21.331789 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.207853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
--rw-r--r--   0        0        0     5087 2023-05-02 20:11:35.207853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
--rw-r--r--   0        0        0     6011 2023-05-02 20:11:21.523790 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.211853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
--rw-r--r--   0        0        0    12309 2023-05-02 20:11:35.211853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
--rw-r--r--   0        0        0     9244 2023-05-02 20:11:21.719791 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
--rw-r--r--   0        0        0    17071 2023-05-02 20:11:35.211853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
--rw-r--r--   0        0        0    11014 2023-05-02 20:11:35.211853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
--rw-r--r--   0        0        0    15865 2023-05-02 20:11:21.907792 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.215853 qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
--rw-r--r--   0        0        0     4727 2023-05-02 20:11:35.319853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
--rw-r--r--   0        0        0     5122 2023-05-02 20:11:31.123834 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.319853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4648 2023-05-02 20:11:35.319853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4170 2023-05-02 20:11:31.307835 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-02 20:11:35.319853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     5349 2023-05-02 20:11:35.323853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
--rw-r--r--   0        0        0     5363 2023-05-02 20:11:31.499836 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.323853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     4437 2023-05-02 20:11:35.323853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
--rw-r--r--   0        0        0     4127 2023-05-02 20:11:31.695837 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
--rw-r--r--   0        0        0     5151 2023-05-02 20:11:35.323853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
--rw-r--r--   0        0        0     6073 2023-05-02 20:11:35.327853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
--rw-r--r--   0        0        0     5366 2023-05-02 20:11:31.911838 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
--rw-r--r--   0        0        0     7395 2023-05-02 20:11:35.327853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
--rw-r--r--   0        0        0     4636 2023-05-02 20:11:35.327853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
--rw-r--r--   0        0        0     4239 2023-05-02 20:11:32.111839 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.331853 qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
--rw-r--r--   0        0        0     2376 2023-05-02 20:11:35.283853 qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
--rw-r--r--   0        0        0     3018 2023-05-02 20:11:28.283821 qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.287853 qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
--rw-r--r--   0        0        0     4325 2023-05-02 20:11:35.287853 qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
--rw-r--r--   0        0        0     2501 2023-05-02 20:11:28.471822 qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
--rw-r--r--   0        0        0     5028 2023-05-02 20:11:35.287853 qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
--rw-r--r--   0        0        0     6401 2023-05-02 20:11:35.171853 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/constructs_pb2.py
--rw-r--r--   0        0        0    10192 2023-05-02 20:11:19.003779 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.175853 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
--rw-r--r--   0        0        0     2742 2023-05-02 20:11:35.175853 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_pb2.py
--rw-r--r--   0        0        0     4115 2023-05-02 20:11:19.191779 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.179853 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
--rw-r--r--   0        0        0     7123 2023-05-02 20:11:35.179853 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
--rw-r--r--   0        0        0     3981 2023-05-02 20:11:19.383780 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
--rw-r--r--   0        0        0     8546 2023-05-02 20:11:35.183853 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
--rw-r--r--   0        0        0     8428 2023-05-02 20:11:35.187853 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/status_pb2.py
--rw-r--r--   0        0        0    12205 2023-05-02 20:11:19.579781 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/status_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.187853 qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
--rw-r--r--   0        0        0     8196 2023-05-02 20:11:35.259853 qwak_core-0.0.42/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
--rw-r--r--   0        0        0    10867 2023-05-02 20:11:26.151811 qwak_core-0.0.42/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
--rw-r--r--   0        0        0     4700 2023-05-02 20:11:35.263853 qwak_core-0.0.42/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
--rw-r--r--   0        0        0     7803 2023-05-02 20:11:35.331853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
--rw-r--r--   0        0        0    10487 2023-05-02 20:11:32.299839 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.331853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
--rw-r--r--   0        0        0     3704 2023-05-02 20:11:35.331853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
--rw-r--r--   0        0        0     3759 2023-05-02 20:11:32.491840 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.335853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
--rw-r--r--   0        0        0    22089 2023-05-02 20:11:35.335853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
--rw-r--r--   0        0        0    25879 2023-05-02 20:11:32.687841 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.335853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
--rw-r--r--   0        0        0    13157 2023-05-02 20:11:35.335853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
--rw-r--r--   0        0        0    21705 2023-05-02 20:11:32.879842 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.339853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
--rw-r--r--   0        0        0    12174 2023-05-02 20:11:35.339853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
--rw-r--r--   0        0        0    16128 2023-05-02 20:11:33.075843 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.339853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
--rw-r--r--   0        0        0    45273 2023-05-02 20:11:35.343853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
--rw-r--r--   0        0        0    35031 2023-05-02 20:11:33.287844 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
--rw-r--r--   0        0        0    67567 2023-05-02 20:11:35.343853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
--rw-r--r--   0        0        0     2411 2023-05-02 20:11:35.343853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
--rw-r--r--   0        0        0     2637 2023-05-02 20:11:33.475845 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.343853 qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
--rw-r--r--   0        0        0     3459 2023-05-02 20:11:35.291853 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_filter_pb2.py
--rw-r--r--   0        0        0     4169 2023-05-02 20:11:28.847824 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_filter_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.291853 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
--rw-r--r--   0        0        0     2233 2023-05-02 20:11:35.299853 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_line_pb2.py
--rw-r--r--   0        0        0     2135 2023-05-02 20:11:29.411826 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_line_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.299853 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
--rw-r--r--   0        0        0     3126 2023-05-02 20:11:35.295853 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_reader_service_pb2.py
--rw-r--r--   0        0        0     3479 2023-05-02 20:11:29.035825 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
--rw-r--r--   0        0        0     2831 2023-05-02 20:11:35.295853 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
--rw-r--r--   0        0        0     9322 2023-05-02 20:11:35.295853 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_source_pb2.py
--rw-r--r--   0        0        0    13291 2023-05-02 20:11:29.223825 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_source_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.295853 qwak_core-0.0.42/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
--rw-r--r--   0        0        0    22744 2023-05-02 20:11:35.279853 qwak_core-0.0.42/_qwak_proto/qwak/models/models_pb2.py
--rw-r--r--   0        0        0    27142 2023-05-02 20:11:27.715819 qwak_core-0.0.42/_qwak_proto/qwak/models/models_pb2.pyi
--rw-r--r--   0        0        0    14733 2023-05-02 20:11:35.279853 qwak_core-0.0.42/_qwak_proto/qwak/models/models_pb2_grpc.py
--rw-r--r--   0        0        0    10745 2023-05-02 20:11:35.151852 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
--rw-r--r--   0        0        0     6790 2023-05-02 20:11:18.619777 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
--rw-r--r--   0        0        0    13657 2023-05-02 20:11:35.151852 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
--rw-r--r--   0        0        0    11564 2023-05-02 20:11:35.147853 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
--rw-r--r--   0        0        0    14927 2023-05-02 20:11:18.427776 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.151852 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
--rw-r--r--   0        0        0     5283 2023-05-02 20:11:35.151852 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
--rw-r--r--   0        0        0     3745 2023-05-02 20:11:18.811778 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
--rw-r--r--   0        0        0     5551 2023-05-02 20:11:35.155852 qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
--rw-r--r--   0        0        0     8701 2023-05-02 20:11:35.275853 qwak_core-0.0.42/_qwak_proto/qwak/projects/projects_pb2.py
--rw-r--r--   0        0        0     9794 2023-05-02 20:11:27.303817 qwak_core-0.0.42/_qwak_proto/qwak/projects/projects_pb2.pyi
--rw-r--r--   0        0        0     7931 2023-05-02 20:11:35.279853 qwak_core-0.0.42/_qwak_proto/qwak/projects/projects_pb2_grpc.py
--rw-r--r--   0        0        0     4752 2023-05-02 20:11:35.291853 qwak_core-0.0.42/_qwak_proto/qwak/secret_service/secret_service_pb2.py
--rw-r--r--   0        0        0     2818 2023-05-02 20:11:28.663823 qwak_core-0.0.42/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
--rw-r--r--   0        0        0     6253 2023-05-02 20:11:35.291853 qwak_core-0.0.42/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
--rw-r--r--   0        0        0     6225 2023-05-02 20:11:35.147853 qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
--rw-r--r--   0        0        0     7267 2023-05-02 20:11:16.175766 qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.147853 qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
--rw-r--r--   0        0        0    16176 2023-05-02 20:11:35.143852 qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
--rw-r--r--   0        0        0    10166 2023-05-02 20:11:15.979765 qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
--rw-r--r--   0        0        0    19988 2023-05-02 20:11:35.143852 qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
--rw-r--r--   0        0        0     1751 2023-05-02 20:11:35.139852 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
--rw-r--r--   0        0        0      777 2023-05-02 20:11:15.399762 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.139852 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
--rw-r--r--   0        0        0     2392 2023-05-02 20:11:35.139852 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
--rw-r--r--   0        0        0     2129 2023-05-02 20:11:15.591763 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.139852 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
--rw-r--r--   0        0        0    10389 2023-05-02 20:11:35.143852 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
--rw-r--r--   0        0        0     8148 2023-05-02 20:11:15.783764 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
--rw-r--r--   0        0        0    10512 2023-05-02 20:11:35.143852 qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
--rw-r--r--   0        0        0     6843 2023-05-02 20:11:35.347853 qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
--rw-r--r--   0        0        0     4585 2023-05-02 20:11:33.855847 qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
--rw-r--r--   0        0        0     8228 2023-05-02 20:11:35.351853 qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
--rw-r--r--   0        0        0     7816 2023-05-02 20:11:35.347853 qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
--rw-r--r--   0        0        0    11958 2023-05-02 20:11:33.667846 qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.347853 qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
--rw-r--r--   0        0        0     4083 2023-05-02 20:11:35.163853 qwak_core-0.0.42/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
--rw-r--r--   0        0        0     4036 2023-05-02 20:11:17.515772 qwak_core-0.0.42/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.163853 qwak_core-0.0.42/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
--rw-r--r--   0        0        0     2993 2023-05-02 20:11:35.163853 qwak_core-0.0.42/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
--rw-r--r--   0        0        0     2568 2023-05-02 20:11:17.723773 qwak_core-0.0.42/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
--rw-r--r--   0        0        0      159 2023-05-02 20:11:35.163853 qwak_core-0.0.42/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
--rw-r--r--   0        0        0     2661 2023-05-02 20:11:36.911861 qwak_core-0.0.42/pyproject.toml
--rw-r--r--   0        0        0      447 2023-05-02 20:11:36.911861 qwak_core-0.0.42/qwak/__init__.py
--rw-r--r--   0        0        0     1204 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/automations/__init__.py
--rw-r--r--   0        0        0     3132 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/automations/automation_executions.py
--rw-r--r--   0        0        0    32539 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/automations/automations.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/clients/__init__.py
--rw-r--r--   0        0        0      224 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/clients/administration/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/clients/administration/authenticated_user/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/clients/administration/authenticated_user/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/clients/administration/authentication/__init__.py
--rw-r--r--   0        0        0     1076 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/clients/administration/authentication/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.767386 qwak_core-0.0.42/qwak/clients/administration/eco_system/__init__.py
--rw-r--r--   0        0        0     5362 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/administration/eco_system/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/administration/environment/__init__.py
--rw-r--r--   0        0        0     2704 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/administration/environment/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/administration/self_service/__init__.py
--rw-r--r--   0        0        0     2602 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/administration/self_service/client.py
--rw-r--r--   0        0        0       43 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/alert_management/__init__.py
--rw-r--r--   0        0        0     2226 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/alert_management/client.py
--rw-r--r--   0        0        0       42 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/analytics/__init__.py
--rw-r--r--   0        0        0     3093 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/analytics/client.py
--rw-r--r--   0        0        0       35 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/audience/__init__.py
--rw-r--r--   0        0        0     2110 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/audience/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/automation_management/__init__.py
--rw-r--r--   0        0        0     8836 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/automation_management/client.py
--rw-r--r--   0        0        0       38 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/autoscaling/__init__.py
--rw-r--r--   0        0        0     1240 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/autoscaling/client.py
--rw-r--r--   0        0        0       77 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/batch_job_management/__init__.py
--rw-r--r--   0        0        0    17275 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/batch_job_management/client.py
--rw-r--r--   0        0        0     6242 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/batch_job_management/executions_config.py
--rw-r--r--   0        0        0     1846 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/batch_job_management/results.py
--rw-r--r--   0        0        0       43 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/build_management/__init__.py
--rw-r--r--   0        0        0     4731 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/build_management/client.py
--rw-r--r--   0        0        0       44 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/build_orchestrator/__init__.py
--rw-r--r--   0        0        0    14950 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/build_orchestrator/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/data_versioning/__init__.py
--rw-r--r--   0        0        0     1835 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/data_versioning/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/deployment/__init__.py
--rw-r--r--   0        0        0     6269 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/deployment/client.py
--rw-r--r--   0        0        0       53 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/feature_store/__init__.py
--rw-r--r--   0        0        0     2635 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/feature_store/job_registry_client.py
--rw-r--r--   0        0        0    15898 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/feature_store/management_client.py
--rw-r--r--   0        0        0     4963 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/feature_store/operator_client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/file_versioning/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/file_versioning/client.py
--rw-r--r--   0        0        0       41 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/kube_deployment_captain/__init__.py
--rw-r--r--   0        0        0     9276 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/kube_deployment_captain/client.py
--rw-r--r--   0        0        0       34 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/logging_client/__init__.py
--rw-r--r--   0        0        0     4906 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/logging_client/client.py
--rw-r--r--   0        0        0       43 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/model_management/__init__.py
--rw-r--r--   0        0        0     3695 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/model_management/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/project/__init__.py
--rw-r--r--   0        0        0     2128 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/project/client.py
--rw-r--r--   0        0        0       40 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/secret_service/__init__.py
--rw-r--r--   0        0        0     3316 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/secret_service/client.py
--rw-r--r--   0        0        0       50 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/user_application_instance/__init__.py
--rw-r--r--   0        0        0     6013 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/clients/user_application_instance/client.py
--rw-r--r--   0        0        0      380 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/__init__.py
--rw-r--r--   0        0        0      559 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/quiet_error.py
--rw-r--r--   0        0        0      469 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_build_exception.py
--rw-r--r--   0        0        0      135 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_exception.py
--rw-r--r--   0        0        0      579 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_http_exception.py
--rw-r--r--   0        0        0      100 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_inference_exception.py
--rw-r--r--   0        0        0      274 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_load_model_failed_exception.py
--rw-r--r--   0        0        0      211 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_login_exception.py
--rw-r--r--   0        0        0      152 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_mock_http_exception.py
--rw-r--r--   0        0        0      153 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_model_initialization_exception.py
--rw-r--r--   0        0        0      152 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_not_found_exception.py
--rw-r--r--   0        0        0      356 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/exceptions/qwak_quiet_build_exception.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/_common/__init__.py
--rw-r--r--   0        0        0     4707 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/_common/featureset_asterisk_handler.py
--rw-r--r--   0        0        0     1298 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/_common/functions.py
--rw-r--r--   0        0        0     1201 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/__init__.py
--rw-r--r--   0        0        0     2108 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/_batch.py
--rw-r--r--   0        0        0      666 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/_jdbc.py
--rw-r--r--   0        0        0     3059 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/big_query.py
--rw-r--r--   0        0        0     2006 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/csv.py
--rw-r--r--   0        0        0     2167 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/elastic_search.py
--rw-r--r--   0        0        0     2961 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
--rw-r--r--   0        0        0     1930 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/mongodb.py
--rw-r--r--   0        0        0     1669 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/mysql.py
--rw-r--r--   0        0        0     1730 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/parquet.py
--rw-r--r--   0        0        0     1722 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/postgres.py
--rw-r--r--   0        0        0     3216 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/redshift.py
--rw-r--r--   0        0        0     2616 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/snowflake.py
--rw-r--r--   0        0        0     1839 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/vertica.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/entities/__init__.py
--rw-r--r--   0        0        0     1794 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/entities/entity.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/feature_sets/__init__.py
--rw-r--r--   0        0        0     1547 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/feature_sets/backfill.py
--rw-r--r--   0        0        0    17012 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/feature_sets/batch.py
--rw-r--r--   0        0        0      263 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/feature_sets/context.py
--rw-r--r--   0        0        0     1630 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/feature_sets/execution_spec.py
--rw-r--r--   0        0        0      584 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/feature_sets/metadata.py
--rw-r--r--   0        0        0     6820 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/feature_sets/read_policies.py
--rw-r--r--   0        0        0     1554 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/feature_sets/transformations.py
--rw-r--r--   0        0        0       89 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/offline/__init__.py
--rw-r--r--   0        0        0      738 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/offline/_query_engine.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/offline/athena/__init__.py
--rw-r--r--   0        0        0     5182 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/offline/athena/athena_query_engine.py
--rw-r--r--   0        0        0    28013 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/offline/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/online/__init__.py
--rw-r--r--   0        0        0     9480 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/feature_store/online/client.py
--rw-r--r--   0        0        0      226 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/__init__.py
--rw-r--r--   0        0        0      954 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/const.py
--rw-r--r--   0        0        0     1377 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/di_configuration/__init__.py
--rw-r--r--   0        0        0     4768 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/di_configuration/account.py
--rw-r--r--   0        0        0       73 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/di_configuration/config.yml
--rw-r--r--   0        0        0      621 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/di_configuration/containers.py
--rw-r--r--   0        0        0      344 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/di_configuration/session.py
--rw-r--r--   0        0        0     2336 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/model_loggers_utils.py
--rw-r--r--   0        0        0      266 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/runtime_di/__init__.py
--rw-r--r--   0        0        0      349 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/runtime_di/containers.py
--rw-r--r--   0        0        0      627 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/singleton_meta.py
--rw-r--r--   0        0        0       74 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/__init__.py
--rw-r--r--   0        0        0     3414 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/auth.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/grpc/__init__.py
--rw-r--r--   0        0        0      560 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/grpc/grpc_auth.py
--rw-r--r--   0        0        0     5804 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/grpc/grpc_tools.py
--rw-r--r--   0        0        0      473 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/grpc/grpc_try_wrapping.py
--rw-r--r--   0        0        0      435 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/retry_utils.py
--rw-r--r--   0        0        0      218 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/run_config/__init__.py
--rw-r--r--   0        0        0     3148 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/run_config/base.py
--rw-r--r--   0        0        0     6071 2023-05-02 20:09:52.771386 qwak_core-0.0.42/qwak/inner/tool/run_config/utils.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      198 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/base_input_adapter.py
--rw-r--r--   0        0        0      210 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/file_input_adapter.py
--rw-r--r--   0        0        0      206 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/image_input_adapter.py
--rw-r--r--   0        0        0      205 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/json_input_adapter.py
--rw-r--r--   0        0        0     2175 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/multi_input_adapter.py
--rw-r--r--   0        0        0     3208 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/numpy_input_adapter.py
--rw-r--r--   0        0        0      862 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/proto_input_adapter.py
--rw-r--r--   0        0        0      207 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/string_input_adapter.py
--rw-r--r--   0        0        0      209 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      315 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/base_output_adapter.py
--rw-r--r--   0        0        0      221 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
--rw-r--r--   0        0        0      219 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/default_output_adapter.py
--rw-r--r--   0        0        0      216 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/json_output_adapter.py
--rw-r--r--   0        0        0     1065 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/numpy_output_adapter.py
--rw-r--r--   0        0        0      517 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/proto_output_adapter.py
--rw-r--r--   0        0        0      115 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
--rw-r--r--   0        0        0      220 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
--rw-r--r--   0        0        0      303 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/analytics_logging.py
--rw-r--r--   0        0        0     2825 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/base.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/decorators/__init__.py
--rw-r--r--   0        0        0     1288 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/decorators/api.py
--rw-r--r--   0        0        0      861 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/decorators/api_implementation.py
--rw-r--r--   0        0        0     1503 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/experiment_tracking.py
--rw-r--r--   0        0        0      829 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/schema.py
--rw-r--r--   0        0        0     2970 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/schema_entities.py
--rw-r--r--   0        0        0      338 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/__init__.py
--rw-r--r--   0        0        0     1193 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/encoders.py
--rw-r--r--   0        0        0     1963 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/__init__.py
--rw-r--r--   0        0        0      606 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/base_input.py
--rw-r--r--   0        0        0      848 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/dataframe_input.py
--rw-r--r--   0        0        0      178 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/file_input.py
--rw-r--r--   0        0        0     1449 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/image_input.py
--rw-r--r--   0        0        0      608 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/json_input.py
--rw-r--r--   0        0        0      151 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/string_input.py
--rw-r--r--   0        0        0     1363 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
--rw-r--r--   0        0        0     2511 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/output.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/__init__.py
--rw-r--r--   0        0        0      343 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/base_output.py
--rw-r--r--   0        0        0      650 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/dataframe_output.py
--rw-r--r--   0        0        0     1738 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/default_output.py
--rw-r--r--   0        0        0      568 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/json_output.py
--rw-r--r--   0        0        0     1076 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
--rw-r--r--   0        0        0      975 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/tools/run_model_locally.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/utils/__init__.py
--rw-r--r--   0        0        0      320 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model/utils/extract_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model_loggers/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model_loggers/artifact_logger.py
--rw-r--r--   0        0        0     5186 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model_loggers/data_logger.py
--rw-r--r--   0        0        0      852 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/model_loggers/model_logger.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/builds/__init__.py
--rw-r--r--   0        0        0     3698 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/builds/build.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/builds/filters/__init__.py
--rw-r--r--   0        0        0     1185 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/builds/filters/metric_filter.py
--rw-r--r--   0        0        0     1088 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/builds/filters/parameter_filter.py
--rw-r--r--   0        0        0    15535 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/deployments/__init__.py
--rw-r--r--   0        0        0    13221 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/deployments/deployment.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/models/__init__.py
--rw-r--r--   0        0        0     1921 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/models/model.py
--rw-r--r--   0        0        0      533 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/models/model_metadata.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/projects/__init__.py
--rw-r--r--   0        0        0     2284 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/qwak_client/projects/project.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/testing/__init__.py
--rw-r--r--   0        0        0      318 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak/testing/fixtures.py
--rw-r--r--   0        0        0       46 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/__init__.py
--rw-r--r--   0        0        0     2150 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/alert_manager_service_api.py
--rw-r--r--   0        0        0     2129 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/analytics_api.py
--rw-r--r--   0        0        0     2647 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/audience_service_api.py
--rw-r--r--   0        0        0     1067 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/authentication_service.py
--rw-r--r--   0        0        0     8211 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/automation_management_service.py
--rw-r--r--   0        0        0     1019 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/autoscaling_service_api.py
--rw-r--r--   0        0        0    12145 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/batch_job_manager_service.py
--rw-r--r--   0        0        0     3841 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/build_management.py
--rw-r--r--   0        0        0     3909 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/build_orchestrator_build_api.py
--rw-r--r--   0        0        0     4150 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/build_orchestrator_service_api.py
--rw-r--r--   0        0        0     1412 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/data_versioning_service.py
--rw-r--r--   0        0        0    18268 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/deployment_management_service.py
--rw-r--r--   0        0        0     1158 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/ecosystem_service_api.py
--rw-r--r--   0        0        0     1536 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
--rw-r--r--   0        0        0     1782 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/feature_store_entities_manager_api.py
--rw-r--r--   0        0        0     3261 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
--rw-r--r--   0        0        0     5806 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/features_online_serving_api.py
--rw-r--r--   0        0        0     1001 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/features_operator_v3_service.py
--rw-r--r--   0        0        0     2276 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/features_set_state_service_api.py
--rw-r--r--   0        0        0     1127 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/feedback_service.py
--rw-r--r--   0        0        0     1412 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/file_versioning_service.py
--rw-r--r--   0        0        0     2696 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/job_registry_service_api.py
--rw-r--r--   0        0        0     1583 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/kube_captain_service_api.py
--rw-r--r--   0        0        0     7381 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/logging_service.py
--rw-r--r--   0        0        0     3566 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/model_management_service.py
--rw-r--r--   0        0        0     3090 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/project_manager_service.py
--rw-r--r--   0        0        0     3995 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/qwak_mocks.py
--rw-r--r--   0        0        0     1406 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/secret_service.py
--rw-r--r--   0        0        0     1205 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/self_service_user_service.py
--rw-r--r--   0        0        0     4083 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/user_application_instance_service_api.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/utils/__init__.py
--rw-r--r--   0        0        0      159 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/mocks/utils/exception_handlers.py
--rw-r--r--   0        0        0    13054 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/services_mock.py
--rw-r--r--   0        0        0        0 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/utils/__init__.py
--rw-r--r--   0        0        0      265 2023-05-02 20:09:52.775386 qwak_core-0.0.42/qwak_services_mock/utils/service_utils.py
--rw-r--r--   0        0        0     4873 1970-01-01 00:00:00.000000 qwak_core-0.0.42/setup.py
--rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.42/PKG-INFO
+-rw-r--r--   0        0        0      264 2023-05-03 07:49:10.586164 qwak_core-0.0.43/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 07:50:58.374773 qwak_core-0.0.43/_qwak_proto/__init__.py
+-rw-r--r--   0        0        0     5378 2023-05-03 07:50:58.402773 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/account_pb2.py
+-rw-r--r--   0        0        0     6623 2023-05-03 07:50:36.786651 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.402773 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/account_pb2_grpc.py
+-rw-r--r--   0        0        0     2390 2023-05-03 07:50:58.398773 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py
+-rw-r--r--   0        0        0     1475 2023-05-03 07:50:36.410649 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.398773 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     2106 2023-05-03 07:50:58.398773 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py
+-rw-r--r--   0        0        0     1207 2023-05-03 07:50:36.598650 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.398773 qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/preferences_pb2_grpc.py
+-rw-r--r--   0        0        0     6751 2023-05-03 07:50:58.390773 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py
+-rw-r--r--   0        0        0     4346 2023-05-03 07:50:35.842646 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi
+-rw-r--r--   0        0        0     7662 2023-05-03 07:50:58.390773 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-03 07:50:58.394773 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py
+-rw-r--r--   0        0        0     2650 2023-05-03 07:50:36.034647 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.394773 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0     4864 2023-05-03 07:50:58.394773 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py
+-rw-r--r--   0        0        0     5792 2023-05-03 07:50:36.222648 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.394773 qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2_grpc.py
+-rw-r--r--   0        0        0     4635 2023-05-03 07:50:58.378773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py
+-rw-r--r--   0        0        0     3664 2023-05-03 07:50:35.642645 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi
+-rw-r--r--   0        0        0     3167 2023-05-03 07:50:58.378773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5670 2023-05-03 07:50:58.378773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py
+-rw-r--r--   0        0        0     8035 2023-05-03 07:50:36.978652 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.382773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/configuration_pb2_grpc.py
+-rw-r--r--   0        0        0     4512 2023-05-03 07:50:58.382773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py
+-rw-r--r--   0        0        0     5690 2023-05-03 07:50:37.366654 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.386773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_pb2_grpc.py
+-rw-r--r--   0        0        0    16001 2023-05-03 07:50:58.386773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py
+-rw-r--r--   0        0        0    12387 2023-05-03 07:50:37.554655 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi
+-rw-r--r--   0        0        0    16458 2023-05-03 07:50:58.386773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2464 2023-05-03 07:50:58.382773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py
+-rw-r--r--   0        0        0     1347 2023-05-03 07:50:37.170653 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.382773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/personalization_pb2_grpc.py
+-rw-r--r--   0        0        0     6425 2023-05-03 07:50:58.386773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/users/user_pb2.py
+-rw-r--r--   0        0        0    10323 2023-05-03 07:50:37.742656 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.390773 qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/users/user_pb2_grpc.py
+-rw-r--r--   0        0        0     9577 2023-05-03 07:50:58.434773 qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py
+-rw-r--r--   0        0        0    13624 2023-05-03 07:50:40.510672 qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.434773 qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2_grpc.py
+-rw-r--r--   0        0        0     9270 2023-05-03 07:50:58.434773 qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py
+-rw-r--r--   0        0        0     5571 2023-05-03 07:50:40.698673 qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi
+-rw-r--r--   0        0        0    10742 2023-05-03 07:50:58.434773 qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7365 2023-05-03 07:50:58.502774 qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_pb2.py
+-rw-r--r--   0        0        0    11839 2023-05-03 07:50:46.026703 qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.502774 qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_pb2_grpc.py
+-rw-r--r--   0        0        0     9396 2023-05-03 07:50:58.506774 qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_service_pb2.py
+-rw-r--r--   0        0        0     7896 2023-05-03 07:50:46.230704 qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi
+-rw-r--r--   0        0        0    11917 2023-05-03 07:50:58.506774 qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9021 2023-05-03 07:50:58.510774 qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_api_pb2.py
+-rw-r--r--   0        0        0     5865 2023-05-03 07:50:47.342711 qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi
+-rw-r--r--   0        0        0    11486 2023-05-03 07:50:58.510774 qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py
+-rw-r--r--   0        0        0     8807 2023-05-03 07:50:58.506774 qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_pb2.py
+-rw-r--r--   0        0        0    13570 2023-05-03 07:50:47.126709 qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.506774 qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_pb2_grpc.py
+-rw-r--r--   0        0        0     5497 2023-05-03 07:50:58.510774 qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7820 2023-05-03 07:50:47.586712 qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.510774 qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     2937 2023-05-03 07:50:58.514774 qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py
+-rw-r--r--   0        0        0     2014 2023-05-03 07:50:47.798713 qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi
+-rw-r--r--   0        0        0     2991 2023-05-03 07:50:58.514774 qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11441 2023-05-03 07:50:58.574774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/action_pb2.py
+-rw-r--r--   0        0        0    17892 2023-05-03 07:50:53.614746 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.578774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/action_pb2_grpc.py
+-rw-r--r--   0        0        0     5494 2023-05-03 07:50:58.570774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py
+-rw-r--r--   0        0        0     7776 2023-05-03 07:50:53.230744 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.574774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/auto_scaling_pb2_grpc.py
+-rw-r--r--   0        0        0     3373 2023-05-03 07:50:58.574774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py
+-rw-r--r--   0        0        0     4400 2023-05-03 07:50:53.422745 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.574774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_execution_pb2_grpc.py
+-rw-r--r--   0        0        0    17887 2023-05-03 07:50:58.566774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py
+-rw-r--r--   0        0        0    12310 2023-05-03 07:50:52.850742 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi
+-rw-r--r--   0        0        0    23338 2023-05-03 07:50:58.570774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3873 2023-05-03 07:50:58.570774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_pb2.py
+-rw-r--r--   0        0        0     5291 2023-05-03 07:50:53.042743 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.570774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_pb2_grpc.py
+-rw-r--r--   0        0        0     2383 2023-05-03 07:50:58.582774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/common_pb2.py
+-rw-r--r--   0        0        0     2446 2023-05-03 07:50:54.174749 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/common_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.582774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/common_pb2_grpc.py
+-rw-r--r--   0        0        0     5209 2023-05-03 07:50:58.582774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/notification_pb2.py
+-rw-r--r--   0        0        0     5492 2023-05-03 07:50:53.990748 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.582774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/notification_pb2_grpc.py
+-rw-r--r--   0        0        0     4210 2023-05-03 07:50:58.578774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/trigger_pb2.py
+-rw-r--r--   0        0        0     4746 2023-05-03 07:50:53.802747 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.578774 qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/trigger_pb2_grpc.py
+-rw-r--r--   0        0        0    10275 2023-05-03 07:50:58.622774 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py
+-rw-r--r--   0        0        0    14803 2023-05-03 07:50:57.726769 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.622774 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2_grpc.py
+-rw-r--r--   0        0        0     2042 2023-05-03 07:50:58.618775 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py
+-rw-r--r--   0        0        0     1904 2023-05-03 07:50:57.338767 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.618775 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2_grpc.py
+-rw-r--r--   0        0        0    37419 2023-05-03 07:50:58.622774 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py
+-rw-r--r--   0        0        0    48027 2023-05-03 07:50:57.534768 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi
+-rw-r--r--   0        0        0    29918 2023-05-03 07:50:58.622774 qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py
+-rw-r--r--   0        0        0    18658 2023-05-03 07:50:58.538774 qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_api_pb2.py
+-rw-r--r--   0        0        0    15525 2023-05-03 07:50:50.066726 qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_api_pb2.pyi
+-rw-r--r--   0        0        0    18652 2023-05-03 07:50:58.542774 qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py
+-rw-r--r--   0        0        0    16953 2023-05-03 07:50:58.538774 qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_pb2.py
+-rw-r--r--   0        0        0    25941 2023-05-03 07:50:49.822725 qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.538774 qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_pb2_grpc.py
+-rw-r--r--   0        0        0    11034 2023-05-03 07:50:58.530774 qwak_core-0.0.43/_qwak_proto/qwak/builds/build_pb2.py
+-rw-r--r--   0        0        0    18276 2023-05-03 07:50:49.402722 qwak_core-0.0.43/_qwak_proto/qwak/builds/build_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.530774 qwak_core-0.0.43/_qwak_proto/qwak/builds/build_pb2_grpc.py
+-rw-r--r--   0        0        0     4777 2023-05-03 07:50:58.530774 qwak_core-0.0.43/_qwak_proto/qwak/builds/build_url_pb2.py
+-rw-r--r--   0        0        0     5773 2023-05-03 07:50:49.610723 qwak_core-0.0.43/_qwak_proto/qwak/builds/build_url_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.530774 qwak_core-0.0.43/_qwak_proto/qwak/builds/build_url_pb2_grpc.py
+-rw-r--r--   0        0        0    12490 2023-05-03 07:50:58.534774 qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py
+-rw-r--r--   0        0        0     9351 2023-05-03 07:50:50.274727 qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi
+-rw-r--r--   0        0        0    14916 2023-05-03 07:50:58.534774 qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py
+-rw-r--r--   0        0        0    38245 2023-05-03 07:50:58.534774 qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_pb2.py
+-rw-r--r--   0        0        0    52572 2023-05-03 07:50:50.698730 qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_pb2.pyi
+-rw-r--r--   0        0        0    11572 2023-05-03 07:50:58.538774 qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_pb2_grpc.py
+-rw-r--r--   0        0        0     1671 2023-05-03 07:50:58.546774 qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py
+-rw-r--r--   0        0        0     1689 2023-05-03 07:50:51.110732 qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.546774 qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4328 2023-05-03 07:50:58.550774 qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-03 07:50:51.310733 qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-03 07:50:58.550774 qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     7716 2023-05-03 07:50:58.522774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_pb2.py
+-rw-r--r--   0        0        0    11197 2023-05-03 07:50:48.722718 qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.522774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_pb2_grpc.py
+-rw-r--r--   0        0        0    11580 2023-05-03 07:50:58.526774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_service_pb2.py
+-rw-r--r--   0        0        0     7373 2023-05-03 07:50:48.926720 qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_service_pb2.pyi
+-rw-r--r--   0        0        0    12803 2023-05-03 07:50:58.526774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2162 2023-05-03 07:50:58.518774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_messages_pb2.py
+-rw-r--r--   0        0        0     2685 2023-05-03 07:50:48.282716 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.518774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_messages_pb2_grpc.py
+-rw-r--r--   0        0        0    42956 2023-05-03 07:50:58.514774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_pb2.py
+-rw-r--r--   0        0        0    62847 2023-05-03 07:50:48.042715 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.518774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    38320 2023-05-03 07:50:58.518774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_service_pb2.py
+-rw-r--r--   0        0        0    33325 2023-05-03 07:50:48.514717 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi
+-rw-r--r--   0        0        0    20242 2023-05-03 07:50:58.522774 qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2527 2023-05-03 07:50:58.422773 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py
+-rw-r--r--   0        0        0     2791 2023-05-03 07:50:39.494666 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.422773 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/credentials_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-03 07:50:58.422773 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py
+-rw-r--r--   0        0        0    12641 2023-05-03 07:50:39.738668 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.426773 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2_grpc.py
+-rw-r--r--   0        0        0    16366 2023-05-03 07:50:58.426773 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py
+-rw-r--r--   0        0        0    17148 2023-05-03 07:50:39.950669 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi
+-rw-r--r--   0        0        0    10706 2023-05-03 07:50:58.426773 qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4787 2023-05-03 07:50:58.482774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_pb2.py
+-rw-r--r--   0        0        0     6713 2023-05-03 07:50:44.814696 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.482774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_pb2_grpc.py
+-rw-r--r--   0        0        0     9721 2023-05-03 07:50:58.478774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py
+-rw-r--r--   0        0        0     7409 2023-05-03 07:50:44.614695 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi
+-rw-r--r--   0        0        0    12256 2023-05-03 07:50:58.482774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9535 2023-05-03 07:50:58.462774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py
+-rw-r--r--   0        0        0    10460 2023-05-03 07:50:43.038686 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.462774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/aggregation_pb2_grpc.py
+-rw-r--r--   0        0        0     5268 2023-05-03 07:50:58.458773 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/execution_pb2.py
+-rw-r--r--   0        0        0     8525 2023-05-03 07:50:42.850685 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.462774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/execution_pb2_grpc.py
+-rw-r--r--   0        0        0    10074 2023-05-03 07:50:58.454774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py
+-rw-r--r--   0        0        0    14303 2023-05-03 07:50:42.242682 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.454774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_pb2_grpc.py
+-rw-r--r--   0        0        0    27847 2023-05-03 07:50:58.458773 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py
+-rw-r--r--   0        0        0    20073 2023-05-03 07:50:42.658684 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi
+-rw-r--r--   0        0        0    33080 2023-05-03 07:50:58.458773 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py
+-rw-r--r--   0        0        0    12638 2023-05-03 07:50:58.466774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py
+-rw-r--r--   0        0        0    14071 2023-05-03 07:50:43.234687 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.466774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2_grpc.py
+-rw-r--r--   0        0        0    10044 2023-05-03 07:50:58.466774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py
+-rw-r--r--   0        0        0     6846 2023-05-03 07:50:43.450689 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi
+-rw-r--r--   0        0        0    11647 2023-05-03 07:50:58.466774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py
+-rw-r--r--   0        0        0    24876 2023-05-03 07:50:58.454774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py
+-rw-r--r--   0        0        0    36861 2023-05-03 07:50:42.450683 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.458773 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2_grpc.py
+-rw-r--r--   0        0        0     2872 2023-05-03 07:50:58.470774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py
+-rw-r--r--   0        0        0     2428 2023-05-03 07:50:43.638690 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.470774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/monitoring_pb2_grpc.py
+-rw-r--r--   0        0        0     4196 2023-05-03 07:50:58.486774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_pb2.py
+-rw-r--r--   0        0        0     7323 2023-05-03 07:50:57.914770 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.486774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_pb2_grpc.py
+-rw-r--r--   0        0        0     9895 2023-05-03 07:50:58.486774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py
+-rw-r--r--   0        0        0     9029 2023-05-03 07:50:58.102772 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi
+-rw-r--r--   0        0        0    12090 2023-05-03 07:50:58.486774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     3596 2023-05-03 07:50:58.490774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py
+-rw-r--r--   0        0        0     6664 2023-05-03 07:50:45.398700 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.490774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2_grpc.py
+-rw-r--r--   0        0        0    11930 2023-05-03 07:50:58.490774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py
+-rw-r--r--   0        0        0    11052 2023-05-03 07:50:45.610701 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi
+-rw-r--r--   0        0        0    14459 2023-05-03 07:50:58.494774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5158 2023-05-03 07:50:58.494774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/reports/report_pb2.py
+-rw-r--r--   0        0        0     7436 2023-05-03 07:50:45.822702 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.494774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/reports/report_pb2_grpc.py
+-rw-r--r--   0        0        0     4549 2023-05-03 07:50:58.498774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py
+-rw-r--r--   0        0        0     6442 2023-05-03 07:50:46.662707 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.498774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/metadata_pb2_grpc.py
+-rw-r--r--   0        0        0    16693 2023-05-03 07:50:58.494774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/serving_pb2.py
+-rw-r--r--   0        0        0    20355 2023-05-03 07:50:46.446705 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi
+-rw-r--r--   0        0        0     4809 2023-05-03 07:50:58.498774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py
+-rw-r--r--   0        0        0     2553 2023-05-03 07:50:58.498774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py
+-rw-r--r--   0        0        0     4000 2023-05-03 07:50:46.906708 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.502774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/v1/value_pb2_grpc.py
+-rw-r--r--   0        0        0    14046 2023-05-03 07:50:58.470774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/batch_pb2.py
+-rw-r--r--   0        0        0    23615 2023-05-03 07:50:43.830691 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.474774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/batch_pb2_grpc.py
+-rw-r--r--   0        0        0     5087 2023-05-03 07:50:58.474774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py
+-rw-r--r--   0        0        0     6011 2023-05-03 07:50:44.022692 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.474774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_pb2_grpc.py
+-rw-r--r--   0        0        0    12309 2023-05-03 07:50:58.474774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py
+-rw-r--r--   0        0        0     9244 2023-05-03 07:50:44.214693 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi
+-rw-r--r--   0        0        0    17071 2023-05-03 07:50:58.478774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11014 2023-05-03 07:50:58.478774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py
+-rw-r--r--   0        0        0    15865 2023-05-03 07:50:44.422694 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.478774 qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/streaming_pb2_grpc.py
+-rw-r--r--   0        0        0     4727 2023-05-03 07:50:58.586774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py
+-rw-r--r--   0        0        0     5122 2023-05-03 07:50:54.374750 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.586774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4648 2023-05-03 07:50:58.586774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4170 2023-05-03 07:50:54.574751 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-03 07:50:58.586774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     5349 2023-05-03 07:50:58.590774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py
+-rw-r--r--   0        0        0     5363 2023-05-03 07:50:54.806753 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.590774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     4437 2023-05-03 07:50:58.590774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py
+-rw-r--r--   0        0        0     4127 2023-05-03 07:50:55.014754 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi
+-rw-r--r--   0        0        0     5151 2023-05-03 07:50:58.594774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6073 2023-05-03 07:50:58.594774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py
+-rw-r--r--   0        0        0     5366 2023-05-03 07:50:55.238755 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi
+-rw-r--r--   0        0        0     7395 2023-05-03 07:50:58.594774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py
+-rw-r--r--   0        0        0     4636 2023-05-03 07:50:58.594774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py
+-rw-r--r--   0        0        0     4239 2023-05-03 07:50:55.434756 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.598774 qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_pb2_grpc.py
+-rw-r--r--   0        0        0     2376 2023-05-03 07:50:58.550774 qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py
+-rw-r--r--   0        0        0     3018 2023-05-03 07:50:51.502734 qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.554774 qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_pb2_grpc.py
+-rw-r--r--   0        0        0     4325 2023-05-03 07:50:58.554774 qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py
+-rw-r--r--   0        0        0     2501 2023-05-03 07:50:51.698735 qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi
+-rw-r--r--   0        0        0     5028 2023-05-03 07:50:58.554774 qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6401 2023-05-03 07:50:58.438773 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/constructs_pb2.py
+-rw-r--r--   0        0        0    10192 2023-05-03 07:50:41.458677 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.442773 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/constructs_pb2_grpc.py
+-rw-r--r--   0        0        0     2742 2023-05-03 07:50:58.442773 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_pb2.py
+-rw-r--r--   0        0        0     4115 2023-05-03 07:50:41.642678 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.446773 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_pb2_grpc.py
+-rw-r--r--   0        0        0     7123 2023-05-03 07:50:58.446773 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py
+-rw-r--r--   0        0        0     3981 2023-05-03 07:50:41.842680 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi
+-rw-r--r--   0        0        0     8546 2023-05-03 07:50:58.450774 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8428 2023-05-03 07:50:58.450774 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/status_pb2.py
+-rw-r--r--   0        0        0    12205 2023-05-03 07:50:42.038681 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/status_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.450774 qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/status_pb2_grpc.py
+-rw-r--r--   0        0        0     8196 2023-05-03 07:50:58.526774 qwak_core-0.0.43/_qwak_proto/qwak/inference/feedback/feedback_pb2.py
+-rw-r--r--   0        0        0    10867 2023-05-03 07:50:49.178721 qwak_core-0.0.43/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi
+-rw-r--r--   0        0        0     4700 2023-05-03 07:50:58.526774 qwak_core-0.0.43/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py
+-rw-r--r--   0        0        0     7803 2023-05-03 07:50:58.598774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py
+-rw-r--r--   0        0        0    10487 2023-05-03 07:50:55.626757 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.598774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alert_pb2_grpc.py
+-rw-r--r--   0        0        0     3704 2023-05-03 07:50:58.598774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py
+-rw-r--r--   0        0        0     3759 2023-05-03 07:50:55.814759 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.602774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2_grpc.py
+-rw-r--r--   0        0        0    22089 2023-05-03 07:50:58.602774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py
+-rw-r--r--   0        0        0    25879 2023-05-03 07:50:56.010760 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.602774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2_grpc.py
+-rw-r--r--   0        0        0    13157 2023-05-03 07:50:58.606774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py
+-rw-r--r--   0        0        0    21705 2023-05-03 07:50:56.198761 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.606774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    12174 2023-05-03 07:50:58.606774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py
+-rw-r--r--   0        0        0    16128 2023-05-03 07:50:56.390762 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.606774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2_grpc.py
+-rw-r--r--   0        0        0    45273 2023-05-03 07:50:58.610774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py
+-rw-r--r--   0        0        0    35031 2023-05-03 07:50:56.598763 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi
+-rw-r--r--   0        0        0    67567 2023-05-03 07:50:58.610774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py
+-rw-r--r--   0        0        0     2411 2023-05-03 07:50:58.610774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py
+-rw-r--r--   0        0        0     2637 2023-05-03 07:50:56.782764 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.614774 qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2_grpc.py
+-rw-r--r--   0        0        0     3459 2023-05-03 07:50:58.558774 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_filter_pb2.py
+-rw-r--r--   0        0        0     4169 2023-05-03 07:50:52.078737 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_filter_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.558774 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_filter_pb2_grpc.py
+-rw-r--r--   0        0        0     2233 2023-05-03 07:50:58.566774 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_line_pb2.py
+-rw-r--r--   0        0        0     2135 2023-05-03 07:50:52.658741 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_line_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.566774 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_line_pb2_grpc.py
+-rw-r--r--   0        0        0     3126 2023-05-03 07:50:58.558774 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_reader_service_pb2.py
+-rw-r--r--   0        0        0     3479 2023-05-03 07:50:52.266739 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi
+-rw-r--r--   0        0        0     2831 2023-05-03 07:50:58.562774 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py
+-rw-r--r--   0        0        0     9322 2023-05-03 07:50:58.562774 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_source_pb2.py
+-rw-r--r--   0        0        0    13291 2023-05-03 07:50:52.458740 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_source_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.562774 qwak_core-0.0.43/_qwak_proto/qwak/logging/log_source_pb2_grpc.py
+-rw-r--r--   0        0        0    22744 2023-05-03 07:50:58.546774 qwak_core-0.0.43/_qwak_proto/qwak/models/models_pb2.py
+-rw-r--r--   0        0        0    27142 2023-05-03 07:50:50.910731 qwak_core-0.0.43/_qwak_proto/qwak/models/models_pb2.pyi
+-rw-r--r--   0        0        0    14733 2023-05-03 07:50:58.546774 qwak_core-0.0.43/_qwak_proto/qwak/models/models_pb2_grpc.py
+-rw-r--r--   0        0        0    10745 2023-05-03 07:50:58.418773 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py
+-rw-r--r--   0        0        0     6790 2023-05-03 07:50:41.078675 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi
+-rw-r--r--   0        0        0    13657 2023-05-03 07:50:58.418773 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py
+-rw-r--r--   0        0        0    11564 2023-05-03 07:50:58.414773 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py
+-rw-r--r--   0        0        0    14927 2023-05-03 07:50:40.890674 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.414773 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2_grpc.py
+-rw-r--r--   0        0        0     5283 2023-05-03 07:50:58.418773 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py
+-rw-r--r--   0        0        0     3745 2023-05-03 07:50:41.270676 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi
+-rw-r--r--   0        0        0     5551 2023-05-03 07:50:58.418773 qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py
+-rw-r--r--   0        0        0     8701 2023-05-03 07:50:58.542774 qwak_core-0.0.43/_qwak_proto/qwak/projects/projects_pb2.py
+-rw-r--r--   0        0        0     9794 2023-05-03 07:50:50.482728 qwak_core-0.0.43/_qwak_proto/qwak/projects/projects_pb2.pyi
+-rw-r--r--   0        0        0     7931 2023-05-03 07:50:58.542774 qwak_core-0.0.43/_qwak_proto/qwak/projects/projects_pb2_grpc.py
+-rw-r--r--   0        0        0     4752 2023-05-03 07:50:58.554774 qwak_core-0.0.43/_qwak_proto/qwak/secret_service/secret_service_pb2.py
+-rw-r--r--   0        0        0     2818 2023-05-03 07:50:51.882736 qwak_core-0.0.43/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi
+-rw-r--r--   0        0        0     6253 2023-05-03 07:50:58.558774 qwak_core-0.0.43/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6225 2023-05-03 07:50:58.414773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py
+-rw-r--r--   0        0        0     7267 2023-05-03 07:50:38.702662 qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.414773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2_grpc.py
+-rw-r--r--   0        0        0    16176 2023-05-03 07:50:58.410773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py
+-rw-r--r--   0        0        0    10166 2023-05-03 07:50:38.514661 qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi
+-rw-r--r--   0        0        0    19988 2023-05-03 07:50:58.410773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1751 2023-05-03 07:50:58.402773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py
+-rw-r--r--   0        0        0      777 2023-05-03 07:50:37.930657 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.406773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/api_key_pb2_grpc.py
+-rw-r--r--   0        0        0     2392 2023-05-03 07:50:58.406773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_pb2.py
+-rw-r--r--   0        0        0     2129 2023-05-03 07:50:38.118658 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.406773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_pb2_grpc.py
+-rw-r--r--   0        0        0    10389 2023-05-03 07:50:58.406773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py
+-rw-r--r--   0        0        0     8148 2023-05-03 07:50:38.306660 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi
+-rw-r--r--   0        0        0    10512 2023-05-03 07:50:58.410773 qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py
+-rw-r--r--   0        0        0     6843 2023-05-03 07:50:58.614774 qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py
+-rw-r--r--   0        0        0     4585 2023-05-03 07:50:57.154766 qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi
+-rw-r--r--   0        0        0     8228 2023-05-03 07:50:58.618775 qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py
+-rw-r--r--   0        0        0     7816 2023-05-03 07:50:58.614774 qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_pb2.py
+-rw-r--r--   0        0        0    11958 2023-05-03 07:50:56.966765 qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.614774 qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_pb2_grpc.py
+-rw-r--r--   0        0        0     4083 2023-05-03 07:50:58.426773 qwak_core-0.0.43/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py
+-rw-r--r--   0        0        0     4036 2023-05-03 07:50:40.134670 qwak_core-0.0.43/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.430773 qwak_core-0.0.43/_qwak_proto/qwak/user_application/common/v0/resources_pb2_grpc.py
+-rw-r--r--   0        0        0     2993 2023-05-03 07:50:58.430773 qwak_core-0.0.43/_qwak_proto/qwak/user_application/v0/user_application_pb2.py
+-rw-r--r--   0        0        0     2568 2023-05-03 07:50:40.322671 qwak_core-0.0.43/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-05-03 07:50:58.430773 qwak_core-0.0.43/_qwak_proto/qwak/user_application/v0/user_application_pb2_grpc.py
+-rw-r--r--   0        0        0     2661 2023-05-03 07:50:59.950782 qwak_core-0.0.43/pyproject.toml
+-rw-r--r--   0        0        0      447 2023-05-03 07:50:59.950782 qwak_core-0.0.43/qwak/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-03 07:49:10.586164 qwak_core-0.0.43/qwak/automations/__init__.py
+-rw-r--r--   0        0        0     3132 2023-05-03 07:49:10.586164 qwak_core-0.0.43/qwak/automations/automation_executions.py
+-rw-r--r--   0        0        0    32539 2023-05-03 07:49:10.586164 qwak_core-0.0.43/qwak/automations/automations.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.586164 qwak_core-0.0.43/qwak/clients/__init__.py
+-rw-r--r--   0        0        0      224 2023-05-03 07:49:10.586164 qwak_core-0.0.43/qwak/clients/administration/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.586164 qwak_core-0.0.43/qwak/clients/administration/authenticated_user/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-03 07:49:10.586164 qwak_core-0.0.43/qwak/clients/administration/authenticated_user/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/administration/authentication/__init__.py
+-rw-r--r--   0        0        0     1076 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/administration/authentication/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/administration/eco_system/__init__.py
+-rw-r--r--   0        0        0     5362 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/administration/eco_system/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/administration/environment/__init__.py
+-rw-r--r--   0        0        0     2704 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/administration/environment/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/administration/self_service/__init__.py
+-rw-r--r--   0        0        0     2602 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/administration/self_service/client.py
+-rw-r--r--   0        0        0       43 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/alert_management/__init__.py
+-rw-r--r--   0        0        0     2226 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/alert_management/client.py
+-rw-r--r--   0        0        0       42 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/analytics/__init__.py
+-rw-r--r--   0        0        0     3093 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/analytics/client.py
+-rw-r--r--   0        0        0       35 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/audience/__init__.py
+-rw-r--r--   0        0        0     2110 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/audience/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/automation_management/__init__.py
+-rw-r--r--   0        0        0     8836 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/automation_management/client.py
+-rw-r--r--   0        0        0       38 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/autoscaling/__init__.py
+-rw-r--r--   0        0        0     1240 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/autoscaling/client.py
+-rw-r--r--   0        0        0       77 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/batch_job_management/__init__.py
+-rw-r--r--   0        0        0    17275 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/batch_job_management/client.py
+-rw-r--r--   0        0        0     6242 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/batch_job_management/executions_config.py
+-rw-r--r--   0        0        0     1846 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/batch_job_management/results.py
+-rw-r--r--   0        0        0       43 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/build_management/__init__.py
+-rw-r--r--   0        0        0     4731 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/build_management/client.py
+-rw-r--r--   0        0        0       44 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/build_orchestrator/__init__.py
+-rw-r--r--   0        0        0    14950 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/build_orchestrator/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/data_versioning/__init__.py
+-rw-r--r--   0        0        0     1835 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/data_versioning/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/deployment/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/deployment/client.py
+-rw-r--r--   0        0        0       53 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/feature_store/__init__.py
+-rw-r--r--   0        0        0     2635 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/feature_store/job_registry_client.py
+-rw-r--r--   0        0        0    15898 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/feature_store/management_client.py
+-rw-r--r--   0        0        0     4963 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/feature_store/operator_client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/file_versioning/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/file_versioning/client.py
+-rw-r--r--   0        0        0       41 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/kube_deployment_captain/__init__.py
+-rw-r--r--   0        0        0     9276 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/kube_deployment_captain/client.py
+-rw-r--r--   0        0        0       34 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/logging_client/__init__.py
+-rw-r--r--   0        0        0     4906 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/logging_client/client.py
+-rw-r--r--   0        0        0       43 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/model_management/__init__.py
+-rw-r--r--   0        0        0     3695 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/model_management/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/project/__init__.py
+-rw-r--r--   0        0        0     2128 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/project/client.py
+-rw-r--r--   0        0        0       40 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/secret_service/__init__.py
+-rw-r--r--   0        0        0     3316 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/secret_service/client.py
+-rw-r--r--   0        0        0       50 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/user_application_instance/__init__.py
+-rw-r--r--   0        0        0     6013 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/clients/user_application_instance/client.py
+-rw-r--r--   0        0        0      380 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/__init__.py
+-rw-r--r--   0        0        0      559 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/quiet_error.py
+-rw-r--r--   0        0        0      469 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_build_exception.py
+-rw-r--r--   0        0        0      135 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_exception.py
+-rw-r--r--   0        0        0      579 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_http_exception.py
+-rw-r--r--   0        0        0      100 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_inference_exception.py
+-rw-r--r--   0        0        0      274 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_load_model_failed_exception.py
+-rw-r--r--   0        0        0      211 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_login_exception.py
+-rw-r--r--   0        0        0      152 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_mock_http_exception.py
+-rw-r--r--   0        0        0      153 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_model_initialization_exception.py
+-rw-r--r--   0        0        0      152 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_not_found_exception.py
+-rw-r--r--   0        0        0      356 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/exceptions/qwak_quiet_build_exception.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/_common/__init__.py
+-rw-r--r--   0        0        0     4707 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/_common/featureset_asterisk_handler.py
+-rw-r--r--   0        0        0     1298 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/_common/functions.py
+-rw-r--r--   0        0        0     1263 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/_batch.py
+-rw-r--r--   0        0        0      666 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/_jdbc.py
+-rw-r--r--   0        0        0     3059 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/big_query.py
+-rw-r--r--   0        0        0     1941 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/csv.py
+-rw-r--r--   0        0        0     2167 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/elastic_search.py
+-rw-r--r--   0        0        0     2987 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/filesystem_config.py
+-rw-r--r--   0        0        0     1930 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/mongodb.py
+-rw-r--r--   0        0        0     1669 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/mysql.py
+-rw-r--r--   0        0        0     1717 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/parquet.py
+-rw-r--r--   0        0        0     1722 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/postgres.py
+-rw-r--r--   0        0        0     3216 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/redshift.py
+-rw-r--r--   0        0        0     2616 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/snowflake.py
+-rw-r--r--   0        0        0     1839 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/vertica.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/entities/__init__.py
+-rw-r--r--   0        0        0     1794 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/entities/entity.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/feature_sets/__init__.py
+-rw-r--r--   0        0        0     1547 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/feature_sets/backfill.py
+-rw-r--r--   0        0        0    17012 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/feature_sets/batch.py
+-rw-r--r--   0        0        0      263 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/feature_sets/context.py
+-rw-r--r--   0        0        0     1630 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/feature_sets/execution_spec.py
+-rw-r--r--   0        0        0      584 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/feature_sets/metadata.py
+-rw-r--r--   0        0        0     6820 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/feature_sets/read_policies.py
+-rw-r--r--   0        0        0     1554 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/feature_sets/transformations.py
+-rw-r--r--   0        0        0       89 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/offline/__init__.py
+-rw-r--r--   0        0        0      738 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/offline/_query_engine.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/offline/athena/__init__.py
+-rw-r--r--   0        0        0     5182 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/offline/athena/athena_query_engine.py
+-rw-r--r--   0        0        0    28013 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/offline/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/online/__init__.py
+-rw-r--r--   0        0        0     9480 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/feature_store/online/client.py
+-rw-r--r--   0        0        0      226 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/__init__.py
+-rw-r--r--   0        0        0      954 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/const.py
+-rw-r--r--   0        0        0     1377 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/di_configuration/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/di_configuration/account.py
+-rw-r--r--   0        0        0       73 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/di_configuration/config.yml
+-rw-r--r--   0        0        0      621 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/di_configuration/containers.py
+-rw-r--r--   0        0        0      344 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/di_configuration/session.py
+-rw-r--r--   0        0        0     2336 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/model_loggers_utils.py
+-rw-r--r--   0        0        0      266 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/runtime_di/__init__.py
+-rw-r--r--   0        0        0      349 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/runtime_di/containers.py
+-rw-r--r--   0        0        0      627 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/singleton_meta.py
+-rw-r--r--   0        0        0       74 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/tool/__init__.py
+-rw-r--r--   0        0        0     3414 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/tool/auth.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/tool/grpc/__init__.py
+-rw-r--r--   0        0        0      560 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/tool/grpc/grpc_auth.py
+-rw-r--r--   0        0        0     5804 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/tool/grpc/grpc_tools.py
+-rw-r--r--   0        0        0      473 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/tool/grpc/grpc_try_wrapping.py
+-rw-r--r--   0        0        0      435 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/tool/retry_utils.py
+-rw-r--r--   0        0        0      218 2023-05-03 07:49:10.590164 qwak_core-0.0.43/qwak/inner/tool/run_config/__init__.py
+-rw-r--r--   0        0        0     3148 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/inner/tool/run_config/base.py
+-rw-r--r--   0        0        0     6071 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/inner/tool/run_config/utils.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      198 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/base_input_adapter.py
+-rw-r--r--   0        0        0      210 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/dataframe_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/file_input_adapter.py
+-rw-r--r--   0        0        0      206 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/image_input_adapter.py
+-rw-r--r--   0        0        0      205 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/json_input_adapter.py
+-rw-r--r--   0        0        0     2175 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/multi_input_adapter.py
+-rw-r--r--   0        0        0     3208 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/numpy_input_adapter.py
+-rw-r--r--   0        0        0      862 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/proto_input_adapter.py
+-rw-r--r--   0        0        0      207 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/string_input_adapter.py
+-rw-r--r--   0        0        0      209 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/input_adapters/tf_tensor_input_adapter.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/base_output_adapter.py
+-rw-r--r--   0        0        0      221 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/dataframe_output_adapter.py
+-rw-r--r--   0        0        0      219 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/default_output_adapter.py
+-rw-r--r--   0        0        0      216 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/json_output_adapter.py
+-rw-r--r--   0        0        0     1065 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/numpy_output_adapter.py
+-rw-r--r--   0        0        0      517 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/proto_output_adapter.py
+-rw-r--r--   0        0        0      115 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/qwak_with_default_fallback.py
+-rw-r--r--   0        0        0      220 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/adapters/output_adapters/tf_tensor_output_adapter.py
+-rw-r--r--   0        0        0      303 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/analytics_logging.py
+-rw-r--r--   0        0        0     2825 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/base.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/decorators/__init__.py
+-rw-r--r--   0        0        0     1288 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/decorators/api.py
+-rw-r--r--   0        0        0      861 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/decorators/api_implementation.py
+-rw-r--r--   0        0        0     1503 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/experiment_tracking.py
+-rw-r--r--   0        0        0      829 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/schema.py
+-rw-r--r--   0        0        0     2970 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/schema_entities.py
+-rw-r--r--   0        0        0      338 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/__init__.py
+-rw-r--r--   0        0        0     1193 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/encoders.py
+-rw-r--r--   0        0        0     1963 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/__init__.py
+-rw-r--r--   0        0        0      606 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/base_input.py
+-rw-r--r--   0        0        0      848 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/dataframe_input.py
+-rw-r--r--   0        0        0      178 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/file_input.py
+-rw-r--r--   0        0        0     1449 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/image_input.py
+-rw-r--r--   0        0        0      608 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/json_input.py
+-rw-r--r--   0        0        0      151 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/string_input.py
+-rw-r--r--   0        0        0     1363 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py
+-rw-r--r--   0        0        0     2511 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/output.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/__init__.py
+-rw-r--r--   0        0        0      343 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/base_output.py
+-rw-r--r--   0        0        0      650 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/dataframe_output.py
+-rw-r--r--   0        0        0     1738 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/default_output.py
+-rw-r--r--   0        0        0      568 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/json_output.py
+-rw-r--r--   0        0        0     1076 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py
+-rw-r--r--   0        0        0      975 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/tools/run_model_locally.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/utils/__init__.py
+-rw-r--r--   0        0        0      320 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model/utils/extract_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model_loggers/__init__.py
+-rw-r--r--   0        0        0     2701 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model_loggers/artifact_logger.py
+-rw-r--r--   0        0        0     5186 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model_loggers/data_logger.py
+-rw-r--r--   0        0        0      852 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/model_loggers/model_logger.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/builds/__init__.py
+-rw-r--r--   0        0        0     3698 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/builds/build.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/builds/filters/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/builds/filters/metric_filter.py
+-rw-r--r--   0        0        0     1088 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/builds/filters/parameter_filter.py
+-rw-r--r--   0        0        0    15535 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/client.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/deployments/__init__.py
+-rw-r--r--   0        0        0    13221 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/deployments/deployment.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/models/__init__.py
+-rw-r--r--   0        0        0     1921 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/models/model.py
+-rw-r--r--   0        0        0      533 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/models/model_metadata.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/projects/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/qwak_client/projects/project.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/testing/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak/testing/fixtures.py
+-rw-r--r--   0        0        0       46 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/__init__.py
+-rw-r--r--   0        0        0     2150 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/alert_manager_service_api.py
+-rw-r--r--   0        0        0     2129 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/analytics_api.py
+-rw-r--r--   0        0        0     2647 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/audience_service_api.py
+-rw-r--r--   0        0        0     1067 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/authentication_service.py
+-rw-r--r--   0        0        0     8211 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/automation_management_service.py
+-rw-r--r--   0        0        0     1019 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/autoscaling_service_api.py
+-rw-r--r--   0        0        0    12145 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/batch_job_manager_service.py
+-rw-r--r--   0        0        0     3841 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/build_management.py
+-rw-r--r--   0        0        0     3909 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/build_orchestrator_build_api.py
+-rw-r--r--   0        0        0     4150 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/build_orchestrator_service_api.py
+-rw-r--r--   0        0        0     1412 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/data_versioning_service.py
+-rw-r--r--   0        0        0    18268 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/deployment_management_service.py
+-rw-r--r--   0        0        0     1158 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/ecosystem_service_api.py
+-rw-r--r--   0        0        0     1536 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py
+-rw-r--r--   0        0        0     1782 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/feature_store_entities_manager_api.py
+-rw-r--r--   0        0        0     3261 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py
+-rw-r--r--   0        0        0     5806 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/features_online_serving_api.py
+-rw-r--r--   0        0        0     1001 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/features_operator_v3_service.py
+-rw-r--r--   0        0        0     2276 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/features_set_state_service_api.py
+-rw-r--r--   0        0        0     1127 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/feedback_service.py
+-rw-r--r--   0        0        0     1412 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/file_versioning_service.py
+-rw-r--r--   0        0        0     2696 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/job_registry_service_api.py
+-rw-r--r--   0        0        0     1583 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/kube_captain_service_api.py
+-rw-r--r--   0        0        0     7381 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/logging_service.py
+-rw-r--r--   0        0        0     3566 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/model_management_service.py
+-rw-r--r--   0        0        0     3090 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/project_manager_service.py
+-rw-r--r--   0        0        0     3995 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/qwak_mocks.py
+-rw-r--r--   0        0        0     1406 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/secret_service.py
+-rw-r--r--   0        0        0     1205 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/self_service_user_service.py
+-rw-r--r--   0        0        0     4083 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/user_application_instance_service_api.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/utils/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/mocks/utils/exception_handlers.py
+-rw-r--r--   0        0        0    13054 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/services_mock.py
+-rw-r--r--   0        0        0        0 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/utils/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-03 07:49:10.594164 qwak_core-0.0.43/qwak_services_mock/utils/service_utils.py
+-rw-r--r--   0        0        0     4873 1970-01-01 00:00:00.000000 qwak_core-0.0.43/setup.py
+-rw-r--r--   0        0        0     1628 1970-01-01 00:00:00.000000 qwak_core-0.0.43/PKG-INFO
```

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/account_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/account_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/account_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/preferences_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/account/v1/preferences_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/authenticated_user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/authenticated_user/v1/details_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/authentication/authentication_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/configuration_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/environment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/environments/personalization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/users/user_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/administration/v0/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/admiral/user_application_instance/v0/user_application_instance_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/analytics/analytics_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_api_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/audience/v1/audience_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/audience/v1/audience_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/auto_scaling/v1/auto_scaling_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/action_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/action_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/action_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/auto_scaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/automation_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/automation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/common_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/common_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/notification_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/notification_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/trigger_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/trigger_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/automation/v1/trigger_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/batch_job/v1/batch_job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_api_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_api_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/build/v1/build_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/build/v1/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/build_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/build_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/build_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/build_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/build_url_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/build_url_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/build_url_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/build_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_orchestrator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/builds/builds_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/builds/builds_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/data_versioning/data_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/alert_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_messages_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_messages_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/deployment/deployment_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/credentials_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/ecosystem/v0/ecosystem_runtime_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/entities/entity_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/aggregation_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/aggregation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/execution_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/execution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_state_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/feature_set_types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/features/monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/jobs/v1/job_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/reports/report_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/reports/report_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/reports/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/serving_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/serving_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/serving_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/serving_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/serving/v1/value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/batch_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/batch_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/data_source_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/streaming_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/feature_store/sources/streaming_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v1/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v2/features_operator_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_async_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/features_operator/v3/features_operator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/file_versioning/file_versioning_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/constructs_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/constructs_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/constructs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/fitness_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/status_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/status_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/fitness_service/status_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/fitness_service/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/inference/feedback/feedback_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/inference/feedback/feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/inference/feedback/feedback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/inference/feedback/feedback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/alerting_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/batch_job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/feature_set_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/kube_deployment_captain_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/kube_deployment_captain/traffic_mapping_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_filter_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_filter_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_filter_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_line_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_line_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_line_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_reader_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_reader_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_reader_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_reader_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_source_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_source_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/logging/log_source_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/logging/log_source_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/models/models_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/models/models_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/models/models_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/models/models_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/models/models_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/models/models_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_management_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/monitoring/v0/alerting_channel_sync_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/projects/projects_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/projects/projects_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/projects/projects_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/projects/projects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/projects/projects_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/projects/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/secret_service/secret_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/secret_service/secret_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/secret_service/secret_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/secret_service/secret_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/account/v0/account_membership_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/api_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/self_service/user/v1/user_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_api_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py` & `qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/traffic/v1/traffic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/user_application/common/v0/resources_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/user_application/common/v0/resources_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/user_application/v0/user_application_pb2.py` & `qwak_core-0.0.43/_qwak_proto/qwak/user_application/v0/user_application_pb2.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi` & `qwak_core-0.0.43/_qwak_proto/qwak/user_application/v0/user_application_pb2.pyi`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/pyproject.toml` & `qwak_core-0.0.43/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-core"
-version = "0.0.42"
+version = "0.0.43"
 description = "Qwak Core contains the necessary objects and communication tools for using the Qwak Platform"
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 packages = [
     { include = "qwak" },
     { include = "_qwak_proto" },
```

### Comparing `qwak_core-0.0.42/qwak/automations/__init__.py` & `qwak_core-0.0.43/qwak/automations/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/automations/automation_executions.py` & `qwak_core-0.0.43/qwak/automations/automation_executions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/automations/automations.py` & `qwak_core-0.0.43/qwak/automations/automations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/administration/authenticated_user/client.py` & `qwak_core-0.0.43/qwak/clients/administration/authenticated_user/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/administration/authentication/client.py` & `qwak_core-0.0.43/qwak/clients/administration/authentication/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/administration/eco_system/client.py` & `qwak_core-0.0.43/qwak/clients/administration/eco_system/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/administration/environment/client.py` & `qwak_core-0.0.43/qwak/clients/administration/environment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/administration/self_service/client.py` & `qwak_core-0.0.43/qwak/clients/administration/self_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/alert_management/client.py` & `qwak_core-0.0.43/qwak/clients/alert_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/analytics/client.py` & `qwak_core-0.0.43/qwak/clients/analytics/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/audience/client.py` & `qwak_core-0.0.43/qwak/clients/audience/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/automation_management/client.py` & `qwak_core-0.0.43/qwak/clients/automation_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/autoscaling/client.py` & `qwak_core-0.0.43/qwak/clients/autoscaling/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/batch_job_management/client.py` & `qwak_core-0.0.43/qwak/clients/batch_job_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/batch_job_management/executions_config.py` & `qwak_core-0.0.43/qwak/clients/batch_job_management/executions_config.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/batch_job_management/results.py` & `qwak_core-0.0.43/qwak/clients/batch_job_management/results.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/build_management/client.py` & `qwak_core-0.0.43/qwak/clients/build_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/build_orchestrator/client.py` & `qwak_core-0.0.43/qwak/clients/build_orchestrator/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/data_versioning/client.py` & `qwak_core-0.0.43/qwak/clients/data_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/deployment/client.py` & `qwak_core-0.0.43/qwak/clients/deployment/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/feature_store/job_registry_client.py` & `qwak_core-0.0.43/qwak/clients/feature_store/job_registry_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/feature_store/management_client.py` & `qwak_core-0.0.43/qwak/clients/feature_store/management_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/feature_store/operator_client.py` & `qwak_core-0.0.43/qwak/clients/feature_store/operator_client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/file_versioning/client.py` & `qwak_core-0.0.43/qwak/clients/file_versioning/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/kube_deployment_captain/client.py` & `qwak_core-0.0.43/qwak/clients/kube_deployment_captain/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/logging_client/client.py` & `qwak_core-0.0.43/qwak/clients/logging_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/model_management/client.py` & `qwak_core-0.0.43/qwak/clients/model_management/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/project/client.py` & `qwak_core-0.0.43/qwak/clients/project/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/secret_service/client.py` & `qwak_core-0.0.43/qwak/clients/secret_service/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/clients/user_application_instance/client.py` & `qwak_core-0.0.43/qwak/clients/user_application_instance/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/exceptions/quiet_error.py` & `qwak_core-0.0.43/qwak/exceptions/quiet_error.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/exceptions/qwak_http_exception.py` & `qwak_core-0.0.43/qwak/exceptions/qwak_http_exception.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/_common/featureset_asterisk_handler.py` & `qwak_core-0.0.43/qwak/feature_store/_common/featureset_asterisk_handler.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/_common/functions.py` & `qwak_core-0.0.43/qwak/feature_store/_common/functions.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/__init__.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from qwak.feature_store.data_sources.batch_sources.big_query import BigQuerySource
 from qwak.feature_store.data_sources.batch_sources.csv import CsvSource
 from qwak.feature_store.data_sources.batch_sources.elastic_search import (
     ElasticSearchSource,
 )
 from qwak.feature_store.data_sources.batch_sources.filesystem_config import (
+    AnonymousS3Configuration,
     AwsS3FileSystemConfiguration,
 )
 from qwak.feature_store.data_sources.batch_sources.mongodb import MongoDbSource
 from qwak.feature_store.data_sources.batch_sources.mysql import MysqlSource
 from qwak.feature_store.data_sources.batch_sources.parquet import ParquetSource
 from qwak.feature_store.data_sources.batch_sources.postgres import PostgresSource
 from qwak.feature_store.data_sources.batch_sources.redshift import RedshiftSource
@@ -22,8 +23,9 @@
     "ParquetSource",
     "RedshiftSource",
     "PostgresSource",
     "SnowflakeSource",
     "VerticaSource",
     "ElasticSearchSource",
     "AwsS3FileSystemConfiguration",
+    "AnonymousS3Configuration",
 ]
```

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/_batch.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/_batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/_jdbc.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/_jdbc.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/big_query.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/big_query.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/csv.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/csv.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,55 +7,52 @@
 from _qwak_proto.qwak.feature_store.sources.batch_pb2 import CsvSource as ProtoCsvSource
 from _qwak_proto.qwak.feature_store.sources.data_source_pb2 import (
     DataSourceSpec as ProtoDataSourceSpec,
 )
 from qwak.feature_store.data_sources.batch_sources._batch import BaseBatchSource
 from qwak.feature_store.data_sources.batch_sources.filesystem_config import (
     FileSystemConfiguration,
-    _filesystem_configuration_data_source_from_proto,
-    _filesystem_configuration_data_source_to_proto,
+    get_fs_config_from_proto,
 )
 
 
 @dataclass
 class CsvSource(BaseBatchSource):
     path: str
     quote_character: str = '"'
     escape_character: str = '"'
     filesystem_configuration: Optional[FileSystemConfiguration] = None
 
     @classmethod
     def _from_proto(cls, proto):
         csv = proto.csvSource
 
-        fs_conf = _filesystem_configuration_data_source_from_proto(
-            csv.filesystem_configuration
-        )
+        fs_conf = get_fs_config_from_proto(csv.filesystem_configuration)
 
         return cls(
             name=proto.name,
             date_created_column=proto.date_created_column,
             description=proto.description,
             path=csv.path,
             quote_character=csv.quote_character,
             escape_character=csv.escape_character,
-            **fs_conf,
+            filesystem_configuration=fs_conf,
         )
 
     def _to_proto(self):
-        fs_conf = _filesystem_configuration_data_source_to_proto(
-            self.filesystem_configuration
-        )
+        fs_conf = None
+        if self.filesystem_configuration:
+            fs_conf = self.filesystem_configuration._to_proto()
 
         return ProtoDataSourceSpec(
             batch_source=ProtoBatchSource(
                 name=self.name,
                 description=self.description,
                 date_created_column=self.date_created_column,
                 csvSource=ProtoCsvSource(
                     path=self.path,
                     quote_character=self.quote_character,
                     escape_character=self.escape_character,
-                    **fs_conf,
+                    filesystem_configuration=fs_conf,
                 ),
             )
         )
```

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/elastic_search.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/elastic_search.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/filesystem_config.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/filesystem_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Optional
 
 from _qwak_proto.qwak.feature_store.sources.batch_pb2 import (
+    AnonymousS3Configuration as ProtoAnonymousS3Configuration,
+)
+from _qwak_proto.qwak.feature_store.sources.batch_pb2 import (
     AwsS3FileSystemConfiguration as ProtoAwsS3FileSystemConfiguration,
 )
 from _qwak_proto.qwak.feature_store.sources.batch_pb2 import (
     FileSystemConfiguration as FileSystemConfigurationProto,
 )
 from qwak.exceptions import QwakException
 
@@ -19,14 +22,26 @@
 
     @abstractmethod
     def _from_proto(self, proto):
         pass
 
 
 @dataclass
+class AnonymousS3Configuration(FileSystemConfiguration):
+    def _to_proto(self):
+        return FileSystemConfigurationProto(
+            aws_s3_anonymous=ProtoAnonymousS3Configuration()
+        )
+
+    @classmethod
+    def _from_proto(cls, proto):
+        return cls()
+
+
+@dataclass
 class AwsS3FileSystemConfiguration(FileSystemConfiguration):
     access_key_secret_name: str
     secret_key_secret_name: str
     bucket: str
     session_token_secret_name: Optional[str] = ""
 
     def __post_init__(self):
@@ -57,35 +72,24 @@
             access_key_secret_name=proto.access_key_secret_name,
             secret_key_secret_name=proto.secret_key_secret_name,
             bucket=proto.bucket,
             session_token_secret_name=proto.session_token_secret_name,
         )
 
 
-def _filesystem_configuration_data_source_to_proto(filesystem_conf):
-    if not filesystem_conf:
-        return {}
-
-    if filesystem_conf:
-        if isinstance(filesystem_conf, AwsS3FileSystemConfiguration):
-            return {"filesystem_configuration": filesystem_conf._to_proto()}
-        else:
-            raise QwakException(
-                f"Unsupported FileSystemConfiguration: {filesystem_conf}"
-            )
-
-
-def _filesystem_configuration_data_source_from_proto(filesystem_conf):
+def get_fs_config_from_proto(filesystem_conf):
     if not filesystem_conf:
         return {}
 
     fs_conf_type = filesystem_conf.WhichOneof("type")
 
     if not fs_conf_type:
         return {}
 
     fs_conf = getattr(filesystem_conf, fs_conf_type)
     if isinstance(fs_conf, ProtoAwsS3FileSystemConfiguration):
-        aws_s3_fs = AwsS3FileSystemConfiguration._from_proto(fs_conf)
-        return {"filesystem_configuration": aws_s3_fs}
+        return AwsS3FileSystemConfiguration._from_proto(fs_conf)
+
+    elif isinstance(fs_conf, ProtoAnonymousS3Configuration):
+        return AnonymousS3Configuration._from_proto(fs_conf)
     else:
         raise QwakException(f"Unsupported FileSystemConfiguration: {fs_conf_type}")
```

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/mongodb.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/mongodb.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/mysql.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/mysql.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/parquet.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/postgres.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,53 +1,49 @@
 from dataclasses import dataclass
-from typing import Optional
 
 from _qwak_proto.qwak.feature_store.sources.batch_pb2 import (
     BatchSource as ProtoBatchSource,
 )
 from _qwak_proto.qwak.feature_store.sources.batch_pb2 import (
-    ParquetSource as ProtoParquetSource,
+    JdbcSource as ProtoJdbcSource,
+)
+from _qwak_proto.qwak.feature_store.sources.batch_pb2 import (
+    PostgresqlSource as ProtoPostgresqlSource,
 )
 from _qwak_proto.qwak.feature_store.sources.data_source_pb2 import (
     DataSourceSpec as ProtoDataSourceSpec,
 )
-from qwak.feature_store.data_sources.batch_sources._batch import BaseBatchSource
-from qwak.feature_store.data_sources.batch_sources.filesystem_config import (
-    FileSystemConfiguration,
-    _filesystem_configuration_data_source_from_proto,
-    _filesystem_configuration_data_source_to_proto,
-)
+from qwak.feature_store.data_sources.batch_sources._jdbc import JdbcSource
 
 
 @dataclass
-class ParquetSource(BaseBatchSource):
-    path: str
-    filesystem_configuration: Optional[FileSystemConfiguration] = None
-
-    @classmethod
-    def _from_proto(cls, proto):
-        parquet: ProtoParquetSource = proto.parquetSource
-        fs_conf = _filesystem_configuration_data_source_from_proto(
-            parquet.filesystem_configuration
-        )
-
-        return cls(
-            name=proto.name,
-            date_created_column=proto.date_created_column,
-            description=proto.description,
-            path=parquet.path,
-            **fs_conf,
-        )
-
+class PostgresSource(JdbcSource):
     def _to_proto(self):
-        fs_conf = _filesystem_configuration_data_source_to_proto(
-            self.filesystem_configuration
-        )
-
         return ProtoDataSourceSpec(
             batch_source=ProtoBatchSource(
                 name=self.name,
                 description=self.description,
                 date_created_column=self.date_created_column,
-                parquetSource=ProtoParquetSource(path=self.path, **fs_conf),
+                jdbcSource=ProtoJdbcSource(
+                    url=self.url,
+                    username_secret_name=self.username_secret_name,
+                    password_secret_name=self.password_secret_name,
+                    db_table=self.db_table,
+                    query=self.query,
+                    postgresqlSource=ProtoPostgresqlSource(),
+                ),
             )
         )
+
+    @classmethod
+    def _from_proto(cls, proto):
+        postgresql = proto.jdbcSource
+        return cls(
+            name=proto.name,
+            date_created_column=proto.date_created_column,
+            description=proto.description,
+            url=postgresql.url,
+            username_secret_name=postgresql.username_secret_name,
+            password_secret_name=postgresql.password_secret_name,
+            db_table=postgresql.db_table,
+            query=postgresql.query,
+        )
```

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/redshift.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/redshift.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/snowflake.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/snowflake.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/data_sources/batch_sources/vertica.py` & `qwak_core-0.0.43/qwak/feature_store/data_sources/batch_sources/vertica.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/entities/entity.py` & `qwak_core-0.0.43/qwak/feature_store/entities/entity.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/feature_sets/backfill.py` & `qwak_core-0.0.43/qwak/feature_store/feature_sets/backfill.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/feature_sets/batch.py` & `qwak_core-0.0.43/qwak/feature_store/feature_sets/batch.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/feature_sets/execution_spec.py` & `qwak_core-0.0.43/qwak/feature_store/feature_sets/execution_spec.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/feature_sets/metadata.py` & `qwak_core-0.0.43/qwak/feature_store/feature_sets/metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/feature_sets/read_policies.py` & `qwak_core-0.0.43/qwak/feature_store/feature_sets/read_policies.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/feature_sets/transformations.py` & `qwak_core-0.0.43/qwak/feature_store/feature_sets/transformations.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/offline/_query_engine.py` & `qwak_core-0.0.43/qwak/feature_store/offline/_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/offline/athena/athena_query_engine.py` & `qwak_core-0.0.43/qwak/feature_store/offline/athena/athena_query_engine.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/offline/client.py` & `qwak_core-0.0.43/qwak/feature_store/offline/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/feature_store/online/client.py` & `qwak_core-0.0.43/qwak/feature_store/online/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/const.py` & `qwak_core-0.0.43/qwak/inner/const.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/di_configuration/__init__.py` & `qwak_core-0.0.43/qwak/inner/di_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/di_configuration/account.py` & `qwak_core-0.0.43/qwak/inner/di_configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/di_configuration/containers.py` & `qwak_core-0.0.43/qwak/inner/di_configuration/containers.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/model_loggers_utils.py` & `qwak_core-0.0.43/qwak/inner/model_loggers_utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/singleton_meta.py` & `qwak_core-0.0.43/qwak/inner/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/tool/auth.py` & `qwak_core-0.0.43/qwak/inner/tool/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/tool/grpc/grpc_auth.py` & `qwak_core-0.0.43/qwak/inner/tool/grpc/grpc_auth.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/tool/grpc/grpc_tools.py` & `qwak_core-0.0.43/qwak/inner/tool/grpc/grpc_tools.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/tool/run_config/base.py` & `qwak_core-0.0.43/qwak/inner/tool/run_config/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/inner/tool/run_config/utils.py` & `qwak_core-0.0.43/qwak/inner/tool/run_config/utils.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/adapters/__init__.py` & `qwak_core-0.0.43/qwak/model/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/adapters/input_adapters/multi_input_adapter.py` & `qwak_core-0.0.43/qwak/model/adapters/input_adapters/multi_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/adapters/input_adapters/numpy_input_adapter.py` & `qwak_core-0.0.43/qwak/model/adapters/input_adapters/numpy_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/adapters/input_adapters/proto_input_adapter.py` & `qwak_core-0.0.43/qwak/model/adapters/input_adapters/proto_input_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/adapters/output_adapters/numpy_output_adapter.py` & `qwak_core-0.0.43/qwak/model/adapters/output_adapters/numpy_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/adapters/output_adapters/proto_output_adapter.py` & `qwak_core-0.0.43/qwak/model/adapters/output_adapters/proto_output_adapter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/base.py` & `qwak_core-0.0.43/qwak/model/base.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/decorators/api.py` & `qwak_core-0.0.43/qwak/model/decorators/api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/decorators/api_implementation.py` & `qwak_core-0.0.43/qwak/model/decorators/api_implementation.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/experiment_tracking.py` & `qwak_core-0.0.43/qwak/model/experiment_tracking.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/schema.py` & `qwak_core-0.0.43/qwak/model/schema.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/schema_entities.py` & `qwak_core-0.0.43/qwak/model/schema_entities.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/encoders.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/encoders.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/input.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/base_input.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/base_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/dataframe_input.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/dataframe_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/image_input.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/image_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/json_input.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/json_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/input_adapters/tf_tensor_input.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/output.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/dataframe_output.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/dataframe_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/default_output.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/default_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/json_output.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/json_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py` & `qwak_core-0.0.43/qwak/model/tools/adapters/output_adapters/tf_tensor_output.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model/tools/run_model_locally.py` & `qwak_core-0.0.43/qwak/model/tools/run_model_locally.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model_loggers/artifact_logger.py` & `qwak_core-0.0.43/qwak/model_loggers/artifact_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model_loggers/data_logger.py` & `qwak_core-0.0.43/qwak/model_loggers/data_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/model_loggers/model_logger.py` & `qwak_core-0.0.43/qwak/model_loggers/model_logger.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/qwak_client/builds/build.py` & `qwak_core-0.0.43/qwak/qwak_client/builds/build.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/qwak_client/builds/filters/metric_filter.py` & `qwak_core-0.0.43/qwak/qwak_client/builds/filters/metric_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/qwak_client/builds/filters/parameter_filter.py` & `qwak_core-0.0.43/qwak/qwak_client/builds/filters/parameter_filter.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/qwak_client/client.py` & `qwak_core-0.0.43/qwak/qwak_client/client.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/qwak_client/deployments/deployment.py` & `qwak_core-0.0.43/qwak/qwak_client/deployments/deployment.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/qwak_client/models/model.py` & `qwak_core-0.0.43/qwak/qwak_client/models/model.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/qwak_client/models/model_metadata.py` & `qwak_core-0.0.43/qwak/qwak_client/models/model_metadata.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak/qwak_client/projects/project.py` & `qwak_core-0.0.43/qwak/qwak_client/projects/project.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/alert_manager_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/alert_manager_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/analytics_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/analytics_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/audience_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/audience_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/authentication_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/authentication_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/automation_management_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/automation_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/autoscaling_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/autoscaling_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/batch_job_manager_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/batch_job_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/build_management.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/build_management.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/build_orchestrator_build_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/build_orchestrator_build_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/build_orchestrator_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/build_orchestrator_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/data_versioning_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/data_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/deployment_management_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/deployment_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/ecosystem_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/ecosystem_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/feature_store_data_sources_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/feature_store_entities_manager_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/feature_store_entities_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/feature_store_feature_set_manager_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/features_online_serving_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/features_online_serving_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/features_operator_v3_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/features_operator_v3_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/features_set_state_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/features_set_state_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/feedback_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/feedback_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/file_versioning_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/file_versioning_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/job_registry_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/job_registry_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/kube_captain_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/kube_captain_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/logging_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/logging_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/model_management_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/model_management_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/project_manager_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/project_manager_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/qwak_mocks.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/qwak_mocks.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/secret_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/secret_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/self_service_user_service.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/self_service_user_service.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/mocks/user_application_instance_service_api.py` & `qwak_core-0.0.43/qwak_services_mock/mocks/user_application_instance_service_api.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/qwak_services_mock/services_mock.py` & `qwak_core-0.0.43/qwak_services_mock/services_mock.py`

 * *Files identical despite different names*

### Comparing `qwak_core-0.0.42/setup.py` & `qwak_core-0.0.43/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
  'typeguard>=2,<3']
 
 extras_require = \
 {'feature-store': ['pyarrow>=6.0.0', 'pyathena>=2.2.0,!=2.18.0']}
 
 setup_kwargs = {
     'name': 'qwak-core',
-    'version': '0.0.42',
+    'version': '0.0.43',
     'description': 'Qwak Core contains the necessary objects and communication tools for using the Qwak Platform',
     'long_description': '# Qwak Core\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Core contains all the objects and tools necessary to use the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_core-0.0.42/PKG-INFO` & `qwak_core-0.0.43/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-core
-Version: 0.0.42
+Version: 0.0.43
 Summary: Qwak Core contains the necessary objects and communication tools for using the Qwak Platform
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

