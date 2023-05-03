# Comparing `tmp/malbench-0.3.3.tar.gz` & `tmp/malbench-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malbench-0.3.3.tar", max compression
+gzip compressed data, was "malbench-0.3.4.tar", max compression
```

## Comparing `malbench-0.3.3.tar` & `malbench-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,17 @@
--rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.3/data/banner.txt
--rw-r--r--   0        0        0      508 2023-04-25 12:39:55.627552 malbench-0.3.3/data/disclaimer.txt
--rw-r--r--   0        0        0        5 2023-05-01 12:47:17.593190 malbench-0.3.3/data/version.txt
--rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.3/LICENSE
--rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.3/malbench/__init__.py
--rw-r--r--   0        0        0     2905 2023-04-27 03:15:45.560814 malbench-0.3.3/malbench/__main__.py
--rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.3/malbench/args.py
--rw-r--r--   0        0        0     4830 2023-04-26 15:12:59.929156 malbench-0.3.3/malbench/malware.py
--rw-r--r--   0        0        0     8362 2023-04-27 03:29:38.237716 malbench-0.3.3/malbench/message.py
--rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.3/malbench/version.py
--rw-r--r--   0        0        0      892 2023-05-01 12:47:25.525781 malbench-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     7144 2023-05-01 04:55:05.817341 malbench-0.3.3/README.md
--rw-r--r--   0        0        0     7896 1970-01-01 00:00:00.000000 malbench-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      545 2023-04-13 19:49:08.177178 malbench-0.3.4/data/banner.txt
+-rw-r--r--   0        0        0   526052 2023-05-02 19:55:33.359376 malbench-0.3.4/data/demo.gif
+-rw-r--r--   0        0        0      567 2023-05-01 23:24:48.296033 malbench-0.3.4/data/disclaimer.txt
+-rwxr-xr-x   0        0        0    45056 2022-05-07 05:20:05.904971 malbench-0.3.4/data/samples/calc.exe
+-rwxr-xr-x   0        0        0   211968 2021-11-23 07:13:38.663950 malbench-0.3.4/data/samples/notepad.exe
+-rw-r--r--   0        0        0       15 2023-04-15 21:23:53.510662 malbench-0.3.4/data/samples/test.txt
+-rw-r--r--   0        0        0        5 2023-05-02 12:50:01.138775 malbench-0.3.4/data/version.txt
+-rw-r--r--   0        0        0    35803 2023-04-02 22:37:30.790768 malbench-0.3.4/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-02 12:57:46.205523 malbench-0.3.4/malbench/__init__.py
+-rw-r--r--   0        0        0     3000 2023-05-02 19:13:53.949742 malbench-0.3.4/malbench/__main__.py
+-rw-r--r--   0        0        0     4941 2023-04-27 03:46:07.566126 malbench-0.3.4/malbench/args.py
+-rw-r--r--   0        0        0     4924 2023-05-02 13:19:11.884051 malbench-0.3.4/malbench/malware.py
+-rw-r--r--   0        0        0     8362 2023-05-02 19:13:53.949742 malbench-0.3.4/malbench/message.py
+-rw-r--r--   0        0        0      435 2023-04-21 13:20:47.394154 malbench-0.3.4/malbench/version.py
+-rw-r--r--   0        0        0      893 2023-05-03 13:11:23.650700 malbench-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     8083 2023-05-03 13:15:07.824595 malbench-0.3.4/README.md
+-rw-r--r--   0        0        0     8880 1970-01-01 00:00:00.000000 malbench-0.3.4/PKG-INFO
```

### Comparing `malbench-0.3.3/data/banner.txt` & `malbench-0.3.4/data/banner.txt`

 * *Files identical despite different names*

### Comparing `malbench-0.3.3/LICENSE` & `malbench-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `malbench-0.3.3/malbench/__main__.py` & `malbench-0.3.4/malbench/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
         # Parse arguments and load tool.
         args = ArgParser.parse()
         message = Message(args["color"])
 
         if args["banner"]:
             print(message.banner())
 
+        if args["dev"]:
+            print(f"Running in {message.blue('DEV')} mode.\n")
+
         if args["warning"]:
             print(message.disclaimer())
             _confirm_continue()
 
         # Start the malware samples.
         print("Loading malware...")
         malwares = []
@@ -48,15 +51,15 @@
         detection_rate = results.detection_rate()
 
         if detection_rate == 1:
             print(f"\nDone. Detection rate:  {message.green('100%')}.")
             print("No malware went undetected!\n")
         else:
             detection_rate_percent = f"{round(detection_rate * 100)}%"
-            undetected_malware = results.failed_samples()
+            undetected_malware = results.undetected_samples()
 
             print(f"\nDone. Detection rate: { message.red(detection_rate_percent)} ({len(undetected_malware)} failed):")
 
             for malware in undetected_malware:
                 print(malware.name)
             print("")
     except KeyboardInterrupt:
```

