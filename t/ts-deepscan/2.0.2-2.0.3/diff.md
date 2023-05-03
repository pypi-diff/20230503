# Comparing `tmp/ts-deepscan-2.0.2.tar.gz` & `tmp/ts-deepscan-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts-deepscan-2.0.2.tar", last modified: Tue Apr  4 21:33:55 2023, max compression
+gzip compressed data, was "ts-deepscan-2.0.3.tar", last modified: Wed May  3 16:44:35 2023, max compression
```

## Comparing `ts-deepscan-2.0.2.tar` & `ts-deepscan-2.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.617545 ts-deepscan-2.0.2/
--rw-r--r--   0 markin     (501) staff       (20)    11340 2020-12-10 19:17:15.000000 ts-deepscan-2.0.2/LICENSE
--rw-rw----   0 markin     (501) staff       (20)      174 2020-11-03 19:33:21.000000 ts-deepscan-2.0.2/MANIFEST.in
--rw-r--r--   0 markin     (501) staff       (20)      342 2023-04-04 21:33:55.617721 ts-deepscan-2.0.2/PKG-INFO
--rw-r--r--   0 markin     (501) staff       (20)     7658 2022-11-29 15:54:46.000000 ts-deepscan-2.0.2/README.md
--rw-rw----   0 markin     (501) staff       (20)       26 2017-03-20 16:02:56.000000 ts-deepscan-2.0.2/_config.yml
--rw-rw----   0 markin     (501) staff       (20)       79 2023-04-04 21:33:55.618390 ts-deepscan-2.0.2/setup.cfg
--rw-r--r--   0 markin     (501) staff       (20)     1134 2023-04-04 21:32:50.000000 ts-deepscan-2.0.2/setup.py
--rwxr-xr-x   0 markin     (501) staff       (20)       94 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts-deepscan
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.592522 ts-deepscan-2.0.2/ts_deepscan/
--rw-r--r--   0 markin     (501) staff       (20)     4853 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)      145 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/__main__.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.608087 ts-deepscan-2.0.2/ts_deepscan/analyser/
--rw-r--r--   0 markin     (501) staff       (20)     2494 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/analyser/CommentAnalyser.py
--rw-r--r--   0 markin     (501) staff       (20)      922 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/analyser/CryptoAnalyser.py
--rw-r--r--   0 markin     (501) staff       (20)     2419 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/analyser/Dataset.py
--rw-r--r--   0 markin     (501) staff       (20)     1183 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/analyser/LicenseAnalyser.py
--rw-r--r--   0 markin     (501) staff       (20)      731 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/analyser/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)  2702144 2023-01-06 17:43:03.000000 ts-deepscan-2.0.2/ts_deepscan/analyser/licenses.json
--rw-r--r--   0 markin     (501) staff       (20)     2472 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/analyser/spdx.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.608842 ts-deepscan-2.0.2/ts_deepscan/analyser/textutils/
--rw-r--r--   0 markin     (501) staff       (20)     7695 2023-04-03 15:08:19.000000 ts-deepscan-2.0.2/ts_deepscan/analyser/textutils/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)     2124 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/cli.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.610317 ts-deepscan-2.0.2/ts_deepscan/commentparser/
--rw-rw----   0 markin     (501) staff       (20)     6865 2020-12-09 20:37:42.000000 ts-deepscan-2.0.2/ts_deepscan/commentparser/__init__.py
--rw-rw----   0 markin     (501) staff       (20)     6712 2020-12-09 20:37:42.000000 ts-deepscan-2.0.2/ts_deepscan/commentparser/language.py
--rw-r--r--   0 markin     (501) staff       (20)      582 2022-06-10 12:08:39.000000 ts-deepscan-2.0.2/ts_deepscan/config.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.611040 ts-deepscan-2.0.2/ts_deepscan/scancode/
--rw-r--r--   0 markin     (501) staff       (20)       94 2020-12-10 19:16:09.000000 ts-deepscan-2.0.2/ts_deepscan/scancode/__init__.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.615209 ts-deepscan-2.0.2/ts_deepscan/scancode/cluecode/
--rw-r--r--   0 markin     (501) staff       (20)        0 2020-12-10 19:15:52.000000 ts-deepscan-2.0.2/ts_deepscan/scancode/cluecode/__init__.py
--rw-r--r--   0 markin     (501) staff       (20)   103777 2020-12-10 19:14:48.000000 ts-deepscan-2.0.2/ts_deepscan/scancode/cluecode/copyrights.py
--rw-r--r--   0 markin     (501) staff       (20)     3538 2020-12-10 19:14:55.000000 ts-deepscan-2.0.2/ts_deepscan/scancode/cluecode/copyrights_hint.py
--rw-r--r--   0 markin     (501) staff       (20)     3272 2020-12-10 19:15:05.000000 ts-deepscan-2.0.2/ts_deepscan/scancode/cluecode/utils.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.617069 ts-deepscan-2.0.2/ts_deepscan/scanner/
--rw-r--r--   0 markin     (501) staff       (20)     4123 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/scanner/ParallelScanner.py
--rw-r--r--   0 markin     (501) staff       (20)     4050 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/scanner/Scanner.py
--rw-r--r--   0 markin     (501) staff       (20)     2376 2023-04-03 13:51:08.000000 ts-deepscan-2.0.2/ts_deepscan/scanner/__init__.py
-drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-04-04 21:33:55.595323 ts-deepscan-2.0.2/ts_deepscan.egg-info/
--rw-r--r--   0 markin     (501) staff       (20)      342 2023-04-04 21:33:55.000000 ts-deepscan-2.0.2/ts_deepscan.egg-info/PKG-INFO
--rw-r--r--   0 markin     (501) staff       (20)     1049 2023-04-04 21:33:55.000000 ts-deepscan-2.0.2/ts_deepscan.egg-info/SOURCES.txt
--rw-r--r--   0 markin     (501) staff       (20)        1 2023-04-04 21:33:55.000000 ts-deepscan-2.0.2/ts_deepscan.egg-info/dependency_links.txt
--rw-r--r--   0 markin     (501) staff       (20)       53 2023-04-04 21:33:55.000000 ts-deepscan-2.0.2/ts_deepscan.egg-info/entry_points.txt
--rw-r--r--   0 markin     (501) staff       (20)      126 2023-04-04 21:33:55.000000 ts-deepscan-2.0.2/ts_deepscan.egg-info/requires.txt
--rw-r--r--   0 markin     (501) staff       (20)       12 2023-04-04 21:33:55.000000 ts-deepscan-2.0.2/ts_deepscan.egg-info/top_level.txt
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.033877 ts-deepscan-2.0.3/
+-rw-r--r--   0 markin     (501) staff       (20)    11340 2020-12-10 19:17:15.000000 ts-deepscan-2.0.3/LICENSE
+-rw-rw----   0 markin     (501) staff       (20)      174 2020-11-03 19:33:21.000000 ts-deepscan-2.0.3/MANIFEST.in
+-rw-r--r--   0 markin     (501) staff       (20)      342 2023-05-03 16:44:35.033995 ts-deepscan-2.0.3/PKG-INFO
+-rw-r--r--   0 markin     (501) staff       (20)     8719 2023-04-25 11:49:51.000000 ts-deepscan-2.0.3/README.md
+-rw-rw----   0 markin     (501) staff       (20)       26 2017-03-20 16:02:56.000000 ts-deepscan-2.0.3/_config.yml
+-rw-rw----   0 markin     (501) staff       (20)       79 2023-05-03 16:44:35.034423 ts-deepscan-2.0.3/setup.cfg
+-rw-r--r--   0 markin     (501) staff       (20)     1110 2023-05-03 16:43:45.000000 ts-deepscan-2.0.3/setup.py
+-rwxr-xr-x   0 markin     (501) staff       (20)       94 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts-deepscan
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.015913 ts-deepscan-2.0.3/ts_deepscan/
+-rw-r--r--   0 markin     (501) staff       (20)     4853 2023-05-03 16:43:27.000000 ts-deepscan-2.0.3/ts_deepscan/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)      145 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/__main__.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.027157 ts-deepscan-2.0.3/ts_deepscan/analyser/
+-rw-r--r--   0 markin     (501) staff       (20)     2494 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/analyser/CommentAnalyser.py
+-rw-r--r--   0 markin     (501) staff       (20)      922 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/analyser/CryptoAnalyser.py
+-rw-r--r--   0 markin     (501) staff       (20)     2419 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/analyser/Dataset.py
+-rw-r--r--   0 markin     (501) staff       (20)     1183 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/analyser/LicenseAnalyser.py
+-rw-r--r--   0 markin     (501) staff       (20)      731 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/analyser/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)  2702144 2023-01-06 17:43:03.000000 ts-deepscan-2.0.3/ts_deepscan/analyser/licenses.json
+-rw-r--r--   0 markin     (501) staff       (20)     2472 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/analyser/spdx.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.027886 ts-deepscan-2.0.3/ts_deepscan/analyser/textutils/
+-rw-r--r--   0 markin     (501) staff       (20)     7695 2023-04-03 15:08:19.000000 ts-deepscan-2.0.3/ts_deepscan/analyser/textutils/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)     2171 2023-05-03 16:44:14.000000 ts-deepscan-2.0.3/ts_deepscan/cli.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.029210 ts-deepscan-2.0.3/ts_deepscan/commentparser/
+-rw-rw----   0 markin     (501) staff       (20)     6865 2020-12-09 20:37:42.000000 ts-deepscan-2.0.3/ts_deepscan/commentparser/__init__.py
+-rw-rw----   0 markin     (501) staff       (20)     6712 2020-12-09 20:37:42.000000 ts-deepscan-2.0.3/ts_deepscan/commentparser/language.py
+-rw-r--r--   0 markin     (501) staff       (20)      582 2022-06-10 12:08:39.000000 ts-deepscan-2.0.3/ts_deepscan/config.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.029749 ts-deepscan-2.0.3/ts_deepscan/scancode/
+-rw-r--r--   0 markin     (501) staff       (20)       94 2020-12-10 19:16:09.000000 ts-deepscan-2.0.3/ts_deepscan/scancode/__init__.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.032469 ts-deepscan-2.0.3/ts_deepscan/scancode/cluecode/
+-rw-r--r--   0 markin     (501) staff       (20)        0 2020-12-10 19:15:52.000000 ts-deepscan-2.0.3/ts_deepscan/scancode/cluecode/__init__.py
+-rw-r--r--   0 markin     (501) staff       (20)   103777 2020-12-10 19:14:48.000000 ts-deepscan-2.0.3/ts_deepscan/scancode/cluecode/copyrights.py
+-rw-r--r--   0 markin     (501) staff       (20)     3538 2020-12-10 19:14:55.000000 ts-deepscan-2.0.3/ts_deepscan/scancode/cluecode/copyrights_hint.py
+-rw-r--r--   0 markin     (501) staff       (20)     3272 2020-12-10 19:15:05.000000 ts-deepscan-2.0.3/ts_deepscan/scancode/cluecode/utils.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.033602 ts-deepscan-2.0.3/ts_deepscan/scanner/
+-rw-r--r--   0 markin     (501) staff       (20)     4123 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/scanner/ParallelScanner.py
+-rw-r--r--   0 markin     (501) staff       (20)     4050 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/scanner/Scanner.py
+-rw-r--r--   0 markin     (501) staff       (20)     2376 2023-04-03 13:51:08.000000 ts-deepscan-2.0.3/ts_deepscan/scanner/__init__.py
+drwxr-xr-x   0 markin     (501) staff       (20)        0 2023-05-03 16:44:35.018099 ts-deepscan-2.0.3/ts_deepscan.egg-info/
+-rw-r--r--   0 markin     (501) staff       (20)      342 2023-05-03 16:44:34.000000 ts-deepscan-2.0.3/ts_deepscan.egg-info/PKG-INFO
+-rw-r--r--   0 markin     (501) staff       (20)     1049 2023-05-03 16:44:35.000000 ts-deepscan-2.0.3/ts_deepscan.egg-info/SOURCES.txt
+-rw-r--r--   0 markin     (501) staff       (20)        1 2023-05-03 16:44:34.000000 ts-deepscan-2.0.3/ts_deepscan.egg-info/dependency_links.txt
+-rw-r--r--   0 markin     (501) staff       (20)       53 2023-05-03 16:44:34.000000 ts-deepscan-2.0.3/ts_deepscan.egg-info/entry_points.txt
+-rw-r--r--   0 markin     (501) staff       (20)      113 2023-05-03 16:44:34.000000 ts-deepscan-2.0.3/ts_deepscan.egg-info/requires.txt
+-rw-r--r--   0 markin     (501) staff       (20)       12 2023-05-03 16:44:34.000000 ts-deepscan-2.0.3/ts_deepscan.egg-info/top_level.txt
```

### Comparing `ts-deepscan-2.0.2/LICENSE` & `ts-deepscan-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/README.md` & `ts-deepscan-2.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # TrustSource DeepScan 
 Repository scanner for the identification of *_effective licenses and copyright information_*. 
 
 ## What it does? 
 DeepScan takes the URL of a git repository as input, clones the content and scans all files contained (see below) for license indicators and copyright comments. All *findings* will be returned in a hirarchical structure (including references) and the cloned repo will be deleted afterwards. 
 
