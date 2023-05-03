# Comparing `tmp/purgelogs-0.2.1.tar.gz` & `tmp/purgelogs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "purgelogs-0.2.1.tar", last modified: Thu Apr 13 07:29:48 2023, max compression
+gzip compressed data, was "purgelogs-0.2.3.tar", last modified: Wed May  3 10:35:06 2023, max compression
```

## Comparing `purgelogs-0.2.1.tar` & `purgelogs-0.2.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:29:48.113049 purgelogs-0.2.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-13 07:28:31.000000 purgelogs-0.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-13 07:29:48.112049 purgelogs-0.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       37 2023-04-13 07:28:31.000000 purgelogs-0.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-13 07:29:48.112049 purgelogs-0.2.1/purgelogs.egg-info/
--rw-r--r--   0 root         (0) root         (0)       75 2023-04-13 07:29:47.000000 purgelogs-0.2.1/purgelogs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      207 2023-04-13 07:29:48.000000 purgelogs-0.2.1/purgelogs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-13 07:29:47.000000 purgelogs-0.2.1/purgelogs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-04-13 07:29:47.000000 purgelogs-0.2.1/purgelogs.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-13 07:29:47.000000 purgelogs-0.2.1/purgelogs.egg-info/top_level.txt
--rwxr-xr-x   0 root         (0) root         (0)     4644 2023-04-13 07:28:32.000000 purgelogs-0.2.1/purgelogs.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-13 07:29:48.113049 purgelogs-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      772 2023-04-13 07:28:32.000000 purgelogs-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:35:06.969640 purgelogs-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-03 10:33:45.000000 purgelogs-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-03 10:35:06.969640 purgelogs-0.2.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-03 10:33:45.000000 purgelogs-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 10:35:06.969640 purgelogs-0.2.3/purgelogs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       75 2023-05-03 10:35:06.000000 purgelogs-0.2.3/purgelogs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      207 2023-05-03 10:35:06.000000 purgelogs-0.2.3/purgelogs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 10:35:06.000000 purgelogs-0.2.3/purgelogs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-03 10:35:06.000000 purgelogs-0.2.3/purgelogs.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-03 10:35:06.000000 purgelogs-0.2.3/purgelogs.egg-info/top_level.txt
+-rwxr-xr-x   0 root         (0) root         (0)     4648 2023-05-03 10:33:45.000000 purgelogs-0.2.3/purgelogs.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 10:35:06.969640 purgelogs-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      772 2023-05-03 10:33:45.000000 purgelogs-0.2.3/setup.py
```

### Comparing `purgelogs-0.2.1/LICENSE` & `purgelogs-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `purgelogs-0.2.1/purgelogs.py` & `purgelogs-0.2.3/purgelogs.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,21 +106,21 @@
         level=logging.DEBUG if debug else logging.INFO)
     return logging.getLogger()
 
 def main() -> None:
     """The script entrypoint"""
     args = usage(sys.argv[1:])
     root = check_dir_path(args.log_path_dir)
-    calculated_time = datetime.now() - timedelta(days=args.retention_days)
     log = setup_logging(args.debug)
     if not root:
         log.error("The provided log path dir does not exists")
         exit(1)
     while True:
         logging.info("Starting cleaning-up log dir...")
+        calculated_time = datetime.now() - timedelta(days=args.retention_days)
         search_and_destroy(log, calculated_time, args.dry_run, root)
         if not args.loop:
             break
         logging.info("Cleanup done! Sleeping %s..." % args.loop)
         time.sleep(args.loop)
 
 if __name__ == "__main__":
```

### Comparing `purgelogs-0.2.1/setup.py` & `purgelogs-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 # License for the specific language governing permissions and limitations
 # under the License.
 
 from setuptools import setup
 
 setup(
     name='purgelogs',
-    version='0.2.1',
+    version='0.2.3',
     py_modules=['purgelogs'],
     entry_points = {
         'console_scripts': ['purgelogs=purgelogs:main']
     }
 )
```

