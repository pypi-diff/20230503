# Comparing `tmp/html_generators-2.6.0.tar.gz` & `tmp/html_generators-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/html_generators-2.6.0.tar", last modified: Wed Mar 16 21:58:39 2022, max compression
+gzip compressed data, was "dist/html_generators-2.7.0.tar", last modified: Wed May  3 15:13:57 2023, max compression
```

## Comparing `html_generators-2.6.0.tar` & `html_generators-2.7.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-03-16 21:58:39.000000 html_generators-2.6.0/
--rw-r--r--   0 alex       (502) staff       (20)    10706 2022-03-16 21:58:39.000000 html_generators-2.6.0/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)       68 2020-06-19 15:05:16.000000 html_generators-2.6.0/MANIFEST.in
--rw-r--r--   0 alex       (502) staff       (20)     8429 2021-11-03 17:26:27.000000 html_generators-2.6.0/README.md
--rw-r--r--   0 alex       (502) staff       (20)      818 2020-06-19 16:20:50.000000 html_generators-2.6.0/setup.py
--rw-r--r--   0 alex       (502) staff       (20)        5 2022-03-16 21:57:25.000000 html_generators-2.6.0/VERSION
--rw-r--r--   0 alex       (502) staff       (20)     2479 2022-03-16 21:58:28.000000 html_generators-2.6.0/RELEASE_NOTES.md
--rw-r--r--   0 alex       (502) staff       (20)       38 2022-03-16 21:58:39.000000 html_generators-2.6.0/setup.cfg
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-03-16 21:58:39.000000 html_generators-2.6.0/src/
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-03-16 21:58:39.000000 html_generators-2.6.0/src/html_generators.egg-info/
--rw-r--r--   0 alex       (502) staff       (20)    10706 2022-03-16 21:58:38.000000 html_generators-2.6.0/src/html_generators.egg-info/PKG-INFO
--rw-r--r--   0 alex       (502) staff       (20)     1784 2022-03-16 21:58:38.000000 html_generators-2.6.0/src/html_generators.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (502) staff       (20)       16 2022-03-16 21:58:38.000000 html_generators-2.6.0/src/html_generators.egg-info/top_level.txt
--rw-r--r--   0 alex       (502) staff       (20)        1 2022-03-16 21:58:38.000000 html_generators-2.6.0/src/html_generators.egg-info/dependency_links.txt
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-03-16 21:58:39.000000 html_generators-2.6.0/src/html_generators/
--rw-r--r--   0 alex       (502) staff       (20)     2355 2021-11-04 16:18:23.000000 html_generators-2.6.0/src/html_generators/django.py
--rw-r--r--   0 alex       (502) staff       (20)     3595 2022-03-16 21:55:51.000000 html_generators-2.6.0/src/html_generators/_base.py
--rw-r--r--   0 alex       (502) staff       (20)      430 2021-04-01 21:25:30.000000 html_generators-2.6.0/src/html_generators/_comment.py
--rw-r--r--   0 alex       (502) staff       (20)     5435 2021-04-01 21:25:30.000000 html_generators-2.6.0/src/html_generators/_standard_elements.py
--rw-r--r--   0 alex       (502) staff       (20)      762 2022-03-16 21:53:30.000000 html_generators-2.6.0/src/html_generators/__init__.py
--rw-r--r--   0 alex       (502) staff       (20)     4666 2022-03-16 21:56:28.000000 html_generators-2.6.0/src/html_generators/_element.py
-drwxr-xr-x   0 alex       (502) staff       (20)        0 2022-03-16 21:58:39.000000 html_generators-2.6.0/src/html_generators/__pycache__/
--rw-r--r--   0 alex       (502) staff       (20)     3029 2022-03-16 21:04:41.000000 html_generators-2.6.0/src/html_generators/__pycache__/_template.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     2730 2021-11-04 16:18:35.000000 html_generators-2.6.0/src/html_generators/__pycache__/django.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      599 2020-06-19 15:59:09.000000 html_generators-2.6.0/src/html_generators/__pycache__/mark_safe.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      896 2021-04-01 21:29:01.000000 html_generators-2.6.0/src/html_generators/__pycache__/_comment.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     1038 2022-03-16 21:55:52.000000 html_generators-2.6.0/src/html_generators/__pycache__/_format.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     4348 2020-06-19 16:00:18.000000 html_generators-2.6.0/src/html_generators/__pycache__/elements.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     1134 2021-04-01 21:29:01.000000 html_generators-2.6.0/src/html_generators/__pycache__/_join.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      982 2021-08-17 18:01:17.000000 html_generators-2.6.0/src/html_generators/__pycache__/_document.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      664 2020-06-19 15:59:09.000000 html_generators-2.6.0/src/html_generators/__pycache__/document.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     1026 2021-04-01 21:29:01.000000 html_generators-2.6.0/src/html_generators/__pycache__/_fragment.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      876 2021-04-01 21:29:01.000000 html_generators-2.6.0/src/html_generators/__pycache__/_mark_safe.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      623 2022-03-16 21:55:52.000000 html_generators-2.6.0/src/html_generators/__pycache__/_utils.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      937 2020-06-19 15:59:09.000000 html_generators-2.6.0/src/html_generators/__pycache__/base.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     3492 2021-04-01 21:29:01.000000 html_generators-2.6.0/src/html_generators/__pycache__/_standard_elements.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     6122 2022-03-16 21:56:46.000000 html_generators-2.6.0/src/html_generators/__pycache__/_element.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     3002 2022-03-16 21:55:52.000000 html_generators-2.6.0/src/html_generators/__pycache__/_base.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      866 2022-03-16 21:55:25.000000 html_generators-2.6.0/src/html_generators/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)      963 2020-06-19 17:00:05.000000 html_generators-2.6.0/src/html_generators/__pycache__/fragment.cpython-36.pyc
--rw-r--r--   0 alex       (502) staff       (20)     8429 2021-11-03 17:26:27.000000 html_generators-2.6.0/src/html_generators/README.md
--rw-r--r--   0 alex       (502) staff       (20)     2896 2022-03-16 21:03:27.000000 html_generators-2.6.0/src/html_generators/_template.py
--rw-r--r--   0 alex       (502) staff       (20)      537 2021-08-17 18:01:15.000000 html_generators-2.6.0/src/html_generators/_document.py
--rw-r--r--   0 alex       (502) staff       (20)      795 2022-03-16 21:57:44.000000 html_generators-2.6.0/src/html_generators/_format.py
--rw-r--r--   0 alex       (502) staff       (20)      931 2021-04-01 21:25:30.000000 html_generators-2.6.0/src/html_generators/_join.py
--rw-r--r--   0 alex       (502) staff       (20)        5 2022-03-16 21:57:25.000000 html_generators-2.6.0/src/html_generators/VERSION
--rw-r--r--   0 alex       (502) staff       (20)      557 2021-04-01 21:25:30.000000 html_generators-2.6.0/src/html_generators/_fragment.py
--rw-r--r--   0 alex       (502) staff       (20)     2479 2022-03-16 21:58:28.000000 html_generators-2.6.0/src/html_generators/RELEASE_NOTES.md
--rw-rw-r--   0 alex       (502) staff       (20)      299 2020-06-19 15:10:48.000000 html_generators-2.6.0/src/html_generators/__init__.pyc
--rw-r--r--   0 alex       (502) staff       (20)      402 2021-04-01 21:25:30.000000 html_generators-2.6.0/src/html_generators/_mark_safe.py
--rw-r--r--   0 alex       (502) staff       (20)      344 2022-03-16 21:40:36.000000 html_generators-2.6.0/src/html_generators/_utils.py
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-03 15:13:57.000000 html_generators-2.7.0/
+-rw-r--r--   0 alex       (502) staff       (20)    10706 2023-05-03 15:13:57.000000 html_generators-2.7.0/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)       68 2020-06-19 15:05:16.000000 html_generators-2.7.0/MANIFEST.in
+-rw-r--r--   0 alex       (502) staff       (20)     8429 2022-03-28 19:25:58.000000 html_generators-2.7.0/README.md
+-rw-r--r--   0 alex       (502) staff       (20)      818 2020-06-19 16:20:50.000000 html_generators-2.7.0/setup.py
+-rw-r--r--   0 alex       (502) staff       (20)        5 2023-05-03 15:09:54.000000 html_generators-2.7.0/VERSION
+-rw-r--r--   0 alex       (502) staff       (20)     2516 2023-05-03 15:10:16.000000 html_generators-2.7.0/RELEASE_NOTES.md
+-rw-r--r--   0 alex       (502) staff       (20)       38 2023-05-03 15:13:57.000000 html_generators-2.7.0/setup.cfg
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-03 15:13:57.000000 html_generators-2.7.0/src/
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-03 15:13:57.000000 html_generators-2.7.0/src/html_generators.egg-info/
+-rw-r--r--   0 alex       (502) staff       (20)    10706 2023-05-03 15:13:57.000000 html_generators-2.7.0/src/html_generators.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (502) staff       (20)     1944 2023-05-03 15:13:57.000000 html_generators-2.7.0/src/html_generators.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (502) staff       (20)       16 2023-05-03 15:13:57.000000 html_generators-2.7.0/src/html_generators.egg-info/top_level.txt
+-rw-r--r--   0 alex       (502) staff       (20)        1 2023-05-03 15:13:57.000000 html_generators-2.7.0/src/html_generators.egg-info/dependency_links.txt
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-03 15:13:57.000000 html_generators-2.7.0/src/html_generators/
+-rw-r--r--   0 alex       (502) staff       (20)     2355 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/django.py
+-rw-r--r--   0 alex       (502) staff       (20)     3769 2023-05-03 15:03:04.000000 html_generators-2.7.0/src/html_generators/_base.py
+-rw-r--r--   0 alex       (502) staff       (20)      430 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/_comment.py
+-rw-r--r--   0 alex       (502) staff       (20)     5435 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/_standard_elements.py
+-rw-r--r--   0 alex       (502) staff       (20)      828 2023-05-03 15:06:00.000000 html_generators-2.7.0/src/html_generators/__init__.py
+-rw-r--r--   0 alex       (502) staff       (20)     4656 2023-05-03 15:04:22.000000 html_generators-2.7.0/src/html_generators/_element.py
+drwxr-xr-x   0 alex       (502) staff       (20)        0 2023-05-03 15:13:57.000000 html_generators-2.7.0/src/html_generators/__pycache__/
+-rw-r--r--   0 alex       (502) staff       (20)     3029 2022-03-16 21:04:41.000000 html_generators-2.7.0/src/html_generators/__pycache__/_template.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     2730 2021-11-04 16:18:35.000000 html_generators-2.7.0/src/html_generators/__pycache__/django.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      615 2022-03-28 19:18:20.000000 html_generators-2.7.0/src/html_generators/__pycache__/mark_safe.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      896 2021-04-01 21:29:01.000000 html_generators-2.7.0/src/html_generators/__pycache__/_comment.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      638 2022-03-28 19:18:20.000000 html_generators-2.7.0/src/html_generators/__pycache__/comment.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     1041 2022-03-28 19:01:54.000000 html_generators-2.7.0/src/html_generators/__pycache__/_format.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     6876 2022-03-28 19:20:06.000000 html_generators-2.7.0/src/html_generators/__pycache__/elements.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     1134 2021-04-01 21:29:01.000000 html_generators-2.7.0/src/html_generators/__pycache__/_join.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      982 2021-08-17 18:01:17.000000 html_generators-2.7.0/src/html_generators/__pycache__/_document.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      680 2022-03-28 19:18:20.000000 html_generators-2.7.0/src/html_generators/__pycache__/document.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      937 2022-03-28 19:18:20.000000 html_generators-2.7.0/src/html_generators/__pycache__/join.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     1026 2021-04-01 21:29:01.000000 html_generators-2.7.0/src/html_generators/__pycache__/_fragment.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      876 2021-04-01 21:29:01.000000 html_generators-2.7.0/src/html_generators/__pycache__/_mark_safe.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      623 2022-03-16 21:55:52.000000 html_generators-2.7.0/src/html_generators/__pycache__/_utils.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     1510 2022-03-28 19:20:44.000000 html_generators-2.7.0/src/html_generators/__pycache__/base.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     3492 2021-04-01 21:29:01.000000 html_generators-2.7.0/src/html_generators/__pycache__/_standard_elements.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     6122 2022-03-16 21:56:46.000000 html_generators-2.7.0/src/html_generators/__pycache__/_element.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      489 2022-03-28 19:18:20.000000 html_generators-2.7.0/src/html_generators/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     3002 2022-03-16 21:55:52.000000 html_generators-2.7.0/src/html_generators/__pycache__/_base.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      523 2022-03-28 19:18:20.000000 html_generators-2.7.0/src/html_generators/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      966 2022-03-28 19:18:20.000000 html_generators-2.7.0/src/html_generators/__pycache__/fragment.cpython-36.pyc
+-rw-r--r--   0 alex       (502) staff       (20)     8429 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/README.md
+-rw-r--r--   0 alex       (502) staff       (20)     2896 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/_template.py
+-rw-r--r--   0 alex       (502) staff       (20)      537 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/_document.py
+-rw-r--r--   0 alex       (502) staff       (20)      795 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/_format.py
+-rw-r--r--   0 alex       (502) staff       (20)      943 2023-05-03 15:05:02.000000 html_generators-2.7.0/src/html_generators/_join.py
+-rw-r--r--   0 alex       (502) staff       (20)        5 2023-05-03 15:09:54.000000 html_generators-2.7.0/src/html_generators/VERSION
+-rw-r--r--   0 alex       (502) staff       (20)      557 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/_fragment.py
+-rw-r--r--   0 alex       (502) staff       (20)     2516 2023-05-03 15:10:16.000000 html_generators-2.7.0/src/html_generators/RELEASE_NOTES.md
+-rw-rw-r--   0 alex       (502) staff       (20)      299 2020-06-19 15:10:48.000000 html_generators-2.7.0/src/html_generators/__init__.pyc
+-rw-r--r--   0 alex       (502) staff       (20)      402 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/_mark_safe.py
+-rw-r--r--   0 alex       (502) staff       (20)      344 2022-03-28 19:25:58.000000 html_generators-2.7.0/src/html_generators/_utils.py
```

### Comparing `html_generators-2.6.0/PKG-INFO` & `html_generators-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html_generators
-Version: 2.6.0
+Version: 2.7.0
 Summary: Functional, streaming approach to HTML generation
 Home-page: https://github.com/quadrant-newmedia/html_generators
 Author: Alex Fischer
 Author-email: alex@quadrant.net
 License: UNKNOWN
 Description: # html_generators
