# Comparing `tmp/slacc-1.0.0.tar.gz` & `tmp/slacc-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slacc-1.0.0.tar", last modified: Tue May  2 23:46:53 2023, max compression
+gzip compressed data, was "slacc-1.0.1.tar", last modified: Wed May  3 17:11:34 2023, max compression
```

## Comparing `slacc-1.0.0.tar` & `slacc-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 lapo      (1000) lapo      (1000)        0 2023-05-02 23:46:53.682210 slacc-1.0.0/
--rw-r--r--   0 lapo      (1000) lapo      (1000)     1067 2023-03-24 18:05:26.000000 slacc-1.0.0/LICENSE
--rw-r--r--   0 lapo      (1000) lapo      (1000)       30 2023-05-02 22:17:16.000000 slacc-1.0.0/MANIFEST.in
--rw-rw-r--   0 lapo      (1000) lapo      (1000)     6973 2023-05-02 23:46:53.682210 slacc-1.0.0/PKG-INFO
--rw-rw-r--   0 lapo      (1000) lapo      (1000)     6529 2023-05-02 21:41:00.000000 slacc-1.0.0/README.md
--rw-rw-r--   0 lapo      (1000) lapo      (1000)     1155 2023-05-02 23:45:43.000000 slacc-1.0.0/pyproject.toml
--rw-rw-r--   0 lapo      (1000) lapo      (1000)       38 2023-05-02 23:46:53.682210 slacc-1.0.0/setup.cfg
-drwxrwxr-x   0 lapo      (1000) lapo      (1000)        0 2023-05-02 23:46:53.682210 slacc-1.0.0/src/
-drwxrwxr-x   0 lapo      (1000) lapo      (1000)        0 2023-05-02 23:46:53.682210 slacc-1.0.0/src/slacc/
--rw-rw-r--   0 lapo      (1000) lapo      (1000)       22 2023-05-02 23:45:43.000000 slacc-1.0.0/src/slacc/__init__.py
--rw-rw-r--   0 lapo      (1000) lapo      (1000)    11659 2023-05-02 23:42:10.000000 slacc-1.0.0/src/slacc/__main__.py
--rw-rw-r--   0 lapo      (1000) lapo      (1000)      976 2023-05-02 23:30:10.000000 slacc-1.0.0/src/slacc/config.json
-drwxrwxr-x   0 lapo      (1000) lapo      (1000)        0 2023-05-02 23:46:53.682210 slacc-1.0.0/src/slacc.egg-info/
--rw-rw-r--   0 lapo      (1000) lapo      (1000)     6973 2023-05-02 23:46:53.000000 slacc-1.0.0/src/slacc.egg-info/PKG-INFO
--rw-rw-r--   0 lapo      (1000) lapo      (1000)      310 2023-05-02 23:46:53.000000 slacc-1.0.0/src/slacc.egg-info/SOURCES.txt
--rw-rw-r--   0 lapo      (1000) lapo      (1000)        1 2023-05-02 23:46:53.000000 slacc-1.0.0/src/slacc.egg-info/dependency_links.txt
--rw-rw-r--   0 lapo      (1000) lapo      (1000)      122 2023-05-02 23:46:53.000000 slacc-1.0.0/src/slacc.egg-info/entry_points.txt
--rw-rw-r--   0 lapo      (1000) lapo      (1000)       37 2023-05-02 23:46:53.000000 slacc-1.0.0/src/slacc.egg-info/requires.txt
--rw-rw-r--   0 lapo      (1000) lapo      (1000)        6 2023-05-02 23:46:53.000000 slacc-1.0.0/src/slacc.egg-info/top_level.txt
+drwxrwxr-x   0 lapo      (1000) lapo      (1000)        0 2023-05-03 17:11:34.257342 slacc-1.0.1/
+-rw-r--r--   0 lapo      (1000) lapo      (1000)     1067 2023-03-24 18:05:26.000000 slacc-1.0.1/LICENSE
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)       30 2023-05-02 23:57:40.000000 slacc-1.0.1/MANIFEST.in
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)     8766 2023-05-03 17:11:34.257342 slacc-1.0.1/PKG-INFO
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)     8322 2023-05-03 17:02:05.000000 slacc-1.0.1/README.md
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)     1155 2023-05-03 17:10:10.000000 slacc-1.0.1/pyproject.toml
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)       38 2023-05-03 17:11:34.257342 slacc-1.0.1/setup.cfg
+drwxrwxr-x   0 lapo      (1000) lapo      (1000)        0 2023-05-03 17:11:34.257342 slacc-1.0.1/src/
+drwxrwxr-x   0 lapo      (1000) lapo      (1000)        0 2023-05-03 17:11:34.257342 slacc-1.0.1/src/slacc/
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)       22 2023-05-03 17:10:10.000000 slacc-1.0.1/src/slacc/__init__.py
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)    11659 2023-05-02 23:57:40.000000 slacc-1.0.1/src/slacc/__main__.py
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)      976 2023-05-02 23:57:40.000000 slacc-1.0.1/src/slacc/config.json
+drwxrwxr-x   0 lapo      (1000) lapo      (1000)        0 2023-05-03 17:11:34.257342 slacc-1.0.1/src/slacc.egg-info/
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)     8766 2023-05-03 17:11:34.000000 slacc-1.0.1/src/slacc.egg-info/PKG-INFO
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)      310 2023-05-03 17:11:34.000000 slacc-1.0.1/src/slacc.egg-info/SOURCES.txt
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)        1 2023-05-03 17:11:34.000000 slacc-1.0.1/src/slacc.egg-info/dependency_links.txt
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)      122 2023-05-03 17:11:34.000000 slacc-1.0.1/src/slacc.egg-info/entry_points.txt
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)       37 2023-05-03 17:11:34.000000 slacc-1.0.1/src/slacc.egg-info/requires.txt
+-rw-rw-r--   0 lapo      (1000) lapo      (1000)        6 2023-05-03 17:11:34.000000 slacc-1.0.1/src/slacc.egg-info/top_level.txt
```

### Comparing `slacc-1.0.0/LICENSE` & `slacc-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slacc-1.0.0/PKG-INFO` & `slacc-1.0.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,13 @@
-Metadata-Version: 2.1
-Name: slacc
-Version: 1.0.0
-Summary: Easily control SLURM from python on the VACC.
-Author-email: lfrati <lfrati.github@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/lfrati/slacc
-Keywords: slurm,hpc
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
+<p align="center">
+    <img width="250" alt="Logo" src="https://user-images.githubusercontent.com/3115640/235985755-b6473e9f-e997-46a4-ac5b-b1333ab35470.png">
+</p>
 
 # SLurm on vACC (slacc)
