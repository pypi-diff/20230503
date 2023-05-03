# Comparing `tmp/v2conf-0.1.1.tar.gz` & `tmp/v2conf-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "v2conf-0.1.1.tar", max compression
+gzip compressed data, was "v2conf-0.1.2.tar", max compression
```

## Comparing `v2conf-0.1.1.tar` & `v2conf-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-07 15:17:18.364133 v2conf-0.1.1/LICENSE
--rw-r--r--   0        0        0     4922 2023-04-22 13:18:36.905010 v2conf-0.1.1/README.md
--rw-r--r--   0        0        0      847 2023-04-22 13:17:12.864109 v2conf-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      118 2023-04-07 15:17:18.364133 v2conf-0.1.1/v2conf/__init__.py
--rw-r--r--   0        0        0     9908 2023-04-22 13:17:12.844108 v2conf-0.1.1/v2conf/__main__.py
--rw-r--r--   0        0        0     8654 2023-04-22 13:11:40.808579 v2conf-0.1.1/v2conf/configs.py
--rw-r--r--   0        0        0     1470 2023-04-07 15:17:18.364133 v2conf-0.1.1/v2conf/exclude.py
--rw-r--r--   0        0        0     6646 2023-04-08 12:17:20.508888 v2conf-0.1.1/v2conf/health.py
--rw-r--r--   0        0        0     5847 1970-01-01 00:00:00.000000 v2conf-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-07 15:17:18.364133 v2conf-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5276 2023-05-03 11:26:29.002471 v2conf-0.1.2/README.md
+-rw-r--r--   0        0        0      847 2023-05-03 11:26:29.002471 v2conf-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-04-07 15:17:18.364133 v2conf-0.1.2/v2conf/__init__.py
+-rw-r--r--   0        0        0    10252 2023-05-03 11:26:29.002471 v2conf-0.1.2/v2conf/__main__.py
+-rw-r--r--   0        0        0     8654 2023-04-22 13:11:40.808579 v2conf-0.1.2/v2conf/configs.py
+-rw-r--r--   0        0        0     1470 2023-04-07 15:17:18.364133 v2conf-0.1.2/v2conf/exclude.py
+-rw-r--r--   0        0        0     6646 2023-04-08 12:17:20.508888 v2conf-0.1.2/v2conf/health.py
+-rw-r--r--   0        0        0     6201 1970-01-01 00:00:00.000000 v2conf-0.1.2/PKG-INFO
```

### Comparing `v2conf-0.1.1/LICENSE` & `v2conf-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `v2conf-0.1.1/README.md` & `v2conf-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 ## Recommended Usage
 ```bash
 sudo $(which v2conf) /home/ubuntu/confs -n 10 -s 900 --timeout-penalty 15 --ema 8,2 --no-geoip --country-code 'IR' --log-level error --jalali -w "https://dl-cdn.alpinelinux.org/alpine/v3.17/releases/x86/alpine-minirootfs-3.17.1-x86.tar.gz" --log-file /home/ubuntu/v2conf.log 
 ```
 With these flags and settings, V2Conf will download the selected file every 15 minutes (900 / 60 = 15) 10 times for each outbound.\
 V2Conf will print logs in Jalali date times in `/home/ubuntu/v2conf.log` and `stdout` simultaneously and it will exclude IPs for Iran. (useful for domestic Iranian VPSs) \
 `--timeout-penalty 15` makes the program to consider a failed test as a test with 15 seconds latency and based on exponential moving average of last `8` evaluations (past 2 hours) and weighting more importance on recent evaluations (`2` times for every new evaluation) choose the best outbound and route all data within that.\
-`--log-level error` indicates that **V2Ray** log level will be `error`.
+`--log-level error` indicates that **V2Ray** log level will be `error`.\
+For using it with `xray` you can specify `-c /usr/local/etc/xray/config.json` and `-p xray` flags.\
+
+Be aware that **V2Conf only supports V2Fly V4 JSON configs**.
 
 ## Details
 
 V2Conf expects a directory with this structure from you:
 ```bash
 confs/
 ├── inbounds  # an "inbounds" directory
@@ -47,50 +50,51 @@
 ```
 and **all configs must have a tag!**
 P.S.: Thanks to [Tushar](https://github.com/Mahyar24/V2Conf/pull/2) V2Conf now supports JSON5 format for configs.
 
 
 ## Usage
 ```