```

### Comparing `html_generators-2.6.0/README.md` & `html_generators-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/setup.py` & `html_generators-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/RELEASE_NOTES.md` & `html_generators-2.7.0/RELEASE_NOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## 2.7.0
+Added `Content` type alias
+
 ## 2.6.0
 Added h.format(), and h.Element.open_tag()/close_tag()
 
 ## 2.5.0
 template() now accepts '{x}' placeholders (for xgettext compatibility), as well as '{{x}}'.
 Placeholders not passed in context are left in place, rather than removed.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_l4vavfs4_/tmp7k58yyuf_TarContainer/0/6.md", line 95, column 7: CDATA terminal not found*

 * *File "/tmp/diffoscope_l4vavfs4_/tmp7k58yyuf_TarContainer/0/6.md", line 95, column 7: CDATA terminal not found*

```diff
@@ -1,25 +1,25 @@
-## 2.6.0 Added h.format(), and h.Element.open_tag()/close_tag() ## 2.5.0
-template() now accepts '{x}' placeholders (for xgettext compatibility), as well
-as '{{x}}'. Placeholders not passed in context are left in place, rather than
-removed. ## 2.4.0 Fix behaviour of `html_generators.django.date()`. Technically
-this is a breaking change, but it's definitely the way it should have worked to
-begin with. ## 2.3.0 Add `template` class ## 2.2.0 `Document` now accepts
-kwargs as shortcut for generating html element. ## 2.1.0 Added a few more
-django utilities. ### 2.0.2 Bug fix - name attribute on void elements ### 2.0.1
-Fix import bug in html_generators.django # 2.0.0 Breaking changes: - removed
-add_classes, add_styles - attribute normalization - trim only trailing
-underscores (be sure to replace "_class" with "class_") - all submodules (other
-than django) are private - look for imported submodules ## 1.7.0 Added cloning
-methods ## 1.6.0 `Join()` is now smarter - ignores None/False items, and items
-need not be HTMLGenerators ### 1.5.1 Fix bug introduced in 1.5.0 (void elements
-and raw text elements were not normalizing attribute names). ## 1.5.0 Added
-`classes` and `styles` utility functions, and `add_classes` and `add_styles`
-methods to `Element`. ### 1.4.1 Attributes which clash with python keywords can
-now be postfixed with an underscore, as well as prefixed (PEP 8 recommends
-postfix). ## 1.4 Added `h.Join(joiner, iterable)` ### 1.3.1 Ensure that
-attributes with value 0 are rendered (the only values skipped are False and
-None). ## 1.3.0 Add support for comments. ### 1.2.1 Ensure that children with
-value 0 (any number type) are rendered (the only values skipped are False and
-None). ## 1.2.0 Support "Safe Strings" from frameworks like Django. Children
-with `__html__()` method will not be escaped. ## 1.1.0 Do not escape contents
-of `
+## 2.7.0 Added `Content` type alias ## 2.6.0 Added h.format(), and
+h.Element.open_tag()/close_tag() ## 2.5.0 template() now accepts '{x}'
+placeholders (for xgettext compatibility), as well as '{{x}}'. Placeholders not
+passed in context are left in place, rather than removed. ## 2.4.0 Fix
+behaviour of `html_generators.django.date()`. Technically this is a breaking
+change, but it's definitely the way it should have worked to begin with. ##
+2.3.0 Add `template` class ## 2.2.0 `Document` now accepts kwargs as shortcut
+for generating html element. ## 2.1.0 Added a few more django utilities. ###
+2.0.2 Bug fix - name attribute on void elements ### 2.0.1 Fix import bug in
+html_generators.django # 2.0.0 Breaking changes: - removed add_classes,
+add_styles - attribute normalization - trim only trailing underscores (be sure
+to replace "_class" with "class_") - all submodules (other than django) are
+private - look for imported submodules ## 1.7.0 Added cloning methods ## 1.6.0
+`Join()` is now smarter - ignores None/False items, and items need not be
+HTMLGenerators ### 1.5.1 Fix bug introduced in 1.5.0 (void elements and raw
+text elements were not normalizing attribute names). ## 1.5.0 Added `classes`
+and `styles` utility functions, and `add_classes` and `add_styles` methods to
+`Element`. ### 1.4.1 Attributes which clash with python keywords can now be
+postfixed with an underscore, as well as prefixed (PEP 8 recommends postfix).
+## 1.4 Added `h.Join(joiner, iterable)` ### 1.3.1 Ensure that attributes with
+value 0 are rendered (the only values skipped are False and None). ## 1.3.0 Add
+support for comments. ### 1.2.1 Ensure that children with value 0 (any number
+type) are rendered (the only values skipped are False and None). ## 1.2.0
+Support "Safe Strings" from frameworks like Django. Children with `__html__()`
+method will not be escaped. ## 1.1.0 Do not escape contents of `
```

### Comparing `html_generators-2.6.0/src/html_generators.egg-info/PKG-INFO` & `html_generators-2.7.0/src/html_generators.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-generators
-Version: 2.6.0
+Version: 2.7.0
 Summary: Functional, streaming approach to HTML generation
 Home-page: https://github.com/quadrant-newmedia/html_generators
 Author: Alex Fischer
 Author-email: alex@quadrant.net
 License: UNKNOWN
 Description: # html_generators