-We provided also a hosted version with a nice UI, that you can find [here](https://deepscan.trustsource.io "Link to DeepScan Service"). The hosted version is available for free through the Web-UI. It is also part of the subscription based [TrustSource](https://app.trustsource.io)-Service. This version allows in addition the cloning and scanning of private repositories. It has been setup to support many and large repositories. If you are interested in using it from within your CI/CD pipeline, we offer API-subscriptions.
+We provided also a hosted version with a nice UI, that you can find [here](https://deepscan.trustsource.io "Link to DeepScan Service"). The hosted version is available for free through the Web-UI. It is also part of the subscription based [TrustSource](https://app.trustsource.io)-Service. This version allows in addition the cloning and scanning of private repositories. It has been set up to support many and large repositories. If you are interested in using it from within your CI/CD pipeline, we offer API-subscriptions.
 
 To learn more about TrustSource - the only process focussed Open Source Compliance tool, which supports all aspects of the open source compliance tool chain - visit our website at https://www.trustsource.io.
 
 ## What it covers? 
 Currently, the tool searches all kind of source files for comments. It covers a wide range of programming languages:
 * AppleScript
 * Assembly
@@ -105,25 +105,45 @@
 ```
 To scan a complete directory:
 ```
 ts-deepscan scan ./ts-deepscan
 ```
 
 ## Switching copyright collection on/off
-The default is to scan for license indicators only. If you also want to invest into the costly search for copyright infromation, you must inlcude the *--includeCopyright* parameter, e.g.:  
+The default is to scan for license indicators only. If you also want to invest into the costly search for copyright infromation, you must inlcude the *--include-copyright* parameter, e.g.:  
 ```
 ts-deepscan scan --include-copyright ./ts-deepscan
 ```
 
+## Switching detection of used cryptographic algorithms on/off
+If you want to turn on the search for used cryptographic algorithms in source code files (based on ScanOSS detection algorithms), you must inlcude the *--include-crypto* parameter, e.g.:  
+```
+ts-deepscan scan --include-crypto ./ts-deepscan
+```
+
 ## Selecting the output target
 Default output will be stdout (console). To write in a file instead, use the -o option, e.g.:
 ```
 ts-deepscan scan --include-copyright -o result.json ./ts-deepscan
 ```
 
+## Exclude files from analysis
+If you want to exclude files from analysis while scanning directories, you can specify one or more ignore file patterns using the *--ignore-pattern* option, e.g. the following command 
+```
+ts-deepscan scan --ignore-pattern "*.pyc" -o result.json ./ts-deepscan
+```
+scans the directory 'ts-deepscan' and exludes all Python compiled files with an extension "pyc" from the analysis.  
+
+## Number of parallel jobs
+The default is to use the maximal number of availbale CPU cores (cpu_count - 1) on Unix based systems and one core on Windows (due to slow process forking), if you want to specify the number of parallel jobs manually, you can use *-j* option, e.g.
+
+```
+ts-deepscan scan -j 4 -o result.json ./ts-deepscan
+```
+
 ## Uploading scan results
 For uploading previously stored scan results (scan executed with the '-o' option) to the TrustSource app use the following command: 
 
 ```
 ts-deepscan upload --project-name <YOUR_PROJECT_NAME> --module-name ts-deepscan --api-key <YOUR_API_KEY> result.json
 ```
 
@@ -143,9 +163,9 @@
 
 In case you have specific need for any of the cases mentioned above, feel free to reach out and let us know about your case. If you have additional ideas, feel free to open a feature request in the issues section. 
 
 # Contribution, Contact and Support
 Feel free to reach out to the [TrustSource Team](https://support.trustsource.io/hc/en-us/requests/new "TrustSource Knowledgebase") by dropping us a message or providing [issues](/org/ts-deepscan/issues). We'ld love to hear your feedback to learn and improve.
 Contributions are welcome. Just clone, create your branch and send a pull request. Please make sure to agree to the [contribution agreement](/org/ContributionAgreeemnt.md "Contribution Agreement") and the [coding guidelines](/org/CodingGuidelines.md "Coding Guidelines").
 
-If you like the tool and want to support our further work, feel free to support us with donations or sign a API-usage agreement.
+If you like the tool and want to support our further work, feel free to support us with donations or sign an API-usage agreement.
 Thank you & best regards!
```

### Comparing `ts-deepscan-2.0.2/setup.py` & `ts-deepscan-2.0.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,32 +8,31 @@
         'ts_deepscan.analyser',
         'ts_deepscan.analyser.textutils',
         'ts_deepscan.commentparser',
         'ts_deepscan.scanner',
         'ts_deepscan.scancode',
         'ts_deepscan.scancode.cluecode'
     ],
-    version='2.0.2',
+    version='2.0.3',
     description='Repository scanner for the identification of effective licenses and copyright information.',
     author='EACG GmbH',
     license='Apache 2.0',
     url='https://github.com/TrustSource/ts-deepscan.git',
     download_url='',
     keywords=['DeepScan', 'TrustSource'],
     classifiers=[],
     install_requires=[
         'six',
         'spacy>=2.2.0,<3.0.0',
         'nltk',
         'text-unidecode',
         'requests',
         'progress',
-        'click>=8.0.3',
         'osadl_matrix',
-        'ts-python-client>=2.0.0',
+        'ts-python-client>=2.0.3',
         'pyminr>=0.1.0'
     ],
     scripts=['ts-deepscan'],
     entry_points={
         'console_scripts': ['ts-deepscan=ts_deepscan.cli:main'],
     },
     setup_requires=[
```

### Comparing `ts-deepscan-2.0.2/ts_deepscan/__init__.py` & `ts-deepscan-2.0.3/ts_deepscan/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/analyser/CommentAnalyser.py` & `ts-deepscan-2.0.3/ts_deepscan/analyser/CommentAnalyser.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/analyser/CryptoAnalyser.py` & `ts-deepscan-2.0.3/ts_deepscan/analyser/CryptoAnalyser.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/analyser/Dataset.py` & `ts-deepscan-2.0.3/ts_deepscan/analyser/Dataset.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/analyser/LicenseAnalyser.py` & `ts-deepscan-2.0.3/ts_deepscan/analyser/LicenseAnalyser.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/analyser/__init__.py` & `ts-deepscan-2.0.3/ts_deepscan/analyser/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/analyser/licenses.json` & `ts-deepscan-2.0.3/ts_deepscan/analyser/licenses.json`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/analyser/spdx.py` & `ts-deepscan-2.0.3/ts_deepscan/analyser/spdx.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/analyser/textutils/__init__.py` & `ts-deepscan-2.0.3/ts_deepscan/analyser/textutils/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/cli.py` & `ts-deepscan-2.0.3/ts_deepscan/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,22 +8,23 @@
 import pathlib
 
 from typing import List
 
 from .scanner import Scan
 from . import create_scanner, execute_scan, upload_data, deepscanBaseUrl
 
-from ts_python_client.cli import start, scan
+from ts_python_client.cli import get_start_cmd, scan
 
 
+start = get_start_cmd(version='2.0.3')
+
 def main():
     start()
 
 
-
 @click.option('-j', '--jobs',
               default=-1 if sys.platform != 'win32' else 1, # Turn off multitasking due to the long spawn on Windows
               help='Number of parallel jobs')
 @click.option('--include-copyright',
               default=False,
               is_flag=True,
               help='Enables searching for copyright information in source code files')
```

### Comparing `ts-deepscan-2.0.2/ts_deepscan/commentparser/__init__.py` & `ts-deepscan-2.0.3/ts_deepscan/commentparser/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/commentparser/language.py` & `ts-deepscan-2.0.3/ts_deepscan/commentparser/language.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/config.py` & `ts-deepscan-2.0.3/ts_deepscan/config.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/scancode/cluecode/copyrights.py` & `ts-deepscan-2.0.3/ts_deepscan/scancode/cluecode/copyrights.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/scancode/cluecode/copyrights_hint.py` & `ts-deepscan-2.0.3/ts_deepscan/scancode/cluecode/copyrights_hint.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/scancode/cluecode/utils.py` & `ts-deepscan-2.0.3/ts_deepscan/scancode/cluecode/utils.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/scanner/ParallelScanner.py` & `ts-deepscan-2.0.3/ts_deepscan/scanner/ParallelScanner.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/scanner/Scanner.py` & `ts-deepscan-2.0.3/ts_deepscan/scanner/Scanner.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan/scanner/__init__.py` & `ts-deepscan-2.0.3/ts_deepscan/scanner/__init__.py`

 * *Files identical despite different names*

### Comparing `ts-deepscan-2.0.2/ts_deepscan.egg-info/SOURCES.txt` & `ts-deepscan-2.0.3/ts_deepscan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

