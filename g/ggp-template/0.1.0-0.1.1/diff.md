# Comparing `tmp/ggp_template-0.1.0.tar.gz` & `tmp/ggp_template-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ggp_template-0.1.0.tar", last modified: Wed May  3 04:03:08 2023, max compression
+gzip compressed data, was "ggp_template-0.1.1.tar", last modified: Wed May  3 04:12:08 2023, max compression
```

## Comparing `ggp_template-0.1.0.tar` & `ggp_template-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 04:03:08.193465 ggp_template-0.1.0/
--rw-rw-rw-   0        0        0     1094 2023-05-02 20:29:31.000000 ggp_template-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     3232 2023-05-03 04:03:08.190459 ggp_template-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2677 2023-05-02 19:23:13.000000 ggp_template-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 04:03:08.158002 ggp_template-0.1.0/ggp/
--rw-rw-rw-   0        0        0        0 2023-05-02 19:58:45.000000 ggp_template-0.1.0/ggp/__init__.py
--rw-rw-rw-   0        0        0     1977 2023-05-02 21:47:33.000000 ggp_template-0.1.0/ggp/make.py
--rw-rw-rw-   0        0        0      637 2023-05-02 21:48:54.000000 ggp_template-0.1.0/ggp/new.py
-drwxrwxrwx   0        0        0        0 2023-05-03 04:03:08.174224 ggp_template-0.1.0/ggp/templates/
--rw-rw-rw-   0        0        0     2404 2023-05-02 19:59:54.000000 ggp_template-0.1.0/ggp/templates/sample.html
--rw-rw-rw-   0        0        0     1354 2023-05-02 20:00:31.000000 ggp_template-0.1.0/ggp/templates/sample.js
-drwxrwxrwx   0        0        0        0 2023-05-03 04:03:08.190459 ggp_template-0.1.0/ggp_template.egg-info/
--rw-rw-rw-   0        0        0     3232 2023-05-03 04:03:08.000000 ggp_template-0.1.0/ggp_template.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-03 04:03:08.000000 ggp_template-0.1.0/ggp_template.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 04:03:08.000000 ggp_template-0.1.0/ggp_template.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-03 04:03:08.000000 ggp_template-0.1.0/ggp_template.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      709 2023-05-03 04:02:20.000000 ggp_template-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 04:03:08.193465 ggp_template-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 04:12:08.403733 ggp_template-0.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-05-02 20:29:31.000000 ggp_template-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2979 2023-05-03 04:12:08.403733 ggp_template-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2424 2023-05-03 04:10:59.000000 ggp_template-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 04:12:08.387509 ggp_template-0.1.1/ggp/
+-rw-rw-rw-   0        0        0        0 2023-05-02 19:58:45.000000 ggp_template-0.1.1/ggp/__init__.py
+-rw-rw-rw-   0        0        0     1973 2023-05-03 04:06:12.000000 ggp_template-0.1.1/ggp/make.py
+-rw-rw-rw-   0        0        0      637 2023-05-02 21:48:54.000000 ggp_template-0.1.1/ggp/new.py
+drwxrwxrwx   0        0        0        0 2023-05-03 04:12:08.391723 ggp_template-0.1.1/ggp/templates/
+-rw-rw-rw-   0        0        0     2404 2023-05-02 19:59:54.000000 ggp_template-0.1.1/ggp/templates/sample.html
+-rw-rw-rw-   0        0        0     1354 2023-05-02 20:00:31.000000 ggp_template-0.1.1/ggp/templates/sample.js
+drwxrwxrwx   0        0        0        0 2023-05-03 04:12:08.403733 ggp_template-0.1.1/ggp_template.egg-info/
+-rw-rw-rw-   0        0        0     2979 2023-05-03 04:12:08.000000 ggp_template-0.1.1/ggp_template.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-03 04:12:08.000000 ggp_template-0.1.1/ggp_template.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 04:12:08.000000 ggp_template-0.1.1/ggp_template.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-03 04:12:08.000000 ggp_template-0.1.1/ggp_template.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      709 2023-05-03 04:11:49.000000 ggp_template-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 04:12:08.403733 ggp_template-0.1.1/setup.cfg
```

### Comparing `ggp_template-0.1.0/LICENSE` & `ggp_template-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ggp_template-0.1.0/PKG-INFO` & `ggp_template-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggp_template
-Version: 0.1.0
+Version: 0.1.1
 Summary: Creates and compiles GGP js/html projects
 Author-email: Praneeth Kolichala <praneeth.kolichala@gmail.com>
 Project-URL: Homepage, https://github.com/prakol16/ggp_template
 Project-URL: Bug Tracker, https://github.com/prakol16/ggp_template/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,73 +12,71 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Toolchain for writing General Game Players
 
 This simple script allows you to build
 and organize sophisticated general game playing (GGP)