### Comparing `malbench-0.3.3/malbench/args.py` & `malbench-0.3.4/malbench/args.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.3/malbench/malware.py` & `malbench-0.3.4/malbench/malware.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,33 +115,33 @@
         """
         Calculates the detection rate of the samples.
 
         Returns:
             float: The detection rate of the samples.
         """
 
-        failed = 0
+        detected = len(self.detected_samples())
 
-        for sample in self.samples:
-            if sample.detected is True:
-                failed += 1
-
-        if failed == 0:
+        if detected == 0:
             return 0
 
-        return failed / len(self.samples)
+        return detected / len(self.samples)
 
-    def failed_samples(self) -> List[MalwareLauncher]:
+    def detected_samples(self) -> List[MalwareLauncher]:
         """
-        Returns a list of MalwareLauncher objects that were not detected.
+        Gets detected samples.
 
         Returns:
-            List[MalwareLauncher]: A list of MalwareLauncher objects that were not detected.
+            List[MalwareLauncher]: A list of MalwareLauncher objects that were detected.
         """
 
-        samples = []
+        return [sample for sample in self.samples if sample.detected]
+
+    def undetected_samples(self) -> List[MalwareLauncher]:
+        """
+        Gets undetected samples.
 
-        for sample in self.samples:
-            if sample.detected is False:
-                samples.append(sample)
+        Returns:
+            List[MalwareLauncher]: A list of MalwareLauncher objects that were not detected.
+        """
 
