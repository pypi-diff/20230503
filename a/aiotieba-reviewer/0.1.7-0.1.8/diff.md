# Comparing `tmp/aiotieba-reviewer-0.1.7.tar.gz` & `tmp/aiotieba-reviewer-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotieba-reviewer-0.1.7.tar", last modified: Fri Mar 31 01:55:55 2023, max compression
+gzip compressed data, was "aiotieba-reviewer-0.1.8.tar", last modified: Wed May  3 00:53:43 2023, max compression
```

## Comparing `aiotieba-reviewer-0.1.7.tar` & `aiotieba-reviewer-0.1.8.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.197488 aiotieba-reviewer-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-03-31 01:55:55.197488 aiotieba-reviewer-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.193488 aiotieba-reviewer-0.1.7/aiotieba_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29699 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/imgproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/perf_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/punish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.193488 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.193488 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comment/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comment/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comment/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.197488 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comments/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comments/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comments/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comments/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.197488 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/post/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/post/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/post/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.197488 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/posts/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/posts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/posts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/posts/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/posts/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.197488 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/thread/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/thread/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/thread/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.197488 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/threads/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/threads/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/threads/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/threads/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/user_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.193488 aiotieba-reviewer-0.1.7/aiotieba_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-03-31 01:55:55.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-31 01:55:55.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 01:55:55.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-03-31 01:55:55.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-31 01:55:55.000000 aiotieba-reviewer-0.1.7/aiotieba_reviewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 01:55:55.197488 aiotieba-reviewer-0.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/examples/cmd_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/examples/reviewer_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-31 01:55:33.000000 aiotieba-reviewer-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 01:55:55.201488 aiotieba-reviewer-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.238401 aiotieba-reviewer-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.230401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30093 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/imgproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/perf_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/punish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/user_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    24229 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/examples/cmd_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/examples/reviewer_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:53:43.238401 aiotieba-reviewer-0.1.8/setup.cfg
```

### Comparing `aiotieba-reviewer-0.1.7/LICENSE` & `aiotieba-reviewer-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/PKG-INFO` & `aiotieba-reviewer-0.1.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotieba-reviewer
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reviewer Framework based on aiotieba
 Author-email: Starry-OvO <starry.qvq@gmail.com>
 Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
 Project-URL: Documentation, https://review.aiotieba.cc/
 Keywords: baidu,tieba
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -43,29 +43,26 @@
 
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.03.31更新*
+*2023.05.02更新*
 
 |      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
 | :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 4,836,017  |     1,226,279      |    2,421     |   76,813   |
-|     孙笑川     | 3,795,206  |      876,143       |    6,906     |  225,394   |
-|    原神内鬼    |  577,566   |      663,758       |    1,284     |   45,731   |
-|    lol半价     | 2,056,707  |       77,129       |     384      |   12,415   |
-|    新孙笑川    |  678,479   |       51,621       |     461      |   18,739   |
-|      宫漫      | 1,551,287  |       24,153       |      86      |   1,217    |
-|      嘉然      |   60,779   |       20,470       |     132      |   1,763    |
-|      向晚      |   31,011   |       16,102       |      67      |    799     |
-|     vtuber     |  223,694   |       13,227       |     107      |   1,310    |
-|      贝拉      |   21,907   |       10,186       |      38      |    821     |
-|      乃琳      |   17,404   |       3,925        |      17      |    260     |
-| vtuber自由讨论 |   17,255   |       1,335        |      2       |     25     |
+|    抗压背锅    | 4,942,121  |      994,512       |    2,120     |   77,218   |
+|     孙笑川     | 3,990,805  |      738,723       |    5,832     |  260,811   |
+|    原神内鬼    |  589,938   |      492,120       |    1,122     |   36,464   |
+|      憨批      |   12,647   |      123,632       |    3,807     |   65,148   |
+|    lol半价     | 2,076,007  |       63,190       |     202      |   9,368    |
+|    天堂鸡汤    |  352,324   |       17,699       |     141      |   4,993    |
+|     vtuber     |  224,264   |       14,078       |     112      |   1,731    |
+|      嘉然      |   61,138   |       11,869       |      84      |   1,139    |
+| vtuber自由讨论 |   17,221   |       1,181        |      1       |     15     |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.1.7/README.md` & `aiotieba-reviewer-0.1.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,29 +21,26 @@
 
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.03.31更新*
+*2023.05.02更新*
 
 |      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
 | :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 4,836,017  |     1,226,279      |    2,421     |   76,813   |
