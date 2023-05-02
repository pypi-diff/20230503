# Comparing `tmp/pyloobins-0.1.3.tar.gz` & `tmp/pyloobins-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyloobins-0.1.3.tar", max compression
+gzip compressed data, was "pyloobins-0.1.5.tar", max compression
```

## Comparing `pyloobins-0.1.3.tar` & `pyloobins-0.1.5.tar`

### file list

```diff
@@ -1,10 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.3/LICENSE
--rw-r--r--   0        0        0     1295 2023-04-19 23:03:54.627657 pyloobins-0.1.3/LOOBins/pbpaste.yml
--rw-r--r--   0        0        0      331 2023-04-11 23:56:04.085703 pyloobins-0.1.3/README.md
--rw-r--r--   0        0        0      877 2023-04-19 23:11:53.845950 pyloobins-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.3/src/pyloobins/__init__.py
--rw-r--r--   0        0        0     1538 2023-04-19 23:11:53.846281 pyloobins-0.1.3/src/pyloobins/cli.py
--rw-r--r--   0        0        0     3582 2023-04-19 22:59:33.848606 pyloobins-0.1.3/src/pyloobins/models.py
--rw-r--r--   0        0        0     1177 2023-04-12 00:48:36.484104 pyloobins-0.1.3/src/pyloobins/templates/loobin.md.j2
--rw-r--r--   0        0        0     2610 2023-04-19 22:59:31.417375 pyloobins-0.1.3/src/pyloobins/util.py
--rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 pyloobins-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-11 23:56:04.085551 pyloobins-0.1.5/LICENSE
+-rw-r--r--   0        0        0      885 2023-05-01 23:30:07.408912 pyloobins-0.1.5/LOOBins/GetFileInfo.yml
+-rw-r--r--   0        0        0     1412 2023-05-01 23:30:07.409275 pyloobins-0.1.5/LOOBins/SetFile.yml
+-rw-r--r--   0        0        0     3545 2023-05-01 23:30:07.409751 pyloobins-0.1.5/LOOBins/dscl.yml
+-rw-r--r--   0        0        0     2138 2023-05-01 23:30:07.409978 pyloobins-0.1.5/LOOBins/ioreg.yml
+-rw-r--r--   0        0        0     1538 2023-05-01 01:46:27.775139 pyloobins-0.1.5/LOOBins/last.yml
+-rw-r--r--   0        0        0     1224 2023-05-01 23:30:07.410602 pyloobins-0.1.5/LOOBins/mdfind.yml
+-rw-r--r--   0        0        0     4420 2023-05-01 23:30:07.410858 pyloobins-0.1.5/LOOBins/networksetup.yml
+-rw-r--r--   0        0        0     3237 2023-05-01 23:30:07.411097 pyloobins-0.1.5/LOOBins/osascript.yml
+-rw-r--r--   0        0        0     1263 2023-05-01 23:30:07.411462 pyloobins-0.1.5/LOOBins/pbpaste.yml
+-rw-r--r--   0        0        0     1051 2023-05-01 01:46:27.801548 pyloobins-0.1.5/LOOBins/screencapture.yml
+-rw-r--r--   0        0        0     2458 2023-05-01 01:46:27.474479 pyloobins-0.1.5/LOOBins/security.yml
+-rw-r--r--   0        0        0      840 2023-05-01 23:30:07.411670 pyloobins-0.1.5/LOOBins/softwareupdate.yml
+-rw-r--r--   0        0        0      790 2023-05-01 23:30:07.411980 pyloobins-0.1.5/LOOBins/sysctl.yml
+-rw-r--r--   0        0        0     1636 2023-04-23 17:34:43.219172 pyloobins-0.1.5/LOOBins/xattr.yml
+-rw-r--r--   0        0        0      331 2023-04-11 23:56:04.085703 pyloobins-0.1.5/README.md
+-rw-r--r--   0        0        0      877 2023-05-02 22:58:45.096617 pyloobins-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-07 02:06:55.452190 pyloobins-0.1.5/src/pyloobins/__init__.py
+-rw-r--r--   0        0        0     1538 2023-04-19 23:44:40.581452 pyloobins-0.1.5/src/pyloobins/cli.py
+-rw-r--r--   0        0        0     3776 2023-05-02 22:58:45.096968 pyloobins-0.1.5/src/pyloobins/models.py
+-rw-r--r--   0        0        0     1311 2023-05-01 23:30:07.412430 pyloobins-0.1.5/src/pyloobins/templates/loobin.md.j2
+-rw-r--r--   0        0        0     2729 2023-04-23 17:34:43.219963 pyloobins-0.1.5/src/pyloobins/util.py
+-rw-r--r--   0        0        0     1214 1970-01-01 00:00:00.000000 pyloobins-0.1.5/PKG-INFO
```

### Comparing `pyloobins-0.1.3/LICENSE` & `pyloobins-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.3/LOOBins/pbpaste.yml` & `pyloobins-0.1.5/LOOBins/pbpaste.yml`

 * *Files 10% similar despite different names*

```diff
@@ -13,11 +13,11 @@
   tags:
   - bash
   - oneliner
 paths:
 - /usr/bin/pbpaste
 detections:
 - name: No detections at time of publishing
-  url: https://loobins.io/binaries/pbpaste
+  url: N/A
 resources:
 - name: 'Hacking macOS: How to Dump 1Password, KeePassX & LastPass Passwords in Plaintext'
   url: https://medium.com/@NullByteWht/hacking-macos-how-to-dump-1password-keepassx-lastpass-passwords-in-plaintext-723c5b1c311b
