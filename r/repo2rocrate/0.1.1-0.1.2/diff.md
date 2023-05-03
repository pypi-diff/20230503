# Comparing `tmp/repo2rocrate-0.1.1.tar.gz` & `tmp/repo2rocrate-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repo2rocrate-0.1.1.tar", last modified: Wed Jul 13 13:23:56 2022, max compression
+gzip compressed data, was "repo2rocrate-0.1.2.tar", last modified: Wed May  3 13:56:44 2023, max compression
```

## Comparing `repo2rocrate-0.1.1.tar` & `repo2rocrate-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 13:23:56.501803 repo2rocrate-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-07-13 13:23:56.501803 repo2rocrate-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 13:23:56.497803 repo2rocrate-0.1.1/repo2rocrate/
--rw-r--r--   0 runner    (1001) docker     (121)     1013 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/repo2rocrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2947 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/repo2rocrate/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4620 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/repo2rocrate/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     5506 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/repo2rocrate/galaxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     4925 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/repo2rocrate/nextflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/repo2rocrate/snakemake.py
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/repo2rocrate/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/repo2rocrate/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 13:23:56.501803 repo2rocrate-0.1.1/repo2rocrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2571 2022-07-13 13:23:56.000000 repo2rocrate-0.1.1/repo2rocrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      597 2022-07-13 13:23:56.000000 repo2rocrate-0.1.1/repo2rocrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-13 13:23:56.000000 repo2rocrate-0.1.1/repo2rocrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-07-13 13:23:56.000000 repo2rocrate-0.1.1/repo2rocrate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-07-13 13:23:56.000000 repo2rocrate-0.1.1/repo2rocrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-13 13:23:56.000000 repo2rocrate-0.1.1/repo2rocrate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-13 13:23:56.000000 repo2rocrate-0.1.1/repo2rocrate.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-07-13 13:23:56.501803 repo2rocrate-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1866 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 13:23:56.501803 repo2rocrate-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4475 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/test/test_galaxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     6018 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/test/test_nextflow.py
--rw-r--r--   0 runner    (1001) docker     (121)     4502 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/test/test_snakemake.py
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/test/test_top_level.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-07-13 13:23:53.000000 repo2rocrate-0.1.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:44.700750 repo2rocrate-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-03 13:56:44.700750 repo2rocrate-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:44.696750 repo2rocrate-0.1.2/repo2rocrate/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/repo2rocrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/repo2rocrate/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/repo2rocrate/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/repo2rocrate/galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/repo2rocrate/nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/repo2rocrate/snakemake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/repo2rocrate/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/repo2rocrate/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:44.696750 repo2rocrate-0.1.2/repo2rocrate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-05-03 13:56:44.000000 repo2rocrate-0.1.2/repo2rocrate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-03 13:56:44.000000 repo2rocrate-0.1.2/repo2rocrate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:56:44.000000 repo2rocrate-0.1.2/repo2rocrate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 13:56:44.000000 repo2rocrate-0.1.2/repo2rocrate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 13:56:44.000000 repo2rocrate-0.1.2/repo2rocrate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 13:56:44.000000 repo2rocrate-0.1.2/repo2rocrate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:56:44.000000 repo2rocrate-0.1.2/repo2rocrate.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-03 13:56:44.700750 repo2rocrate-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:56:44.700750 repo2rocrate-0.1.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4761 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/test/test_galaxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/test/test_nextflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/test/test_snakemake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/test/test_top_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-03 13:56:37.000000 repo2rocrate-0.1.2/test/test_utils.py
```

### Comparing `repo2rocrate-0.1.1/LICENSE` & `repo2rocrate-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/PKG-INFO` & `repo2rocrate-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo2rocrate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate RO-Crates from workflow repositories
 Home-page: https://github.com/crs4/repo2rocrate
 Author: Simone Leo
 Author-email: <simone.leo@crs4.it>
 License: Apache-2.0
 Platform: Linux
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 License-File: LICENSE
 
 # repo2rocrate
 
 Generate a [Workflow Testing RO-Crate](https://crs4.github.io/life_monitor/workflow_testing_ro_crate) from a "best-practices" workflow repository. In this context, "best-practices" means the set of guidelines, especially regarding repository structure and metadata, put together by the workflow language community. Here is the list of currently supported workflow languages, together with the community resources used as a reference:
 
 * Galaxy: [IWC's howto for adding workflows](https://github.com/galaxyproject/iwc/blob/main/workflows/README.md)
-* Nextflow: nf-core [guidelines](https://nf-co.re/contributing/guidelines) and [info on pipeline structure](https://nf-co.re/developers/adding_pipelines#nf-core-pipeline-structure) (and ultimately the template generated by `nf-core create`)
+* Nextflow: nf-core [guidelines](https://nf-co.re/docs/contributing/guidelines) and [info on pipeline structure](https://nf-co.re/developers/adding_pipelines#nf-core-pipeline-structure) (and ultimately the template generated by `nf-core create`)
 * Snakemake: [snakemake-workflows](https://github.com/snakemake-workflows/docs) guidelines, Snakemake [distribution and reproducibility docs](https://snakemake.readthedocs.io/en/stable/snakefiles/deployment.html)
 
 ## Installation
 
 ```
 pip install repo2rocrate
 ```
@@ -44,9 +44,7 @@
 ```
 git clone https://github.com/nf-core/rnaseq
 cd rnaseq/
 repo2rocrate
 ```
 
 The above commands add an `ro-crate-metadata.json` file to the repository directory. To generate an RO-Crate in a separate directory, use the `-o` option. Run `repo2rocrate --help` to get a description of all available options.
-
-
```

### Comparing `repo2rocrate-0.1.1/README.md` & `repo2rocrate-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # repo2rocrate
 
 Generate a [Workflow Testing RO-Crate](https://crs4.github.io/life_monitor/workflow_testing_ro_crate) from a "best-practices" workflow repository. In this context, "best-practices" means the set of guidelines, especially regarding repository structure and metadata, put together by the workflow language community. Here is the list of currently supported workflow languages, together with the community resources used as a reference:
 
 * Galaxy: [IWC's howto for adding workflows](https://github.com/galaxyproject/iwc/blob/main/workflows/README.md)
-* Nextflow: nf-core [guidelines](https://nf-co.re/contributing/guidelines) and [info on pipeline structure](https://nf-co.re/developers/adding_pipelines#nf-core-pipeline-structure) (and ultimately the template generated by `nf-core create`)
+* Nextflow: nf-core [guidelines](https://nf-co.re/docs/contributing/guidelines) and [info on pipeline structure](https://nf-co.re/developers/adding_pipelines#nf-core-pipeline-structure) (and ultimately the template generated by `nf-core create`)
 * Snakemake: [snakemake-workflows](https://github.com/snakemake-workflows/docs) guidelines, Snakemake [distribution and reproducibility docs](https://snakemake.readthedocs.io/en/stable/snakefiles/deployment.html)
 
 ## Installation
 
 ```
 pip install repo2rocrate
 ```
```

### Comparing `repo2rocrate-0.1.1/repo2rocrate/__init__.py` & `repo2rocrate-0.1.2/repo2rocrate/__init__.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/repo2rocrate/cli.py` & `repo2rocrate-0.1.2/repo2rocrate/cli.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/repo2rocrate/common.py` & `repo2rocrate-0.1.2/repo2rocrate/common.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/repo2rocrate/galaxy.py` & `repo2rocrate-0.1.2/repo2rocrate/galaxy.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/repo2rocrate/nextflow.py` & `repo2rocrate-0.1.2/repo2rocrate/nextflow.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/repo2rocrate/snakemake.py` & `repo2rocrate-0.1.2/repo2rocrate/snakemake.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/repo2rocrate/utils.py` & `repo2rocrate-0.1.2/repo2rocrate/utils.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/repo2rocrate/version.py` & `repo2rocrate-0.1.2/repo2rocrate/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations
 # under the License.
 
-VERSION = "0.1.1"
+VERSION = "0.1.2"
```

### Comparing `repo2rocrate-0.1.1/repo2rocrate.egg-info/PKG-INFO` & `repo2rocrate-0.1.2/repo2rocrate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repo2rocrate
-Version: 0.1.1
+Version: 0.1.2
 Summary: Generate RO-Crates from workflow repositories
 Home-page: https://github.com/crs4/repo2rocrate
 Author: Simone Leo
 Author-email: <simone.leo@crs4.it>
 License: Apache-2.0
 Platform: Linux
 Classifier: Programming Language :: Python :: 3
@@ -17,15 +17,15 @@
 License-File: LICENSE
 
 # repo2rocrate
 
 Generate a [Workflow Testing RO-Crate](https://crs4.github.io/life_monitor/workflow_testing_ro_crate) from a "best-practices" workflow repository. In this context, "best-practices" means the set of guidelines, especially regarding repository structure and metadata, put together by the workflow language community. Here is the list of currently supported workflow languages, together with the community resources used as a reference:
 
 * Galaxy: [IWC's howto for adding workflows](https://github.com/galaxyproject/iwc/blob/main/workflows/README.md)
-* Nextflow: nf-core [guidelines](https://nf-co.re/contributing/guidelines) and [info on pipeline structure](https://nf-co.re/developers/adding_pipelines#nf-core-pipeline-structure) (and ultimately the template generated by `nf-core create`)
+* Nextflow: nf-core [guidelines](https://nf-co.re/docs/contributing/guidelines) and [info on pipeline structure](https://nf-co.re/developers/adding_pipelines#nf-core-pipeline-structure) (and ultimately the template generated by `nf-core create`)
 * Snakemake: [snakemake-workflows](https://github.com/snakemake-workflows/docs) guidelines, Snakemake [distribution and reproducibility docs](https://snakemake.readthedocs.io/en/stable/snakefiles/deployment.html)
 
 ## Installation
 
 ```
 pip install repo2rocrate
 ```
@@ -44,9 +44,7 @@
 ```
 git clone https://github.com/nf-core/rnaseq
 cd rnaseq/
 repo2rocrate
 ```
 
 The above commands add an `ro-crate-metadata.json` file to the repository directory. To generate an RO-Crate in a separate directory, use the `-o` option. Run `repo2rocrate --help` to get a description of all available options.
-
-
```

### Comparing `repo2rocrate-0.1.1/repo2rocrate.egg-info/SOURCES.txt` & `repo2rocrate-0.1.2/repo2rocrate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/setup.py` & `repo2rocrate-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/test/test_cli.py` & `repo2rocrate-0.1.2/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/test/test_galaxy.py` & `repo2rocrate-0.1.2/test/test_galaxy.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/test/test_nextflow.py` & `repo2rocrate-0.1.2/test/test_nextflow.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/test/test_snakemake.py` & `repo2rocrate-0.1.2/test/test_snakemake.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/test/test_top_level.py` & `repo2rocrate-0.1.2/test/test_top_level.py`

 * *Files identical despite different names*

### Comparing `repo2rocrate-0.1.1/test/test_utils.py` & `repo2rocrate-0.1.2/test/test_utils.py`

 * *Files identical despite different names*