```

### Comparing `html_generators-2.6.0/src/html_generators.egg-info/SOURCES.txt` & `html_generators-2.7.0/src/html_generators.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -33,12 +33,15 @@
 src/html_generators/__pycache__/_fragment.cpython-36.pyc
 src/html_generators/__pycache__/_join.cpython-36.pyc
 src/html_generators/__pycache__/_mark_safe.cpython-36.pyc
 src/html_generators/__pycache__/_standard_elements.cpython-36.pyc
 src/html_generators/__pycache__/_template.cpython-36.pyc
 src/html_generators/__pycache__/_utils.cpython-36.pyc
 src/html_generators/__pycache__/base.cpython-36.pyc
+src/html_generators/__pycache__/comment.cpython-36.pyc
 src/html_generators/__pycache__/django.cpython-36.pyc
 src/html_generators/__pycache__/document.cpython-36.pyc
 src/html_generators/__pycache__/elements.cpython-36.pyc
 src/html_generators/__pycache__/fragment.cpython-36.pyc
-src/html_generators/__pycache__/mark_safe.cpython-36.pyc
+src/html_generators/__pycache__/join.cpython-36.pyc
+src/html_generators/__pycache__/mark_safe.cpython-36.pyc
+src/html_generators/__pycache__/utils.cpython-36.pyc
```

### Comparing `html_generators-2.6.0/src/html_generators/django.py` & `html_generators-2.7.0/src/html_generators/django.py`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/_base.py` & `html_generators-2.7.0/src/html_generators/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from html import escape
 from typing import Any, Iterable, Iterator
 
+#: type alias; content that is intended to be passed to an HTMLGenerator
+#: see generate_child_html to understand how different types will be rendered
+Content = Any
+
 class SafeString(str):
 	'''
 	A str of HTML that plays nicely with other web frameworks.
 
 	These objects will _not_ be escaped when passed to:
 	- django templates
 	- django.utils.html.conditional_escape
@@ -57,15 +61,15 @@
 		Calling this multiple times _may_ produce inconsistent results.
 
 		The returned str is a SafeString, which won't be escaped when passed
 		to django templates or markupsafe.
 		'''
 		return SafeString(''.join(iter(self)))
 
-def generate_child_html(child: Any) -> Iterator[str]:
+def generate_child_html(child: Content) -> Iterator[str]:
 	'''
 	Generate a sequence of HTML strings from the given object.
 
 	The sequence of strings, as a whole, will be a balanced HTML fragment.
 
 	We can't really describe the behaviour of this function any more 
 	concisely than the code does, so just read the code.
@@ -107,10 +111,10 @@
 		for grandchild in i :
 			yield from generate_child_html(grandchild)
 		return
 
 	yield escape(str(child))
 
 
-def generate_html(children: Iterable[Any]) -> Iterator[str]:
+def generate_html(children: Iterable[Content]) -> Iterator[str]:
 	for child in children :
 		yield from generate_child_html(child)
```

### Comparing `html_generators-2.6.0/src/html_generators/_standard_elements.py` & `html_generators-2.7.0/src/html_generators/_standard_elements.py`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__init__.py` & `html_generators-2.7.0/src/html_generators/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 '''
 html_generators - functional html generation
 
 Note - all of our submodules (with the exception)
 '''
+from ._base import Content
 from ._document import Document  # noqa
 from ._element import Element  # noqa
 from ._standard_elements import *  # noqa
 from ._standard_elements import __all__ as _all_elements
 from ._comment import Comment  # noqa
 from ._format import format  # noqa
 from ._fragment import Fragment  # noqa
 from ._join import Join  # noqa
 from ._mark_safe import MarkSafe  # noqa
 from ._template import template # noqa
 from ._utils import classes, styles  # noqa
 
-# This is for pydoc support, not for "import *" support
+# This is for pydoc support, not for "import *" support (which we don't recommend)
 __all__ = [
+	'Content',
 	'Document',
 	'Element',
 	'Comment',
 	'Fragment',
 	'format',
 	'Join',
 	'MarkSafe',
```

### Comparing `html_generators-2.6.0/src/html_generators/_element.py` & `html_generators-2.7.0/src/html_generators/_element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Any
 from . import _utils as utils
-from ._base import HTMLGenerator, escape, generate_html, SafeString
+from ._base import Content, HTMLGenerator, escape, generate_html, SafeString
 from ._mark_safe import MarkSafe
 
 def open_tag(name, attrs):
 	yield '<'+name
 	for key, value in attrs.items() :
 		if value is False or value is None :
 			continue
@@ -46,15 +45,15 @@
 	*children:
 	- these are the child nodes (text and elements) of this element
 
 	**attrs:
 	- the HTML attributes of this element
 	'''
 	# TODO - document that attrs are OPTIONAL strings
