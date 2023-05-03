# Comparing `tmp/snakesay-0.10.2.tar.gz` & `tmp/snakesay-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/fjl/pa-repos/snakesay/dist/.tmp-0ieewi_n/snakesay-0.10.2.tar", last modified: Wed May  3 13:06:39 2023, max compression
+gzip compressed data, was "snakesay-0.9.0.tar", max compression
```

## Comparing `snakesay-0.10.2.tar` & `snakesay-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,5 @@
-drwxr-xr-x   0 fjl       (1000) fjl       (1000)        0 2023-05-03 13:06:39.000000 snakesay-0.10.2/
--rw-r--r--   0 fjl       (1000) fjl       (1000)     1080 2022-03-25 16:44:18.000000 snakesay-0.10.2/LICENSE
--rw-r--r--   0 fjl       (1000) fjl       (1000)      777 2023-05-03 13:06:39.000000 snakesay-0.10.2/PKG-INFO
--rw-r--r--   0 fjl       (1000) fjl       (1000)      229 2022-10-21 13:39:01.000000 snakesay-0.10.2/README.md
--rw-r--r--   0 fjl       (1000) fjl       (1000)      673 2023-05-03 13:01:08.000000 snakesay-0.10.2/pyproject.toml
--rw-r--r--   0 fjl       (1000) fjl       (1000)       38 2023-05-03 13:06:39.000000 snakesay-0.10.2/setup.cfg
-drwxr-xr-x   0 fjl       (1000) fjl       (1000)        0 2023-05-03 13:06:39.000000 snakesay-0.10.2/snakesay/
--rw-r--r--   0 fjl       (1000) fjl       (1000)       39 2022-10-21 13:37:44.000000 snakesay-0.10.2/snakesay/__init__.py
--rwxr-xr-x   0 fjl       (1000) fjl       (1000)      989 2022-07-31 13:59:11.000000 snakesay-0.10.2/snakesay/snakesay.py
-drwxr-xr-x   0 fjl       (1000) fjl       (1000)        0 2023-05-03 13:06:39.000000 snakesay-0.10.2/snakesay.egg-info/
--rw-r--r--   0 fjl       (1000) fjl       (1000)      777 2023-05-03 13:06:39.000000 snakesay-0.10.2/snakesay.egg-info/PKG-INFO
--rw-r--r--   0 fjl       (1000) fjl       (1000)      260 2023-05-03 13:06:39.000000 snakesay-0.10.2/snakesay.egg-info/SOURCES.txt
--rw-r--r--   0 fjl       (1000) fjl       (1000)        1 2023-05-03 13:06:39.000000 snakesay-0.10.2/snakesay.egg-info/dependency_links.txt
--rw-r--r--   0 fjl       (1000) fjl       (1000)       52 2023-05-03 13:06:39.000000 snakesay-0.10.2/snakesay.egg-info/entry_points.txt
--rw-r--r--   0 fjl       (1000) fjl       (1000)        9 2023-05-03 13:06:39.000000 snakesay-0.10.2/snakesay.egg-info/top_level.txt
-drwxr-xr-x   0 fjl       (1000) fjl       (1000)        0 2023-05-03 13:06:39.000000 snakesay-0.10.2/tests/
--rw-r--r--   0 fjl       (1000) fjl       (1000)      836 2022-10-21 13:37:44.000000 snakesay-0.10.2/tests/test_snakesay.py
+-rw-r--r--   0        0        0     1080 2022-03-25 16:44:18.112825 snakesay-0.9.0/LICENSE
+-rw-r--r--   0        0        0      378 2022-03-25 17:32:12.908281 snakesay-0.9.0/pyproject.toml
+-rwxr-xr-x   0        0        0      964 2022-03-25 17:46:40.001567 snakesay-0.9.0/snakesay/snakesay.py
+-rw-r--r--   0        0        0      528 2022-03-25 20:31:46.087105 snakesay-0.9.0/setup.py
+-rw-r--r--   0        0        0      490 2022-03-25 20:31:46.087231 snakesay-0.9.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `snakesay-0.10.2/LICENSE` & `snakesay-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakesay-0.10.2/snakesay/snakesay.py` & `snakesay-0.9.0/snakesay/snakesay.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,13 +34,9 @@
 
 def rewrap(speech: str) -> Tuple[List[str], int]:
     lines = textwrap.wrap(speech)
     width = max(len(l) for l in lines) if lines else 0
     return [line.ljust(width) for line in lines], width
 
 
-def main():
-    print(snakesay(*sys.argv[1:]))
-
-
 if __name__ == '__main__':
-    main()
+    print(snakesay(*sys.argv[1:]))
```