-$ v2conf --help
-usage: v2conf [-h] [-c CONFIG_FILE] [--country-code COUNTRY_CODE] [--no-geoip] [-t TIMEOUT] [-w WEBSITE] [-n NUM_OF_TRIES] [--timeout-penalty TIMEOUT_PENALTY] [--ema EMA] [-s SLEEP_TIME]
+usage: v2conf [-h] [-c CONFIG_FILE] [-p PROCESS_NAME] [--country-code COUNTRY_CODE] [--no-geoip] [-t TIMEOUT] [-w WEBSITE] [-n NUM_OF_TRIES] [--timeout-penalty TIMEOUT_PENALTY] [--ema EMA] [-s SLEEP_TIME]
                    [-l {debug,info,warning,error,none}] [-q | --log-file LOG_FILE] [--jalali] [-v]
                    [path_conf_dir]
 
 positional arguments:
   path_conf_dir         Select configuration directory, default is $PWD.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -c CONFIG_FILE, --config-file CONFIG_FILE
                         Select configuration file, default is '/usr/local/etc/v2ray/config.json'.
+  -p PROCESS_NAME, --process-name PROCESS_NAME
+                        Select the process name, default is 'v2ray'. If you are using 'xray' set it here and in the custom config file path in '-c' flag.
   --country-code COUNTRY_CODE
                         Exclude a country from the list of IPs to be routed; default is 'IR'. (ISO 3166-1 alpha-2)
   --no-geoip            Instead of using V2Ray GeoIP database, downloading IPs from 'ripe.net' (more recent IPs but may slow V2Ray)
   -t TIMEOUT, --timeout TIMEOUT
                         Set the timeout for checking the health of proxies, default is 15 seconds.
   -w WEBSITE, --website WEBSITE
                         Set the website to be used for checking the health of proxies, default is 'https://facebook.com'.
   -n NUM_OF_TRIES, --num-of-tries NUM_OF_TRIES
                         Set the number of tries for checking the health of proxies, default is 10.
   --timeout-penalty TIMEOUT_PENALTY
                         Converting timeouts to latency by this factor (in seconds), DISABLED by default.
-  --ema EMA             Instead of choosing OutBound based on latest evaluation, rank based on exponential moving average of last Nth tests and smoothing variable. (e.g. --ema 10,2.5), DISABLED by default.
+  --ema EMA             Instead of choosing OutBound based on latest evaluation, rank based on exponential moving average of last Nth tests and smoothing variable. (e.g. --ema 10,2.5) DISABLED by default.
   -s SLEEP_TIME, --sleep-time SLEEP_TIME
                         Set the sleep time between each checkup, default is 1,800s. (in seconds)
   -l {debug,info,warning,error,none}, --log-level {debug,info,warning,error,none}
                         Set the V2Ray log level, default is 'warning'.
   -q, --quiet           No log file (V2Conf). (printing to stdout anyway)
   --log-file LOG_FILE   Path for V2Conf log file. default is '$PWD/V2Conf.log'
   --jalali              Use Jalali datetime for V2Conf logging
   -v, --version         Show version and exit.
 
 Written by: Mahyar Mahdavi <Mahyar@Mahyar24.com>. License: GNU GPLv3. Source Code: <https://github.com/mahyar24/V2Conf>. Reporting Bugs and PRs are welcomed. :)
-
 ```
+
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Contact me: <OSS@Mahyar24.com> :)
 
 ## License
-[GNU GPLv3 ](https://choosealicense.com/licenses/gpl-3.0/)
+[GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/)
```

### Comparing `v2conf-0.1.1/pyproject.toml` & `v2conf-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "v2conf"
-version = "0.1.1"
+version = "0.1.2"
 description = "V2Conf helps you build V2Ray Config file automatically and evaluate and change config rules based on outbounds performances."
 authors = ["Mahyar Mahdavi <Mahyar@Mahyar24.com>"]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/mahyar24/V2Conf/"
 repository = "https://github.com/Mahyar24/V2Conf/"
 readme = "README.md"
 keywords = [
```

### Comparing `v2conf-0.1.1/v2conf/__main__.py` & `v2conf-0.1.2/v2conf/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,27 +29,27 @@
 from time import struct_time
 from typing import Optional
 from zoneinfo import ZoneInfo
 
 from .configs import make_conf, write_conf
 from .health import rank_outbounds
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __author__ = "Mahyar Mahdavi"
 __email__ = "Mahyar@Mahyar24.com"
 __license__ = "GPLv3"
 __url__ = "https://GitHub.com/Mahyar24/V2Conf"
 __pypi__ = "https://PyPI.org/project/V2Conf"
 
 
 def check_requirements() -> None:
     """
     Assert if user is running the script with root privileges.
     """
-    assert os.getuid() == 0, "You must have super user permissions to run this program."
+    assert os.getuid() != 0, "You must have super user permissions to run this program."
 
 
 def tehran_time(*_, **__) -> time.struct_time:
     """
     Struct_time for Jalali date-time.
     """
 
@@ -168,14 +168,23 @@
         "--config-file",
         default=Path("/usr/local/etc/v2ray/config.json"),
         type=Path,
         help="Select configuration file, default is '/usr/local/etc/v2ray/config.json'.",
     )
 
     parser.add_argument(
+        "-p",
+        "--process-name",
+        default="v2ray",
+        type=str,
+        help="Select the process name, default is 'v2ray'. If you are using 'xray'"
+        " set it here and in the custom config file path in '-c' flag.",
+    )
+
+    parser.add_argument(
         "--country-code",
         help="Exclude a country from the list of IPs to be routed; "
         "default is 'IR'. (ISO 3166-1 alpha-2)",
         type=lambda x: x.upper(),
         default="IR",
     )
 