-        return samples
+        return [sample for sample in self.samples if not sample.detected]
```

### Comparing `malbench-0.3.3/malbench/message.py` & `malbench-0.3.4/malbench/message.py`

 * *Files identical despite different names*

### Comparing `malbench-0.3.3/pyproject.toml` & `malbench-0.3.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "malbench"
-version = "0.3.3"
+version = "0.3.4"
 description = "A tool used to benchmark antivirus solutions against real-world malware samples."
 repository = "https://github.com/youkergav/Malbench"
 authors = ["Gavin Youker <youkergav@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-only"
 include = ["data/*"]
 exclude = ["data/samples"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8.1"
 colorama = "^0.4.6"
 toml = "^0.10.2"
 holidays = "^0.22"
 python-dotenv = "^1.0.0"
 types-setuptools = "^67.7.0.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `malbench-0.3.3/README.md` & `malbench-0.3.4/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 # Malbench
 Malbench is a command-line tool for testing and evaluating the effectiveness of malware detection tools (such as antivirus solutions). It does this by running a set of malware samples, and checking if the malware is flagged by the detection tool we are evaluating. Malbench is built to be modular and configurable, so it can be customized to meet the specific needs of different users and environments.
+![Malbench Terminal Demo](data/demo.gif)
 
 ## About
-
-
 ### Disclaimer 
-**⚠ WARNING**: Malbench is designed to run malicious code that can harm your computer. Malbench should only be run on secure and isolated environments by users who know what they are doing. Do **not** run Malbench on a computer or network that contains sensitive information or data that you are not willing to lose or become compromised. By downloading and/or using this software, you acknowledge and understand the risks of using this software; and assume full responsibility for any damages that may result from running Malbench.
+**⚠ WARNING**: Malbench is a tool for testing antivirus software against real-world malware samples. While it does not contain any malware on its own, it is designed to run malware samples provided by the user. Use Malbench only in secure and isolated environments that you are authorized in doing so. Do **not** use Malbench on a computer or network that contains sensitive information or data that you are not willing to lose and/or become compromised. By using Malbench, you acknowledge the risks and assume full responsibility for any damages that may result.
 
-**ℹ️ NOTE**: It is important to note that Malbench does not include any malware samples. Therefore, users are expected to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically; and that users have control over the types of malware being tested.
+**ℹ️ NOTE**: As stated above: *Malbench does not come with any malicious code installed*. It is the user's responsibility to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically, and that users have control over the types of malware being tested.
 
-### Why Use Malbench?
+### Why Use Malbench
 Malware detection tools are an essential component of any computer security strategy, but they are not foolproof. New techniques and methods are constantly being developed to evade detection. It is important to regularly test and evaluate the effectiveness of detection tools to ensure that we are keeping up with these evolving threats.
 
 With all the different features and algorithms of modern antivirus solutions, it can be hard to find practical and objective results on what-all they defend against. Malbench can be leveraged to bulk-test known malware samples against antivirus solutions to deliver real and practical results. This is done by automatically launching multiple malware payloads on a system and seeing what samples are detected and which ones were evaded. With Malbench, users can customize their testing to meet their specific needs, selecting the malware samples they want to run, and the duration of a test.
 
+### How Antivirus is Benchmarked
+Malbench launches each malware sample selected by the user and monitors its execution. If the sample completes without error, it is flagged as `UNDETECTED`. If the sample is terminated with an error code, it is flagged as `DETECTED`, indicating that it was killed by the antivirus solution. If the sample is still running after a designated time (defaults to 2 seconds), Malbench forcibly kills the program and flags it as `UNDETECTED`, as the antivirus solution did not detect it in time.
+
+After each sample is run, Malbench displays the detection rate. The detection rate is a percentage representing the amount of samples the antivirus successfully defended against. 
+
+$$
+\text{Detection rate} = \frac{\text{Number of samples flagged as detected}}{\text{Total number of samples}} \times 100\%
+$$
+
 ## Installation
 There are two ways to install Malbench, depending on whether you are a user or a developer.
 
 ### For Users
 To install Malbench for general use, follow these simple steps:
 
-1.  Ensure that the following is installed on your system: [Python 3.9](https://www.python.org/downloads/)+, and [PIP](https://pypi.org/project/pip/) (included with most Python installations).
+1.  Ensure that the following is installed on your system: [Python 3.8.1+](https://www.python.org/downloads/), and [PIP](https://pypi.org/project/pip/) (included with most Python installations).
 2.  Install Malbench via pip by running the following command:
     ```bash
     pip install malbench
     ```
 
 ### For Developers
 If you are a developer who wants to contribute to Malbench or modify the source code, you will need to follow a different set of installation steps: 
 
-1.  Ensure the following is installed on your system: [Python 3.9](https://www.python.org/downloads/)+, [PIP](https://pypi.org/project/pip/) (included with most Python installations), [Git](https://git-scm.com/downloads), [Poetry](https://python-poetry.org/docs/), and an IDE of your choice ([VSCode](https://code.visualstudio.com/download) recommended).
+1.  Ensure the following is installed on your system: [Python 3.8.1+](https://www.python.org/downloads/), [PIP](https://pypi.org/project/pip/) (included with most Python installations), [Git](https://git-scm.com/downloads), [Poetry](https://python-poetry.org/docs/), and an IDE of your choice ([VSCode](https://code.visualstudio.com/download) recommended).
 2.  Clone (or fork) the Malbench repository using Git:
     ```bash
     git clone https://github.com/youkergav/Malbench.git
     ```
 3.  Navigate to the project directory:
     ```bash
     cd malbench
@@ -54,15 +62,15 @@
 To use Malbench, simply run the following command inside your virtual environment:
 ```bash
 python -m malbench /path/to/malware
 ```
 
 Replace `/path/to/malware` with your `path` argument. The `path` argument should be the path to the malware samples you want to test. This can be either a single file or a folder containing multiple files. Only executable files will be ran by Malbench.
 
-By default, Malbench will show a banner when it starts, and will prompt you to confirm that you understand the risks involved before running the malware samples. You can disable the banner using the `--no-banner` flag, and disable the confirmation prompt using the `--no-warning` flag.
+By default, Malbench will show a banner when it starts, and will prompt you to confirm that you understand the risks involved before running the malware samples. You can disable the banner using the `--no-banner` flag, and disable the confirmation prompt using the `--no-warning` flag (as seen in the demo).
 
 Malware samples are run one by one, and Malbench will wait for each sample to be stopped by the detection software or reach the specified 2 second timeout before moving on to the next sample. This timeout can be changed with the `--timeout` flag. If a sample completes successfully, Malbench will print a red message with a `[-]` prefix, indicating it wasn't stopped by the detection software. If a sample has to be forcibly terminated by the detection software, Malbench will print a green message with a `[+]` prefix, indicating is was successfully detected and stopped.
 
 A full list of arguments to use with Malbench are below. This can be displayed with `--help`.
 ```bash
 usage: malbench [-h] [-v] [-t TIMEOUT] [-nB] [-nW] [-d] path
```

### Comparing `malbench-0.3.3/PKG-INFO` & `malbench-0.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,60 +1,69 @@
 Metadata-Version: 2.1
 Name: malbench
-Version: 0.3.3
+Version: 0.3.4
 Summary: A tool used to benchmark antivirus solutions against real-world malware samples.
 Home-page: https://github.com/youkergav/Malbench
 License: GPL-3.0-only
 Author: Gavin Youker
 Author-email: youkergav@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: holidays (>=0.22,<0.23)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: types-setuptools (>=67.7.0.0,<68.0.0.0)
 Project-URL: Repository, https://github.com/youkergav/Malbench
 Description-Content-Type: text/markdown
 
 # Malbench
 Malbench is a command-line tool for testing and evaluating the effectiveness of malware detection tools (such as antivirus solutions). It does this by running a set of malware samples, and checking if the malware is flagged by the detection tool we are evaluating. Malbench is built to be modular and configurable, so it can be customized to meet the specific needs of different users and environments.
+![Malbench Terminal Demo](data/demo.gif)
 
 ## About
-
-
 ### Disclaimer 
-**⚠ WARNING**: Malbench is designed to run malicious code that can harm your computer. Malbench should only be run on secure and isolated environments by users who know what they are doing. Do **not** run Malbench on a computer or network that contains sensitive information or data that you are not willing to lose or become compromised. By downloading and/or using this software, you acknowledge and understand the risks of using this software; and assume full responsibility for any damages that may result from running Malbench.
+**⚠ WARNING**: Malbench is a tool for testing antivirus software against real-world malware samples. While it does not contain any malware on its own, it is designed to run malware samples provided by the user. Use Malbench only in secure and isolated environments that you are authorized in doing so. Do **not** use Malbench on a computer or network that contains sensitive information or data that you are not willing to lose and/or become compromised. By using Malbench, you acknowledge the risks and assume full responsibility for any damages that may result.
 
-**ℹ️ NOTE**: It is important to note that Malbench does not include any malware samples. Therefore, users are expected to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically; and that users have control over the types of malware being tested.
+**ℹ️ NOTE**: As stated above: *Malbench does not come with any malicious code installed*. It is the user's responsibility to provide their own samples for testing purposes. This is to ensure that Malbench is used responsibly and ethically, and that users have control over the types of malware being tested.
 
-### Why Use Malbench?
+### Why Use Malbench
 Malware detection tools are an essential component of any computer security strategy, but they are not foolproof. New techniques and methods are constantly being developed to evade detection. It is important to regularly test and evaluate the effectiveness of detection tools to ensure that we are keeping up with these evolving threats.
 
 With all the different features and algorithms of modern antivirus solutions, it can be hard to find practical and objective results on what-all they defend against. Malbench can be leveraged to bulk-test known malware samples against antivirus solutions to deliver real and practical results. This is done by automatically launching multiple malware payloads on a system and seeing what samples are detected and which ones were evaded. With Malbench, users can customize their testing to meet their specific needs, selecting the malware samples they want to run, and the duration of a test.
 
+### How Antivirus is Benchmarked
+Malbench launches each malware sample selected by the user and monitors its execution. If the sample completes without error, it is flagged as `UNDETECTED`. If the sample is terminated with an error code, it is flagged as `DETECTED`, indicating that it was killed by the antivirus solution. If the sample is still running after a designated time (defaults to 2 seconds), Malbench forcibly kills the program and flags it as `UNDETECTED`, as the antivirus solution did not detect it in time.
+
+After each sample is run, Malbench displays the detection rate. The detection rate is a percentage representing the amount of samples the antivirus successfully defended against. 
+
+$$
+\text{Detection rate} = \frac{\text{Number of samples flagged as detected}}{\text{Total number of samples}} \times 100\%
+$$
+
 ## Installation
 There are two ways to install Malbench, depending on whether you are a user or a developer.
 
 ### For Users
 To install Malbench for general use, follow these simple steps:
 
-1.  Ensure that the following is installed on your system: [Python 3.9](https://www.python.org/downloads/)+, and [PIP](https://pypi.org/project/pip/) (included with most Python installations).
+1.  Ensure that the following is installed on your system: [Python 3.8.1+](https://www.python.org/downloads/), and [PIP](https://pypi.org/project/pip/) (included with most Python installations).
 2.  Install Malbench via pip by running the following command:
     ```bash
     pip install malbench
     ```
 
 ### For Developers
 If you are a developer who wants to contribute to Malbench or modify the source code, you will need to follow a different set of installation steps: 
 
-1.  Ensure the following is installed on your system: [Python 3.9](https://www.python.org/downloads/)+, [PIP](https://pypi.org/project/pip/) (included with most Python installations), [Git](https://git-scm.com/downloads), [Poetry](https://python-poetry.org/docs/), and an IDE of your choice ([VSCode](https://code.visualstudio.com/download) recommended).
+1.  Ensure the following is installed on your system: [Python 3.8.1+](https://www.python.org/downloads/), [PIP](https://pypi.org/project/pip/) (included with most Python installations), [Git](https://git-scm.com/downloads), [Poetry](https://python-poetry.org/docs/), and an IDE of your choice ([VSCode](https://code.visualstudio.com/download) recommended).
 2.  Clone (or fork) the Malbench repository using Git:
     ```bash
     git clone https://github.com/youkergav/Malbench.git
     ```
 3.  Navigate to the project directory:
     ```bash
     cd malbench
@@ -75,15 +84,15 @@
 To use Malbench, simply run the following command inside your virtual environment:
 ```bash
 python -m malbench /path/to/malware
 ```
 
 Replace `/path/to/malware` with your `path` argument. The `path` argument should be the path to the malware samples you want to test. This can be either a single file or a folder containing multiple files. Only executable files will be ran by Malbench.
 
-By default, Malbench will show a banner when it starts, and will prompt you to confirm that you understand the risks involved before running the malware samples. You can disable the banner using the `--no-banner` flag, and disable the confirmation prompt using the `--no-warning` flag.
+By default, Malbench will show a banner when it starts, and will prompt you to confirm that you understand the risks involved before running the malware samples. You can disable the banner using the `--no-banner` flag, and disable the confirmation prompt using the `--no-warning` flag (as seen in the demo).
 
 Malware samples are run one by one, and Malbench will wait for each sample to be stopped by the detection software or reach the specified 2 second timeout before moving on to the next sample. This timeout can be changed with the `--timeout` flag. If a sample completes successfully, Malbench will print a red message with a `[-]` prefix, indicating it wasn't stopped by the detection software. If a sample has to be forcibly terminated by the detection software, Malbench will print a green message with a `[+]` prefix, indicating is was successfully detected and stopped.
 
 A full list of arguments to use with Malbench are below. This can be displayed with `--help`.
 ```bash
 usage: malbench [-h] [-v] [-t TIMEOUT] [-nB] [-nW] [-d] path
```