-|     孙笑川     | 3,795,206  |      876,143       |    6,906     |  225,394   |
-|    原神内鬼    |  577,566   |      663,758       |    1,284     |   45,731   |
-|    lol半价     | 2,056,707  |       77,129       |     384      |   12,415   |
-|    新孙笑川    |  678,479   |       51,621       |     461      |   18,739   |
-|      宫漫      | 1,551,287  |       24,153       |      86      |   1,217    |
-|      嘉然      |   60,779   |       20,470       |     132      |   1,763    |
-|      向晚      |   31,011   |       16,102       |      67      |    799     |
-|     vtuber     |  223,694   |       13,227       |     107      |   1,310    |
-|      贝拉      |   21,907   |       10,186       |      38      |    821     |
-|      乃琳      |   17,404   |       3,925        |      17      |    260     |
-| vtuber自由讨论 |   17,255   |       1,335        |      2       |     25     |
+|    抗压背锅    | 4,942,121  |      994,512       |    2,120     |   77,218   |
+|     孙笑川     | 3,990,805  |      738,723       |    5,832     |  260,811   |
+|    原神内鬼    |  589,938   |      492,120       |    1,122     |   36,464   |
+|      憨批      |   12,647   |      123,632       |    3,807     |   65,148   |
+|    lol半价     | 2,076,007  |       63,190       |     202      |   9,368    |
+|    天堂鸡汤    |  352,324   |       17,699       |     141      |   4,993    |
+|     vtuber     |  224,264   |       14,078       |     112      |   1,731    |
+|      嘉然      |   61,138   |       11,869       |      84      |   1,139    |
+| vtuber自由讨论 |   17,221   |       1,181        |      1       |     15     |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/client.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/database.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -641,29 +641,35 @@
                     return True
 
         except aiomysql.Error as err:
             LOG().warning(f"{err}. forum={self.fname} img_hash={img_hash}")
             raise
 
     @exec_handler_MySQL(_create_table_imghash, False)
-    async def del_imghash(self, img_hash: int) -> bool:
+    async def del_imghash(self, img_hash: int, *, hamming_dist: int = 0) -> bool:
         """
         从表imghash_{fname}中删除img_hash
 
         Args:
             img_hash (int): 图像的ahash
+            hamming_dist (int): 匹配的最大海明距离 默认为0 即要求图像ahash完全一致
 
         Returns:
             bool: True成功 False失败
         """
 
         try:
             async with self._pool.acquire() as conn:
                 async with conn.cursor() as cursor:
-                    await cursor.execute(f"DELETE FROM `imghash_{self.fname}` WHERE `img_hash`={img_hash}")
+                    if hamming_dist > 0:
+                        await cursor.execute(
+                            f"DELETE FROM `imghash_{self.fname}` WHERE BIT_COUNT(`img_hash`^{img_hash})<={hamming_dist}"
+                        )
+                    else:
+                        await cursor.execute(f"DELETE FROM `imghash_{self.fname}` WHERE `img_hash`={img_hash}")
 
                     LOG().info(f"Succeeded. forum={self.fname} img_hash={img_hash}")
                     return True
 
         except aiomysql.Error as err:
             LOG().warning(f"{err}. forum={self.fname} img_hash={img_hash}")
             raise
