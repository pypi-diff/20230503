# Comparing `tmp/test-clik-0.0.1.tar.gz` & `tmp/test-clik-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test-clik-0.0.1.tar", last modified: Wed May  3 20:29:15 2023, max compression
+gzip compressed data, was "test-clik-0.0.2.tar", last modified: Wed May  3 21:38:04 2023, max compression
```

## Comparing `test-clik-0.0.1.tar` & `test-clik-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 20:29:15.448161 test-clik-0.0.1/
--rw-rw-rw-   0        0        0      478 2023-05-03 20:29:15.446138 test-clik-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       70 2023-05-03 20:00:39.000000 test-clik-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 20:29:15.448161 test-clik-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-05-03 20:28:37.000000 test-clik-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:29:15.397371 test-clik-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 20:29:15.405396 test-clik-0.0.1/src/test_click/
--rw-rw-rw-   0        0        0       39 2023-05-03 18:31:17.000000 test-clik-0.0.1/src/test_click/__init__.py
--rw-rw-rw-   0        0        0     1281 2023-05-03 20:27:27.000000 test-clik-0.0.1/src/test_click/cli.py
--rw-rw-rw-   0        0        0      365 2023-05-03 18:30:25.000000 test-clik-0.0.1/src/test_click/operaciones.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:29:15.410407 test-clik-0.0.1/src/test_click/struct/
--rw-rw-rw-   0        0        0      886 2023-05-03 18:02:16.000000 test-clik-0.0.1/src/test_click/struct/404.py
--rw-rw-rw-   0        0        0        0 2023-05-03 18:02:34.000000 test-clik-0.0.1/src/test_click/struct/__init__.py
--rw-rw-rw-   0        0        0     1105 2023-05-03 18:01:12.000000 test-clik-0.0.1/src/test_click/struct/index.py
--rw-rw-rw-   0        0        0      209 2023-05-03 17:59:59.000000 test-clik-0.0.1/src/test_click/struct/main.py
-drwxrwxrwx   0        0        0        0 2023-05-03 20:29:15.444615 test-clik-0.0.1/src/test_clik.egg-info/
--rw-rw-rw-   0        0        0      478 2023-05-03 20:29:15.000000 test-clik-0.0.1/src/test_clik.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-05-03 20:29:15.000000 test-clik-0.0.1/src/test_clik.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 20:29:15.000000 test-clik-0.0.1/src/test_clik.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-05-03 20:29:15.000000 test-clik-0.0.1/src/test_clik.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-05-03 20:29:15.000000 test-clik-0.0.1/src/test_clik.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-03 20:29:15.000000 test-clik-0.0.1/src/test_clik.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 21:38:04.854205 test-clik-0.0.2/
+-rw-rw-rw-   0        0        0      478 2023-05-03 21:38:04.853205 test-clik-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2023-05-03 20:00:39.000000 test-clik-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 21:38:04.854726 test-clik-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-05-03 21:37:24.000000 test-clik-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 21:38:04.805301 test-clik-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 21:38:04.812845 test-clik-0.0.2/src/test_click/
+-rw-rw-rw-   0        0        0       39 2023-05-03 18:31:17.000000 test-clik-0.0.2/src/test_click/__init__.py
+-rw-rw-rw-   0        0        0     1333 2023-05-03 21:36:01.000000 test-clik-0.0.2/src/test_click/cli.py
+-rw-rw-rw-   0        0        0      365 2023-05-03 18:30:25.000000 test-clik-0.0.2/src/test_click/operaciones.py
+drwxrwxrwx   0        0        0        0 2023-05-03 21:38:04.851209 test-clik-0.0.2/src/test_clik.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-05-03 21:38:04.000000 test-clik-0.0.2/src/test_clik.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-05-03 21:38:04.000000 test-clik-0.0.2/src/test_clik.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 21:38:04.000000 test-clik-0.0.2/src/test_clik.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-05-03 21:38:04.000000 test-clik-0.0.2/src/test_clik.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-05-03 21:38:04.000000 test-clik-0.0.2/src/test_clik.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-03 21:38:04.000000 test-clik-0.0.2/src/test_clik.egg-info/top_level.txt
```

### Comparing `test-clik-0.0.1/setup.py` & `test-clik-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("./README.md", "r", encoding="utf-8") as e:
     long_description = e.read()
 
 setup(
     name="test-clik",
-    version="0.0.1",
+    version="0.0.2",
     author="Dxsxsx",
     author_email="123@pm.me",
     description="test clip",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dxsxsx",
     package_dir={"":"src"},
```

### Comparing `test-clik-0.0.1/src/test_click/cli.py` & `test-clik-0.0.2/src/test_click/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import click
 from pathlib import Path
 
 
 @click.command()
 def init():
-    # creacion archivo main.py
+    # creacion archivo main.pypip
     file_path_main = Path('./') / 'main.py'
     file_path_main.touch()
 
     source_path = Path(__file__).parent / 'struct/main.py'
 
     with open(source_path, 'r') as source_file:
         content = source_file.read()
 
     with open(file_path_main, 'w') as file:
         file.write(content)
 
     # creacion de las vistas/archivos.py
     Path('views').mkdir(exist_ok=True)
-    # file_path_view = file_path_main = Path('./views') / 'main.py'
-    file_list = ['__init__.py', 'index.py', '404.py']
+    file = Path('views') / '__init__.py'
+    file.touch()
+
+    file_list = ['index.py', '404.py']
 
     for file_name in file_list:
         file = Path('views') / file_name
         file.touch()
 
+        source_path = Path(__file__).parent / f'struct/{file_name}'
+
         with open(source_path, 'r') as source_file:
             content = source_file.read()
 
         with open(file, 'w') as file:
             file.write(content)
 
-    print('Se ha creado correctamente!')
+    print('Se ha creado correctamente!', content)
 
     click.echo()
     click.echo(
         f"Generado {len(file_list)} files in the 'view' directory y  el archivo main.py:")
     for files in file_list:
         click.echo(f"● {files}")
     click.echo()
@@ -45,8 +49,8 @@
 def flet_template():
     pass
 
 
 flet_template.add_command(init)
 
 if __name__ == "__main__":
-    flet_template()
+    init()
```