```

### Comparing `pyloobins-0.1.3/pyproject.toml` & `pyloobins-0.1.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PyLOOBins"
-version = "0.1.3"
+version = "0.1.5"
 description = "Python package for managing the LOOBins model and schema."
 authors = ["infosecB <brendan@infosecb.com>"]
 readme = "README.md"
 packages = [{include = "pyloobins", from = "src"}]
 include = ["LOOBins/*.yml"]
 homepage = "https://loobins.io/"
 repository = "https://github.com/infosecB/LOOBins"
```

### Comparing `pyloobins-0.1.3/src/pyloobins/cli.py` & `pyloobins-0.1.5/src/pyloobins/cli.py`

 * *Files identical despite different names*

### Comparing `pyloobins-0.1.3/src/pyloobins/models.py` & `pyloobins-0.1.5/src/pyloobins/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,19 +78,19 @@
     )
     acknowledgements: Optional[List[str]] = Field(
         title="Acknowledgements", description="Acknowledgements for the LOOBin"
     )
 
     def combine_tactics(self) -> List[str]:
         """Returns a list of all tactics across all LOOBin example use cases"""
-        return [t for euc in self.example_use_cases for t in euc.tactics]  # type: ignore
+        return list(dict.fromkeys([t for euc in self.example_use_cases for t in euc.tactics]))  # type: ignore
 
     def combine_tags(self) -> List[str]:
         """Returns a list of all tags across all LOOBin example use cases"""
-        return [t for euc in self.example_use_cases for t in euc.tags]  # type: ignore
+        return list(dict.fromkeys([t for euc in self.example_use_cases for t in euc.tags]))  # type: ignore
 
     def to_yaml(self, exclude_null: bool = True) -> str:
         """Convert a LOOBin object to a YAML string"""
         return yaml.dump(
             self.dict(exclude_none=exclude_null),
             Dumper=yaml.Dumper,
             sort_keys=False,
@@ -111,7 +111,13 @@
         return template
 
     def __str__(self) -> str:
         return self.to_yaml()
 
     def __repr__(self) -> str:
         return self.to_yaml()
+
+
+class LOOBinsGroup(BaseModel):
+    """LOOBin list base class"""
+
+    __root__: List[LOOBin] = Field(title="LOOBins", description="A list of LOOBins")
```

### Comparing `pyloobins-0.1.3/src/pyloobins/templates/loobin.md.j2` & `pyloobins-0.1.5/src/pyloobins/templates/loobin.md.j2`

 * *Files 8% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 pinned: false
 featured: false
 tactics: {{ tactics }}
 tags: {{ tags }}
 ---
 
 # {{ loobin.name }}
+*Created by {{ loobin.author }}*
+
+## Description
 {{ loobin.full_description }}
 | Created | Tactics | Tags |
 |---|---|---|
 | {{ loobin.created }} | {% for t in tactics %}<span class="badge text-bg-danger">{{ t }}</span> {% endfor %}  | {% for t in tags %}<span class="badge text-bg-secondary">{{ t }}</span> {% endfor %} | 
 
 ## Paths
 {% for path in loobin.paths %}
@@ -26,20 +29,27 @@
 {% endfor %}
 
 ## Use Cases
 {% for example in loobin.example_use_cases %}
 #### {{ example.name }}
 {{ example.description }}
 
-`{{ example.code }}`
+```
+{{ example.code }}
+```
+
 {% endfor %}
 
 ## Detections
 {% for detection in loobin.detections %}
+{% if detection.url in "N/A" %}
+- {{ detection.name }}
+{% else %}
 - [{{ detection.name }}]({{ detection.url }})
+{% endif %}
 {% endfor %}
 
 {% if loobin.resources %}
 ## Resources
 {% for resource in loobin.resources %}
 - [{{ resource.name }}]({{ resource.url }})
 {% endfor %}
```

### Comparing `pyloobins-0.1.3/src/pyloobins/util.py` & `pyloobins-0.1.5/src/pyloobins/util.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,18 +4,23 @@
 from datetime import date
 
 import yaml
 
 from .models import Detection, ExampleUseCase, LOOBin, Resource
 
 
-def get_loobins() -> list:
+def get_loobins(path: str = "") -> list:
     """Returns a list of LOOBin objects"""
     loobins = []
-    yml_files = (pathlib.Path(site.getsitepackages()[0]) / "LOOBins").glob("**/*.yml")
+    if path:
+        yml_files = pathlib.Path(path).glob("**/*.yml")
+    else:
+        yml_files = (pathlib.Path(site.getsitepackages()[0]) / "LOOBins").glob(
+            "**/*.yml"
+        )
     for yml_file in yml_files:
         with open(yml_file, "r", encoding="utf-8") as stream:
             try:
                 yml_content = yaml.safe_load(stream)
             except yaml.YAMLError as exc:
                 print(exc)
         try:
```

### Comparing `pyloobins-0.1.3/PKG-INFO` & `pyloobins-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyloobins
-Version: 0.1.3
+Version: 0.1.5
 Summary: Python package for managing the LOOBins model and schema.
 Home-page: https://loobins.io/
 License: GPL-3.0-or-later
 Keywords: cybersecurity,cli,lol
 Author: infosecB
 Author-email: brendan@infosecb.com
 Requires-Python: >=3.8,<4.0
```

