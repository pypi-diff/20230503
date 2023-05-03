# Comparing `tmp/qcs-api-client-0.8.0.dev1457087914.tar.gz` & `tmp/qcs-api-client-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcs-api-client-0.8.0.dev1457087914.tar", max compression
+gzip compressed data, was "qcs-api-client-0.9.0.tar", max compression
```

## Comparing `qcs-api-client-0.8.0.dev1457087914.tar` & `qcs-api-client-0.9.0.tar`

### file list

```diff
@@ -1,127 +1,122 @@
--rw-r--r--   0        0        0    11352 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/LICENSE
--rw-r--r--   0        0        0      815 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/README.md
--rw-r--r--   0        0        0     1105 2021-07-27 22:15:51.767955 qcs-api-client-0.8.0.dev1457087914/pyproject.toml
--rw-r--r--   0        0        0       55 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/__init__.py
--rw-r--r--   0        0        0       47 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/__init__.py
--rw-r--r--   0        0        0     2996 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/add_group_user.py
--rw-r--r--   0        0        0     3117 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/list_group_users.py
--rw-r--r--   0        0        0     3005 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/list_user_groups.py
--rw-r--r--   0        0        0     3029 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/remove_group_user.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/__init__.py
--rw-r--r--   0        0        0     3159 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/auth_email_password_reset_token.py
--rw-r--r--   0        0        0     2471 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/auth_get_user.py
--rw-r--r--   0        0        0     3047 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/auth_reset_password.py
--rw-r--r--   0        0        0     3148 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/auth_reset_password_with_token.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/client_applications/__init__.py
--rw-r--r--   0        0        0     3402 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/client_applications/check_client_application.py
--rw-r--r--   0        0        0     3411 2021-07-27 22:00:59.886083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/client_applications/get_client_application.py
--rw-r--r--   0        0        0     2732 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/client_applications/list_client_applications.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/default/__init__.py
--rw-r--r--   0        0        0     2429 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/default/get_health.py
--rw-r--r--   0        0        0     2364 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/default/health_check.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/__init__.py
--rw-r--r--   0        0        0     3105 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/create_endpoint.py
--rw-r--r--   0        0        0     2918 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/delete_endpoint.py
--rw-r--r--   0        0        0     3334 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/get_default_endpoint.py
--rw-r--r--   0        0        0     3001 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/get_endpoint.py
--rw-r--r--   0        0        0     3857 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/list_endpoints.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/engagements/__init__.py
--rw-r--r--   0        0        0     3261 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/engagements/create_engagement.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/quantum_processors/__init__.py
--rw-r--r--   0        0        0     3522 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/quantum_processors/get_instruction_set_architecture.py
--rw-r--r--   0        0        0     3323 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/quantum_processors/get_quantum_processor.py
--rw-r--r--   0        0        0     3617 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/quantum_processors/list_quantum_processors.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/__init__.py
--rw-r--r--   0        0        0     3144 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/create_reservation.py
--rw-r--r--   0        0        0     2610 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/delete_reservation.py
--rw-r--r--   0        0        0     4129 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/find_available_reservations.py
--rw-r--r--   0        0        0     2653 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/list_reservations.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/translation/__init__.py
--rw-r--r--   0        0        0     3505 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/translation/get_quilt_calibrations.py
--rw-r--r--   0        0        0     4447 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/translation/translate_native_quil_to_encrypted_binary.py
--rw-r--r--   0        0        0      220 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/__init__.py
--rw-r--r--   0        0        0      588 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/__init__.py
--rw-r--r--   0        0        0     2596 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/configuration.py
--rw-r--r--   0        0        0     1674 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/environment.py
--rw-r--r--   0        0        0       55 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/error.py
--rw-r--r--   0        0        0     1942 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/file.py
--rw-r--r--   0        0        0     4125 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/secrets.py
--rw-r--r--   0        0        0     2727 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/settings.py
--rw-r--r--   0        0        0     4614 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/auth.py
--rw-r--r--   0        0        0     1759 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/client.py
--rw-r--r--   0        0        0        0 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/grpc/__init__.py
--rw-r--r--   0        0        0        0 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/grpc/models/__init__.py
--rw-r--r--   0        0        0     4488 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/grpc/models/controller.py
--rw-r--r--   0        0        0     4465 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/grpc/service_stub.py
--rw-r--r--   0        0        0        0 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/grpc/services/__init__.py
--rw-r--r--   0        0        0     2081 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/grpc/services/controller.py
--rw-r--r--   0        0        0     1759 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/grpc/services/translation.py
--rw-r--r--   0        0        0     3167 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/__init__.py
--rw-r--r--   0        0        0     2549 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/add_group_user_request.py
--rw-r--r--   0        0        0     3271 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/architecture.py
--rw-r--r--   0        0        0     1787 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/auth_email_password_reset_token_request.py
--rw-r--r--   0        0        0     1974 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/auth_reset_password_request.py
--rw-r--r--   0        0        0     2028 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/auth_reset_password_with_token_request.py
--rw-r--r--   0        0        0     2773 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/available_reservation.py
--rw-r--r--   0        0        0     2544 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/characteristic.py
--rw-r--r--   0        0        0     1891 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/check_client_application_request.py
--rw-r--r--   0        0        0     2256 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/check_client_application_response.py
--rw-r--r--   0        0        0     1981 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/checksum_description.py
--rw-r--r--   0        0        0      145 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/checksum_description_type.py
--rw-r--r--   0        0        0     3348 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/client_application.py
--rw-r--r--   0        0        0     2834 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/client_applications_download_link.py
--rw-r--r--   0        0        0     1912 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/create_endpoint_parameters.py
--rw-r--r--   0        0        0     2162 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/create_engagement_request.py
--rw-r--r--   0        0        0     2725 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/create_reservation_request.py
--rw-r--r--   0        0        0     1481 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/dictionary.py
--rw-r--r--   0        0        0     1419 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/edge.py
--rw-r--r--   0        0        0     2343 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/endpoint.py
--rw-r--r--   0        0        0     2277 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/engagement_credentials.py
--rw-r--r--   0        0        0     3234 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/engagement_with_credentials.py
--rw-r--r--   0        0        0     2887 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/error.py
--rw-r--r--   0        0        0      131 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/family.py
--rw-r--r--   0        0        0     2405 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/filter.py
--rw-r--r--   0        0        0     2821 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/find_available_reservations_response.py
--rw-r--r--   0        0        0     1745 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/get_quilt_calibrations_response.py
--rw-r--r--   0        0        0     3077 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/group.py
--rw-r--r--   0        0        0     1613 2021-07-27 22:14:50.443153 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/health.py
--rw-r--r--   0        0        0     3033 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/instruction_set_architecture.py
--rw-r--r--   0        0        0     1594 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/internal_create_reservation_request.py
--rw-r--r--   0        0        0     1937 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/invite_user_request.py
--rw-r--r--   0        0        0     2418 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_client_applications_response.py
--rw-r--r--   0        0        0     2426 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_endpoints_response.py
--rw-r--r--   0        0        0     2335 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_group_users_response.py
--rw-r--r--   0        0        0     2333 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_groups_response.py
--rw-r--r--   0        0        0     2697 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_quantum_processors_response.py
--rw-r--r--   0        0        0     2426 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_reservations_response.py
--rw-r--r--   0        0        0     1237 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/node.py
--rw-r--r--   0        0        0     3023 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/operation.py
--rw-r--r--   0        0        0     1788 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/operation_site.py
--rw-r--r--   0        0        0     1856 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/order.py
--rw-r--r--   0        0        0      960 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/parameter.py
--rw-r--r--   0        0        0     1706 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/parameter_spec.py
--rw-r--r--   0        0        0     1640 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/quantum_processor.py
--rw-r--r--   0        0        0     2567 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/remove_group_user_request.py
--rw-r--r--   0        0        0     4189 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/reservation.py
--rw-r--r--   0        0        0     2341 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/translate_native_quil_to_encrypted_binary_request.py
--rw-r--r--   0        0        0     3669 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/translate_native_quil_to_encrypted_binary_response.py
--rw-r--r--   0        0        0     2216 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/translate_native_quil_to_encrypted_binary_response_memory_descriptors.py
--rw-r--r--   0        0        0     2711 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/user.py
--rw-r--r--   0        0        0     1824 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/user_credentials.py
--rw-r--r--   0        0        0     1712 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/user_credentials_password.py
--rw-r--r--   0        0        0     2170 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/user_profile.py
--rw-r--r--   0        0        0     2216 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/validation_error.py
--rw-r--r--   0        0        0      200 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/validation_error_in.py
--rw-r--r--   0        0        0        0 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/__init__.py
--rw-r--r--   0        0        0     2733 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/asyncio/__init__.py
--rw-r--r--   0        0        0     3049 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/asyncio_from_dict/__init__.py
--rw-r--r--   0        0        0     2649 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/sync/__init__.py
--rw-r--r--   0        0        0     2947 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/sync_from_dict/__init__.py
--rw-r--r--   0        0        0       25 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/py.typed
--rw-r--r--   0        0        0     1956 2021-07-27 22:14:50.447154 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/types.py
--rw-r--r--   0        0        0     1109 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/util/errors.py
--rw-r--r--   0        0        0      593 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/util/retry.py
--rw-r--r--   0        0        0       91 2021-07-27 22:00:59.890083 qcs-api-client-0.8.0.dev1457087914/qcs_api_client/util/serialization.py
--rw-r--r--   0        0        0     2466 2021-07-27 22:15:53.654498 qcs-api-client-0.8.0.dev1457087914/setup.py
--rw-r--r--   0        0        0     1756 2021-07-27 22:15:53.654832 qcs-api-client-0.8.0.dev1457087914/PKG-INFO
+-rw-r--r--   0        0        0    11352 2021-09-23 20:33:09.233332 qcs-api-client-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2773 2021-09-23 20:33:09.233332 qcs-api-client-0.9.0/README.md
+-rw-r--r--   0        0        0     1216 2021-09-23 20:33:09.233332 qcs-api-client-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       55 2021-09-23 20:33:09.233332 qcs-api-client-0.9.0/qcs_api_client/__init__.py
+-rw-r--r--   0        0        0       47 2021-09-23 20:33:09.233332 qcs-api-client-0.9.0/qcs_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.233332 qcs-api-client-0.9.0/qcs_api_client/api/account/__init__.py
+-rw-r--r--   0        0        0     2996 2021-09-23 20:33:09.233332 qcs-api-client-0.9.0/qcs_api_client/api/account/add_group_user.py
+-rw-r--r--   0        0        0     3117 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/account/list_group_users.py
+-rw-r--r--   0        0        0     3005 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/account/list_user_groups.py
+-rw-r--r--   0        0        0     3029 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/account/remove_group_user.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/authentication/__init__.py
+-rw-r--r--   0        0        0     3159 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/authentication/auth_email_password_reset_token.py
+-rw-r--r--   0        0        0     2471 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/authentication/auth_get_user.py
+-rw-r--r--   0        0        0     3047 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/authentication/auth_reset_password.py
+-rw-r--r--   0        0        0     3148 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/authentication/auth_reset_password_with_token.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/client_applications/__init__.py
+-rw-r--r--   0        0        0     3402 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/client_applications/check_client_application.py
+-rw-r--r--   0        0        0     3411 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/client_applications/get_client_application.py
+-rw-r--r--   0        0        0     2732 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/client_applications/list_client_applications.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/default/__init__.py
+-rw-r--r--   0        0        0     2429 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/default/get_health.py
+-rw-r--r--   0        0        0     2364 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/default/health_check.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/endpoints/__init__.py
+-rw-r--r--   0        0        0     3105 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/endpoints/create_endpoint.py
+-rw-r--r--   0        0        0     2918 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/endpoints/delete_endpoint.py
+-rw-r--r--   0        0        0     3334 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/endpoints/get_default_endpoint.py
+-rw-r--r--   0        0        0     3001 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/endpoints/get_endpoint.py
+-rw-r--r--   0        0        0     3857 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/endpoints/list_endpoints.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/engagements/__init__.py
+-rw-r--r--   0        0        0     3261 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/engagements/create_engagement.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/quantum_processors/__init__.py
+-rw-r--r--   0        0        0     3522 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/quantum_processors/get_instruction_set_architecture.py
+-rw-r--r--   0        0        0     3323 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/quantum_processors/get_quantum_processor.py
+-rw-r--r--   0        0        0     3617 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/quantum_processors/list_quantum_processors.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/reservations/__init__.py
+-rw-r--r--   0        0        0     3144 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/reservations/create_reservation.py
+-rw-r--r--   0        0        0     2610 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/reservations/delete_reservation.py
+-rw-r--r--   0        0        0     4129 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/reservations/find_available_reservations.py
+-rw-r--r--   0        0        0     2653 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/reservations/list_reservations.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/translation/__init__.py
+-rw-r--r--   0        0        0     3505 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/translation/get_quilt_calibrations.py
+-rw-r--r--   0        0        0     4447 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/api/translation/translate_native_quil_to_encrypted_binary.py
+-rw-r--r--   0        0        0      220 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/__init__.py
+-rw-r--r--   0        0        0      588 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/_configuration/__init__.py
+-rw-r--r--   0        0        0     5877 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/_configuration/configuration.py
+-rw-r--r--   0        0        0     1674 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/_configuration/environment.py
+-rw-r--r--   0        0        0       55 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/_configuration/error.py
+-rw-r--r--   0        0        0     1942 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/_configuration/file.py
+-rw-r--r--   0        0        0     4528 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/_configuration/secrets.py
+-rw-r--r--   0        0        0     3713 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/_configuration/settings.py
+-rw-r--r--   0        0        0     5855 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/auth.py
+-rw-r--r--   0        0        0     1759 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/client/client.py
+-rw-r--r--   0        0        0     3217 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/__init__.py
+-rw-r--r--   0        0        0     2551 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/add_group_user_request.py
+-rw-r--r--   0        0        0     3271 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/architecture.py
+-rw-r--r--   0        0        0     1788 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/auth_email_password_reset_token_request.py
+-rw-r--r--   0        0        0     1975 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/auth_reset_password_request.py
+-rw-r--r--   0        0        0     2030 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/auth_reset_password_with_token_request.py
+-rw-r--r--   0        0        0     2774 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/available_reservation.py
+-rw-r--r--   0        0        0     2546 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/characteristic.py
+-rw-r--r--   0        0        0     1892 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/check_client_application_request.py
+-rw-r--r--   0        0        0     2257 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/check_client_application_response.py
+-rw-r--r--   0        0        0     1982 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/checksum_description.py
+-rw-r--r--   0        0        0      145 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/checksum_description_type.py
+-rw-r--r--   0        0        0     3349 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/client_application.py
+-rw-r--r--   0        0        0     2835 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/client_applications_download_link.py
+-rw-r--r--   0        0        0     1914 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/create_endpoint_parameters.py
+-rw-r--r--   0        0        0     2163 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/create_engagement_request.py
+-rw-r--r--   0        0        0     2726 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/create_reservation_request.py
+-rw-r--r--   0        0        0     1483 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/dictionary.py
+-rw-r--r--   0        0        0     1419 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/edge.py
+-rw-r--r--   0        0        0     2622 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/endpoint.py
+-rw-r--r--   0        0        0     1959 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/endpoint_addresses.py
+-rw-r--r--   0        0        0     2277 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/engagement_credentials.py
+-rw-r--r--   0        0        0     3236 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/engagement_with_credentials.py
+-rw-r--r--   0        0        0     2888 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/error.py
+-rw-r--r--   0        0        0      131 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/family.py
+-rw-r--r--   0        0        0     2405 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/filter.py
+-rw-r--r--   0        0        0     2822 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/find_available_reservations_response.py
+-rw-r--r--   0        0        0     1746 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/get_quilt_calibrations_response.py
+-rw-r--r--   0        0        0     3078 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/group.py
+-rw-r--r--   0        0        0     1614 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/health.py
+-rw-r--r--   0        0        0     3033 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/instruction_set_architecture.py
+-rw-r--r--   0        0        0     1595 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/internal_create_reservation_request.py
+-rw-r--r--   0        0        0     1938 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/invite_user_request.py
+-rw-r--r--   0        0        0     2419 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/list_client_applications_response.py
+-rw-r--r--   0        0        0     2427 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/list_endpoints_response.py
+-rw-r--r--   0        0        0     2336 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/list_group_users_response.py
+-rw-r--r--   0        0        0     2334 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/list_groups_response.py
+-rw-r--r--   0        0        0     2698 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/list_quantum_processors_response.py
+-rw-r--r--   0        0        0     2427 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/list_reservations_response.py
+-rw-r--r--   0        0        0     1237 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/node.py
+-rw-r--r--   0        0        0     3025 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/operation.py
+-rw-r--r--   0        0        0     1790 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/operation_site.py
+-rw-r--r--   0        0        0     1856 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/order.py
+-rw-r--r--   0        0        0      962 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/parameter.py
+-rw-r--r--   0        0        0     1707 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/parameter_spec.py
+-rw-r--r--   0        0        0     1641 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/quantum_processor.py
+-rw-r--r--   0        0        0     2569 2021-09-23 20:33:09.237332 qcs-api-client-0.9.0/qcs_api_client/models/remove_group_user_request.py
+-rw-r--r--   0        0        0     4190 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/reservation.py
+-rw-r--r--   0        0        0     2342 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/translate_native_quil_to_encrypted_binary_request.py
+-rw-r--r--   0        0        0     3670 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/translate_native_quil_to_encrypted_binary_response.py
+-rw-r--r--   0        0        0     2217 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/translate_native_quil_to_encrypted_binary_response_memory_descriptors.py
+-rw-r--r--   0        0        0     2712 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/user.py
+-rw-r--r--   0        0        0     1825 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/user_credentials.py
+-rw-r--r--   0        0        0     1713 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/user_credentials_password.py
+-rw-r--r--   0        0        0     2171 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/user_profile.py
+-rw-r--r--   0        0        0     2217 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/validation_error.py
+-rw-r--r--   0        0        0      200 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/models/validation_error_in.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/operations/__init__.py
+-rw-r--r--   0        0        0     2733 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/operations/asyncio/__init__.py
+-rw-r--r--   0        0        0     3049 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/operations/asyncio_from_dict/__init__.py
+-rw-r--r--   0        0        0     2649 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/operations/sync/__init__.py
+-rw-r--r--   0        0        0     2947 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/operations/sync_from_dict/__init__.py
+-rw-r--r--   0        0        0       25 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/py.typed
+-rw-r--r--   0        0        0     1960 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/types.py
+-rw-r--r--   0        0        0        0 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/util/__init__.py
+-rw-r--r--   0        0        0     1109 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/util/errors.py
+-rw-r--r--   0        0        0      593 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/util/retry.py
+-rw-r--r--   0        0        0       91 2021-09-23 20:33:09.241332 qcs-api-client-0.9.0/qcs_api_client/util/serialization.py
+-rw-r--r--   0        0        0     4380 2021-09-23 20:33:21.098512 qcs-api-client-0.9.0/setup.py
+-rw-r--r--   0        0        0     3884 2021-09-23 20:33:21.099110 qcs-api-client-0.9.0/PKG-INFO
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/LICENSE` & `qcs-api-client-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/pyproject.toml` & `qcs-api-client-0.9.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [tool.poetry]
 name = "qcs-api-client"
