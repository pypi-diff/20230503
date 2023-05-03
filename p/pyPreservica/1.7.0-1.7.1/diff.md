# Comparing `tmp/pyPreservica-1.7.0.tar.gz` & `tmp/pyPreservica-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyPreservica-1.7.0.tar", last modified: Mon Apr 17 14:19:21 2023, max compression
+gzip compressed data, was "pyPreservica-1.7.1.tar", last modified: Wed May  3 11:04:45 2023, max compression
```

## Comparing `pyPreservica-1.7.0.tar` & `pyPreservica-1.7.1.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:19:21.805726 pyPreservica-1.7.0/
--rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.7.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2581 2023-04-17 14:19:21.790105 pyPreservica-1.7.0/PKG-INFO
--rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.7.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 14:19:21.751688 pyPreservica-1.7.0/pyPreservica/
--rw-rw-rw-   0        0        0      970 2023-02-02 16:53:09.000000 pyPreservica-1.7.0/pyPreservica/__init__.py
--rw-rw-rw-   0        0        0    37713 2023-03-01 16:08:31.000000 pyPreservica-1.7.0/pyPreservica/adminAPI.py
--rw-rw-rw-   0        0        0    31931 2023-03-01 16:00:56.000000 pyPreservica-1.7.0/pyPreservica/common.py
--rw-rw-rw-   0        0        0    16189 2023-03-01 16:04:47.000000 pyPreservica-1.7.0/pyPreservica/contentAPI.py
--rw-rw-rw-   0        0        0   105659 2023-03-01 16:04:03.000000 pyPreservica-1.7.0/pyPreservica/entityAPI.py
--rw-rw-rw-   0        0        0     6260 2023-03-01 16:11:00.000000 pyPreservica-1.7.0/pyPreservica/monitorAPI.py
--rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.7.0/pyPreservica/opex.py
--rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.7.0/pyPreservica/parAPI.py
--rw-rw-rw-   0        0        0    23541 2023-04-17 14:03:38.000000 pyPreservica-1.7.0/pyPreservica/retentionAPI.py
--rw-rw-rw-   0        0        0    92270 2023-03-21 17:44:59.000000 pyPreservica-1.7.0/pyPreservica/uploadAPI.py
--rw-rw-rw-   0        0        0    17812 2023-03-01 16:08:31.000000 pyPreservica-1.7.0/pyPreservica/workflowAPI.py
-drwxrwxrwx   0        0        0        0 2023-04-17 14:19:21.790105 pyPreservica-1.7.0/pyPreservica.egg-info/
--rw-rw-rw-   0        0        0     2581 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-17 14:19:20.000000 pyPreservica-1.7.0/pyPreservica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 14:19:21.805726 pyPreservica-1.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1645 2023-02-02 16:53:09.000000 pyPreservica-1.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:04:45.537330 pyPreservica-1.7.1/
+-rw-rw-rw-   0        0        0    11558 2020-08-17 10:38:19.000000 pyPreservica-1.7.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2581 2023-05-03 11:04:45.536330 pyPreservica-1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1602 2022-03-16 17:04:00.000000 pyPreservica-1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:04:45.491828 pyPreservica-1.7.1/pyPreservica/
+-rw-rw-rw-   0        0        0     1021 2023-05-03 11:03:51.000000 pyPreservica-1.7.1/pyPreservica/__init__.py
+-rw-rw-rw-   0        0        0    37685 2023-05-03 10:58:47.000000 pyPreservica-1.7.1/pyPreservica/adminAPI.py
+-rw-rw-rw-   0        0        0    32269 2023-05-03 10:51:09.000000 pyPreservica-1.7.1/pyPreservica/common.py
+-rw-rw-rw-   0        0        0    16189 2023-03-01 16:04:47.000000 pyPreservica-1.7.1/pyPreservica/contentAPI.py
+-rw-rw-rw-   0        0        0   105659 2023-03-01 16:04:03.000000 pyPreservica-1.7.1/pyPreservica/entityAPI.py
+-rw-rw-rw-   0        0        0     6260 2023-03-01 16:11:00.000000 pyPreservica-1.7.1/pyPreservica/monitorAPI.py
+-rw-rw-rw-   0        0        0     4875 2022-04-21 08:22:10.000000 pyPreservica-1.7.1/pyPreservica/opex.py
+-rw-rw-rw-   0        0        0    10522 2021-11-17 14:16:50.000000 pyPreservica-1.7.1/pyPreservica/parAPI.py
+-rw-rw-rw-   0        0        0    23541 2023-04-17 14:03:38.000000 pyPreservica-1.7.1/pyPreservica/retentionAPI.py
+-rw-rw-rw-   0        0        0    92270 2023-03-21 17:44:59.000000 pyPreservica-1.7.1/pyPreservica/uploadAPI.py
+-rw-rw-rw-   0        0        0     2179 2023-05-02 15:51:54.000000 pyPreservica-1.7.1/pyPreservica/webHooksAPI.py
+-rw-rw-rw-   0        0        0    17812 2023-03-01 16:08:31.000000 pyPreservica-1.7.1/pyPreservica/workflowAPI.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:04:45.530403 pyPreservica-1.7.1/pyPreservica.egg-info/
+-rw-rw-rw-   0        0        0     2581 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      517 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 11:04:43.000000 pyPreservica-1.7.1/pyPreservica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:04:45.540275 pyPreservica-1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1645 2023-05-03 11:03:51.000000 pyPreservica-1.7.1/setup.py
```

### Comparing `pyPreservica-1.7.0/LICENSE.txt` & `pyPreservica-1.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/PKG-INFO` & `pyPreservica-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.7.0/README.md` & `pyPreservica-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica/__init__.py` & `pyPreservica-1.7.1/pyPreservica/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 from .uploadAPI import UploadAPI, simple_asset_package, complex_asset_package, cvs_to_xsd, cvs_to_xml, \
                     cvs_to_cmis_xslt, csv_to_search_xml, generic_asset_package, upload_config, multi_asset_package
 from .workflowAPI import WorkflowAPI, WorkflowContext, WorkflowInstance
 from .retentionAPI import RetentionAPI, RetentionAssignment, RetentionPolicy
 from .parAPI import PreservationActionRegistry
 from .adminAPI import AdminAPI
 from .monitorAPI import MonitorAPI, MonitorCategory, MonitorStatus, MessageStatus