-projects. Currently, players are defined by a single `html` file,
+projects. Currently, players are defined by a single `.html` file,
 which means that projects are either confined to a single file
 or require a lot of tedious, error-prone manual copy-and-paste if functionality
 is spread across different files.
 
 This script allows you to define *only* the functionality
 for the player that you are creating, avoiding all the boilerplate
-and copying and pasting. It also allows you to manage slightly larger projects
+and copying and pasting. It also allows you to manage larger projects
 by generating an `html` file from a template and (potentially multiple)
-given javascript files.
+javascript files.
 
 ## Setup
+Make sure you have python and pip installed. Then run the following
+in a terminal:
 
-Just clone the repository and optionally add it to your `PYTHONPATH`.
-This has been tested on Python 3.10.5 (no dependencies), but it is
-simple enough that it should work with essentially any version
-of Python 3
+```
+pip install ggp-template
+```
 
 ## Usage
 
 To create a new player from the sample template, run
 
 ```
-python ggp_template.py new myplayer.js
+python -m ggp.new new myplayer.js
 ```
 
 To build an HTML file from a player, run
 
 ```
-python ggp_template.py make myplayer.js --out=out.html --ident=your_identifier
+python -m ggp.make myplayer.js --ident=your_identifier
 ```
 
 You can build multiple javascript files by simply passing multiple
 arguments (no dependency resolution is done; the scripts are added
 to the HTML file in the order they are passed in):
 
 ```
-python ggp_template.py make lib.js myplayer.js --out=out.html --ident=your_identifier
+python ggp.make lib.js myplayer.js --ident=your_identifier
 ```
 
 ## Options
 
 The `make` subcommand takes the following options:
   - `template` The template HTML file to use (defaults to [sample.html](http://ggp.stanford.edu/gamemaster/gameplayers/sample.html))        
   - `ident` The identifier for your player
   - `strategy` The strategy name that is displayed on the page
   - `title` The title for the page (defaults to the strategy and identifier)
   - `out` The html file to write to (defaults to stdout)
 
-While javascript files are convereted to `data:text,` (hence URI encoded),
-none of the other options are escaped. Therefore,
+While javascript files are converted to `data:text,` (hence URI encoded),
+none of the other parameters are escaped. Therefore,
 if the `title` contains valid HTML, it will simply be inserted into the HTML
 file without any extra escaping.
 
 ## Recommendations
 
-Add this repository to your PYTHONPATH so that you can
-access the file from anywhere.
-
 Most editors will allow you to set up a custom build
 command. In vscode, for example, you can create a `tasks.json`
 file in the project directory and set this to be the default
 build task as described [here](https://code.visualstudio.com/docs/editor/tasks).
 
 If you want more sophisticated tooling, such as automatic dependency resolution
 or compiling from e.g. Typescript, use `webpack`.
```

### Comparing `ggp_template-0.1.0/README.md` & `ggp_template-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,70 +1,68 @@
 # Toolchain for writing General Game Players
 
 This simple script allows you to build
 and organize sophisticated general game playing (GGP)
-projects. Currently, players are defined by a single `html` file,
+projects. Currently, players are defined by a single `.html` file,
 which means that projects are either confined to a single file
 or require a lot of tedious, error-prone manual copy-and-paste if functionality
 is spread across different files.
 
 This script allows you to define *only* the functionality
 for the player that you are creating, avoiding all the boilerplate
-and copying and pasting. It also allows you to manage slightly larger projects
+and copying and pasting. It also allows you to manage larger projects
 by generating an `html` file from a template and (potentially multiple)
-given javascript files.
+javascript files.
 
 ## Setup
+Make sure you have python and pip installed. Then run the following
+in a terminal:
 
-Just clone the repository and optionally add it to your `PYTHONPATH`.
-This has been tested on Python 3.10.5 (no dependencies), but it is
-simple enough that it should work with essentially any version
-of Python 3
+```
+pip install ggp-template
+```
 
 ## Usage
 
 To create a new player from the sample template, run
 
 ```
-python ggp_template.py new myplayer.js
+python -m ggp.new new myplayer.js
 ```
 
 To build an HTML file from a player, run
 
 ```
-python ggp_template.py make myplayer.js --out=out.html --ident=your_identifier
+python -m ggp.make myplayer.js --ident=your_identifier
 ```
 
 You can build multiple javascript files by simply passing multiple
 arguments (no dependency resolution is done; the scripts are added
 to the HTML file in the order they are passed in):
 
 ```
-python ggp_template.py make lib.js myplayer.js --out=out.html --ident=your_identifier
+python ggp.make lib.js myplayer.js --ident=your_identifier
 ```
 
 ## Options
 
 The `make` subcommand takes the following options:
   - `template` The template HTML file to use (defaults to [sample.html](http://ggp.stanford.edu/gamemaster/gameplayers/sample.html))        
   - `ident` The identifier for your player
   - `strategy` The strategy name that is displayed on the page
   - `title` The title for the page (defaults to the strategy and identifier)
   - `out` The html file to write to (defaults to stdout)
 
-While javascript files are convereted to `data:text,` (hence URI encoded),
-none of the other options are escaped. Therefore,
+While javascript files are converted to `data:text,` (hence URI encoded),
+none of the other parameters are escaped. Therefore,
 if the `title` contains valid HTML, it will simply be inserted into the HTML
 file without any extra escaping.
 
 ## Recommendations
 
-Add this repository to your PYTHONPATH so that you can
-access the file from anywhere.
-
 Most editors will allow you to set up a custom build
 command. In vscode, for example, you can create a `tasks.json`
 file in the project directory and set this to be the default
 build task as described [here](https://code.visualstudio.com/docs/editor/tasks).
 
 If you want more sophisticated tooling, such as automatic dependency resolution
 or compiling from e.g. Typescript, use `webpack`.
```

### Comparing `ggp_template-0.1.0/ggp/make.py` & `ggp_template-0.1.1/ggp/make.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,14 @@
 
 if __name__ == "__main__":
     parser = ArgumentParser(
                     prog='ggp.make',
                     description='Automatically generate an HTML for your player given the javascript source')
     parser.add_argument('filename', nargs="+", type=FileType('r'))
     parser.add_argument('--template', help='The template HTML file to use (defaults to sample.html from '
-                                               'http://ggp.stanford.edu/gamemaster/gameplayers/sample.html)')
+                                           'http://ggp.stanford.edu/gamemaster/gameplayers/sample.html)')
     parser.add_argument('--ident', help='The identifier for your player', default='template')
     parser.add_argument('--strategy', help='The strategy name that is displayed on the page', default='secret')
     parser.add_argument('--title', help='The title for the page (defaults to the strategy and identifier)')
     parser.add_argument('--out', help='The html file to write to (defaults to out.html)',
                             type=FileType('w'), default='out.html')
     make(parser.parse_args())
```

### Comparing `ggp_template-0.1.0/ggp/new.py` & `ggp_template-0.1.1/ggp/new.py`

 * *Files identical despite different names*

### Comparing `ggp_template-0.1.0/ggp/templates/sample.html` & `ggp_template-0.1.1/ggp/templates/sample.html`

 * *Files identical despite different names*

### Comparing `ggp_template-0.1.0/ggp/templates/sample.js` & `ggp_template-0.1.1/ggp/templates/sample.js`

 * *Files identical despite different names*

### Comparing `ggp_template-0.1.0/ggp_template.egg-info/PKG-INFO` & `ggp_template-0.1.1/ggp_template.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggp-template
-Version: 0.1.0
+Version: 0.1.1
 Summary: Creates and compiles GGP js/html projects
 Author-email: Praneeth Kolichala <praneeth.kolichala@gmail.com>
 Project-URL: Homepage, https://github.com/prakol16/ggp_template
 Project-URL: Bug Tracker, https://github.com/prakol16/ggp_template/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,73 +12,71 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Toolchain for writing General Game Players
 
 This simple script allows you to build
 and organize sophisticated general game playing (GGP)
-projects. Currently, players are defined by a single `html` file,
+projects. Currently, players are defined by a single `.html` file,
 which means that projects are either confined to a single file
 or require a lot of tedious, error-prone manual copy-and-paste if functionality
 is spread across different files.
 
 This script allows you to define *only* the functionality
 for the player that you are creating, avoiding all the boilerplate
-and copying and pasting. It also allows you to manage slightly larger projects
+and copying and pasting. It also allows you to manage larger projects
 by generating an `html` file from a template and (potentially multiple)
-given javascript files.
+javascript files.
 
 ## Setup
+Make sure you have python and pip installed. Then run the following
+in a terminal:
 
-Just clone the repository and optionally add it to your `PYTHONPATH`.
-This has been tested on Python 3.10.5 (no dependencies), but it is
-simple enough that it should work with essentially any version
-of Python 3
+```
+pip install ggp-template
+```
 
 ## Usage
 
 To create a new player from the sample template, run
 
 ```
-python ggp_template.py new myplayer.js
+python -m ggp.new new myplayer.js
 ```
 
 To build an HTML file from a player, run
 
 ```
-python ggp_template.py make myplayer.js --out=out.html --ident=your_identifier
+python -m ggp.make myplayer.js --ident=your_identifier
 ```
 
 You can build multiple javascript files by simply passing multiple
 arguments (no dependency resolution is done; the scripts are added
 to the HTML file in the order they are passed in):
 
 ```
-python ggp_template.py make lib.js myplayer.js --out=out.html --ident=your_identifier
+python ggp.make lib.js myplayer.js --ident=your_identifier
 ```
 
 ## Options
 
 The `make` subcommand takes the following options:
   - `template` The template HTML file to use (defaults to [sample.html](http://ggp.stanford.edu/gamemaster/gameplayers/sample.html))        
   - `ident` The identifier for your player
   - `strategy` The strategy name that is displayed on the page
   - `title` The title for the page (defaults to the strategy and identifier)
   - `out` The html file to write to (defaults to stdout)
 
-While javascript files are convereted to `data:text,` (hence URI encoded),
-none of the other options are escaped. Therefore,
+While javascript files are converted to `data:text,` (hence URI encoded),
+none of the other parameters are escaped. Therefore,
 if the `title` contains valid HTML, it will simply be inserted into the HTML
 file without any extra escaping.
 
 ## Recommendations
 
-Add this repository to your PYTHONPATH so that you can
-access the file from anywhere.
-
 Most editors will allow you to set up a custom build
 command. In vscode, for example, you can create a `tasks.json`
 file in the project directory and set this to be the default
 build task as described [here](https://code.visualstudio.com/docs/editor/tasks).
 
 If you want more sophisticated tooling, such as automatic dependency resolution
 or compiling from e.g. Typescript, use `webpack`.
```

### Comparing `ggp_template-0.1.0/pyproject.toml` & `ggp_template-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ggp_template"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Praneeth Kolichala", email="praneeth.kolichala@gmail.com" },
 ]
 description = "Creates and compiles GGP js/html projects"
 readme = "README.md"
 requires-python = ">=3.4"
 classifiers = [
```