```

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/executor.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     global delete_list
     delete_list = _delete_list
 
 
 TypePunishExecutor = Callable[[Punish], Awaitable[Optional[Punish]]]
 
 
-async def default_punish_executor(punish: Punish) -> Optional[Punish]:
+async def group_punish_executor(punish: Punish) -> Optional[Punish]:
     if day := punish.day:
         client = await get_client()
         await client.block(get_fname(), punish.obj.user.portrait, day=day, reason=punish.note)
 
     op = punish.op
     if op == Ops.NORMAL:
         return
@@ -105,14 +105,52 @@
         return
     if op == Ops.DEBUG:
         LOG().info(
             f"Debug {punish.obj.__class__.__name__}. obj={punish.obj} user={punish.obj.user!r} note={punish.note}"
         )
         return
     if op == Ops.HIDE:
+        LOG().info(
+            f"Hide {punish.obj.__class__.__name__}. text={punish.obj.text} user={punish.obj.user!r} note={punish.note}"
+        )
+        client = await get_client()
+        await client.hide_thread(get_fname(), punish.obj.tid)
+        return
+    if op & Ops.PARENT == Ops.PARENT:
+        op &= ~Ops.PARENT
+        punish.op = op
+        return punish
+    if op & Ops.GRANDPARENT == Ops.GRANDPARENT:
+        op &= ~Ops.GRANDPARENT
+        op &= Ops.PARENT
+        punish.op = op
+        return punish
+
+
+async def default_punish_executor(punish: Punish) -> Optional[Punish]:
+    if day := punish.day:
+        client = await get_client()
+        await client.block(get_fname(), punish.obj.user.portrait, day=day, reason=punish.note)
+
+    op = punish.op
+    if op == Ops.NORMAL:
+        return
+    if op == Ops.DELETE:
+        LOG().info(
+            f"Del {punish.obj.__class__.__name__}. text={punish.obj.text} user={punish.obj.user!r} note={punish.note}"
+        )
+        client = await get_client()
+        await client.del_post(punish.obj.fid, punish.obj.pid)
+        return
+    if op == Ops.DEBUG:
+        LOG().info(
+            f"Debug {punish.obj.__class__.__name__}. obj={punish.obj} user={punish.obj.user!r} note={punish.note}"
+        )
+        return
+    if op == Ops.HIDE:
         LOG().info(
             f"Hide {punish.obj.__class__.__name__}. text={punish.obj.text} user={punish.obj.user!r} note={punish.note}"
         )
         client = await get_client()
         await client.hide_thread(get_fname(), punish.obj.tid)
         return
     if op & Ops.PARENT == Ops.PARENT:
```

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/imgproc.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/imgproc.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/perf_stat.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/perf_stat.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/punish.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/punish.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comment/checker.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comment/runner.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comments/producer.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/comments/runner.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/entry.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/entry.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,15 +54,17 @@
     post.set_checker(True, False)(post.checker.ori_checker)
     comment.set_checker(True, False)(comment.checker.ori_checker)
 
     for pn in pn_gen:
         await threads.runner.runner(client._fname, pn)
 
 
-async def run_multi_pn_with_time_threshold(time_threshold: int, pn_gen: Generator[int, None, None] = range(4, 0, -1)) -> None:
+async def run_multi_pn_with_time_threshold(
+    time_threshold: int, pn_gen: Generator[int, None, None] = range(4, 0, -1)
+) -> None:
     """
     清洗多个页码中的较新内容 将禁用历史状态缓存以允许重复检查
 
     Args:
         time_threshold (int): 创建时间晚于该值的内容都会被检查. 10位时间戳 以秒为单位.
         pn_gen (Generator[int, None, None], optional): 页码生成器. Defaults to range(4, 0, -1).
     """
@@ -103,40 +105,43 @@
 
         return post_list
 
     for pn in pn_gen:
         await threads.runner.runner(client._fname, pn)
 
 
-async def test(tid: int, pid: int = 0, is_floor: bool = False) -> Optional[Punish]:
+async def test(tid: int, pid: int = 0, is_comment: bool = False) -> Optional[Punish]:
     client = await get_client()
     if not pid:
         posts = await client.get_posts(tid, rn=0)
         thread.checker.set_checker(True, False)(thread.checker.ori_checker)
         return await thread.checker.checker(posts.thread)
     else:
-        if not is_floor:
-            comments = await client.get_comments(tid, pid, is_floor=False)
+        if not is_comment:
+            comments = await client.get_comments(tid, pid, is_comment=False)
             post.checker.set_checker(True, False)(post.checker.ori_checker)
             return await post.checker.checker(comments.post)
         else:
-            comments = await client.get_comments(tid, pid, is_floor=True)
+            comments = await client.get_comments(tid, pid, is_comment=True)
             for _comment in comments:
                 if _comment.pid == pid:
                     comment.checker.set_checker(True, False)(comment.checker.ori_checker)
                     return await comment.checker.checker(_comment)
             LOG().warning("Comment not exist")
 
 
 @contextlib.contextmanager
