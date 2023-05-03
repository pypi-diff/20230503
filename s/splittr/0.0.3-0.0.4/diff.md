# Comparing `tmp/splittr-0.0.3.tar.gz` & `tmp/splittr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splittr-0.0.3.tar", last modified: Mon May  1 22:47:57 2023, max compression
+gzip compressed data, was "splittr-0.0.4.tar", last modified: Wed May  3 20:43:33 2023, max compression
```

## Comparing `splittr-0.0.3.tar` & `splittr-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:47:57.956873 splittr-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-01 22:47:45.000000 splittr-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 22:47:57.956873 splittr-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-01 22:47:45.000000 splittr-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 22:47:57.956873 splittr-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3291 2023-05-01 22:47:45.000000 splittr-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:47:57.956873 splittr-0.0.3/splittr/
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-01 22:47:45.000000 splittr-0.0.3/splittr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 22:47:57.956873 splittr-0.0.3/splittr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 22:47:57.000000 splittr-0.0.3/splittr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-01 22:47:57.000000 splittr-0.0.3/splittr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 22:47:57.000000 splittr-0.0.3/splittr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-01 22:47:57.000000 splittr-0.0.3/splittr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:43:33.798086 splittr-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-03 20:43:23.000000 splittr-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 20:43:33.798086 splittr-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-03 20:43:23.000000 splittr-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:43:33.798086 splittr-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3291 2023-05-03 20:43:23.000000 splittr-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:43:33.798086 splittr-0.0.4/splittr/
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-05-03 20:43:23.000000 splittr-0.0.4/splittr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:43:33.798086 splittr-0.0.4/splittr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-03 20:43:33.000000 splittr-0.0.4/splittr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-03 20:43:33.000000 splittr-0.0.4/splittr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:43:33.000000 splittr-0.0.4/splittr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 20:43:33.000000 splittr-0.0.4/splittr.egg-info/top_level.txt
```

### Comparing `splittr-0.0.3/LICENSE` & `splittr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `splittr-0.0.3/setup.py` & `splittr-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

### Comparing `splittr-0.0.3/splittr/__init__.py` & `splittr-0.0.4/splittr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,34 +67,38 @@
 	parser.add_argument("--split", help="Split the file up", action="store_true",default=False)
 	parser.add_argument("--join", help="Recreate the file", action="store_true",default=False)
 	parser.add_argument("--template", help="Create a copy of this file specific to a large file", action="store_true",default=False)
 	return parser.parse_args()
 
 def splitt(foil):
 	hash(foil);split(foil)
+
 def joinn(foil):
 	join(foil);verify(foil)
 
+def template(workingfoil):
+	with open(__file__, "r") as reader:
+		with open(workingfoil + ".py", "w+") as writer:
+			for line in reader.readlines():
+				line = line.rstrip()
+				if "workingfoil = argz.file[0]" in line:
+					line = line.replace("argz.file[0]", "\""+workingfoil+"\"")
+				writer.write(line+"\n")
+
 def main(foil:str,splitfile:bool=False, joinfile:bool=False):
 	if splitfile:
 		splitt(foil)
 	elif joinfile:
 		joinn(foil)
 
 if __name__ == '__main__':
 	argz = arguments();workingfoil = argz.file[0]
 	if argz.template:
-		with open(__file__, "r") as reader:
-			with open(workingfoil + ".py", "w+") as writer:
-				for line in reader.readlines():
-					line = line.rstrip()
-					if "workingfoil = argz.file[0]" in line:
-						line = line.replace("argz.file[0]", "\""+workingfoil+"\"")
-					writer.write(line+"\n")
+		template(workingfoil)
 		print(workingfoil + ".py")
 	else:
 		if argz.split and argz.join:
 			print("Cannot use both both split and join")
 		elif not os.path.exists(argz.file[0]):
 			print("The file {file} does not exist".format(file=argz.file[0]))
 		else:
-			main(workingfoil, splitfile=argz.split, joinfile=argz.join)
+			main(workingfoil, splitfile=argz.split, joinfile=argz.join)
```