-	def __init__(self, name_, *children: Any, **attrs: str):
+	def __init__(self, name_, *children: Content, **attrs: str):
 		self._name = name_
 		self._children = children
 		self._attrs = normalize_dict(attrs)
 
 	def __iter__(self):
 		yield from open_tag(self._name, self._attrs)
 		yield from generate_html(self._children)
```

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_template.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_template.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/django.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/django.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/mark_safe.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/comment.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-00000000: 330d 0d0a 78d5 ec5e 9d00 0000 e300 0000  3...x..^........
+00000000: 330d 0d0a f809 4262 db00 0000 e300 0000  3.....Bb........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 2000 0000 6400 6401 6c00 6d01 5a01  .s ...d.d.l.m.Z.
 00000030: 0100 4700 6402 6403 8400 6403 6501 8303  ..G.d.d...d.e...
 00000040: 5a02 6404 5300 2905 e901 0000 0029 01da  Z.d.S.)......)..
 00000050: 0d48 544d 4c47 656e 6572 6174 6f72 6300  .HTMLGeneratorc.
 00000060: 0000 0000 0000 0000 0000 0002 0000 0040  ...............@
 00000070: 0000 0073 1c00 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
 00000080: 6401 6402 8400 5a03 6403 6404 8400 5a04  d.d...Z.d.d...Z.
-00000090: 6405 5300 2906 da08 4d61 726b 5361 6665  d.S.)...MarkSafe
-000000a0: 6302 0000 0000 0000 0002 0000 0002 0000  c...............
-000000b0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
-000000c0: 6400 5300 2901 4e29 01da 0673 7472 696e  d.S.).N)...strin
-000000d0: 6729 02da 0473 656c 6672 0400 0000 a900  g)...selfr......
-000000e0: 7206 0000 00fa 422f 5573 6572 732f 616c  r.....B/Users/al
+00000090: 6405 5300 2906 da07 436f 6d6d 656e 7463  d.S.)...Commentc
+000000a0: 0200 0000 0000 0000 0200 0000 0200 0000  ................
+000000b0: 4300 0000 730a 0000 007c 017c 005f 0064  C...s....|.|._.d
+000000c0: 0053 0029 014e 2901 da07 636f 6e74 656e  .S.).N)...conten
+000000d0: 7429 02da 0473 656c 6672 0400 0000 a900  t)...selfr......
+000000e0: 7206 0000 00fa 502f 5573 6572 732f 616c  r.....P/Users/al
 000000f0: 6578 2f70 726f 6a65 6374 732f 7069 705f  ex/projects/pip_
 00000100: 7061 636b 6167 6573 2f68 746d 6c5f 6765  packages/html_ge
-00000110: 6e65 7261 746f 7273 2f73 7263 2f6d 6172  nerators/src/mar
-00000120: 6b5f 7361 6665 2e70 79da 085f 5f69 6e69  k_safe.py..__ini
-00000130: 745f 5f04 0000 0073 0200 0000 0001 7a11  t__....s......z.
-00000140: 4d61 726b 5361 6665 2e5f 5f69 6e69 745f  MarkSafe.__init_
-00000150: 5f63 0100 0000 0000 0000 0100 0000 0100  _c..............
-00000160: 0000 6300 0000 730c 0000 007c 006a 0056  ..c...s....|.j.V
-00000170: 0001 0064 0053 0029 014e 2901 7204 0000  ...d.S.).N).r...
-00000180: 0029 0172 0500 0000 7206 0000 0072 0600  .).r....r....r..
-00000190: 0000 7207 0000 00da 085f 5f69 7465 725f  ..r......__iter_
-000001a0: 5f07 0000 0073 0200 0000 0001 7a11 4d61  _....s......z.Ma
-000001b0: 726b 5361 6665 2e5f 5f69 7465 725f 5f4e  rkSafe.__iter__N
-000001c0: 2905 da08 5f5f 6e61 6d65 5f5f da0a 5f5f  )...__name__..__
-000001d0: 6d6f 6475 6c65 5f5f da0c 5f5f 7175 616c  module__..__qual
-000001e0: 6e61 6d65 5f5f 7208 0000 0072 0900 0000  name__r....r....
-000001f0: 7206 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
-00000200: 0700 0000 7203 0000 0003 0000 0073 0400  ....r........s..
-00000210: 0000 0801 0803 7203 0000 004e 2903 da04  ......r....N)...
-00000220: 6261 7365 7202 0000 0072 0300 0000 7206  baser....r....r.
-00000230: 0000 0072 0600 0000 7206 0000 0072 0700  ...r....r....r..
-00000240: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
-00000250: 7302 0000 000c 02                        s......
+00000110: 6e65 7261 746f 7273 2f73 7263 2f68 746d  nerators/src/htm
+00000120: 6c5f 6765 6e65 7261 746f 7273 2f63 6f6d  l_generators/com
+00000130: 6d65 6e74 2e70 79da 085f 5f69 6e69 745f  ment.py..__init_
+00000140: 5f04 0000 0073 0200 0000 0001 7a10 436f  _....s......z.Co
+00000150: 6d6d 656e 742e 5f5f 696e 6974 5f5f 6301  mment.__init__c.
+00000160: 0000 0000 0000 0001 0000 0001 0000 0063  ...............c
+00000170: 0000 0073 1800 0000 6401 5600 0100 7c00  ...s....d.V...|.
+00000180: 6a00 5600 0100 6402 5600 0100 6400 5300  j.V...d.V...d.S.
+00000190: 2903 4e7a 043c 212d 2d7a 032d 2d3e 2901  ).Nz.<!--z.-->).
+000001a0: 7204 0000 0029 0172 0500 0000 7206 0000  r....).r....r...
+000001b0: 0072 0600 0000 7207 0000 00da 085f 5f69  .r....r......__i
+000001c0: 7465 725f 5f07 0000 0073 0600 0000 0001  ter__....s......
+000001d0: 0601 0801 7a10 436f 6d6d 656e 742e 5f5f  ....z.Comment.__
+000001e0: 6974 6572 5f5f 4e29 05da 085f 5f6e 616d  iter__N)...__nam
+000001f0: 655f 5fda 0a5f 5f6d 6f64 756c 655f 5fda  e__..__module__.
+00000200: 0c5f 5f71 7561 6c6e 616d 655f 5f72 0800  .__qualname__r..
+00000210: 0000 7209 0000 0072 0600 0000 7206 0000  ..r....r....r...
+00000220: 0072 0600 0000 7207 0000 0072 0300 0000  .r....r....r....
+00000230: 0300 0000 7304 0000 0008 0108 0372 0300  ....s........r..
+00000240: 0000 4e29 03da 0462 6173 6572 0200 0000  ..N)...baser....
+00000250: 7203 0000 0072 0600 0000 7206 0000 0072  r....r....r....r
+00000260: 0600 0000 7207 0000 00da 083c 6d6f 6475  ....r......<modu
+00000270: 6c65 3e01 0000 0073 0200 0000 0c02       le>....s......
```

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_comment.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_comment.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_format.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_format.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,66 @@
-00000000: 330d 0d0a fb5b 3262 1803 0000 e300 0000  3....[2b........
+00000000: 330d 0d0a 585d 3262 1b03 0000 e300 0000  3...X]2b........
 00000010: 0000 0000 0000 0000 0002 0000 0040 0000  .............@..
 00000020: 0073 2400 0000 6400 6401 6c00 6d01 5a01  .s$...d.d.l.m.Z.
 00000030: 0100 6400 6402 6c02 6d03 5a03 0100 6403  ..d.d.l.m.Z...d.
 00000040: 6404 8400 5a04 6405 5300 2906 e901 0000  d...Z.d.S.).....
 00000050: 0029 01da 0846 7261 676d 656e 7429 01da  .)...Fragment)..
 00000060: 084d 6172 6b53 6166 6563 0000 0000 0000  .MarkSafec......
 00000070: 0000 0200 0000 0500 0000 4f00 0000 732a  ..........O...s*
 00000080: 0000 0074 0074 017c 0083 0183 017d 0074  ...t.t.|.....}.t
 00000090: 027c 006a 0366 0064 0164 0284 007c 016a  .|.j.f.d.d...|.j
 000000a0: 0483 0044 0083 018e 0183 0153 0029 0361  ...D.......S.).a
