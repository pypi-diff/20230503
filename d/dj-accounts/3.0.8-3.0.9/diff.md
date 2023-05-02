# Comparing `tmp/dj-accounts-3.0.8.tar.gz` & `tmp/dj-accounts-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-accounts-3.0.8.tar", last modified: Tue May  2 19:57:22 2023, max compression
+gzip compressed data, was "dj-accounts-3.0.9.tar", last modified: Tue May  2 23:15:12 2023, max compression
```

## Comparing `dj-accounts-3.0.8.tar` & `dj-accounts-3.0.9.tar`

### file list

```diff
@@ -1,106 +1,111 @@
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.831144 dj-accounts-3.0.8/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1145 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/LICENSE
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      100 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/MANIFEST.in
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1902 2023-05-02 19:57:22.835145 dj-accounts-3.0.8/PKG-INFO
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      628 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/README.md
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.403144 dj-accounts-3.0.8/accounts_pkg/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/accounts_pkg/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       79 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/accounts_pkg/api_urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/accounts_pkg/asgi.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4139 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/accounts_pkg/settings-multi-auth.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4119 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/accounts_pkg/settings.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      378 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/accounts_pkg/urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/accounts_pkg/wsgi.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.435145 dj-accounts-3.0.8/dj_accounts/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.0.8/dj_accounts/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      153 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/apps.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      838 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/backends.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8485 2023-05-02 17:05:25.000000 dj-accounts-3.0.8/dj_accounts/forms.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     4695 2023-05-02 17:11:11.000000 dj-accounts-3.0.8/dj_accounts/serializers.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.307144 dj-accounts-3.0.8/dj_accounts/templates/
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.599145 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      335 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/auth_base.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      573 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/confirm_email_template.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      202 2023-05-02 17:52:57.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/email_verification_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      948 2023-05-02 17:54:18.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/login.html
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.603145 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.663144 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1108 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      710 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      840 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/first_name.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      797 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/gender.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      809 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/last_name.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      634 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      655 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password1.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password2.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      668 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/phone.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      236 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/terms&conditions.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      735 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/username.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1052 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login-tabs.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      938 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login_with_email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      940 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login_with_phone.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/logo.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      383 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/social_login.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      954 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_confirm.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      659 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_done.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      615 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_email.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      555 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      132 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_subject.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/phone_verification_complete.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       34 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/profile.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      553 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/profile_base.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      449 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/register.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1652 2023-05-02 18:00:25.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/sidebar.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      304 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_email_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      313 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_phone_number_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      339 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_user_data_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      813 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_user_password_form.html
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/verify_phone.html
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.703144 dj-accounts-3.0.8/dj_accounts/tests/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      163 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/apps.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      718 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/factories.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.703144 dj-accounts-3.0.8/dj_accounts/tests/migrations/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3188 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/migrations/0001_initial.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/migrations/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      456 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/mocks.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2927 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/models.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2843 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_backends.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    20397 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_forms.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8201 2023-05-02 19:50:05.000000 dj-accounts-3.0.8/dj_accounts/tests/test_serializers.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      550 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_tokens.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3918 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_urls.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1425 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_verify_phone.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    24255 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_view_api.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    29865 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/tests/test_views.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.703144 dj-accounts-3.0.8/dj_accounts/urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/__init__.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.703144 dj-accounts-3.0.8/dj_accounts/urls/api_urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/api_urls/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1317 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/api_urls/urls_auth_api.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      386 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/api_urls/urls_profile_api.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.707145 dj-accounts-3.0.8/dj_accounts/urls/site_urls/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/site_urls/__init__.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     2334 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/site_urls/urls_auth.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      352 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/urls/site_urls/urls_profile.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1120 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/utils.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      911 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/verify_phone.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     8724 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/views.py
--rw-rw-r--   0 codtail   (1000) codtail   (1000)    10759 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/dj_accounts/views_api.py
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.435145 dj-accounts-3.0.8/dj_accounts.egg-info/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1902 2023-05-02 19:57:20.000000 dj-accounts-3.0.8/dj_accounts.egg-info/PKG-INFO
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3716 2023-05-02 19:57:21.000000 dj-accounts-3.0.8/dj_accounts.egg-info/SOURCES.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        1 2023-05-02 19:57:20.000000 dj-accounts-3.0.8/dj_accounts.egg-info/dependency_links.txt
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       25 2023-05-02 19:57:20.000000 dj-accounts-3.0.8/dj_accounts.egg-info/top_level.txt
-drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 19:57:22.795144 dj-accounts-3.0.8/docs/
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/APIAuth.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/APIProfile.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     1371 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/PhoneVerificationService.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/Profile.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/docs/SessionAuth.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)     3630 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/docs/index.md
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      108 2023-05-02 16:33:59.000000 dj-accounts-3.0.8/pyproject.toml
--rw-rw-r--   0 codtail   (1000) codtail   (1000)      906 2023-05-02 19:57:22.835145 dj-accounts-3.0.8/setup.cfg
--rw-rw-r--   0 codtail   (1000) codtail   (1000)       38 2023-05-02 16:33:28.000000 dj-accounts-3.0.8/setup.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.479567 dj-accounts-3.0.9/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1145 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/LICENSE
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      139 2023-05-02 23:14:17.000000 dj-accounts-3.0.9/MANIFEST.in
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1917 2023-05-02 23:15:12.479567 dj-accounts-3.0.9/PKG-INFO
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      628 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/README.md
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.839567 dj-accounts-3.0.9/accounts_pkg/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/accounts_pkg/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       79 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/accounts_pkg/api_urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/accounts_pkg/asgi.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     4139 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/accounts_pkg/settings-multi-auth.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     4119 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/accounts_pkg/settings.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      378 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/accounts_pkg/urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      401 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/accounts_pkg/wsgi.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.915567 dj-accounts-3.0.9/dj_accounts/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:27.000000 dj-accounts-3.0.9/dj_accounts/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      153 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/apps.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      838 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/backends.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8485 2023-05-02 17:05:25.000000 dj-accounts-3.0.9/dj_accounts/forms.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.731567 dj-accounts-3.0.9/dj_accounts/locale/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.731567 dj-accounts-3.0.9/dj_accounts/locale/ar/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.915567 dj-accounts-3.0.9/dj_accounts/locale/ar/LC_MESSAGES/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8091 2023-05-02 19:54:37.000000 dj-accounts-3.0.9/dj_accounts/locale/ar/LC_MESSAGES/django.mo
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    12344 2023-05-02 19:54:27.000000 dj-accounts-3.0.9/dj_accounts/locale/ar/LC_MESSAGES/django.po
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     4695 2023-05-02 17:11:11.000000 dj-accounts-3.0.9/dj_accounts/serializers.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.731567 dj-accounts-3.0.9/dj_accounts/templates/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.139567 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      335 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/auth_base.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      573 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/confirm_email_template.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      202 2023-05-02 17:52:57.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/email_verification_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      948 2023-05-02 17:54:18.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/login.html
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.143567 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.207567 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1108 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      710 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      840 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/first_name.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      797 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/gender.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      809 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/last_name.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      634 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      655 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password1.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      689 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password2.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      668 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/phone.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      236 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/terms&conditions.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      735 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/username.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1052 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login-tabs.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      938 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login_with_email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      940 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login_with_phone.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/logo.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      383 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/social_login.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      954 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_confirm.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      659 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_done.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      615 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_email.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      555 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      132 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_subject.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      466 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/phone_verification_complete.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       34 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/profile.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      553 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/profile_base.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      449 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/register.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1652 2023-05-02 18:00:25.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/sidebar.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      304 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_email_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      313 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_phone_number_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      339 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_user_data_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      813 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_user_password_form.html
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/verify_phone.html
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.271567 dj-accounts-3.0.9/dj_accounts/tests/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      163 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/apps.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      718 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/factories.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.299567 dj-accounts-3.0.9/dj_accounts/tests/migrations/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3188 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/migrations/0001_initial.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/migrations/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      456 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/mocks.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2927 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/models.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2843 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_backends.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    20397 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_forms.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8201 2023-05-02 19:50:05.000000 dj-accounts-3.0.9/dj_accounts/tests/test_serializers.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      550 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_tokens.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3918 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_urls.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1425 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_verify_phone.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    24255 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_view_api.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    29865 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/tests/test_views.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.299567 dj-accounts-3.0.9/dj_accounts/urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/__init__.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.303567 dj-accounts-3.0.9/dj_accounts/urls/api_urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/api_urls/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1317 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/api_urls/urls_auth_api.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      386 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/api_urls/urls_profile_api.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.303567 dj-accounts-3.0.9/dj_accounts/urls/site_urls/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/site_urls/__init__.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     2334 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/site_urls/urls_auth.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      352 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/urls/site_urls/urls_profile.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1120 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/utils.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      911 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/verify_phone.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     8724 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/views.py
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)    10759 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/dj_accounts/views_api.py
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:11.915567 dj-accounts-3.0.9/dj_accounts.egg-info/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1917 2023-05-02 23:15:11.000000 dj-accounts-3.0.9/dj_accounts.egg-info/PKG-INFO
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3804 2023-05-02 23:15:11.000000 dj-accounts-3.0.9/dj_accounts.egg-info/SOURCES.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        1 2023-05-02 23:15:11.000000 dj-accounts-3.0.9/dj_accounts.egg-info/dependency_links.txt
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       25 2023-05-02 23:15:11.000000 dj-accounts-3.0.9/dj_accounts.egg-info/top_level.txt
+drwxrwxr-x   0 codtail   (1000) codtail   (1000)        0 2023-05-02 23:15:12.431567 dj-accounts-3.0.9/docs/
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/APIAuth.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/APIProfile.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     1371 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/PhoneVerificationService.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/Profile.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)        0 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/docs/SessionAuth.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)     3630 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/docs/index.md
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      108 2023-05-02 16:33:59.000000 dj-accounts-3.0.9/pyproject.toml
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)      921 2023-05-02 23:15:12.479567 dj-accounts-3.0.9/setup.cfg
+-rw-rw-r--   0 codtail   (1000) codtail   (1000)       38 2023-05-02 16:33:28.000000 dj-accounts-3.0.9/setup.py
```

### Comparing `dj-accounts-3.0.8/LICENSE` & `dj-accounts-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/PKG-INFO` & `dj-accounts-3.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-accounts
-Version: 3.0.8
+Version: 3.0.9
 Summary: this application is for handling all auth operations
 Home-page: https://github.com/fritill-team/django-accounts
 Author: fritill
 Author-email: dev@fritill.com
 License: MIT
 Description: ## Installation
         