+from .webHooksAPI import WebHooksAPI, TriggerType
 
 
 __author__ = "James Carr (drjamescarr@gmail.com)"
 
 # Version of the Preservica API package
-__version__ = "1.7.0"
+__version__ = "1.7.1"
 
 __license__ = "Apache License Version 2.0"
```

### Comparing `pyPreservica-1.7.0/pyPreservica/adminAPI.py` & `pyPreservica-1.7.1/pyPreservica/adminAPI.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,34 +15,30 @@
 from pyPreservica.common import *
 
 logger = logging.getLogger(__name__)
 
 
 class AdminAPI(AuthenticatedAPI):
 
-    def __check_if_user_has_manager_role(self):
-        if ('ROLE_SDB_MANAGER_USER' not in self.roles) or ('ROLE_SDB_ADMIN_USER' not in self.roles):
-            logger.error(f"The AdminAPI requires the user to have ROLE_SDB_MANAGER_USER")
-            raise RuntimeError(f"The AdminAPI requires the user to have ROLE_SDB_MANAGER_USER")
-
     def delete_system_role(self, role_name):
         """
         Delete a system role
 
         :param role_name: The role to delete
         :type role_name: str
 
         """
         if (self.major_version < 7) and (self.minor_version < 5):
             raise RuntimeError(
                 "delete_system_role API call is only available with a Preservica v6.5.0 system or higher")
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.delete(f'{self.protocol}://{self.server}/api/admin/security/roles/{role_name}', headers=headers)
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/admin/security/roles/{role_name}',
+                                      headers=headers)
         if request.status_code == requests.codes.no_content:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.delete_system_role(role_name)
         else:
             logger.error(request.content.decode('utf-8'))
@@ -56,17 +52,18 @@
         :type tag_name: str
 
         """
         if (self.major_version < 7) and (self.minor_version < 4):
             raise RuntimeError(
                 "delete_security_tag API call is only available with a Preservica v6.4.0 system or higher")
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.delete(f'{self.protocol}://{self.server}/api/admin/security/tags/{tag_name}', headers=headers)
+        request = self.session.delete(f'{self.protocol}://{self.server}/api/admin/security/tags/{tag_name}',
+                                      headers=headers)
         if request.status_code == requests.codes.no_content:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.delete_security_tag(tag_name)
         else:
             logger.error(request.content.decode('utf-8'))
@@ -82,15 +79,15 @@
         :return: The new role
         :rtype: str
 
         """
         if (self.major_version < 7) and (self.minor_version < 5):
             raise RuntimeError("add_system_role API call is only available with a Preservica v6.5.0 system or higher")
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         xml_tag = xml.etree.ElementTree.Element('Role', {"xmlns": self.admin_ns})
         xml_tag.text = str(role_name).strip()
         xml_request = xml.etree.ElementTree.tostring(xml_tag, encoding='utf-8')
         request = self.session.post(f'{self.protocol}://{self.server}/api/admin/security/roles', data=xml_request,
                                     headers=headers)