-000000b0: c801 0000 0a20 2020 2055 7365 6675 6c20  .....    Useful 
+000000b0: cb01 0000 0a20 2020 2055 7365 6675 6c20  .....    Useful 
 000000c0: 7768 656e 2069 6e6a 6563 7469 6e67 2068  when injecting h
 000000d0: 746d 6c20 696e 746f 2074 7261 6e73 6c61  tml into transla
 000000e0: 7461 626c 6520 7374 7269 6e67 732e 0a20  table strings.. 
 000000f0: 2020 2054 6865 2074 656d 706c 6174 6520     The template 
 00000100: 6765 7473 2028 636f 6e64 6974 696f 6e61  gets (conditiona
 00000110: 6c6c 7929 2065 7363 6170 6564 2c20 6173  lly) escaped, as
 00000120: 2064 6f20 616c 6c20 6f66 2074 6865 2063   do all of the c
 00000130: 6f6e 7465 7874 2076 616c 7565 732e 0a20  ontext values.. 
 00000140: 2020 2054 6869 7320 7761 792c 2079 6f75     This way, you
 00000150: 7220 7472 616e 736c 6174 6f72 2064 6f65  r translator doe
 00000160: 736e 2774 206e 6565 6420 746f 2062 6520  sn't need to be 
 00000170: 6874 6d6c 2d61 7761 7265 2e0a 2020 2020  html-aware..    
 00000180: 0a20 2020 2049 653a 0a20 2020 2068 2e66  .    Ie:.    h.f