-version = "0.8.0.dev1457087914"
+version = "0.9.0"
 description = "A client library for accessing the Rigetti QCS API"
 license = "Apache-2.0"
+repository = "https://github.com/rigetti/qcs-api-client-python"
+documentation = "https://qcs-api-client-python.readthedocs.io/en/latest/index.html"
 
 authors = []
 
 readme = "README.md"
 packages = [
     {include = "qcs_api_client"},
 ]
@@ -20,15 +22,14 @@
 pydantic = "^1.7.2"
 pyjwt = "^1.7.1"
 python = "^3.6"
 python-dateutil = "^2.8.1"
 retrying = "^1.3.3"
 rfc3339 = "^6.2"
 toml = "^0.10.2"
-betterproto = "^1.2.5"
 
 
 [tool.poetry.dev-dependencies]
 black = "20.8b1"
 flake8 = "^3.8.4"
 pytest = "^6.1.2"
 respx = "^0.15.1"
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/add_group_user.py` & `qcs-api-client-0.9.0/qcs_api_client/api/account/add_group_user.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/list_group_users.py` & `qcs-api-client-0.9.0/qcs_api_client/api/account/list_group_users.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/list_user_groups.py` & `qcs-api-client-0.9.0/qcs_api_client/api/account/list_user_groups.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/account/remove_group_user.py` & `qcs-api-client-0.9.0/qcs_api_client/api/account/remove_group_user.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/auth_email_password_reset_token.py` & `qcs-api-client-0.9.0/qcs_api_client/api/authentication/auth_email_password_reset_token.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/auth_get_user.py` & `qcs-api-client-0.9.0/qcs_api_client/api/authentication/auth_get_user.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/auth_reset_password.py` & `qcs-api-client-0.9.0/qcs_api_client/api/authentication/auth_reset_password.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/authentication/auth_reset_password_with_token.py` & `qcs-api-client-0.9.0/qcs_api_client/api/authentication/auth_reset_password_with_token.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/client_applications/check_client_application.py` & `qcs-api-client-0.9.0/qcs_api_client/api/client_applications/check_client_application.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/client_applications/get_client_application.py` & `qcs-api-client-0.9.0/qcs_api_client/api/client_applications/get_client_application.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/client_applications/list_client_applications.py` & `qcs-api-client-0.9.0/qcs_api_client/api/client_applications/list_client_applications.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/default/get_health.py` & `qcs-api-client-0.9.0/qcs_api_client/api/default/get_health.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/default/health_check.py` & `qcs-api-client-0.9.0/qcs_api_client/api/default/health_check.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/create_endpoint.py` & `qcs-api-client-0.9.0/qcs_api_client/api/endpoints/create_endpoint.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/delete_endpoint.py` & `qcs-api-client-0.9.0/qcs_api_client/api/endpoints/delete_endpoint.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/get_default_endpoint.py` & `qcs-api-client-0.9.0/qcs_api_client/api/endpoints/get_default_endpoint.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/get_endpoint.py` & `qcs-api-client-0.9.0/qcs_api_client/api/endpoints/get_endpoint.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/endpoints/list_endpoints.py` & `qcs-api-client-0.9.0/qcs_api_client/api/endpoints/list_endpoints.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/engagements/create_engagement.py` & `qcs-api-client-0.9.0/qcs_api_client/api/engagements/create_engagement.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/quantum_processors/get_instruction_set_architecture.py` & `qcs-api-client-0.9.0/qcs_api_client/api/quantum_processors/get_instruction_set_architecture.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/quantum_processors/get_quantum_processor.py` & `qcs-api-client-0.9.0/qcs_api_client/api/quantum_processors/get_quantum_processor.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/quantum_processors/list_quantum_processors.py` & `qcs-api-client-0.9.0/qcs_api_client/api/quantum_processors/list_quantum_processors.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/create_reservation.py` & `qcs-api-client-0.9.0/qcs_api_client/api/reservations/create_reservation.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/delete_reservation.py` & `qcs-api-client-0.9.0/qcs_api_client/api/reservations/delete_reservation.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/find_available_reservations.py` & `qcs-api-client-0.9.0/qcs_api_client/api/reservations/find_available_reservations.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/reservations/list_reservations.py` & `qcs-api-client-0.9.0/qcs_api_client/api/reservations/list_reservations.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/translation/get_quilt_calibrations.py` & `qcs-api-client-0.9.0/qcs_api_client/api/translation/get_quilt_calibrations.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/api/translation/translate_native_quil_to_encrypted_binary.py` & `qcs-api-client-0.9.0/qcs_api_client/api/translation/translate_native_quil_to_encrypted_binary.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/__init__.py` & `qcs-api-client-0.9.0/qcs_api_client/client/_configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/environment.py` & `qcs-api-client-0.9.0/qcs_api_client/client/_configuration/environment.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/file.py` & `qcs-api-client-0.9.0/qcs_api_client/client/_configuration/file.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/secrets.py` & `qcs-api-client-0.9.0/qcs_api_client/client/_configuration/secrets.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,93 +10,97 @@
 from qcs_api_client.client._configuration.file import QCSClientConfigurationFile
 
 _TOKEN_REFRESH_PREEMPT_INTERVAL = timedelta(seconds=15)
 _secrets_write_lock = threading.RLock()
 
 
 class TokenPayload(BaseModel):
