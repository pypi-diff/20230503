# Comparing `tmp/aws_hcs_cli-6.0.0.tar.gz` & `tmp/aws_hcs_cli-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_hcs_cli-6.0.0.tar", max compression
+gzip compressed data, was "aws_hcs_cli-6.3.0.tar", max compression
```

## Comparing `aws_hcs_cli-6.0.0.tar` & `aws_hcs_cli-6.3.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      165 2023-03-14 12:06:22.329321 aws_hcs_cli-6.0.0/aws_hcs_cli/__init__.py
--rw-r--r--   0        0        0     2842 2023-03-14 09:35:38.303484 aws_hcs_cli-6.0.0/aws_hcs_cli/_azure_cloud_mfa_authenticator.py
--rw-r--r--   0        0        0     1910 2023-03-14 09:35:38.304481 aws_hcs_cli-6.0.0/aws_hcs_cli/_azure_mfa_authenticator.py
--rw-r--r--   0        0        0    21090 2023-03-14 09:35:38.305478 aws_hcs_cli-6.0.0/aws_hcs_cli/_duo_authenticator.py
--rw-r--r--   0        0        0    21898 2023-03-14 09:35:38.305478 aws_hcs_cli-6.0.0/aws_hcs_cli/_duo_universal_prompt_authenticator.py
--rw-r--r--   0        0        0     2198 2023-03-14 09:35:38.306482 aws_hcs_cli-6.0.0/aws_hcs_cli/_rsa_authenticator.py
--rw-r--r--   0        0        0     2535 2023-03-14 09:35:38.307473 aws_hcs_cli-6.0.0/aws_hcs_cli/_symantec_vip_access.py
--rw-r--r--   0        0        0    19006 2021-09-15 15:32:43.439610 aws_hcs_cli-6.0.0/aws_hcs_cli/_version.py
--rw-r--r--   0        0        0     1563 2023-03-14 09:35:38.307473 aws_hcs_cli-6.0.0/aws_hcs_cli/account_aliases_fetcher.py
--rw-r--r--   0        0        0     7559 2023-03-14 10:17:51.601383 aws_hcs_cli-6.0.0/aws_hcs_cli/authenticator.py
--rw-r--r--   0        0        0     1382 2023-03-14 09:35:38.308470 aws_hcs_cli-6.0.0/aws_hcs_cli/commands.py
--rw-r--r--   0        0        0      221 2023-03-14 09:35:38.309468 aws_hcs_cli-6.0.0/aws_hcs_cli/consts.py
--rw-r--r--   0        0        0      888 2023-03-14 09:35:38.309468 aws_hcs_cli-6.0.0/aws_hcs_cli/helpers.py
--rw-r--r--   0        0        0     4525 2023-03-14 10:19:43.533533 aws_hcs_cli-6.0.0/aws_hcs_cli/html_roles_fetcher.py
--rw-r--r--   0        0        0      810 2023-03-14 09:35:38.310465 aws_hcs_cli-6.0.0/aws_hcs_cli/list_profiles.py
--rw-r--r--   0        0        0    26695 2023-03-14 15:48:56.445464 aws_hcs_cli-6.0.0/aws_hcs_cli/login.py
--rw-r--r--   0        0        0    11122 2023-03-14 10:28:17.650315 aws_hcs_cli-6.0.0/aws_hcs_cli/prepare.py
--rw-r--r--   0        0        0     1288 2023-03-14 09:35:38.312460 aws_hcs_cli-6.0.0/aws_hcs_cli/reset.py
--rw-r--r--   0        0        0     2957 2023-03-14 18:06:27.526261 aws_hcs_cli-6.0.0/aws_hcs_cli/role_chooser.py
--rw-r--r--   0        0        0     3822 2023-03-14 10:15:31.038107 aws_hcs_cli-6.0.0/aws_hcs_cli/roles_assertion_extractor.py
--rw-r--r--   0        0        0     1087 2021-08-20 19:23:18.812869 aws_hcs_cli-6.0.0/LICENSE
--rw-r--r--   0        0        0     1559 2023-03-14 18:06:59.577401 aws_hcs_cli-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     1103 2021-09-07 19:09:25.073383 aws_hcs_cli-6.0.0/README.md
--rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 aws_hcs_cli-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0      165 2023-03-14 12:06:22.329321 aws_hcs_cli-6.3.0/aws_hcs_cli/__init__.py
+-rw-r--r--   0        0        0     2842 2023-03-14 09:35:38.303484 aws_hcs_cli-6.3.0/aws_hcs_cli/_azure_cloud_mfa_authenticator.py
+-rw-r--r--   0        0        0     1910 2023-03-14 09:35:38.304481 aws_hcs_cli-6.3.0/aws_hcs_cli/_azure_mfa_authenticator.py
+-rw-r--r--   0        0        0    21090 2023-03-14 09:35:38.305478 aws_hcs_cli-6.3.0/aws_hcs_cli/_duo_authenticator.py
+-rw-r--r--   0        0        0    22040 2023-05-03 09:47:12.359371 aws_hcs_cli-6.3.0/aws_hcs_cli/_duo_universal_prompt_authenticator.py
+-rw-r--r--   0        0        0     2198 2023-03-14 09:35:38.306482 aws_hcs_cli-6.3.0/aws_hcs_cli/_rsa_authenticator.py
+-rw-r--r--   0        0        0     2535 2023-03-14 09:35:38.307473 aws_hcs_cli-6.3.0/aws_hcs_cli/_symantec_vip_access.py
+-rw-r--r--   0        0        0    19006 2021-09-15 15:32:43.439610 aws_hcs_cli-6.3.0/aws_hcs_cli/_version.py
+-rw-r--r--   0        0        0     1563 2023-03-14 09:35:38.307473 aws_hcs_cli-6.3.0/aws_hcs_cli/account_aliases_fetcher.py
+-rw-r--r--   0        0        0     7559 2023-03-14 10:17:51.601383 aws_hcs_cli-6.3.0/aws_hcs_cli/authenticator.py
+-rw-r--r--   0        0        0     1382 2023-03-14 09:35:38.308470 aws_hcs_cli-6.3.0/aws_hcs_cli/commands.py
+-rw-r--r--   0        0        0      221 2023-03-14 09:35:38.309468 aws_hcs_cli-6.3.0/aws_hcs_cli/consts.py
+-rw-r--r--   0        0        0      888 2023-03-14 09:35:38.309468 aws_hcs_cli-6.3.0/aws_hcs_cli/helpers.py
+-rw-r--r--   0        0        0     4525 2023-03-14 10:19:43.533533 aws_hcs_cli-6.3.0/aws_hcs_cli/html_roles_fetcher.py
+-rw-r--r--   0        0        0      810 2023-03-14 09:35:38.310465 aws_hcs_cli-6.3.0/aws_hcs_cli/list_profiles.py
+-rw-r--r--   0        0        0    26695 2023-03-14 15:48:56.445464 aws_hcs_cli-6.3.0/aws_hcs_cli/login.py
+-rw-r--r--   0        0        0    11122 2023-03-14 10:28:17.650315 aws_hcs_cli-6.3.0/aws_hcs_cli/prepare.py
+-rw-r--r--   0        0        0     1288 2023-03-14 09:35:38.312460 aws_hcs_cli-6.3.0/aws_hcs_cli/reset.py
+-rw-r--r--   0        0        0     2957 2023-03-14 18:06:27.526261 aws_hcs_cli-6.3.0/aws_hcs_cli/role_chooser.py
+-rw-r--r--   0        0        0     3822 2023-03-14 10:15:31.038107 aws_hcs_cli-6.3.0/aws_hcs_cli/roles_assertion_extractor.py
+-rw-r--r--   0        0        0     1087 2021-08-20 19:23:18.812869 aws_hcs_cli-6.3.0/LICENSE
+-rw-r--r--   0        0        0     1559 2023-05-03 09:46:24.138666 aws_hcs_cli-6.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1103 2021-09-07 19:09:25.073383 aws_hcs_cli-6.3.0/README.md
+-rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 aws_hcs_cli-6.3.0/PKG-INFO
```

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/_azure_cloud_mfa_authenticator.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/_azure_cloud_mfa_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/_azure_mfa_authenticator.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/_azure_mfa_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/_duo_authenticator.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/_duo_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/_duo_universal_prompt_authenticator.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/_duo_universal_prompt_authenticator.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,19 +34,21 @@
     from urlparse import urlparse, parse_qs
     import Queue as queue
 
 from . import roles_assertion_extractor
 
 _headers = {
     "Accept-Language": "en",
-    "User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko",
+    "User-Agent": "Mozilla/5.0 (X11; Ubuntu; Linux i686; rv:24.0) Gecko/20100101 Firefox/24.0",
     "Content-Type": "application/x-www-form-urlencoded; charset=UTF-8",
     "Accept": "text/plain, */*; q=0.01",
 }
 
+    #"User-Agent": "Mozilla/5.0 (Windows NT 6.1; WOW64; Trident/7.0; rv:11.0) like Gecko",
+
 
 def extract(html_response, ssl_verification_enabled, session, duo_factor, duo_device):
     """
     this strategy is based on description from: https://guide.duo.com/universal-prompt
     :param response: raw http response
     :param html_response: html result of parsing http response
     :return:
@@ -541,14 +543,15 @@
         err=True,
     )
 
     data = {
         "sid": sid,
         "factor": preferred_factor,
         "device": preferred_device,
+        "post_auth_action": "OIDC_EXIT",
     }
 
     # Prompt for a passcode?
     if preferred_factor == DUO_UNIVERSAL_PROMPT_FACTOR_PASSCODE:
         passcode = None
         while not passcode or not re.match(r'^[0-9]{6,}$', passcode):
             passcode = click.prompt('Enter passcode (6+ digit number)', hide_input=True)
```

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/_rsa_authenticator.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/_rsa_authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/_symantec_vip_access.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/_symantec_vip_access.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/_version.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/_version.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/account_aliases_fetcher.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/account_aliases_fetcher.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/authenticator.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/authenticator.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/commands.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/commands.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/helpers.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/helpers.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/html_roles_fetcher.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/html_roles_fetcher.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/list_profiles.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/list_profiles.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/login.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/login.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/prepare.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/prepare.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/reset.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/reset.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/role_chooser.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/role_chooser.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/aws_hcs_cli/roles_assertion_extractor.py` & `aws_hcs_cli-6.3.0/aws_hcs_cli/roles_assertion_extractor.py`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/LICENSE` & `aws_hcs_cli-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/pyproject.toml` & `aws_hcs_cli-6.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool]
 [tool.poetry]
 name = "aws-hcs-cli"
-version = "6.0.0"
+version = "6.3.0"
 description = "AWS CLI authenticator via ADFS - small command-line tool to authenticate via ADFS and assume chosen role"
 keywords = ["aws", "adfs", "console", "tool"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Developers",
```

### Comparing `aws_hcs_cli-6.0.0/README.md` & `aws_hcs_cli-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aws_hcs_cli-6.0.0/PKG-INFO` & `aws_hcs_cli-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-hcs-cli
-Version: 6.0.0
+Version: 6.3.0
 Summary: AWS CLI authenticator via ADFS - small command-line tool to authenticate via ADFS and assume chosen role
 Keywords: aws,adfs,console,tool
 Author: Venth
 Author-email: artur.krysiak.warszawa@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