@@ -117,22 +114,23 @@
         :rtype: str
 
         """
 
         if (self.major_version < 7) and (self.minor_version < 4):
             raise RuntimeError("add_security_tag API call is only available with a Preservica v6.4.0 system or higher")
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         xml_tag = xml.etree.ElementTree.Element('Tag', {"xmlns": self.admin_ns})
         xml_tag.text = str(tag_name).strip()
         xml_request = xml.etree.ElementTree.tostring(xml_tag, encoding='utf-8')
 
-        request = self.session.post(f'{self.protocol}://{self.server}/api/admin/security/tags', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/admin/security/tags', data=xml_request,
+                                    headers=headers)
         if request.status_code == requests.codes.created:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             return entity_response.text
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
@@ -145,15 +143,15 @@
         """
         List all the user access roles in the system
 
         :return: list of roles
         :rtype: list
 
         """
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
 
         if (self.major_version < 7) and (self.minor_version < 5):
             raise RuntimeError(
                 "system_roles API call is only available with a Preservica v6.5.0 system or higher")
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         request = self.session.get(f'{self.protocol}://{self.server}/api/admin/security/roles', headers=headers)
@@ -177,15 +175,15 @@
         """
         List all the security tags in the system
 
         :return: list of security tags
         :rtype: list
 
         """
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         request = self.session.get(f'{self.protocol}://{self.server}/api/admin/security/tags', headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             tags = entity_response.findall(f'.//{{{self.admin_ns}}}Tag')
@@ -204,15 +202,15 @@
         """
         Delete a user
 
         :param username: email address of the preservica user
         :type username: str
 
         """
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         self.disable_user(username)
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         request = self.session.delete(f'{self.protocol}://{self.server}/api/admin/users/{username}', headers=headers)
         if request.status_code == requests.codes.no_content:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
@@ -235,29 +233,30 @@
 
         :param roles: List of roles assigned to the user
         :type roles: list
 
         :return: dictionary of user attributes
         :rtype: dict
         """
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         xml_object = xml.etree.ElementTree.Element('User ', {"xmlns": self.admin_ns})
         xml.etree.ElementTree.SubElement(xml_object, "FullName").text = full_name
         xml.etree.ElementTree.SubElement(xml_object, "Email").text = username
         if externally_authenticated:
             xml.etree.ElementTree.SubElement(xml_object, "externallyAuthenticated").text = "true"
             xml.etree.ElementTree.SubElement(xml_object, "userName").text = username
         xml_roles = xml.etree.ElementTree.SubElement(xml_object, "Roles")
         for role in roles:
             xml.etree.ElementTree.SubElement(xml_roles, "Role").text = role
         xml_request = xml.etree.ElementTree.tostring(xml_object, encoding='utf-8')
         logger.debug(xml_request)
-        request = self.session.post(f'{self.protocol}://{self.server}/api/admin/users', data=xml_request, headers=headers)
+        request = self.session.post(f'{self.protocol}://{self.server}/api/admin/users', data=xml_request,
+                                    headers=headers)
         if request.status_code == requests.codes.created:
             return self.user_details(username)
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_user(username, full_name, roles)
         else:
             logger.error(request.content.decode('utf-8'))
