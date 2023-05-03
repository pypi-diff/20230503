# Comparing `tmp/open-pyxl-sql-0.13.tar.gz` & `tmp/open_pyxl_sql-1.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-pyxl-sql-0.13.tar", last modified: Wed May  3 14:07:16 2023, max compression
+gzip compressed data, was "open_pyxl_sql-1.1rc3.tar", last modified: Tue Mar 21 22:14:12 2023, max compression
```

## Comparing `open-pyxl-sql-0.13.tar` & `open_pyxl_sql-1.1rc3.tar`

### file list

```diff
@@ -1,13 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 14:07:16.320599 open-pyxl-sql-0.13/
--rw-rw-rw-   0        0        0      700 2023-05-03 14:07:16.318173 open-pyxl-sql-0.13/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 14:07:16.283040 open-pyxl-sql-0.13/PyxlSql/
--rw-rw-rw-   0        0        0      496 2023-04-24 07:16:16.000000 open-pyxl-sql-0.13/PyxlSql/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-03 14:04:45.000000 open-pyxl-sql-0.13/PyxlSql/__main__.py
--rw-rw-rw-   0        0        0      333 2023-05-03 13:53:46.000000 open-pyxl-sql-0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 14:07:16.315169 open-pyxl-sql-0.13/open_pyxl_sql.egg-info/
--rw-rw-rw-   0        0        0      700 2023-05-03 14:07:16.000000 open-pyxl-sql-0.13/open_pyxl_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-03 14:07:16.000000 open-pyxl-sql-0.13/open_pyxl_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 14:07:16.000000 open-pyxl-sql-0.13/open_pyxl_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 14:07:16.000000 open-pyxl-sql-0.13/open_pyxl_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 14:07:16.321130 open-pyxl-sql-0.13/setup.cfg
--rw-rw-rw-   0        0        0     1040 2023-05-03 14:03:03.000000 open-pyxl-sql-0.13/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-21 22:14:12.821927 open_pyxl_sql-1.1rc3/
+-rw-rw-rw-   0        0        0    14408 2023-03-13 18:23:44.000000 open_pyxl_sql-1.1rc3/LICENCE
+-rw-rw-rw-   0        0        0     7002 2023-03-21 22:14:12.819560 open_pyxl_sql-1.1rc3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-03-21 22:14:12.770251 open_pyxl_sql-1.1rc3/PyxlSql/
+-rw-rw-rw-   0        0        0      563 2023-03-13 18:23:44.000000 open_pyxl_sql-1.1rc3/PyxlSql/__init__.py
+-rw-rw-rw-   0        0        0     7107 2023-03-20 17:20:35.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlAbstracts.py
+-rw-rw-rw-   0        0        0    15428 2023-03-21 21:54:41.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlArgs.py
+-rw-rw-rw-   0        0        0    33782 2023-03-21 21:46:02.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlEngine.py
+-rw-rw-rw-   0        0        0     2934 2023-03-13 18:23:44.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlErrors.py
+-rw-rw-rw-   0        0        0    25458 2023-03-21 21:54:40.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlGrammar.py
+-rw-rw-rw-   0        0        0     9165 2023-03-21 21:54:41.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlPivot.py
+-rw-rw-rw-   0        0        0     7231 2023-03-21 21:57:15.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlResults.py
+-rw-rw-rw-   0        0        0     9087 2023-03-21 21:47:23.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlSheets.py
+-rw-rw-rw-   0        0        0    12913 2023-03-21 21:57:15.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlSql.py
+-rw-rw-rw-   0        0        0    14413 2023-03-20 16:49:03.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlStages.py
+-rw-rw-rw-   0        0        0     5355 2023-03-21 21:07:46.000000 open_pyxl_sql-1.1rc3/PyxlSql/pyxlWorkbook.py
+-rw-rw-rw-   0        0        0     6337 2023-03-18 22:32:03.000000 open_pyxl_sql-1.1rc3/README.md
+drwxrwxrwx   0        0        0        0 2023-03-21 22:14:12.808971 open_pyxl_sql-1.1rc3/open_pyxl_sql.egg-info/
+-rw-rw-rw-   0        0        0     7002 2023-03-21 22:14:12.000000 open_pyxl_sql-1.1rc3/open_pyxl_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      483 2023-03-21 22:14:12.000000 open_pyxl_sql-1.1rc3/open_pyxl_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-21 22:14:12.000000 open_pyxl_sql-1.1rc3/open_pyxl_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-03-21 22:14:12.000000 open_pyxl_sql-1.1rc3/open_pyxl_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-21 22:14:12.821927 open_pyxl_sql-1.1rc3/setup.cfg
+-rw-rw-rw-   0        0        0      934 2023-03-21 22:10:45.000000 open_pyxl_sql-1.1rc3/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-21 22:14:12.815484 open_pyxl_sql-1.1rc3/tests/
+-rw-rw-rw-   0        0        0     7695 2023-03-21 21:48:10.000000 open_pyxl_sql-1.1rc3/tests/test_Northwind.py
+-rw-rw-rw-   0        0        0     6365 2023-03-21 21:33:07.000000 open_pyxl_sql-1.1rc3/tests/test_tooling.py
```

### Comparing `open-pyxl-sql-0.13/setup.py` & `open_pyxl_sql-1.1rc3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import setuptools
 
-# see https://setuptools.pypa.io/en/latest/references/keywords.html
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
 setuptools.setup(
-    name="open-pyxl-sql",
-    version='0.13',
-    author="Fabien BATTINI",                    # noqa
+    name="open_pyxl_sql",
+    version="1.1.RC3",
+    author="Fabien BATTINI",
     author_email="fabien.battini@gmail.com",
-    description="A tiny SQL engine for Excel files, moved to excel-sql-engine",
-    long_description='moved to excel-sql-engine',
+    description="A tiny SQL engine for Excel files, based on Openpyxl",
+    long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/fabien.battini/pyxlsql",
-    license_files=["LICENCE"],
-    keywords='excel sql',
     packages=setuptools.find_packages(),
     classifiers=[
         # see https://pypi.org/classifiers/
         "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",  # noqa
+        "License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)",
         "Operating System :: OS Independent",
-        "Development Status :: 7 - Inactive",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: End Users/Desktop",
         "Topic :: Office/Business :: Office Suites",
     ],
     python_requires='>=3.6',
-)
+)
+
```