+> "Take it easy and let the VACC work for you." - the wise grad
 
 Isn't it fun to have a nice GPU in your computer and to experiment left and right? You just write some python scripts
 and then launch them on your machine, wait, repeat. Life is simple and beautiful.
 
 But then inevitably it happens. You want to launch more scripts, longer scripts, test different parameters... 
 
 So you have to go beg the SLURM gods to assist you. Evil bash scripts start popping up everywhere, requesting resources, launching jobs....
@@ -26,17 +16,46 @@
 
 ## Prerequisites
 
 - Python >=3.9
 
 That's it.
 
+## Installation
+### Step 1. Get the thing.
+```bash
+pip install slacc
+```
+>Note: as of May 2023 the `spack` software on the VACC doesn't like python 3.10, so it is suggested to install `slacc` in a 3.9 environment
+>If you are using `conda` (recommended) you can use grab an installer for 3.9 from the [miniconda](https://docs.conda.io/en/latest/miniconda.html) page
+>
+><img src="https://user-images.githubusercontent.com/3115640/235952021-489cc26a-d153-46be-89d4-3e3500ca1ac1.png" width="600"/>
+>
+>This will make your conda `base` environment use python 3.9
+>
+>Alternatively you can create an custom environment with `conda create -n <pick_a_name> python=3.9` and run `pip install slacc` in this new environment.
+
+### Step 2. Customize the thing.
+After installing `slacc` (it should be quick since there are no dependencies) run 
+```bash
+sconfig
+```
+This will copy the default `config.json` file that ships with `slacc`, to `$HOME/.config/slacc/config.json`.
+Feel free to customize it to your needs, or keep it as it is. The most important thing is to make sure that the conda environments declared in config.json
+```
+{ 
+  "dggpu":{ "env": "conda activate dgenv",
+            ...
+}
+```
+match the ones available on your system.
+
 # How does it work?
 
-This package provides 2 commands you can use in your CLI: `slaunch` and `sinteract`
+This package provides 2 main commands you can use in your CLI: `slaunch` and `sinteract` (plus `sconfig` to make a copy default configs)
 
 ## 1. Slurm LAUNCH (slaunch)
 
 This is a wrapper around SLURM's [sbatch](https://slurm.schedmd.com/sbatch.html) to make it way easier to launch python scripts asynchronously.
 
 Let's say that you wanted to run this locally:
 ```shell
@@ -193,14 +212,14 @@
       "mem": "8000"
     }
   }
 }
 ```
 A few default configurations are provided as part of the package [config.json](src/slacc/config.json).
 
-:warning: To customize the resources and environment names the launcher scripts look at (increasing priority):
-1. (LOW PRIO) [Defaults](src/slacc/config.json) provided by slacc 
-2. (MED PRIO) $HOME/.config/slacc/config.json (User)
-3. (MAX PRIO) Directory containing the job script. (e.g. when launching ~/scratch/agi_net/train.py looks for ~/scratch/agi_net/config.json)
+:warning: There are 3 places where slacc looks for configuration files. If the same resource is defined in multiple places, only the one with highest priority is considered:
+1. (LOW PRIO) [Defaults](src/slacc/config.json) provided by slacc (use this if you are happy with the defaults and don't want to change anything)
+2. (MED PRIO) $HOME/.config/slacc/config.json (use this if you want to create custom configurations that you are planning to re-use)
+3. (MAX PRIO) Directory containing the job script, e.g. when launching ~/scratch/agi_net/train.py looks for ~/scratch/agi_net/config.json (use this if you want each individual run to use a different configuration)
 
-So use $HOME/.config/slacc/config.json for user wide settings and the job's folders for fine grained settings.
+:hammer_and_wrench: Use `sconfig` to copy the default settings to $HOME/.config/slacc/config.json.
```

### Comparing `slacc-1.0.0/README.md` & `slacc-1.0.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,28 @@
+Metadata-Version: 2.1
+Name: slacc
+Version: 1.0.1
+Summary: Easily control SLURM from python on the VACC.
+Author-email: lfrati <lfrati.github@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/lfrati/slacc
+Keywords: slurm,hpc
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+<p align="center">
+    <img width="250" alt="Logo" src="https://user-images.githubusercontent.com/3115640/235985755-b6473e9f-e997-46a4-ac5b-b1333ab35470.png">
+</p>
+
 # SLurm on vACC (slacc)
+> "Take it easy and let the VACC work for you." - the wise grad
 
 Isn't it fun to have a nice GPU in your computer and to experiment left and right? You just write some python scripts
 and then launch them on your machine, wait, repeat. Life is simple and beautiful.
 
 But then inevitably it happens. You want to launch more scripts, longer scripts, test different parameters... 
 
 So you have to go beg the SLURM gods to assist you. Evil bash scripts start popping up everywhere, requesting resources, launching jobs....
@@ -11,17 +31,46 @@
 
 ## Prerequisites
 
 - Python >=3.9
 
 That's it.
 
+## Installation
+### Step 1. Get the thing.
+```bash
+pip install slacc
+```
+>Note: as of May 2023 the `spack` software on the VACC doesn't like python 3.10, so it is suggested to install `slacc` in a 3.9 environment
+>If you are using `conda` (recommended) you can use grab an installer for 3.9 from the [miniconda](https://docs.conda.io/en/latest/miniconda.html) page
+>
+><img src="https://user-images.githubusercontent.com/3115640/235952021-489cc26a-d153-46be-89d4-3e3500ca1ac1.png" width="600"/>
+>
+>This will make your conda `base` environment use python 3.9
+>
+>Alternatively you can create an custom environment with `conda create -n <pick_a_name> python=3.9` and run `pip install slacc` in this new environment.
+
+### Step 2. Customize the thing.
+After installing `slacc` (it should be quick since there are no dependencies) run 
+```bash
+sconfig
+```
+This will copy the default `config.json` file that ships with `slacc`, to `$HOME/.config/slacc/config.json`.
+Feel free to customize it to your needs, or keep it as it is. The most important thing is to make sure that the conda environments declared in config.json
+```
+{ 
+  "dggpu":{ "env": "conda activate dgenv",
+            ...
+}
+```
+match the ones available on your system.
+
 # How does it work?
 
-This package provides 2 commands you can use in your CLI: `slaunch` and `sinteract`
+This package provides 2 main commands you can use in your CLI: `slaunch` and `sinteract` (plus `sconfig` to make a copy default configs)
 
 ## 1. Slurm LAUNCH (slaunch)
 
 This is a wrapper around SLURM's [sbatch](https://slurm.schedmd.com/sbatch.html) to make it way easier to launch python scripts asynchronously.
 
 Let's say that you wanted to run this locally:
 ```shell
@@ -178,14 +227,14 @@
       "mem": "8000"
     }
   }
 }
 ```
 A few default configurations are provided as part of the package [config.json](src/slacc/config.json).
 
-:warning: To customize the resources and environment names the launcher scripts look at (increasing priority):
-1. (LOW PRIO) [Defaults](src/slacc/config.json) provided by slacc 
-2. (MED PRIO) $HOME/.config/slacc/config.json (User)
-3. (MAX PRIO) Directory containing the job script. (e.g. when launching ~/scratch/agi_net/train.py looks for ~/scratch/agi_net/config.json)
+:warning: There are 3 places where slacc looks for configuration files. If the same resource is defined in multiple places, only the one with highest priority is considered:
+1. (LOW PRIO) [Defaults](src/slacc/config.json) provided by slacc (use this if you are happy with the defaults and don't want to change anything)
+2. (MED PRIO) $HOME/.config/slacc/config.json (use this if you want to create custom configurations that you are planning to re-use)
+3. (MAX PRIO) Directory containing the job script, e.g. when launching ~/scratch/agi_net/train.py looks for ~/scratch/agi_net/config.json (use this if you want each individual run to use a different configuration)
 
-So use $HOME/.config/slacc/config.json for user wide settings and the job's folders for fine grained settings.
+:hammer_and_wrench: Use `sconfig` to copy the default settings to $HOME/.config/slacc/config.json.
```

### Comparing `slacc-1.0.0/pyproject.toml` & `slacc-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "slacc"
-version = "1.0.0"
+version = "1.0.1"
 description = "Easily control SLURM from python on the VACC."
 readme = "README.md"
 authors = [{ name = "lfrati", email = "lfrati.github@gmail.com" }]
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
@@ -25,15 +25,15 @@
     [project.optional-dependencies]
     dev = ["bumpver", "pip-tools", "build", "twine"]
 
     [project.urls]
     Homepage = "https://github.com/lfrati/slacc"
 
 [tool.bumpver]
-current_version = "1.0.0"
+current_version = "1.0.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `slacc-1.0.0/src/slacc/__main__.py` & `slacc-1.0.1/src/slacc/__main__.py`

 * *Files identical despite different names*

### Comparing `slacc-1.0.0/src/slacc/config.json` & `slacc-1.0.1/src/slacc/config.json`

 * *Files identical despite different names*

### Comparing `slacc-1.0.0/src/slacc.egg-info/PKG-INFO` & `slacc-1.0.1/src/slacc.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 Metadata-Version: 2.1
 Name: slacc
-Version: 1.0.0
+Version: 1.0.1
 Summary: Easily control SLURM from python on the VACC.
 Author-email: lfrati <lfrati.github@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lfrati/slacc
 Keywords: slurm,hpc
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
+<p align="center">
+    <img width="250" alt="Logo" src="https://user-images.githubusercontent.com/3115640/235985755-b6473e9f-e997-46a4-ac5b-b1333ab35470.png">
+</p>
+
 # SLurm on vACC (slacc)
+> "Take it easy and let the VACC work for you." - the wise grad
 
 Isn't it fun to have a nice GPU in your computer and to experiment left and right? You just write some python scripts
 and then launch them on your machine, wait, repeat. Life is simple and beautiful.
 
 But then inevitably it happens. You want to launch more scripts, longer scripts, test different parameters... 
 
 So you have to go beg the SLURM gods to assist you. Evil bash scripts start popping up everywhere, requesting resources, launching jobs....
@@ -26,17 +31,46 @@
 
 ## Prerequisites
 
 - Python >=3.9
 
 That's it.
 
+## Installation
+### Step 1. Get the thing.
+```bash
+pip install slacc
+```
+>Note: as of May 2023 the `spack` software on the VACC doesn't like python 3.10, so it is suggested to install `slacc` in a 3.9 environment
+>If you are using `conda` (recommended) you can use grab an installer for 3.9 from the [miniconda](https://docs.conda.io/en/latest/miniconda.html) page
+>
+><img src="https://user-images.githubusercontent.com/3115640/235952021-489cc26a-d153-46be-89d4-3e3500ca1ac1.png" width="600"/>
+>
+>This will make your conda `base` environment use python 3.9
+>
+>Alternatively you can create an custom environment with `conda create -n <pick_a_name> python=3.9` and run `pip install slacc` in this new environment.
+
+### Step 2. Customize the thing.
+After installing `slacc` (it should be quick since there are no dependencies) run 
+```bash
+sconfig
+```
+This will copy the default `config.json` file that ships with `slacc`, to `$HOME/.config/slacc/config.json`.
+Feel free to customize it to your needs, or keep it as it is. The most important thing is to make sure that the conda environments declared in config.json
+```
+{ 
+  "dggpu":{ "env": "conda activate dgenv",
+            ...
+}
+```
+match the ones available on your system.
+
 # How does it work?
 
-This package provides 2 commands you can use in your CLI: `slaunch` and `sinteract`
+This package provides 2 main commands you can use in your CLI: `slaunch` and `sinteract` (plus `sconfig` to make a copy default configs)
 
 ## 1. Slurm LAUNCH (slaunch)
 
 This is a wrapper around SLURM's [sbatch](https://slurm.schedmd.com/sbatch.html) to make it way easier to launch python scripts asynchronously.
 
 Let's say that you wanted to run this locally:
 ```shell
@@ -193,14 +227,14 @@
       "mem": "8000"
     }
   }
 }
 ```
 A few default configurations are provided as part of the package [config.json](src/slacc/config.json).
 
-:warning: To customize the resources and environment names the launcher scripts look at (increasing priority):
-1. (LOW PRIO) [Defaults](src/slacc/config.json) provided by slacc 
-2. (MED PRIO) $HOME/.config/slacc/config.json (User)
-3. (MAX PRIO) Directory containing the job script. (e.g. when launching ~/scratch/agi_net/train.py looks for ~/scratch/agi_net/config.json)
+:warning: There are 3 places where slacc looks for configuration files. If the same resource is defined in multiple places, only the one with highest priority is considered:
+1. (LOW PRIO) [Defaults](src/slacc/config.json) provided by slacc (use this if you are happy with the defaults and don't want to change anything)
+2. (MED PRIO) $HOME/.config/slacc/config.json (use this if you want to create custom configurations that you are planning to re-use)
+3. (MAX PRIO) Directory containing the job script, e.g. when launching ~/scratch/agi_net/train.py looks for ~/scratch/agi_net/config.json (use this if you want each individual run to use a different configuration)
 
-So use $HOME/.config/slacc/config.json for user wide settings and the job's folders for fine grained settings.
+:hammer_and_wrench: Use `sconfig` to copy the default settings to $HOME/.config/slacc/config.json.
```