@@ -272,26 +271,27 @@
 
          :param new_display_name: Users real name
          :type new_display_name: str
 
          :return: dictionary of user attributes
          :rtype: dict
          """
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         request = self.session.get(f"{self.protocol}://{self.server}/api/admin/users/{username}", headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             fullname = entity_response.find(f'.//{{{self.admin_ns}}}FullName')
             fullname.text = new_display_name
             xml_request = xml.etree.ElementTree.tostring(entity_response, encoding='utf-8')
             logger.debug(xml_request)
-            update_request = self.session.put(f'{self.protocol}://{self.server}/api/admin/users/{username}', data=xml_request,
+            update_request = self.session.put(f'{self.protocol}://{self.server}/api/admin/users/{username}',
+                                              data=xml_request,
                                               headers=headers)
             if update_request.status_code == requests.codes.ok:
                 return self.user_details(username)
             elif update_request.status_code == requests.codes.unauthorized:
                 self.token = self.__token__()
                 return self.change_user_display_name(username, new_display_name)
             else:
@@ -311,15 +311,15 @@
         :param username: email address of the preservica user
         :type username: str
 
         :return: dictionary of user attributes
         :rtype: dict
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         request = self.session.get(f"{self.protocol}://{self.server}/api/admin/users/{username}", headers=headers)
         return_dict = {}
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
@@ -343,38 +343,39 @@
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.user_details(username)
         else:
             logger.error(request.content.decode('utf-8'))
             raise RuntimeError(request.status_code, "user_details failed")
 
-    def __account_status_(self, username: str, status: str, name: str):
+    def _account_status_(self, username: str, status: str, name: str):
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'text/plain;charset=UTF-8'}
         data = {"userEnabledStatus": status}
-        request = self.session.put(f"{self.protocol}://{self.server}/api/admin/users/{username}/enabled", headers=headers,
+        request = self.session.put(f"{self.protocol}://{self.server}/api/admin/users/{username}/enabled",
+                                   headers=headers,
                                    data=data)
         if request.status_code == requests.codes.ok:
             return request.content.decode("utf-8")
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
-            return self.__account_status_(username, status, name)
+            return self._account_status_(username, status, name)
         else:
             logger.error(request.content.decode('utf-8'))
             raise RuntimeError(request.status_code, f"{name} failed")
 
     def disable_user(self, username):
         """
          Disable a Preservica User to prevent them logging in
 
         :param username: email address of the preservica user
         :type username: str
 
         """
-        self.__check_if_user_has_manager_role()
-        return self.__account_status_(username, "false", "disable_user")
+        self._check_if_user_has_manager_role()
+        return self._account_status_(username, "false", "disable_user")
 
     # def enable_user(self, username):
     #     """
     #      Enable a Preservica User
     #
     #     :param username: email address of the preservica user
     #     :type username: str
@@ -385,15 +386,15 @@
 
     def user_report(self, report_name="users.csv"):
         """
         Create a report on all tenancy users
         :return:
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
 
         fieldnames = ['UserName', 'FullName', 'Email', 'Tenant', 'Enabled', 'Roles']
 
         with open(report_name, newline='', mode="wt", encoding="utf-8") as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=fieldnames)
             writer.writeheader()
             for username in self.all_users():
@@ -404,15 +405,15 @@
         """
         Return a list of all users in the system
 
         :return list of usernames:
         :rtype: list
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         request = self.session.get(f"{self.protocol}://{self.server}/api/admin/users", headers=headers)
         if request.status_code == requests.codes.ok:
             xml_response = str(request.content.decode('utf-8'))
             logger.debug(xml_response)
             entity_response = xml.etree.ElementTree.fromstring(xml_response)
             users = entity_response.findall(f'.//{{{self.admin_ns}}}User')
@@ -443,26 +444,27 @@
         :param xml_data: The xml schema as a UTF-8 string or a file like object
         :type xml_data: Any
 
         :return: None
         :rtype: None
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
 
         params = {"name": name, "description": description, "originalName": originalName}
 
         if isinstance(xml_data, str):
             xml.etree.ElementTree.fromstring(xml_data)
             xml_data = xml_data.encode("utf-8")
         elif hasattr(xml_data, "read"):
             pass
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/schemas", headers=headers, params=params,
+        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/schemas", headers=headers,
+                                    params=params,
                                     data=xml_data)
         if request.status_code == requests.codes.created:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_xml_schema(name, description, originalName, xml_data)
         else:
@@ -492,26 +494,27 @@
         :type document_type: str
 
         :return: None
         :rtype: None
 
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
 
         params = {"name": name, "type": document_type}
 
         if isinstance(xml_data, str):
             xml.etree.ElementTree.fromstring(xml_data)
             xml_data = xml_data.encode("utf-8")
         elif hasattr(xml_data, "read"):
             pass
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/documents", headers=headers, params=params,
+        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/documents", headers=headers,
+                                    params=params,
                                     data=xml_data)
         if request.status_code == requests.codes.created:
             return
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_xml_document(name, xml_data, document_type)
         else:
@@ -526,22 +529,23 @@
         :type uri: str
 
         :return: None
         :rtype: None
 
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         for document in self.xml_documents():
             if document['SchemaUri'] == uri.strip():
-                request = self.session.delete(f"{self.protocol}://{self.server}/api/admin/documents/{document['ApiId']}",
-                                              headers=headers)
+                request = self.session.delete(
+                    f"{self.protocol}://{self.server}/api/admin/documents/{document['ApiId']}",
+                    headers=headers)
                 if request.status_code == requests.codes.no_content:
                     return
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.delete_xml_document(uri)
                 else:
                     logger.error(request.content.decode('utf-8'))
@@ -555,15 +559,15 @@
         :type uri: str
 
         :return: None
         :rtype: None
 
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         for schema in self.xml_schemas():
             if schema['SchemaUri'] == uri.strip():
                 request = self.session.delete(f"{self.protocol}://{self.server}/api/admin/schemas/{schema['ApiId']}",
                                               headers=headers)
@@ -587,16 +591,17 @@
         :rtype: str
 
          """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         for schema in self.xml_schemas():
             if schema['SchemaUri'] == uri.strip():
-                request = self.session.get(f"{self.protocol}://{self.server}/api/admin/schemas/{schema['ApiId']}/content",
-                                           headers=headers)
+                request = self.session.get(
+                    f"{self.protocol}://{self.server}/api/admin/schemas/{schema['ApiId']}/content",
+                    headers=headers)
                 if request.status_code == requests.codes.ok:
                     xml_response = str(request.content.decode('utf-8'))
                     return xml_response
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.xml_schema(uri)
                 else:
@@ -613,16 +618,17 @@
         :return: The XML document as a string
         :rtype: str
 
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         for document in self.xml_documents():
             if document['SchemaUri'] == uri.strip():
-                request = self.session.get(f"{self.protocol}://{self.server}/api/admin/documents/{document['ApiId']}/content",
-                                           headers=headers)
+                request = self.session.get(
+                    f"{self.protocol}://{self.server}/api/admin/documents/{document['ApiId']}/content",
+                    headers=headers)
                 if request.status_code == requests.codes.ok:
                     xml_response = str(request.content.decode('utf-8'))
                     return xml_response
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.xml_document(uri)
                 else:
@@ -758,16 +764,17 @@
         :return: The XML transform as a string
         :rtype: str
 
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         for transform in self.xml_transforms():
             if (transform['FromSchemaUri'] == input_uri.strip()) and (transform['ToSchemaUri'] == output_uri.strip()):
-                request = self.session.get(f"{self.protocol}://{self.server}/api/admin/transforms/{transform['ApiId']}/content",
-                                           headers=headers)
+                request = self.session.get(
+                    f"{self.protocol}://{self.server}/api/admin/transforms/{transform['ApiId']}/content",
+                    headers=headers)
                 if request.status_code == requests.codes.ok:
                     return str(request.content.decode('utf-8'))
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.xml_transform(input_uri, output_uri)
                 else:
                     logger.error(request.content.decode('utf-8'))
@@ -784,22 +791,23 @@
         :type output_uri: str
 
         :return: None
         :rtype: None
 
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
 
         for transform in self.xml_transforms():
             if (transform['FromSchemaUri'] == input_uri.strip()) and (transform['ToSchemaUri'] == output_uri.strip()):
-                request = self.session.delete(f"{self.protocol}://{self.server}/api/admin/transforms/{transform['ApiId']}",
-                                              headers=headers)
+                request = self.session.delete(
+                    f"{self.protocol}://{self.server}/api/admin/transforms/{transform['ApiId']}",
+                    headers=headers)
                 if request.status_code == requests.codes.no_content:
                     return
                 elif request.status_code == requests.codes.unauthorized:
                     self.token = self.__token__()
                     return self.delete_xml_transform(input_uri, output_uri)
                 else:
                     logger.error(request.content.decode('utf-8'))
@@ -829,27 +837,28 @@
         :type xml_data: Any
 
         :return: None
         :rtype: None
 
         """
 