@@ -49,15 +49,15 @@
             'DEFAULT_AUTHENTICATION_CLASSES': [
                 'rest_framework_simplejwt.authentication.JWTAuthentication',
             ],
         
         }
         
         ```
-Keywords: django translation custom
+Keywords: django account-management authentication
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `dj-accounts-3.0.8/README.md` & `dj-accounts-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/accounts_pkg/settings-multi-auth.py` & `dj-accounts-3.0.9/accounts_pkg/settings-multi-auth.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/accounts_pkg/settings.py` & `dj-accounts-3.0.9/accounts_pkg/settings.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/backends.py` & `dj-accounts-3.0.9/dj_accounts/backends.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/forms.py` & `dj-accounts-3.0.9/dj_accounts/forms.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/serializers.py` & `dj-accounts-3.0.9/dj_accounts/serializers.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/confirm_email_template.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/confirm_email_template.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/login.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/login.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/birthdate.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/email.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/first_name.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/first_name.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/gender.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/gender.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/last_name.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/last_name.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/one-time-code.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password1.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password1.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/password2.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/password2.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/phone.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/phone.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/fields/username.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/fields/username.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login-tabs.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login-tabs.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login_with_email.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login_with_email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/partials/login_with_phone.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/partials/login_with_phone.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_confirm.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_done.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_email.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/password_reset_form.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/profile_base.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/profile_base.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/sidebar.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/sidebar.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/templates/dj_accounts/update_user_password_form.html` & `dj-accounts-3.0.9/dj_accounts/templates/dj_accounts/update_user_password_form.html`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/factories.py` & `dj-accounts-3.0.9/dj_accounts/tests/factories.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/migrations/0001_initial.py` & `dj-accounts-3.0.9/dj_accounts/tests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/models.py` & `dj-accounts-3.0.9/dj_accounts/tests/models.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/test_backends.py` & `dj-accounts-3.0.9/dj_accounts/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/test_forms.py` & `dj-accounts-3.0.9/dj_accounts/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/test_serializers.py` & `dj-accounts-3.0.9/dj_accounts/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/test_tokens.py` & `dj-accounts-3.0.9/dj_accounts/tests/test_tokens.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/test_urls.py` & `dj-accounts-3.0.9/dj_accounts/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/test_verify_phone.py` & `dj-accounts-3.0.9/dj_accounts/tests/test_verify_phone.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/test_view_api.py` & `dj-accounts-3.0.9/dj_accounts/tests/test_view_api.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/tests/test_views.py` & `dj-accounts-3.0.9/dj_accounts/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/urls/api_urls/urls_auth_api.py` & `dj-accounts-3.0.9/dj_accounts/urls/api_urls/urls_auth_api.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/urls/site_urls/urls_auth.py` & `dj-accounts-3.0.9/dj_accounts/urls/site_urls/urls_auth.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/utils.py` & `dj-accounts-3.0.9/dj_accounts/utils.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/verify_phone.py` & `dj-accounts-3.0.9/dj_accounts/verify_phone.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/views.py` & `dj-accounts-3.0.9/dj_accounts/views.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts/views_api.py` & `dj-accounts-3.0.9/dj_accounts/views_api.py`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/dj_accounts.egg-info/PKG-INFO` & `dj-accounts-3.0.9/dj_accounts.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-accounts
-Version: 3.0.8
+Version: 3.0.9
 Summary: this application is for handling all auth operations
 Home-page: https://github.com/fritill-team/django-accounts
 Author: fritill
 Author-email: dev@fritill.com
 License: MIT
 Description: ## Installation
         