-00000190: 6f72 6d61 7428 0a20 2020 2020 2020 2027  ormat(.        '
-000001a0: 506c 6561 7365 207b 6c69 6e6b 5f73 7461  Please {link_sta
-000001b0: 7274 7d63 6c69 636b 2068 6572 657b 6c69  rt}click here{li
-000001c0: 6e6b 5f65 6e64 7d2e 272c 200a 2020 2020  nk_end}.', .    
-000001d0: 2020 2020 6c69 6e6b 5f73 7461 7274 3d68      link_start=h
-000001e0: 2e41 2868 7265 663d 736f 6d65 5f70 6174  .A(href=some_pat
-000001f0: 6829 2e6f 7065 6e5f 7461 6728 292c 200a  h).open_tag(), .
-00000200: 2020 2020 2020 2020 6c69 6e6b 5f65 6e64          link_end
-00000210: 3d68 2e41 2829 2e63 6c6f 7365 5f74 6167  =h.A().close_tag
-00000220: 2829 0a20 2020 2029 0a0a 2020 2020 5769  ().    )..    Wi
-00000230: 6c6c 2074 6872 6f77 204b 6579 4572 726f  ll throw KeyErro
-00000240: 7220 6966 2074 6865 2074 656d 706c 6174  r if the templat
-00000250: 6520 7573 6573 2061 6e79 2070 6172 616d  e uses any param
-00000260: 7320 6e6f 7420 6769 7665 6e20 696e 2063  s not given in c
-00000270: 6f6e 7465 7874 2e0a 2020 2020 6301 0000  ontext..    c...
-00000280: 0000 0000 0003 0000 0005 0000 0053 0000  .............S..
-00000290: 0073 1e00 0000 6900 7c00 5d16 5c02 7d01  .s....i.|.].\.}.
-000002a0: 7d02 7400 7401 7c02 8301 8301 7c01 9302  }.t.t.|.....|...
-000002b0: 7104 5300 a900 2902 da03 7374 7272 0200  q.S...)...strr..
-000002c0: 0000 2903 da02 2e30 da01 6bda 0176 7204  ..)....0..k..vr.
-000002d0: 0000 0072 0400 0000 fa50 2f55 7365 7273  ...r.....P/Users
-000002e0: 2f61 6c65 782f 7072 6f6a 6563 7473 2f70  /alex/projects/p
-000002f0: 6970 5f70 6163 6b61 6765 732f 6874 6d6c  ip_packages/html
-00000300: 5f67 656e 6572 6174 6f72 732f 7372 632f  _generators/src/
-00000310: 6874 6d6c 5f67 656e 6572 6174 6f72 732f  html_generators/
-00000320: 5f66 6f72 6d61 742e 7079 fa0a 3c64 6963  _format.py..<dic
-00000330: 7463 6f6d 703e 1700 0000 7302 0000 0006  tcomp>....s.....
-00000340: 037a 1a66 6f72 6d61 742e 3c6c 6f63 616c  .z.format.<local
-00000350: 733e 2e3c 6469 6374 636f 6d70 3e29 0572  s>.<dictcomp>).r
-00000360: 0500 0000 7202 0000 0072 0300 0000 da06  ....r....r......
-00000370: 666f 726d 6174 da05 6974 656d 7329 02da  format..items)..
-00000380: 0874 656d 706c 6174 655a 0763 6f6e 7465  .templateZ.conte
-00000390: 7874 7204 0000 0072 0400 0000 7209 0000  xtr....r....r...
-000003a0: 0072 0b00 0000 0400 0000 7306 0000 0000  .r........s.....
-000003b0: 110c 020e 0372 0b00 0000 4e29 05da 095f  .....r....N)..._
-000003c0: 6672 6167 6d65 6e74 7202 0000 00da 0a5f  fragmentr......_
-000003d0: 6d61 726b 5f73 6166 6572 0300 0000 720b  mark_safer....r.
-000003e0: 0000 0072 0400 0000 7204 0000 0072 0400  ...r....r....r..
-000003f0: 0000 7209 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00000400: 3e01 0000 0073 0400 0000 0c01 0c02       >....s........
+00000190: 6f72 6d61 7428 0a20 2020 2020 2020 205f  ormat(.        _
+000001a0: 2827 506c 6561 7365 207b 6c69 6e6b 5f73  ('Please {link_s
+000001b0: 7461 7274 7d63 6c69 636b 2068 6572 657b  tart}click here{
+000001c0: 6c69 6e6b 5f65 6e64 7d2e 2729 2c20 0a20  link_end}.'), . 
+000001d0: 2020 2020 2020 206c 696e 6b5f 7374 6172         link_star
+000001e0: 743d 682e 4128 6872 6566 3d73 6f6d 655f  t=h.A(href=some_
+000001f0: 7061 7468 292e 6f70 656e 5f74 6167 2829  path).open_tag()
+00000200: 2c20 0a20 2020 2020 2020 206c 696e 6b5f  , .        link_
+00000210: 656e 643d 682e 4128 292e 636c 6f73 655f  end=h.A().close_
+00000220: 7461 6728 290a 2020 2020 290a 0a20 2020  tag().    )..   
+00000230: 2057 696c 6c20 7468 726f 7720 4b65 7945   Will throw KeyE
+00000240: 7272 6f72 2069 6620 7468 6520 7465 6d70  rror if the temp
+00000250: 6c61 7465 2075 7365 7320 616e 7920 7061  late uses any pa
+00000260: 7261 6d73 206e 6f74 2067 6976 656e 2069  rams not given i
+00000270: 6e20 636f 6e74 6578 742e 0a20 2020 2063  n context..    c
+00000280: 0100 0000 0000 0000 0300 0000 0500 0000  ................
+00000290: 5300 0000 731e 0000 0069 007c 005d 165c  S...s....i.|.].\
+000002a0: 027d 017d 0274 0074 017c 0283 0183 017c  .}.}.t.t.|.....|
+000002b0: 0193 0271 0453 00a9 0029 02da 0373 7472  ...q.S...)...str
+000002c0: 7202 0000 0029 03da 022e 30da 016b da01  r....)....0..k..
+000002d0: 7672 0400 0000 7204 0000 00fa 502f 5573  vr....r.....P/Us
+000002e0: 6572 732f 616c 6578 2f70 726f 6a65 6374  ers/alex/project
+000002f0: 732f 7069 705f 7061 636b 6167 6573 2f68  s/pip_packages/h
+00000300: 746d 6c5f 6765 6e65 7261 746f 7273 2f73  tml_generators/s
+00000310: 7263 2f68 746d 6c5f 6765 6e65 7261 746f  rc/html_generato
+00000320: 7273 2f5f 666f 726d 6174 2e70 79fa 0a3c  rs/_format.py..<
+00000330: 6469 6374 636f 6d70 3e17 0000 0073 0200  dictcomp>....s..
+00000340: 0000 0603 7a1a 666f 726d 6174 2e3c 6c6f  ....z.format.<lo
+00000350: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+00000360: 2905 7205 0000 0072 0200 0000 7203 0000  ).r....r....r...
+00000370: 00da 0666 6f72 6d61 74da 0569 7465 6d73  ...format..items
+00000380: 2902 da08 7465 6d70 6c61 7465 5a07 636f  )...templateZ.co
+00000390: 6e74 6578 7472 0400 0000 7204 0000 0072  ntextr....r....r
+000003a0: 0900 0000 720b 0000 0004 0000 0073 0600  ....r........s..
+000003b0: 0000 0011 0c02 0e03 720b 0000 004e 2905  ........r....N).
+000003c0: da09 5f66 7261 676d 656e 7472 0200 0000  .._fragmentr....
+000003d0: da0a 5f6d 6172 6b5f 7361 6665 7203 0000  .._mark_safer...
+000003e0: 0072 0b00 0000 7204 0000 0072 0400 0000  .r....r....r....
+000003f0: 7204 0000 0072 0900 0000 da08 3c6d 6f64  r....r......<mod
+00000400: 756c 653e 0100 0000 7304 0000 000c 010c  ule>....s.......
+00000410: 02                                       .
```

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_join.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_join.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_document.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_document.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/document.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/document.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-00000000: 330d 0d0a 78d5 ec5e e700 0000 e300 0000  3...x..^........
+00000000: 330d 0d0a f809 4262 e700 0000 e300 0000  3.....Bb........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 2400 0000 6400 6401 6c00 6d01 5a01  .s$...d.d.l.m.Z.
 00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
 00000040: 6501 8303 5a03 6404 5300 2905 e901 0000  e...Z.d.S.).....
 00000050: 0029 02da 0d48 544d 4c47 656e 6572 6174  .)...HTMLGenerat
 00000060: 6f72 da0e 7969 656c 645f 6368 696c 6472  or..yield_childr
 00000070: 656e 6300 0000 0000 0000 0000 0000 0002  enc.............
 00000080: 0000 0040 0000 0073 1c00 0000 6500 5a01  ...@...s....e.Z.
 00000090: 6400 5a02 6401 6402 8400 5a03 6403 6404  d.Z.d.d...Z.d.d.
 000000a0: 8400 5a04 6405 5300 2906 da08 446f 6375  ..Z.d.S.)...Docu
 000000b0: 6d65 6e74 6301 0000 0000 0000 0002 0000  mentc...........
 000000c0: 0002 0000 0047 0000 0073 0a00 0000 7c01  .....G...s....|.
 000000d0: 7c00 5f00 6400 5300 2901 4e29 01da 0863  |._.d.S.).N)...c
 000000e0: 6869 6c64 7265 6e29 02da 0473 656c 6672  hildren)...selfr
-000000f0: 0500 0000 a900 7207 0000 00fa 412f 5573  ......r.....A/Us
+000000f0: 0500 0000 a900 7207 0000 00fa 512f 5573  ......r.....Q/Us
 00000100: 6572 732f 616c 6578 2f70 726f 6a65 6374  ers/alex/project
 00000110: 732f 7069 705f 7061 636b 6167 6573 2f68  s/pip_packages/h
 00000120: 746d 6c5f 6765 6e65 7261 746f 7273 2f73  tml_generators/s
-00000130: 7263 2f64 6f63 756d 656e 742e 7079 da08  rc/document.py..
-00000140: 5f5f 696e 6974 5f5f 0400 0000 7302 0000  __init__....s...
-00000150: 0000 017a 1144 6f63 756d 656e 742e 5f5f  ...z.Document.__
-00000160: 696e 6974 5f5f 6301 0000 0000 0000 0001  init__c.........
-00000170: 0000 0002 0000 0063 0000 0073 1a00 0000  .......c...s....
-00000180: 6401 5600 0100 7400 7c00 6a01 8301 4500  d.V...t.|.j...E.
-00000190: 6400 4800 0100 6400 5300 2902 4e7a 103c  d.H...d.S.).Nz.<
-000001a0: 2144 4f43 5459 5045 2068 746d 6c3e 0a29  !DOCTYPE html>.)
-000001b0: 0272 0300 0000 7205 0000 0029 0172 0600  .r....r....).r..
-000001c0: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
-000001d0: 00da 085f 5f69 7465 725f 5f07 0000 0073  ...__iter__....s
-000001e0: 0400 0000 0001 0601 7a11 446f 6375 6d65  ........z.Docume
-000001f0: 6e74 2e5f 5f69 7465 725f 5f4e 2905 da08  nt.__iter__N)...
-00000200: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000210: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000220: 5f5f 7209 0000 0072 0a00 0000 7207 0000  __r....r....r...
-00000230: 0072 0700 0000 7207 0000 0072 0800 0000  .r....r....r....
-00000240: 7204 0000 0003 0000 0073 0400 0000 0801  r........s......
-00000250: 0803 7204 0000 004e 2904 da04 6261 7365  ..r....N)...base
-00000260: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
-00000270: 0700 0000 7207 0000 0072 0700 0000 7208  ....r....r....r.
-00000280: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000290: 0073 0200 0000 1002                      .s......
+00000130: 7263 2f68 746d 6c5f 6765 6e65 7261 746f  rc/html_generato
+00000140: 7273 2f64 6f63 756d 656e 742e 7079 da08  rs/document.py..
+00000150: 5f5f 696e 6974 5f5f 0400 0000 7302 0000  __init__....s...
+00000160: 0000 017a 1144 6f63 756d 656e 742e 5f5f  ...z.Document.__
+00000170: 696e 6974 5f5f 6301 0000 0000 0000 0001  init__c.........
+00000180: 0000 0002 0000 0063 0000 0073 1a00 0000  .......c...s....
+00000190: 6401 5600 0100 7400 7c00 6a01 8301 4500  d.V...t.|.j...E.
+000001a0: 6400 4800 0100 6400 5300 2902 4e7a 103c  d.H...d.S.).Nz.<
+000001b0: 2144 4f43 5459 5045 2068 746d 6c3e 0a29  !DOCTYPE html>.)
+000001c0: 0272 0300 0000 7205 0000 0029 0172 0600  .r....r....).r..
+000001d0: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
+000001e0: 00da 085f 5f69 7465 725f 5f07 0000 0073  ...__iter__....s
+000001f0: 0400 0000 0001 0601 7a11 446f 6375 6d65  ........z.Docume
+00000200: 6e74 2e5f 5f69 7465 725f 5f4e 2905 da08  nt.__iter__N)...
+00000210: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000220: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+00000230: 5f5f 7209 0000 0072 0a00 0000 7207 0000  __r....r....r...
+00000240: 0072 0700 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000250: 7204 0000 0003 0000 0073 0400 0000 0801  r........s......
+00000260: 0803 7204 0000 004e 2904 da04 6261 7365  ..r....N)...base
+00000270: 7202 0000 0072 0300 0000 7204 0000 0072  r....r....r....r
+00000280: 0700 0000 7207 0000 0072 0700 0000 7208  ....r....r....r.
+00000290: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+000002a0: 0073 0200 0000 1002                      .s......
```

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_fragment.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_fragment.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_mark_safe.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_mark_safe.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_utils.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_standard_elements.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_standard_elements.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_element.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_element.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/_base.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/_base.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/__pycache__/fragment.cpython-36.pyc` & `html_generators-2.7.0/src/html_generators/__pycache__/fragment.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 13% similar despite different names*

