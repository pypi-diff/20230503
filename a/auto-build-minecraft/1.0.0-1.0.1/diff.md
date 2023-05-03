# Comparing `tmp/auto_build_minecraft-1.0.0.tar.gz` & `tmp/auto_build_minecraft-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_build_minecraft-1.0.0.tar", max compression
+gzip compressed data, was "auto_build_minecraft-1.0.1.tar", max compression
```

## Comparing `auto_build_minecraft-1.0.0.tar` & `auto_build_minecraft-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1072 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/LICENSE
--rw-r--r--   0        0        0     1831 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/README.md
--rw-r--r--   0        0        0      762 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/Docker/Dockerfile
--rw-r--r--   0        0        0     4972 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/msab.py
--rw-r--r--   0        0        0     1077 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/playbook.yml
--rw-r--r--   0        0        0      584 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/add-hosts.yml
--rw-r--r--   0        0        0     2436 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/create-instance.yml
--rw-r--r--   0        0        0      921 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/delete-instance.yml
--rw-r--r--   0        0        0      654 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/download-world-data.yml
--rw-r--r--   0        0        0     1196 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/run-server.yml
--rw-r--r--   0        0        0      321 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/start-instance.yml
--rw-r--r--   0        0        0      324 2023-04-28 07:06:24.574220 auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/stop-instance.yml
--rw-r--r--   0        0        0      429 2023-04-28 07:06:24.638220 auto_build_minecraft-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 auto_build_minecraft-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1831 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/README.md
+-rw-r--r--   0        0        0      762 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/Docker/Dockerfile
+-rw-r--r--   0        0        0     4972 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/msab.py
+-rw-r--r--   0        0        0     1077 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/playbook.yml
+-rw-r--r--   0        0        0      584 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/add-hosts.yml
+-rw-r--r--   0        0        0     2436 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/create-instance.yml
+-rw-r--r--   0        0        0      921 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/delete-instance.yml
+-rw-r--r--   0        0        0      596 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/download-world-data.yml
+-rw-r--r--   0        0        0     1196 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/run-server.yml
+-rw-r--r--   0        0        0      321 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/start-instance.yml
+-rw-r--r--   0        0        0      324 2023-05-02 23:58:27.994622 auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/stop-instance.yml
+-rw-r--r--   0        0        0      429 2023-05-02 23:58:28.066625 auto_build_minecraft-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 auto_build_minecraft-1.0.1/PKG-INFO
```

### Comparing `auto_build_minecraft-1.0.0/LICENSE` & `auto_build_minecraft-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/README.md` & `auto_build_minecraft-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/auto_build_minecraft/Docker/Dockerfile` & `auto_build_minecraft-1.0.1/auto_build_minecraft/Docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/auto_build_minecraft/msab.py` & `auto_build_minecraft-1.0.1/auto_build_minecraft/msab.py`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/auto_build_minecraft/playbook.yml` & `auto_build_minecraft-1.0.1/auto_build_minecraft/playbook.yml`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/add-hosts.yml` & `auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/add-hosts.yml`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/create-instance.yml` & `auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/create-instance.yml`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/delete-instance.yml` & `auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/delete-instance.yml`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/download-world-data.yml` & `auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/download-world-data.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ---
 - name: Create downloads folder
   file:
-    path: "{{ resource_file_dest }}/downloads"
+    path: "downloads"
     state: directory
     mode: '0755'
 
 - name: Download files from docker container
-  command: "docker cp minecraft-server:/minecraft/{{ item }} {{ resource_file_dest }}/downloads/"
+  command: "docker cp minecraft-server:/minecraft/{{ item }} downloads"
   loop:
     - eula.txt
     - ops.json
     - server.properties
     - whitelist.json
     - mods
     - world
 
 - name: Get file list
   find:
-    paths: "{{ resource_file_dest }}/downloads"
+    paths: "downloads"
     recurse: true
   register: files
 
 - name: Download files from server to local
   fetch:
     src: "{{ item }}"
-    dest: "./Downloads/"
+    dest: "{{ resources_path }}/Downloads"
   loop: "{{ files.files | map(attribute='path') | list }}"
```

### Comparing `auto_build_minecraft-1.0.0/auto_build_minecraft/tasks/run-server.yml` & `auto_build_minecraft-1.0.1/auto_build_minecraft/tasks/run-server.yml`

 * *Files identical despite different names*

### Comparing `auto_build_minecraft-1.0.0/PKG-INFO` & `auto_build_minecraft-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-build-minecraft
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 License: MIT
 Author: nerianighthawk
 Author-email: neria.nighthawk@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

