# Comparing `tmp/footsteps-0.1.7-py3-none-any.whl.zip` & `tmp/footsteps-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 6034 bytes, number of entries: 7
--rw-r--r--  2.0 unx     4482 b- defN 22-Aug-08 17:41 footsteps/__init__.py
--rw-r--r--  2.0 unx     1147 b- defN 21-Oct-17 15:01 footsteps/footsteps.py
--rw-r--r--  2.0 unx     1059 b- defN 22-Aug-08 17:49 footsteps-0.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     5079 b- defN 22-Aug-08 17:49 footsteps-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Aug-08 17:49 footsteps-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 22-Aug-08 17:49 footsteps-0.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      553 b- defN 22-Aug-08 17:49 footsteps-0.1.7.dist-info/RECORD
-7 files, 12422 bytes uncompressed, 5056 bytes compressed:  59.3%
+Zip file size: 5609 bytes, number of entries: 6
+-rw-rw-r--  2.0 unx     4556 b- defN 23-May-03 18:42 footsteps/__init__.py
+-rw-rw-r--  2.0 unx     1059 b- defN 23-May-03 18:49 footsteps-0.1.8.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     5612 b- defN 23-May-03 18:49 footsteps-0.1.8.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-03 18:49 footsteps-0.1.8.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-03 18:49 footsteps-0.1.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      474 b- defN 23-May-03 18:49 footsteps-0.1.8.dist-info/RECORD
+6 files, 11803 bytes uncompressed, 4751 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
 Filename: footsteps/__init__.py
 Comment: 
 
-Filename: footsteps/footsteps.py
+Filename: footsteps-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: footsteps-0.1.7.dist-info/LICENSE
+Filename: footsteps-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: footsteps-0.1.7.dist-info/METADATA
+Filename: footsteps-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: footsteps-0.1.7.dist-info/WHEEL
+Filename: footsteps-0.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: footsteps-0.1.7.dist-info/top_level.txt
-Comment: 
-
-Filename: footsteps-0.1.7.dist-info/RECORD
+Filename: footsteps-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## footsteps/__init__.py

```diff
@@ -84,21 +84,24 @@
         f.write("Python:\n")
         f.write(sys.executable + "\n")
         f.write("Git Hash:\n")
         git_hash = (
             subprocess.check_output(["git", "describe", "--always"]).strip().decode()
         )
         f.write(git_hash + "\n")
-        origin = (
-            subprocess.check_output(["git", "remote", "get-url", "origin"])
-            .strip()
-            .decode()
-        )
-        if "github" in origin:
-            f.write(origin + "/tree/" + git_hash + "\n")
+        try:
+            origin = (
+                subprocess.check_output(["git", "remote", "get-url", "origin"])
+                .strip()
+                .decode()
+            )
+            if "github" in origin:
+                f.write(origin + "/tree/" + git_hash + "\n")
+        except:
+            pass
         f.write("Uncommitted changes:\n")
         try:
             f.write(
                 subprocess.check_output(
                     ["git", "diff", "HEAD", "--", ":^/*.ipynb"],
                     stderr=subprocess.DEVNULL,
                 ).decode()
```

## Comparing `footsteps-0.1.7.dist-info/LICENSE` & `footsteps-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `footsteps-0.1.7.dist-info/METADATA` & `footsteps-0.1.8.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: footsteps
-Version: 0.1.7
+Version: 0.1.8
 Summary: a minimal experiment logging package
 Home-page: https://github.com/HastingsGreer/footsteps
 Author: Hastings Greer
 Author-email: footsteps@hgreer.com
 Project-URL: Bug Tracker, https://github.com/HastingsGreer/footsteps/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,21 +12,23 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [<img src="https://github.com/HastingsGreer/footsteps/actions/workflows/test.yml/badge.svg">](https://github.com/HastingsGreer/footsteps/actions) [<img src="https://img.shields.io/pypi/v/footsteps.svg?color=blue">](https://pypi.org/project/footsteps/)
 ## Footsteps
 
-A non-configurable experiment logging package.
+We're all heathens: left to our own devices, `torch.save(state_dict, "best-weights-no-aug-tuesday-deeper.trch")` is inevitable.
 
 Footsteps provides an output directory pre-filled with `info.txt` describing your code and the circumstances in which it is running, so that it takes minimal effort to keep track of what code generated what result, even if you are writing a five line throwaway script. Then, 3 years later when you are trying to understand how you generated that figure or trained that network, you have enough information to follow your footsteps and work out exactly what you did.
 
 By default, when your code asks footsteps for an output directory, the user is prompted for an experiment name. Much like git commit messages, this seems like it would be annoying, but I've found it to be worthwhile.
 
 ```bash
+[hastings@$Hastingss-Air ~/sample_project]$ pip install footsteps
+...
 [hastings@$Hastingss-Air ~/sample_project]$ cat sample_project.py
 import footsteps
 
 with open(footsteps.output_dir + "network_weights.csv", "w") as f:
     f.write("6, 9, 42")
 
 [hastings@$Hastingss-Air ~/sample_project]$ python sample_project.py
@@ -94,11 +96,11 @@
 
 Experiment reproduction is hard at two points in time: First, when doing an experiment, it is easy to lack the motivation to meticulously record what you are doing, including details such as package versions or code changes that you may not think are important. Second, when trying to reproduce an experiment, motivation is available in abundance, but the information needed may no longer exist.
 
 To solve this problem, footsteps is designed to require as little motivation as possible at experiment time, and to provide as much information as possible at reproduction time.
 
 ### Usage Details
 
-To use footsteps, just import the package. At runtime, this will prompt the user for a descriptive name to be assosciated with any artifacts generated by this iteration of your code. Then, it will create a directory using that name, dump information into "info.txt" in that directory including the current git hash, command and arguments, which python env is in use etc into that directory. Finally, the path to this directory is available as `footsteps.output_dir`, so that the rest of your code knows where to put any artifacts that it generates.
+To use footsteps, just import the package. At runtime, this will prompt the user for a descriptive name to be assosciated with any artifacts generated by this iteration of your code. Tab completion is available for the experiment name if you want to use a name parallel with previous names. Then, it will create a directory using that name, dump information into "info.txt" in that directory including the current git hash, command and arguments, which python env is in use etc into that directory. Versions of installed packages are dumped into the output directory in the file "package_versions.txt" using `pip list` (specifically `Popen([sys.executable, "-m", "pip", "list"])`), which correctly records versions of packages whether they are installed with conda or pip. Finally, the path to this directory is available as `footsteps.output_dir`, so that the rest of your code knows where to put any artifacts that it generates.
 
 In the event that a project using footsteps grows to the point where you want to configure or specialize footsteps, the recommended process is to copy footsteps/footsteps.py into your codebase, modify it to make any changes you need, and import that instead of this.
```