```diff
@@ -1,61 +1,61 @@
-00000000: 330d 0d0a f5ed ec5e 0902 0000 e300 0000  3......^........
+00000000: 330d 0d0a f809 4262 0c02 0000 e300 0000  3.....Bb........
 00000010: 0000 0000 0000 0000 0004 0000 0040 0000  .............@..
 00000020: 0073 2400 0000 6400 6401 6c00 6d01 5a01  .s$...d.d.l.m.Z.
 00000030: 6d02 5a02 0100 4700 6402 6403 8400 6403  m.Z...G.d.d...d.
 00000040: 6501 8303 5a03 6404 5300 2905 e901 0000  e...Z.d.S.).....
 00000050: 0029 02da 0d48 544d 4c47 656e 6572 6174  .)...HTMLGenerat
 00000060: 6f72 da0e 7969 656c 645f 6368 696c 6472  or..yield_childr
 00000070: 656e 6300 0000 0000 0000 0000 0000 0002  enc.............
 00000080: 0000 0040 0000 0073 2000 0000 6500 5a01  ...@...s ...e.Z.
 00000090: 6400 5a02 6401 5a03 6402 6403 8400 5a04  d.Z.d.Z.d.d...Z.
 000000a0: 6404 6405 8400 5a05 6406 5300 2907 da08  d.d...Z.d.S.)...
-000000b0: 4672 6167 6d65 6e74 6121 0100 000a 2020  Fragmenta!....  
+000000b0: 4672 6167 6d65 6e74 6124 0100 000a 2020  Fragmenta$....  
 000000c0: 2020 2020 2020 5265 7072 6573 656e 7473        Represents
 000000d0: 2061 2066 7261 676d 656e 7420 6f66 206f   a fragment of o
 000000e0: 6e65 206f 7220 6d6f 7265 2068 746d 6c20  ne or more html 
 000000f0: 6e6f 6465 732e 0a0a 2020 2020 2020 2020  nodes...        
 00000100: 4e6f 7465 2074 6861 7420 796f 7520 6765  Note that you ge
 00000110: 6e65 7261 6c6c 7920 776f 6e27 7420 6e65  nerally won't ne
 00000120: 6564 2074 6f20 7573 6520 7468 6973 2063  ed to use this c
 00000130: 6c61 7373 2c20 7369 6e63 6520 796f 7520  lass, since you 
 00000140: 6361 6e20 7061 7373 2069 7465 7261 626c  can pass iterabl
-00000150: 6573 2064 6972 6563 746c 7920 446f 6375  es directly Docu
-00000160: 6d65 6e74 2c20 456c 656d 656e 742c 2065  ment, Element, e
-00000170: 7463 2e20 0a0a 2020 2020 2020 2020 4966  tc. ..        If
-00000180: 2079 6f75 206e 6565 6420 746f 2072 656e   you need to ren
-00000190: 6465 7220 6d75 6c74 6970 6c65 206e 6f64  der multiple nod
-000001a0: 6573 2064 6972 6563 746c 7920 746f 2061  es directly to a
-000001b0: 2073 7472 696e 672c 2068 6f77 6576 6572   string, however
-000001c0: 2c20 796f 7520 6361 6e20 7573 6520 7468  , you can use th
-000001d0: 6973 2063 6c61 7373 2e0a 2020 2020 6301  is class..    c.
-000001e0: 0000 0000 0000 0002 0000 0002 0000 0047  ...............G
-000001f0: 0000 0073 0a00 0000 7c01 7c00 5f00 6400  ...s....|.|._.d.
-00000200: 5300 2901 4e29 01da 0863 6869 6c64 7265  S.).N)...childre
-00000210: 6e29 02da 0473 656c 6672 0500 0000 a900  n)...selfr......
-00000220: 7207 0000 00fa 512f 5573 6572 732f 616c  r.....Q/Users/al
-00000230: 6578 2f70 726f 6a65 6374 732f 7069 705f  ex/projects/pip_
-00000240: 7061 636b 6167 6573 2f68 746d 6c5f 6765  packages/html_ge
-00000250: 6e65 7261 746f 7273 2f73 7263 2f68 746d  nerators/src/htm
-00000260: 6c5f 6765 6e65 7261 746f 7273 2f66 7261  l_generators/fra
-00000270: 676d 656e 742e 7079 da08 5f5f 696e 6974  gment.py..__init
-00000280: 5f5f 0b00 0000 7302 0000 0000 017a 1146  __....s......z.F
-00000290: 7261 676d 656e 742e 5f5f 696e 6974 5f5f  ragment.__init__
-000002a0: 6301 0000 0000 0000 0001 0000 0002 0000  c...............
-000002b0: 0063 0000 0073 1400 0000 7400 7c00 6a01  .c...s....t.|.j.
-000002c0: 8301 4500 6400 4800 0100 6400 5300 2901  ..E.d.H...d.S.).
-000002d0: 4e29 0272 0300 0000 7205 0000 0029 0172  N).r....r....).r
-000002e0: 0600 0000 7207 0000 0072 0700 0000 7208  ....r....r....r.
-000002f0: 0000 00da 085f 5f69 7465 725f 5f0e 0000  .....__iter__...
-00000300: 0073 0200 0000 0001 7a11 4672 6167 6d65  .s......z.Fragme
-00000310: 6e74 2e5f 5f69 7465 725f 5f4e 2906 da08  nt.__iter__N)...
-00000320: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
-00000330: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
-00000340: 5f5f da07 5f5f 646f 635f 5f72 0900 0000  __..__doc__r....
-00000350: 720a 0000 0072 0700 0000 7207 0000 0072  r....r....r....r
-00000360: 0700 0000 7208 0000 0072 0400 0000 0300  ....r....r......
-00000370: 0000 7306 0000 0008 0704 0108 0372 0400  ..s..........r..
-00000380: 0000 4e29 04da 0462 6173 6572 0200 0000  ..N)...baser....
-00000390: 7203 0000 0072 0400 0000 7207 0000 0072  r....r....r....r
-000003a0: 0700 0000 7207 0000 0072 0800 0000 da08  ....r....r......
-000003b0: 3c6d 6f64 756c 653e 0100 0000 7302 0000  <module>....s...
-000003c0: 0010 02                                  ...
+00000150: 6573 2064 6972 6563 746c 7920 746f 2044  es directly to D
+00000160: 6f63 756d 656e 742c 2045 6c65 6d65 6e74  ocument, Element
+00000170: 2c20 6574 632e 200a 0a20 2020 2020 2020  , etc. ..       
+00000180: 2049 6620 796f 7520 6e65 6564 2074 6f20   If you need to 
+00000190: 7265 6e64 6572 206d 756c 7469 706c 6520  render multiple 
+000001a0: 6e6f 6465 7320 6469 7265 6374 6c79 2074  nodes directly t
+000001b0: 6f20 6120 7374 7269 6e67 2c20 686f 7765  o a string, howe
+000001c0: 7665 722c 2079 6f75 2063 616e 2075 7365  ver, you can use
+000001d0: 2074 6869 7320 636c 6173 732e 0a20 2020   this class..   
+000001e0: 2063 0100 0000 0000 0000 0200 0000 0200   c..............
+000001f0: 0000 4700 0000 730a 0000 007c 017c 005f  ..G...s....|.|._
+00000200: 0064 0053 0029 014e 2901 da08 6368 696c  .d.S.).N)...chil
+00000210: 6472 656e 2902 da04 7365 6c66 7205 0000  dren)...selfr...
+00000220: 00a9 0072 0700 0000 fa51 2f55 7365 7273  ...r.....Q/Users
+00000230: 2f61 6c65 782f 7072 6f6a 6563 7473 2f70  /alex/projects/p
+00000240: 6970 5f70 6163 6b61 6765 732f 6874 6d6c  ip_packages/html
+00000250: 5f67 656e 6572 6174 6f72 732f 7372 632f  _generators/src/
+00000260: 6874 6d6c 5f67 656e 6572 6174 6f72 732f  html_generators/
+00000270: 6672 6167 6d65 6e74 2e70 79da 085f 5f69  fragment.py..__i
+00000280: 6e69 745f 5f0b 0000 0073 0200 0000 0001  nit__....s......
+00000290: 7a11 4672 6167 6d65 6e74 2e5f 5f69 6e69  z.Fragment.__ini
+000002a0: 745f 5f63 0100 0000 0000 0000 0100 0000  t__c............
+000002b0: 0200 0000 6300 0000 7314 0000 0074 007c  ....c...s....t.|
+000002c0: 006a 0183 0145 0064 0048 0001 0064 0053  .j...E.d.H...d.S
+000002d0: 0029 014e 2902 7203 0000 0072 0500 0000  .).N).r....r....
+000002e0: 2901 7206 0000 0072 0700 0000 7207 0000  ).r....r....r...
+000002f0: 0072 0800 0000 da08 5f5f 6974 6572 5f5f  .r......__iter__
+00000300: 0e00 0000 7302 0000 0000 017a 1146 7261  ....s......z.Fra
+00000310: 676d 656e 742e 5f5f 6974 6572 5f5f 4e29  gment.__iter__N)
+00000320: 06da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
+00000330: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
+00000340: 616d 655f 5fda 075f 5f64 6f63 5f5f 7209  ame__..__doc__r.
+00000350: 0000 0072 0a00 0000 7207 0000 0072 0700  ...r....r....r..
+00000360: 0000 7207 0000 0072 0800 0000 7204 0000  ..r....r....r...
+00000370: 0003 0000 0073 0600 0000 0807 0401 0803  .....s..........
+00000380: 7204 0000 004e 2904 da04 6261 7365 7202  r....N)...baser.
+00000390: 0000 0072 0300 0000 7204 0000 0072 0700  ...r....r....r..
+000003a0: 0000 7207 0000 0072 0700 0000 7208 0000  ..r....r....r...
+000003b0: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
+000003c0: 0200 0000 1002                           ......
```