@@ -49,15 +49,15 @@
             'DEFAULT_AUTHENTICATION_CLASSES': [
                 'rest_framework_simplejwt.authentication.JWTAuthentication',
             ],
         
         }
         
         ```
-Keywords: django translation custom
+Keywords: django account-management authentication
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

### Comparing `dj-accounts-3.0.8/dj_accounts.egg-info/SOURCES.txt` & `dj-accounts-3.0.9/dj_accounts.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 dj_accounts/verify_phone.py
 dj_accounts/views.py
 dj_accounts/views_api.py
 dj_accounts.egg-info/PKG-INFO
 dj_accounts.egg-info/SOURCES.txt
 dj_accounts.egg-info/dependency_links.txt
 dj_accounts.egg-info/top_level.txt
+dj_accounts/locale/ar/LC_MESSAGES/django.mo
+dj_accounts/locale/ar/LC_MESSAGES/django.po
 dj_accounts/templates/dj_accounts/auth_base.html
 dj_accounts/templates/dj_accounts/confirm_email_template.html
 dj_accounts/templates/dj_accounts/email_verification_complete.html
 dj_accounts/templates/dj_accounts/login.html
 dj_accounts/templates/dj_accounts/password_reset_complete.html
 dj_accounts/templates/dj_accounts/password_reset_confirm.html
 dj_accounts/templates/dj_accounts/password_reset_done.html
```

### Comparing `dj-accounts-3.0.8/docs/PhoneVerificationService.md` & `dj-accounts-3.0.9/docs/PhoneVerificationService.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/docs/index.md` & `dj-accounts-3.0.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `dj-accounts-3.0.8/setup.cfg` & `dj-accounts-3.0.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [metadata]
 name = dj-accounts
-version = 3.0.8
+version = 3.0.9
 author = fritill
 author_email = dev@fritill.com
 description = this application is for handling all auth operations
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/fritill-team/django-accounts
 license = MIT
 platform = any
-keywords = django translation custom
+keywords = django account-management authentication
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Intended Audience :: Developers
 	License :: OSI Approved :: BSD License
 	Operating System :: OS Independent
 	Programming Language :: Python
```