@@ -267,21 +276,21 @@
         action="version",
         version=f"%(prog)s {__version__}",
     )
 
     return checking_args(parser)
 
 
-def restart_v2ray(logger: logging.Logger) -> None:
+def restart_v2ray(logger: logging.Logger, process_name: str = "v2ray") -> None:
     """
     Restart V2Ray service. (systemctl)
     When `check=True` is passed to `run`, `CalledProcessError` is raised if the
     exit code was non-zero.
     """
-    subprocess.run(["systemctl", "restart", "v2ray"], check=True)
+    subprocess.run(["systemctl", "restart", process_name], check=True)
     logger.warning("V2Ray is restarted")
 
 
 def main() -> None:
     """
     Main function.
     """
@@ -295,15 +304,15 @@
 
     # At the first run, we will make a naive configuration file.
     # and all inbounds will route to a randomly selected outbound.
     conf = make_conf(args, logger)
     write_conf(args.config_file, conf)
     logger.info("Naive configuration file is written")
 
-    restart_v2ray(logger)
+    restart_v2ray(logger, args.process_name)
 
     time.sleep(30)
 
     previous_outbound: Optional[str] = None
 
     # Saving records in case of ema flag
     historical_results: list[dict[str, tuple[int, float]]] = []
@@ -327,15 +336,15 @@
         if previous_outbound is None or ranked_outbounds[0] != previous_outbound:
             # Make the new configuration file and set all inbounds to the best inbound.
             conf = make_conf(args, logger, ranked_outbounds[0])
             # Write the new configuration file.
             write_conf(args.config_file, conf)
             logger.info("New configuration file is written")
             # Restarting to apply the new configuration file.
-            restart_v2ray(logger)
+            restart_v2ray(logger, args.process_name)
             previous_outbound = ranked_outbounds[0]
         else:
             logger.info("Keeping same configurations")
 
         # Sleeping until the next checkup.
         logger.info(f"Sleeping for {args.sleep_time:,} seconds")
         time.sleep(args.sleep_time)
```

### Comparing `v2conf-0.1.1/v2conf/configs.py` & `v2conf-0.1.2/v2conf/configs.py`

 * *Files identical despite different names*

### Comparing `v2conf-0.1.1/v2conf/exclude.py` & `v2conf-0.1.2/v2conf/exclude.py`

 * *Files identical despite different names*

### Comparing `v2conf-0.1.1/v2conf/health.py` & `v2conf-0.1.2/v2conf/health.py`

 * *Files identical despite different names*

### Comparing `v2conf-0.1.1/PKG-INFO` & `v2conf-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: v2conf
-Version: 0.1.1
+Version: 0.1.2
 Summary: V2Conf helps you build V2Ray Config file automatically and evaluate and change config rules based on outbounds performances.
 Home-page: https://github.com/mahyar24/V2Conf/
 License: GPL-3.0-or-later
 Keywords: V2Ray,V2Fly,X2Ray
 Author: Mahyar Mahdavi
 Author-email: Mahyar@Mahyar24.com
 Requires-Python: >=3.9,<4.0
@@ -33,15 +33,18 @@
 ## Recommended Usage
 ```bash
 sudo $(which v2conf) /home/ubuntu/confs -n 10 -s 900 --timeout-penalty 15 --ema 8,2 --no-geoip --country-code 'IR' --log-level error --jalali -w "https://dl-cdn.alpinelinux.org/alpine/v3.17/releases/x86/alpine-minirootfs-3.17.1-x86.tar.gz" --log-file /home/ubuntu/v2conf.log 
 ```
 With these flags and settings, V2Conf will download the selected file every 15 minutes (900 / 60 = 15) 10 times for each outbound.\
 V2Conf will print logs in Jalali date times in `/home/ubuntu/v2conf.log` and `stdout` simultaneously and it will exclude IPs for Iran. (useful for domestic Iranian VPSs) \
 `--timeout-penalty 15` makes the program to consider a failed test as a test with 15 seconds latency and based on exponential moving average of last `8` evaluations (past 2 hours) and weighting more importance on recent evaluations (`2` times for every new evaluation) choose the best outbound and route all data within that.\