-        self.__check_if_user_has_manager_role()
+        self._check_if_user_has_manager_role()
 
         params = {"name": name, "from": input_uri, "to": output_uri, "purpose": purpose.lower(),
                   "originalName": originalName}
 
         if isinstance(xml_data, str):
             xml.etree.ElementTree.fromstring(xml_data)
             xml_data = xml_data.encode("utf-8")
         elif hasattr(xml_data, "read"):
             pass
 
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
-        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/transforms", headers=headers, params=params,
+        request = self.session.post(f"{self.protocol}://{self.server}/api/admin/transforms", headers=headers,
+                                    params=params,
                                     data=xml_data)
         if request.status_code == requests.codes.created:
             return
 
         if request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
             return self.add_xml_transform(name, input_uri, output_uri, purpose, originalName, xml_data)
```

### Comparing `pyPreservica-1.7.0/pyPreservica/common.py` & `pyPreservica-1.7.1/pyPreservica/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -605,27 +605,32 @@
 
 
 class AuthenticatedAPI:
     """
     Base class for authenticated calls which need access token
     """
 
-    def __find_user_roles_(self) -> list:
+    def _check_if_user_has_manager_role(self):
+        if ('ROLE_SDB_MANAGER_USER' not in self.roles) and ('ROLE_SDB_ADMIN_USER' not in self.roles):
+            logger.error(f"The AdminAPI requires the user to have ROLE_SDB_MANAGER_USER")
+            raise RuntimeError(f"The AdminAPI requires the user to have ROLE_SDB_MANAGER_USER")
+
+    def _find_user_roles_(self) -> list:
         """
         Get a list of roles for the user
         :return list of roles:
         """
         headers = {HEADER_TOKEN: self.token, 'Content-Type': 'application/xml;charset=UTF-8'}
         request = self.session.get(f"{self.protocol}://{self.server}/api/user/details", headers=headers)
         if request.status_code == requests.codes.ok:
             roles = json.loads(str(request.content.decode('utf-8')))['roles']
             return roles
         elif request.status_code == requests.codes.unauthorized:
             self.token = self.__token__()
-            return self.__find_user_roles_()
+            return self._find_user_roles_()
 
     def security_tags_base(self, with_permissions: bool = False) -> dict:
         """
              Return  security tags available for the  current user
 
              :return: dict of security tags
              :rtype:  dict
@@ -846,11 +851,11 @@
             raise RuntimeError(msg)
         else:
             self.server = server
 
         self.token = self.__token__()
         self.version = self.__version_number__()
         self.__version_namespace__()
-        self.roles = self.__find_user_roles_()
+        self.roles = self._find_user_roles_()
 
         logger.debug(self.xip_ns)
         logger.debug(self.entity_ns)
```

### Comparing `pyPreservica-1.7.0/pyPreservica/contentAPI.py` & `pyPreservica-1.7.1/pyPreservica/contentAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica/entityAPI.py` & `pyPreservica-1.7.1/pyPreservica/entityAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica/monitorAPI.py` & `pyPreservica-1.7.1/pyPreservica/monitorAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica/opex.py` & `pyPreservica-1.7.1/pyPreservica/opex.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica/parAPI.py` & `pyPreservica-1.7.1/pyPreservica/parAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica/retentionAPI.py` & `pyPreservica-1.7.1/pyPreservica/retentionAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica/uploadAPI.py` & `pyPreservica-1.7.1/pyPreservica/uploadAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica/workflowAPI.py` & `pyPreservica-1.7.1/pyPreservica/workflowAPI.py`

 * *Files identical despite different names*

### Comparing `pyPreservica-1.7.0/pyPreservica.egg-info/PKG-INFO` & `pyPreservica-1.7.1/pyPreservica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyPreservica
-Version: 1.7.0
+Version: 1.7.1
 Summary: Python library for the Preservica API
 Home-page: https://pypreservica.readthedocs.io/
 Author: James Carr
 Author-email: drjamescarr@gmail.com
 License: Apache License 2.0
 Project-URL: Documentation, https://pypreservica.readthedocs.io
 Project-URL: Source, https://github.com/carj/pyPreservica
```

### Comparing `pyPreservica-1.7.0/setup.py` & `pyPreservica-1.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     os.system('twine upload dist/*')
     sys.exit()
 
 
 # This call to setup() does all the work
 setup(
     name=PKG,
-    version="1.7.0",
+    version="1.7.1",
     description="Python library for the Preservica API",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://pypreservica.readthedocs.io/",
     author="James Carr",
     author_email="drjamescarr@gmail.com",
     license="Apache License 2.0",
```