-def no_test() -> None:
+def no_test(use_del_list=False) -> None:
     """
     取消测试模式以实际执行删封
+
+    Args:
+        use_del_list (bool): 是否使用更节省带宽但延迟更高的批量删除模式. Defaults to False.
     """
 
-    executor.punish_executor = executor.default_punish_executor
+    executor.punish_executor = executor.group_punish_executor if use_del_list else executor.default_punish_executor
     thread.runner.set_thread_runner(False)(thread.runner.ori_runner)
     threads.runner.set_threads_runner(False)(threads.runner.ori_runner)
     yield
     executor.punish_executor = executor.default_punish_executor_test
     thread.runner.set_thread_runner(True)(thread.runner.ori_runner)
     threads.runner.set_threads_runner(True)(threads.runner.ori_runner)
```

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/post/checker.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/post/runner.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/posts/producer.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/posts/runner.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/thread/runner.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/threads/producer.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/threads/runner.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer/reviewer/user_checker.py` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/user_checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer.egg-info/PKG-INFO` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotieba-reviewer
-Version: 0.1.7
+Version: 0.1.8
 Summary: Reviewer Framework based on aiotieba
 Author-email: Starry-OvO <starry.qvq@gmail.com>
 Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
 Project-URL: Documentation, https://review.aiotieba.cc/
 Keywords: baidu,tieba
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -43,29 +43,26 @@
 
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.03.31更新*
+*2023.05.02更新*
 
 |      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
 | :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 4,836,017  |     1,226,279      |    2,421     |   76,813   |
-|     孙笑川     | 3,795,206  |      876,143       |    6,906     |  225,394   |
-|    原神内鬼    |  577,566   |      663,758       |    1,284     |   45,731   |
-|    lol半价     | 2,056,707  |       77,129       |     384      |   12,415   |
-|    新孙笑川    |  678,479   |       51,621       |     461      |   18,739   |
-|      宫漫      | 1,551,287  |       24,153       |      86      |   1,217    |
-|      嘉然      |   60,779   |       20,470       |     132      |   1,763    |
-|      向晚      |   31,011   |       16,102       |      67      |    799     |
-|     vtuber     |  223,694   |       13,227       |     107      |   1,310    |
-|      贝拉      |   21,907   |       10,186       |      38      |    821     |
-|      乃琳      |   17,404   |       3,925        |      17      |    260     |
-| vtuber自由讨论 |   17,255   |       1,335        |      2       |     25     |
+|    抗压背锅    | 4,942,121  |      994,512       |    2,120     |   77,218   |
+|     孙笑川     | 3,990,805  |      738,723       |    5,832     |  260,811   |
+|    原神内鬼    |  589,938   |      492,120       |    1,122     |   36,464   |
+|      憨批      |   12,647   |      123,632       |    3,807     |   65,148   |
+|    lol半价     | 2,076,007  |       63,190       |     202      |   9,368    |
+|    天堂鸡汤    |  352,324   |       17,699       |     141      |   4,993    |
+|     vtuber     |  224,264   |       14,078       |     112      |   1,731    |
+|      嘉然      |   61,138   |       11,869       |      84      |   1,139    |
+| vtuber自由讨论 |   17,221   |       1,181        |      1       |     15     |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.1.7/aiotieba_reviewer.egg-info/SOURCES.txt` & `aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/examples/cmd_handler.py` & `aiotieba-reviewer-0.1.8/examples/cmd_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -119,17 +119,17 @@
         self.__init_args()
         return True
 
     async def init_full(self) -> bool:
         if self._init_full_success:
             return True
 
-        if self.at.is_floor:
+        if self.at.is_comment:
             await asyncio.sleep(3.0)
-            comments = await self.admin.get_comments(self.tid, self.pid, is_floor=True)
+            comments = await self.admin.get_comments(self.tid, self.pid, is_comment=True)
             self.parent = comments.post
             for comment in comments:
                 if comment.pid == self.pid:
                     self.text = comment.text
 
         elif self.at.is_thread:
             await asyncio.sleep(3.0)
@@ -140,20 +140,22 @@
             self.parent = posts.thread
 
         else:
             await asyncio.sleep(2.0)
             posts = await self.admin.get_posts(self.tid, pn=8192, rn=20, sort=tb.enums.PostSortType.DESC)
             for post in posts:
                 if post.pid == self.pid:
-                    self.text = post.text
+                    self.text = post.contents.text
                     break
             posts = await self.admin.get_posts(self.tid, rn=0)
             self.parent = posts.thread
 
+        self.__init_args()
         self._init_full_success = True
+
         return True
 
     def __init_args(self) -> None:
         self._args = []
         self._cmd_type = ''
 
         text = re.sub(r'.*?@.*? ', '', self.text, count=1)
@@ -360,14 +362,16 @@
     @check_and_log(need_permission=2, need_arg_num=1)
     async def cmd_recover(self, ctx: Context) -> None:
         """
         recover指令
         恢复删帖
         """
 
+        await ctx.init_full()
+
         _id = ctx.args[0]
         _id = _id[_id.rfind('#') + 1 :]
         _id = int(_id)
 
         if _id < 1e11:
             success = await ctx.admin.recover_thread(ctx.fname, _id)
         else:
@@ -762,56 +766,14 @@
         """
 
         user = await self.__arg2user_info(ctx.args[0])
 
         if await ctx.admin.blacklist_del(ctx.fname, user.user_id):
             await ctx.admin.del_post(ctx.fname, ctx.pid)
 
-    @check_and_log(need_permission=2, need_arg_num=0)
-    async def cmd_water(self, ctx: Context) -> None:
-        """
-        water指令
-        将指令所在主题帖标记为无关水，并临时屏蔽
-        """
-
-        if await ctx.admin_db.add_tid(ctx.tid, tag=1) and await ctx.admin.hide_thread(ctx.fname, ctx.tid):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
-
-    @check_and_log(need_permission=2, need_arg_num=0)
-    async def cmd_unwater(self, ctx: Context) -> None:
-        """
-        unwater指令
-        清除指令所在主题帖的无关水标记，并立刻解除屏蔽
-        """
-
-        if await ctx.admin_db.del_tid(ctx.tid) and await ctx.admin.unhide_thread(ctx.fname, ctx.tid):
-            await ctx.admin.del_post(ctx.fname, ctx.pid)
-
-    @check_and_log(need_permission=3, need_arg_num=1)
-    async def cmd_water_restrict(self, ctx: Context) -> None:
-        """
-        water_restrict指令
-        控制当前吧的云审查脚本的无关水管控状态
-        """
-
-        if ctx.args[0] == "enter":
-            if await ctx.admin_db.add_tid(0, tag=1):
-                await ctx.admin.del_post(ctx.fname, ctx.pid)
-        elif ctx.args[0] == "exit":
-            if await ctx.admin_db.add_tid(0, tag=0):
-                await ctx.admin.del_post(ctx.fname, ctx.pid)
-            limit = 128
-            tids = await ctx.admin_db.get_tid_list(1, limit=limit)
-            while 1:
-                for tid in tids:
-                    if await ctx.admin.unhide_thread(ctx.fname, tid):
-                        await ctx.admin_db.add_tid(tid, tag=1)
-                if len(tids) != limit:
-                    break
-
     @check_and_log(need_permission=1, need_arg_num=0)
     async def cmd_ping(self, ctx: Context) -> None:
         """
         ping指令
         用于测试bot可用性的空指令
         """
```

### Comparing `aiotieba-reviewer-0.1.7/examples/reviewer_example.py` & `aiotieba-reviewer-0.1.8/examples/reviewer_example.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.7/pyproject.toml` & `aiotieba-reviewer-0.1.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Internet :: WWW/HTTP :: Session",
 ]
-dependencies = ["aiotieba[img,speedup]<4.0,>=3.3.0", "aiomysql<0.2,>=0.1.0"]
+dependencies = ["aiotieba[img,speedup]<4.0,>=3.4.0", "aiomysql<0.2,>=0.1.0"]
 dynamic = ["version"]
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [tool.setuptools.dynamic]
 version = { attr = "aiotieba_reviewer.__version__.__version__" }
```