-`--log-level error` indicates that **V2Ray** log level will be `error`.
+`--log-level error` indicates that **V2Ray** log level will be `error`.\
+For using it with `xray` you can specify `-c /usr/local/etc/xray/config.json` and `-p xray` flags.\
+
+Be aware that **V2Conf only supports V2Fly V4 JSON configs**.
 
 ## Details
 
 V2Conf expects a directory with this structure from you:
 ```bash
 confs/
 ├── inbounds  # an "inbounds" directory
@@ -69,51 +72,52 @@
 ```
 and **all configs must have a tag!**
 P.S.: Thanks to [Tushar](https://github.com/Mahyar24/V2Conf/pull/2) V2Conf now supports JSON5 format for configs.
 
 
 ## Usage
 ```
-$ v2conf --help
-usage: v2conf [-h] [-c CONFIG_FILE] [--country-code COUNTRY_CODE] [--no-geoip] [-t TIMEOUT] [-w WEBSITE] [-n NUM_OF_TRIES] [--timeout-penalty TIMEOUT_PENALTY] [--ema EMA] [-s SLEEP_TIME]
+usage: v2conf [-h] [-c CONFIG_FILE] [-p PROCESS_NAME] [--country-code COUNTRY_CODE] [--no-geoip] [-t TIMEOUT] [-w WEBSITE] [-n NUM_OF_TRIES] [--timeout-penalty TIMEOUT_PENALTY] [--ema EMA] [-s SLEEP_TIME]
                    [-l {debug,info,warning,error,none}] [-q | --log-file LOG_FILE] [--jalali] [-v]
                    [path_conf_dir]
 
 positional arguments:
   path_conf_dir         Select configuration directory, default is $PWD.
 
-optional arguments:
+options:
   -h, --help            show this help message and exit
   -c CONFIG_FILE, --config-file CONFIG_FILE
                         Select configuration file, default is '/usr/local/etc/v2ray/config.json'.
+  -p PROCESS_NAME, --process-name PROCESS_NAME
+                        Select the process name, default is 'v2ray'. If you are using 'xray' set it here and in the custom config file path in '-c' flag.
   --country-code COUNTRY_CODE
                         Exclude a country from the list of IPs to be routed; default is 'IR'. (ISO 3166-1 alpha-2)
   --no-geoip            Instead of using V2Ray GeoIP database, downloading IPs from 'ripe.net' (more recent IPs but may slow V2Ray)
   -t TIMEOUT, --timeout TIMEOUT
                         Set the timeout for checking the health of proxies, default is 15 seconds.
   -w WEBSITE, --website WEBSITE
                         Set the website to be used for checking the health of proxies, default is 'https://facebook.com'.
   -n NUM_OF_TRIES, --num-of-tries NUM_OF_TRIES
                         Set the number of tries for checking the health of proxies, default is 10.
   --timeout-penalty TIMEOUT_PENALTY
                         Converting timeouts to latency by this factor (in seconds), DISABLED by default.
-  --ema EMA             Instead of choosing OutBound based on latest evaluation, rank based on exponential moving average of last Nth tests and smoothing variable. (e.g. --ema 10,2.5), DISABLED by default.
+  --ema EMA             Instead of choosing OutBound based on latest evaluation, rank based on exponential moving average of last Nth tests and smoothing variable. (e.g. --ema 10,2.5) DISABLED by default.
   -s SLEEP_TIME, --sleep-time SLEEP_TIME
                         Set the sleep time between each checkup, default is 1,800s. (in seconds)
   -l {debug,info,warning,error,none}, --log-level {debug,info,warning,error,none}
                         Set the V2Ray log level, default is 'warning'.
   -q, --quiet           No log file (V2Conf). (printing to stdout anyway)
   --log-file LOG_FILE   Path for V2Conf log file. default is '$PWD/V2Conf.log'
   --jalali              Use Jalali datetime for V2Conf logging
   -v, --version         Show version and exit.
 
 Written by: Mahyar Mahdavi <Mahyar@Mahyar24.com>. License: GNU GPLv3. Source Code: <https://github.com/mahyar24/V2Conf>. Reporting Bugs and PRs are welcomed. :)
-
 ```
+
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 
 Contact me: <OSS@Mahyar24.com> :)
 
 ## License
-[GNU GPLv3 ](https://choosealicense.com/licenses/gpl-3.0/)
+[GNU GPLv3](https://choosealicense.com/licenses/gpl-3.0/)
```