-    """
-    TokenPayload represents a response from the OAuth2 POST /token endpoint.
+    """TokenPayload represents a response from the OAuth2 POST /token endpoint.
+
+    It contains an `access_token` which may be set as a Bearer token in the
+    Authorization header on HTTP requests to the QCS API.
+
+    ``QCSAuth`` will use the ``refresh_token`` to refresh the ``access_token`` if the
+    token expires.
     """
 
     refresh_token: Optional[str]
     access_token: Optional[str]
     scope: Optional[str]
     expires_in: Optional[int]
     id_token: Optional[str]
     token_type: Optional[str]
 
     def get_access_token_claims(self, key: Union[None, bytes, str] = None):
-        """
-        Return the claims within the encoded access token.
+        """Return the claims within the encoded access token.
 
         If a JWK is provided as ``key``, verify the claims as well. If no key is provided, be aware
         that the returned claims might be forged or invalid.
         """
         if key is None:
             return decode(self.access_token, verify=False)
 
         return decode(self.access_token, key=key)
 
     @property
     def access_token_expires_at(self) -> Optional[datetime]:
-        """
-        Return the datetime that the token expires (if any).
-        """
+        """Return the datetime that the token expires (if any)."""
         claims = self.get_access_token_claims()
         iat = claims.get("iat")
         if iat is None:
             return None
         return datetime.utcfromtimestamp(int(iat))
 
     def should_refresh(self) -> bool:
-        """
-        Return True if the token is past or nearing expiration and should be refreshed from the
-        auth server.
-        """
+        """Return True if the token is past or nearing expiration and should be refreshed."""
         iat = self.access_token_expires_at
         if iat is None:
             return False
         return iat - _TOKEN_REFRESH_PREEMPT_INTERVAL < datetime.now().astimezone(timezone.utc)
 
 
 class QCSClientConfigurationSecretsCredentials(BaseModel):
+    """A set of credentials containing a ``TokenPayload``."""
+
     token_payload: Optional[TokenPayload] = None
 
     @property
     def access_token(self) -> Optional[str]:
         if self.token_payload is not None:
             return self.token_payload.access_token
 
     @property
     def refresh_token(self) -> Optional[str]:
         if self.token_payload is not None:
             return self.token_payload.refresh_token
 
 
 class QCSClientConfigurationSecrets(QCSClientConfigurationFile):
+    """The user's full set of QCS secrets.
+
+    This class maps ``QCSClientConfigurationSecretsCredentials`` by
+    user specified names. Each set of credentials, in turn,
+    contains a ``TokenPayload``.
+    """
+
     credentials: Dict[str, QCSClientConfigurationSecretsCredentials] = Field(
         default_factory=lambda: dict(default=QCSClientConfigurationSecretsCredentials())
     )
 
     def update_token(self, *, credentials_name: str, token: TokenPayload) -> None:
-        """
-        Update the value of a token payload in memory and (if appropriate) on disk.
-        """
+        """Update the value of a token payload in memory and (if appropriate) on disk."""
         with _secrets_write_lock:
             if credentials_name not in self.credentials:
                 self.credentials[credentials_name] = QCSClientConfigurationSecretsCredentials()
             self.credentials[credentials_name].token_payload = token
 
             self._write_token_to_file(credentials_name=credentials_name, token=token)
 
     def _write_token_to_file(self, *, credentials_name: str, token: TokenPayload) -> None:
-        """
-        Update the value of a token payload within the file, if a file path is provided.
-        """
+        """Update the value of a token payload within the file, if a file path is provided."""
         if self.file_path is None:
             return
 
         with open(self.file_path, "r") as f:
             current_data = toml.load(f)
 
         try:
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/_configuration/settings.py` & `qcs-api-client-0.9.0/qcs_api_client/client/_configuration/settings.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from pydantic.fields import Field
 from pydantic.networks import HttpUrl
 from qcs_api_client.client._configuration.environment import EnvironmentModel
 from qcs_api_client.client._configuration.file import QCSClientConfigurationFile
 
 
 class QCSAuthServer(BaseModel):
+    """Specifies an OAuth2 authorization server against which to refresh tokens."""
+
     client_id: str
     issuer: str
 
     def authorize_url(self):
         return f"{self.issuer}/v1/authorize"
 
     def token_url(self):
@@ -54,35 +56,59 @@
 
     pyquil: QCSClientConfigurationSettingsApplicationsPyquil = Field(
         default_factory=QCSClientConfigurationSettingsApplicationsPyquil
     )
 
 
 class QCSClientConfigurationSettingsProfile(EnvironmentModel):
-    api_url: HttpUrl = "https://api.qcs.rigetti.com"
-    """URL of the QCS API to use for all JSON HTTP API calls"""
+    """Specifies the authorization server, credentials, and API URL.
 
-    grpc_api_url: HttpUrl = "https://grpc.qcs.rigetti.com"
-    """URL of the QCS API to use for most gRPC API calls"""
+    The attributes of this class can be used to initialize an
+    ``httpx.Client`` with the correct base URL and the ``QCSAuth``
+    middleware for making authenticated API calls against the QCS API.
+
+    ``QCSClientConfigurationSettings`` may contain several profiles, which
+    ``QCSClientConfiguration.profile_name`` may key into.
+    """
+
+    api_url: HttpUrl = "https://api.qcs.rigetti.com"
+    """URL of the QCS API to use for all API calls"""
 
     auth_server_name: str = "default"
+    """Key for `QCSClientConfigurationSettings.auth_servers`."""
 
     applications: QCSClientConfigurationSettingsApplications = Field(
         default_factory=QCSClientConfigurationSettingsApplications
     )
+    """Application specific configuration values."""
 
     credentials_name: str = "default"
+    """Key for ``QCSClientConfigurationSecrets.credentials``."""
 
     class Config:
         env_prefix = "QCS_SETTINGS_"
 
 
 class QCSClientConfigurationSettings(QCSClientConfigurationFile):