### Comparing `html_generators-2.6.0/src/html_generators/README.md` & `html_generators-2.7.0/src/html_generators/README.md`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/_template.py` & `html_generators-2.7.0/src/html_generators/_template.py`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/_document.py` & `html_generators-2.7.0/src/html_generators/_document.py`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/_format.py` & `html_generators-2.7.0/src/html_generators/_format.py`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/_join.py` & `html_generators-2.7.0/src/html_generators/_join.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from ._base import HTMLGenerator, generate_child_html
-from typing import Any, Iterable, Iterator
+from ._base import Content, HTMLGenerator, generate_child_html
+from typing import Iterable, Iterator
 
 class Join(HTMLGenerator):
 	'''
 	Similar to str.join
 	
 	The "joiner" and the "items" need not be strings (they can be other HTMLGenerators, numbers, etc.).
 
 	"items" MAY contain "empty values" (None, False) - 
 	they will NOT cause an extra joiner to be rendered.
 	'''
-	def __init__(self, joiner: Any, items: Iterable[Any]):
+	def __init__(self, joiner: Content, items: Iterable[Content]):
 		# Stringify joiner only once.
 		self._joiner = str(joiner)
 		self._items = items
 
 	def __iter__(self):
 		first_item = True
 		for child in self._items :
```

### Comparing `html_generators-2.6.0/src/html_generators/_fragment.py` & `html_generators-2.7.0/src/html_generators/_fragment.py`

 * *Files identical despite different names*

### Comparing `html_generators-2.6.0/src/html_generators/RELEASE_NOTES.md` & `html_generators-2.7.0/src/html_generators/RELEASE_NOTES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+## 2.7.0
+Added `Content` type alias
+
 ## 2.6.0
 Added h.format(), and h.Element.open_tag()/close_tag()
 
 ## 2.5.0
 template() now accepts '{x}' placeholders (for xgettext compatibility), as well as '{{x}}'.
 Placeholders not passed in context are left in place, rather than removed.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_l4vavfs4_/tmp7k58yyuf_TarContainer/0/47.md", line 95, column 7: CDATA terminal not found*

 * *File "/tmp/diffoscope_l4vavfs4_/tmp7k58yyuf_TarContainer/0/47.md", line 95, column 7: CDATA terminal not found*

```diff
@@ -1,25 +1,25 @@
-## 2.6.0 Added h.format(), and h.Element.open_tag()/close_tag() ## 2.5.0
-template() now accepts '{x}' placeholders (for xgettext compatibility), as well
-as '{{x}}'. Placeholders not passed in context are left in place, rather than
-removed. ## 2.4.0 Fix behaviour of `html_generators.django.date()`. Technically
-this is a breaking change, but it's definitely the way it should have worked to
-begin with. ## 2.3.0 Add `template` class ## 2.2.0 `Document` now accepts
-kwargs as shortcut for generating html element. ## 2.1.0 Added a few more
-django utilities. ### 2.0.2 Bug fix - name attribute on void elements ### 2.0.1
-Fix import bug in html_generators.django # 2.0.0 Breaking changes: - removed
-add_classes, add_styles - attribute normalization - trim only trailing
-underscores (be sure to replace "_class" with "class_") - all submodules (other
-than django) are private - look for imported submodules ## 1.7.0 Added cloning
-methods ## 1.6.0 `Join()` is now smarter - ignores None/False items, and items
-need not be HTMLGenerators ### 1.5.1 Fix bug introduced in 1.5.0 (void elements
-and raw text elements were not normalizing attribute names). ## 1.5.0 Added
-`classes` and `styles` utility functions, and `add_classes` and `add_styles`
-methods to `Element`. ### 1.4.1 Attributes which clash with python keywords can
-now be postfixed with an underscore, as well as prefixed (PEP 8 recommends
-postfix). ## 1.4 Added `h.Join(joiner, iterable)` ### 1.3.1 Ensure that
-attributes with value 0 are rendered (the only values skipped are False and
-None). ## 1.3.0 Add support for comments. ### 1.2.1 Ensure that children with
-value 0 (any number type) are rendered (the only values skipped are False and
-None). ## 1.2.0 Support "Safe Strings" from frameworks like Django. Children
-with `__html__()` method will not be escaped. ## 1.1.0 Do not escape contents
-of `
+## 2.7.0 Added `Content` type alias ## 2.6.0 Added h.format(), and
+h.Element.open_tag()/close_tag() ## 2.5.0 template() now accepts '{x}'
+placeholders (for xgettext compatibility), as well as '{{x}}'. Placeholders not
+passed in context are left in place, rather than removed. ## 2.4.0 Fix
+behaviour of `html_generators.django.date()`. Technically this is a breaking
+change, but it's definitely the way it should have worked to begin with. ##
+2.3.0 Add `template` class ## 2.2.0 `Document` now accepts kwargs as shortcut
+for generating html element. ## 2.1.0 Added a few more django utilities. ###
+2.0.2 Bug fix - name attribute on void elements ### 2.0.1 Fix import bug in
+html_generators.django # 2.0.0 Breaking changes: - removed add_classes,
+add_styles - attribute normalization - trim only trailing underscores (be sure
+to replace "_class" with "class_") - all submodules (other than django) are
+private - look for imported submodules ## 1.7.0 Added cloning methods ## 1.6.0
+`Join()` is now smarter - ignores None/False items, and items need not be
+HTMLGenerators ### 1.5.1 Fix bug introduced in 1.5.0 (void elements and raw
+text elements were not normalizing attribute names). ## 1.5.0 Added `classes`
+and `styles` utility functions, and `add_classes` and `add_styles` methods to
+`Element`. ### 1.4.1 Attributes which clash with python keywords can now be
+postfixed with an underscore, as well as prefixed (PEP 8 recommends postfix).
+## 1.4 Added `h.Join(joiner, iterable)` ### 1.3.1 Ensure that attributes with
+value 0 are rendered (the only values skipped are False and None). ## 1.3.0 Add
+support for comments. ### 1.2.1 Ensure that children with value 0 (any number
+type) are rendered (the only values skipped are False and None). ## 1.2.0
+Support "Safe Strings" from frameworks like Django. Children with `__html__()`
+method will not be escaped. ## 1.1.0 Do not escape contents of `
```