+    """A fully parsed settings configuration file.
+
+    This contains all of the user's configured authorization servers
+    and profiles. It may optionally contain a ``default_profile_name``
+    to use to override the "default" value.
+
+    ``QCSClientConfiguration`` keys into these configured values when
+    instantiated.
+    """
+
     default_profile_name: str = "default"
-    """Which profile to select settings from when none is specified."""
+    """Which profile to select settings from when none is specified.
+
+    See ``QCSClientConfiguration.load``.
+    """
 
     profiles: Dict[str, QCSClientConfigurationSettingsProfile] = Field(
         default_factory=lambda: dict(default=QCSClientConfigurationSettingsProfile())
     )
-    """All available configuration profiles, keyed by profile name."""
+    """All available configuration profiles, keyed by name."""
 
     auth_servers: Dict[str, QCSAuthServer] = Field(default_factory=lambda: {"default": _DEFAULT_AUTH_SERVER})
+    """All available authorization servers, keyed by name."""
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/client/client.py` & `qcs-api-client-0.9.0/qcs_api_client/client/client.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/__init__.py` & `qcs-api-client-0.9.0/qcs_api_client/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .client_applications_download_link import ClientApplicationsDownloadLink
 from .create_endpoint_parameters import CreateEndpointParameters
 from .create_engagement_request import CreateEngagementRequest
 from .create_reservation_request import CreateReservationRequest
 from .dictionary import Dictionary
 from .edge import Edge
 from .endpoint import Endpoint
+from .endpoint_addresses import EndpointAddresses
 from .engagement_credentials import EngagementCredentials
 from .engagement_with_credentials import EngagementWithCredentials
 from .error import Error
 from .family import Family
 from .filter import Filter
 from .find_available_reservations_response import FindAvailableReservationsResponse
 from .get_quilt_calibrations_response import GetQuiltCalibrationsResponse
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/add_group_user_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/add_group_user_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class AddGroupUserRequest:
-    """Must provide either `userId` or `userEmail` and `groupId` or `groupName`."""
+    """ Must provide either `userId` or `userEmail` and `groupId` or `groupName`. """
 
     group_id: Union[Unset, str] = UNSET
     group_name: Union[Unset, str] = UNSET
     user_email: Union[Unset, str] = UNSET
     user_id: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/architecture.py` & `qcs-api-client-0.9.0/qcs_api_client/models/architecture.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/auth_email_password_reset_token_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/auth_email_password_reset_token_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class AuthEmailPasswordResetTokenRequest:
-    """ """
+    """  """
 
     email: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         email = self.email
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/auth_reset_password_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/auth_reset_password_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class AuthResetPasswordRequest:
-    """ """
+    """  """
 
     new_password: str
     old_password: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         new_password = self.new_password
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/auth_reset_password_with_token_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/auth_reset_password_with_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class AuthResetPasswordWithTokenRequest:
-    """Token may be requested with AuthEmailPasswordResetToken."""
+    """ Token may be requested with AuthEmailPasswordResetToken. """
 
     new_password: str
     token: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         new_password = self.new_password
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/available_reservation.py` & `qcs-api-client-0.9.0/qcs_api_client/models/available_reservation.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class AvailableReservation:
-    """ """
+    """  """
 
     duration: str
     end_time: datetime.datetime
     price: int
     quantum_processor_id: str
     start_time: datetime.datetime
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/characteristic.py` & `qcs-api-client-0.9.0/qcs_api_client/models/characteristic.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Characteristic:
-    """A measured characteristic of an operation."""
+    """ A measured characteristic of an operation. """
 
     name: str
     timestamp: datetime.datetime
     value: float
     error: Union[Unset, float] = UNSET
     node_ids: Union[Unset, List[int]] = UNSET
     parameter_values: Union[Unset, List[float]] = UNSET
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/check_client_application_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/check_client_application_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class CheckClientApplicationRequest:
-    """ """
+    """  """
 
     name: str
     version: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         name = self.name
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/check_client_application_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/check_client_application_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class CheckClientApplicationResponse:
-    """ """
+    """  """
 
     is_latest_version: bool
     is_update_required: bool
     message: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/checksum_description.py` & `qcs-api-client-0.9.0/qcs_api_client/models/checksum_description.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.checksum_description_type import ChecksumDescriptionType
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ChecksumDescription:
-    """ """
+    """  """
 
     header_name: str
     type: ChecksumDescriptionType
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         header_name = self.header_name
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/client_application.py` & `qcs-api-client-0.9.0/qcs_api_client/models/client_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.client_applications_download_link import ClientApplicationsDownloadLink
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ClientApplication:
-    """ """
+    """  """
 
     latest_version: str
     name: str
     supported: bool
     details_uri: Union[Unset, str] = UNSET
     links: Union[Unset, List[ClientApplicationsDownloadLink]] = UNSET
     minimum_version: Union[Unset, str] = UNSET
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/client_applications_download_link.py` & `qcs-api-client-0.9.0/qcs_api_client/models/client_applications_download_link.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.checksum_description import ChecksumDescription
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ClientApplicationsDownloadLink:
-    """ """
+    """  """
 
     url: str
     checksum_description: Union[ChecksumDescription, Unset] = UNSET
     platform: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/create_endpoint_parameters.py` & `qcs-api-client-0.9.0/qcs_api_client/models/create_endpoint_parameters.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class CreateEndpointParameters:
-    """A publicly available set of parameters for defining an endpoint."""
+    """ A publicly available set of parameters for defining an endpoint. """
 
     quantum_processor_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         quantum_processor_id = self.quantum_processor_id
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/create_engagement_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/create_engagement_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class CreateEngagementRequest:
-    """ """
+    """  """
 
     endpoint_id: Union[Unset, str] = UNSET
     quantum_processor_id: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         endpoint_id = self.endpoint_id
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/create_reservation_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/create_reservation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class CreateReservationRequest:
-    """ """
+    """  """
 
     end_time: datetime.datetime
     quantum_processor_id: str
     start_time: datetime.datetime
     notes: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/dictionary.py` & `qcs-api-client-0.9.0/qcs_api_client/models/dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Dictionary:
-    """Generic, arbitrary Dictionary"""
+    """ Generic, arbitrary Dictionary """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/edge.py` & `qcs-api-client-0.9.0/qcs_api_client/models/edge.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/endpoint.py` & `qcs-api-client-0.9.0/qcs_api_client/models/endpoint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,43 @@
 from typing import Any, Callable, Dict, List, Optional
 
 import attr
 
+from ..models.endpoint_addresses import EndpointAddresses
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Endpoint:
     """An Endpoint is the entry point for remote access to a QuantumProcessor."""
 
     address: str
+    addresses: EndpointAddresses
     healthy: bool
     id: str
     mock: bool
     quantum_processor_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         address = self.address
+        addresses = self.addresses.to_dict()
+
         healthy = self.healthy
         id = self.id
         mock = self.mock
         quantum_processor_id = self.quantum_processor_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "address": address,
+                "addresses": addresses,
                 "healthy": healthy,
                 "id": id,
                 "mock": mock,
                 "quantumProcessorId": quantum_processor_id,
             }
         )
 
@@ -43,24 +48,27 @@
         return field_dict
 
     @staticmethod
     def from_dict(src_dict: Dict[str, Any]) -> "Endpoint":
         d = src_dict.copy()
         address = d.pop("address")
 
+        addresses = EndpointAddresses.from_dict(d.pop("addresses"))
+
         healthy = d.pop("healthy")
 
         id = d.pop("id")
 
         mock = d.pop("mock")
 
         quantum_processor_id = d.pop("quantumProcessorId")
 
         endpoint = Endpoint(
             address=address,
+            addresses=addresses,
             healthy=healthy,
             id=id,
             mock=mock,
             quantum_processor_id=quantum_processor_id,
         )
 
         endpoint.additional_properties = d
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/engagement_credentials.py` & `qcs-api-client-0.9.0/qcs_api_client/models/engagement_credentials.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/engagement_with_credentials.py` & `qcs-api-client-0.9.0/qcs_api_client/models/engagement_with_credentials.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.engagement_credentials import EngagementCredentials
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class EngagementWithCredentials:
-    """An engagement is the authorization of a user to execute work on a Quantum Processor Endpoint."""
+    """ An engagement is the authorization of a user to execute work on a Quantum Processor Endpoint. """
 
     address: str
     credentials: EngagementCredentials
     endpoint_id: str
     expires_at: str
     quantum_processor_id: str
     user_id: str
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/error.py` & `qcs-api-client-0.9.0/qcs_api_client/models/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.validation_error import ValidationError
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Error:
-    """ """
+    """  """
 
     code: str
     message: str
     request_id: str
     validation_errors: Union[Unset, List[ValidationError]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/filter.py` & `qcs-api-client-0.9.0/qcs_api_client/models/filter.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/find_available_reservations_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/find_available_reservations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.available_reservation import AvailableReservation
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class FindAvailableReservationsResponse:
-    """ """
+    """  """
 
     available_reservations: List[AvailableReservation]
     next_page_token: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         available_reservations = []
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/get_quilt_calibrations_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/get_quilt_calibrations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class GetQuiltCalibrationsResponse:
-    """ """
+    """  """
 
     quilt: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         quilt = self.quilt
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/group.py` & `qcs-api-client-0.9.0/qcs_api_client/models/group.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Group:
-    """ """
+    """  """
 
     created_time: datetime.datetime
     description: str
     id: str
     last_membership_updated_time: datetime.datetime
     name: str
     updated_time: datetime.datetime
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/health.py` & `qcs-api-client-0.9.0/qcs_api_client/models/health.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Health:
-    """ """
+    """  """
 
     status: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         status = self.status
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/instruction_set_architecture.py` & `qcs-api-client-0.9.0/qcs_api_client/models/instruction_set_architecture.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/internal_create_reservation_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/internal_create_reservation_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class InternalCreateReservationRequest:
-    """ """
+    """  """
 
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/invite_user_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/invite_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class InviteUserRequest:
-    """ """
+    """  """
 
     email: str
     group_name: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         email = self.email
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_client_applications_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/list_client_applications_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.client_application import ClientApplication
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ListClientApplicationsResponse:
-    """ """
+    """  """
 
     client_applications: List[ClientApplication]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         client_applications = []
         for client_applications_item_data in self.client_applications:
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_endpoints_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/list_endpoints_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.endpoint import Endpoint
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ListEndpointsResponse:
-    """ """
+    """  """
 
     endpoints: List[Endpoint]
     next_page_token: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         endpoints = []
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_group_users_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/list_group_users_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.user import User
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ListGroupUsersResponse:
-    """ """
+    """  """
 
     users: List[User]
     next_page_token: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         users = []
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_groups_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/list_groups_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.group import Group
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ListGroupsResponse:
-    """ """
+    """  """
 
     groups: List[Group]
     next_page_token: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         groups = []
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_quantum_processors_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/list_quantum_processors_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.quantum_processor import QuantumProcessor
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ListQuantumProcessorsResponse:
-    """ """
+    """  """
 
     quantum_processors: List[QuantumProcessor]
     next_page_token: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         quantum_processors = []
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/list_reservations_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/list_reservations_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.reservation import Reservation
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ListReservationsResponse:
-    """ """
+    """  """
 
     next_page_token: str
     reservations: List[Reservation]
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         next_page_token = self.next_page_token
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/node.py` & `qcs-api-client-0.9.0/qcs_api_client/models/node.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/operation.py` & `qcs-api-client-0.9.0/qcs_api_client/models/operation.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..models.parameter import Parameter
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Operation:
-    """An operation, with its sites and site-independent characteristics."""
+    """ An operation, with its sites and site-independent characteristics. """
 
     characteristics: List[Characteristic]
     name: str
     parameters: List[Parameter]
     sites: List[OperationSite]
     node_count: Union[Unset, int] = UNSET
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/operation_site.py` & `qcs-api-client-0.9.0/qcs_api_client/models/operation_site.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.characteristic import Characteristic
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class OperationSite:
-    """A site for an operation, with its site-dependent characteristics."""
+    """ A site for an operation, with its site-dependent characteristics. """
 
     characteristics: List[Characteristic]
     node_ids: List[int]
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         characteristics = []
         for characteristics_item_data in self.characteristics:
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/order.py` & `qcs-api-client-0.9.0/qcs_api_client/models/order.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/parameter.py` & `qcs-api-client-0.9.0/qcs_api_client/models/parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Parameter:
-    """A parameter to an operation."""
+    """ A parameter to an operation. """
 
     name: str
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         name = self.name
 
         field_dict: Dict[str, Any] = {}
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/parameter_spec.py` & `qcs-api-client-0.9.0/qcs_api_client/models/parameter_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ParameterSpec:
-    """ """
+    """  """
 
     length: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         length = self.length
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/quantum_processor.py` & `qcs-api-client-0.9.0/qcs_api_client/models/quantum_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class QuantumProcessor:
-    """ """
+    """  """
 
     id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         id = self.id
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/remove_group_user_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/remove_group_user_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class RemoveGroupUserRequest:
-    """Must provide either `userId` or `userEmail` and `groupId` or `groupName`."""
+    """ Must provide either `userId` or `userEmail` and `groupId` or `groupName`. """
 
     group_id: Union[Unset, str] = UNSET
     group_name: Union[Unset, str] = UNSET
     user_email: Union[Unset, str] = UNSET
     user_id: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/reservation.py` & `qcs-api-client-0.9.0/qcs_api_client/models/reservation.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class Reservation:
-    """ """
+    """  """
 
     created_time: datetime.datetime
     end_time: datetime.datetime
     id: int
     price: int
     quantum_processor_id: str
     start_time: datetime.datetime
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/translate_native_quil_to_encrypted_binary_request.py` & `qcs-api-client-0.9.0/qcs_api_client/models/translate_native_quil_to_encrypted_binary_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class TranslateNativeQuilToEncryptedBinaryRequest:
-    """ """
+    """  """
 
     num_shots: int
     quil: str
     settings_timestamp: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/translate_native_quil_to_encrypted_binary_response.py` & `qcs-api-client-0.9.0/qcs_api_client/models/translate_native_quil_to_encrypted_binary_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 )
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class TranslateNativeQuilToEncryptedBinaryResponse:
-    """ """
+    """  """
 
     program: str
     memory_descriptors: Union[TranslateNativeQuilToEncryptedBinaryResponseMemoryDescriptors, Unset] = UNSET
     ro_sources: Union[Unset, List[List[str]]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/translate_native_quil_to_encrypted_binary_response_memory_descriptors.py` & `qcs-api-client-0.9.0/qcs_api_client/models/translate_native_quil_to_encrypted_binary_response_memory_descriptors.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.parameter_spec import ParameterSpec
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class TranslateNativeQuilToEncryptedBinaryResponseMemoryDescriptors:
-    """ """
+    """  """
 
     additional_properties: Dict[str, ParameterSpec] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
 
         field_dict: Dict[str, Any] = {}
         for prop_name, prop in self.additional_properties.items():
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/user.py` & `qcs-api-client-0.9.0/qcs_api_client/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from ..models.user_profile import UserProfile
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class User:
-    """ """
+    """  """
 
     created_time: datetime.datetime
     id: int
     idp_id: str
     profile: Union[UserProfile, Unset] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/user_credentials.py` & `qcs-api-client-0.9.0/qcs_api_client/models/user_credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.user_credentials_password import UserCredentialsPassword
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class UserCredentials:
-    """ """
+    """  """
 
     password: UserCredentialsPassword
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         password = self.password.to_dict()
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/user_credentials_password.py` & `qcs-api-client-0.9.0/qcs_api_client/models/user_credentials_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class UserCredentialsPassword:
-    """ """
+    """  """
 
     value: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
         value = self.value
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/user_profile.py` & `qcs-api-client-0.9.0/qcs_api_client/models/user_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from ..types import UNSET
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class UserProfile:
-    """ """
+    """  """
 
     email: str
     first_name: str
     last_name: str
     organization: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/models/validation_error.py` & `qcs-api-client-0.9.0/qcs_api_client/models/validation_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from ..models.validation_error_in import ValidationErrorIn
 from ..types import UNSET, Unset
 from ..util.serialization import is_not_none
 
 
 @attr.s(auto_attribs=True)
 class ValidationError:
-    """ """
+    """  """
 
     in_: ValidationErrorIn
     message: str
     path: Union[Unset, List[str]] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
     def to_dict(self, pick_by_predicate: Optional[Callable[[Any], bool]] = is_not_none) -> Dict[str, Any]:
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/asyncio/__init__.py` & `qcs-api-client-0.9.0/qcs_api_client/operations/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/asyncio_from_dict/__init__.py` & `qcs-api-client-0.9.0/qcs_api_client/operations/asyncio_from_dict/__init__.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/sync/__init__.py` & `qcs-api-client-0.9.0/qcs_api_client/operations/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/operations/sync_from_dict/__init__.py` & `qcs-api-client-0.9.0/qcs_api_client/operations/sync_from_dict/__init__.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/types.py` & `qcs-api-client-0.9.0/qcs_api_client/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 
 
 UNSET: Unset = Unset()
 
 
 @attr.s(auto_attribs=True)
 class File:
-    """Contains information for file uploads"""
+    """ Contains information for file uploads """
 
     payload: Union[BinaryIO, TextIO]
     file_name: Optional[str] = None
     mime_type: Optional[str] = None
 
     def to_tuple(self) -> Tuple[Optional[str], Union[BinaryIO, TextIO], Optional[str]]:
-        """Return a tuple representation that httpx will accept for multipart/form-data"""
+        """ Return a tuple representation that httpx will accept for multipart/form-data """
         return self.file_name, self.payload, self.mime_type
 
 
 T = TypeVar("T")
 
 
 class Response(httpx.Response, Generic[T]):
```

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/util/errors.py` & `qcs-api-client-0.9.0/qcs_api_client/util/errors.py`

 * *Files identical despite different names*

### Comparing `qcs-api-client-0.8.0.dev1457087914/qcs_api_client/util/retry.py` & `qcs-api-client-0.9.0/qcs_api_client/util/retry.py`

 * *Files identical despite different names*

