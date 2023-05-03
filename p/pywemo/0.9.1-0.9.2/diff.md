# Comparing `tmp/pywemo-0.9.1.tar.gz` & `tmp/pywemo-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pywemo-0.9.1.tar", max compression
+gzip compressed data, was "pywemo-0.9.2.tar", max compression
```

## Comparing `pywemo-0.9.1.tar` & `pywemo-0.9.2.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0     2831 2022-06-07 18:35:10.703133 pywemo-0.9.1/LICENSE
--rw-r--r--   0        0        0     7426 2022-06-07 18:35:10.703133 pywemo-0.9.1/README.rst
--rw-r--r--   0        0        0     3889 2022-06-07 18:35:10.703133 pywemo-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     1229 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/__init__.py
--rw-r--r--   0        0        0     2762 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/color.py
--rw-r--r--   0        0        0     6857 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/discovery.py
--rw-r--r--   0        0        0     2780 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/exceptions.py
--rw-r--r--   0        0        0     1468 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/LICENSE
--rw-r--r--   0        0        0    27304 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/__init__.py
--rw-r--r--   0        0        0       23 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/__init__.py
--rw-r--r--   0        0        0     3382 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/attributes.py
--rw-r--r--   0        0        0     6691 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/db_orm.py
--rw-r--r--   0        0        0     6032 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/long_press.py
--rw-r--r--   0        0        0    14840 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/rules_db.py
--rw-r--r--   0        0        0    12344 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/service.py
--rw-r--r--   0        0        0      828 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/wemo_services.py
--rw-r--r--   0        0        0     6390 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/wemo_services.pyi
--rw-r--r--   0        0        0       60 2022-06-07 18:35:10.703133 pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/__init__.py
--rw-r--r--   0        0        0   108170 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/device.py
--rw-r--r--   0        0        0     4305 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/device.xsd
--rw-r--r--   0        0        0   106749 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/service.py
--rw-r--r--   0        0        0     3526 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/service.xsd
--rw-r--r--   0        0        0     7086 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd_types.py
--rw-r--r--   0        0        0    17513 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/bridge.py
--rw-r--r--   0        0        0     2707 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/coffeemaker.py
--rw-r--r--   0        0        0     4210 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/crockpot.py
--rw-r--r--   0        0        0     2652 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/dimmer.py
--rw-r--r--   0        0        0     6193 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/humidifier.py
--rw-r--r--   0        0        0     7069 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/insight.py
--rw-r--r--   0        0        0      328 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/lightswitch.py
--rw-r--r--   0        0        0     2320 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/maker.py
--rw-r--r--   0        0        0      141 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/motion.py
--rw-r--r--   0        0        0      157 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/outdoor_plug.py
--rw-r--r--   0        0        0      991 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ouimeaux_device/switch.py
--rw-r--r--   0        0        0        0 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/py.typed
--rw-r--r--   0        0        0    17281 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/ssdp.py
--rw-r--r--   0        0        0    25195 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/subscribe.py
--rw-r--r--   0        0        0     5453 2022-06-07 18:35:10.707133 pywemo-0.9.1/pywemo/util.py
--rw-r--r--   0        0        0     8405 2022-06-07 18:36:45.024146 pywemo-0.9.1/setup.py
--rw-r--r--   0        0        0     8233 2022-06-07 18:36:45.025471 pywemo-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2831 2023-05-03 05:19:33.307345 pywemo-0.9.2/LICENSE
+-rw-r--r--   0        0        0     7426 2023-05-03 05:19:33.307345 pywemo-0.9.2/README.rst
+-rw-r--r--   0        0        0     3876 2023-05-03 05:19:33.307345 pywemo-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     1229 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/__init__.py
+-rw-r--r--   0        0        0     2762 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/color.py
+-rw-r--r--   0        0        0     6857 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/discovery.py
+-rw-r--r--   0        0        0     2780 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/exceptions.py
+-rw-r--r--   0        0        0     1468 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/ouimeaux_device/LICENSE
+-rw-r--r--   0        0        0    26879 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/ouimeaux_device/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-03 05:19:33.307345 pywemo-0.9.2/pywemo/ouimeaux_device/api/__init__.py
+-rw-r--r--   0        0        0     3382 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/attributes.py
+-rw-r--r--   0        0        0     6691 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/db_orm.py
+-rw-r--r--   0        0        0     6030 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/long_press.py
+-rw-r--r--   0        0        0    14840 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/rules_db.py
+-rw-r--r--   0        0        0    12468 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/service.py
+-rw-r--r--   0        0        0      828 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/wemo_services.py
+-rw-r--r--   0        0        0     6838 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/wemo_services.pyi
+-rw-r--r--   0        0        0       60 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/__init__.py
+-rw-r--r--   0        0        0   108170 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/device.py
+-rw-r--r--   0        0        0     4305 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/device.xsd
+-rw-r--r--   0        0        0   106749 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/service.py
+-rw-r--r--   0        0        0     3526 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/service.xsd
+-rw-r--r--   0        0        0     7086 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd_types.py
+-rw-r--r--   0        0        0    17494 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/bridge.py
+-rw-r--r--   0        0        0     2707 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/coffeemaker.py
+-rw-r--r--   0        0        0     4210 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/crockpot.py
+-rw-r--r--   0        0        0     2652 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/dimmer.py
+-rw-r--r--   0        0        0     6193 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/humidifier.py
+-rw-r--r--   0        0        0     7068 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/insight.py
+-rw-r--r--   0        0        0      328 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/lightswitch.py
+-rw-r--r--   0        0        0     2320 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/maker.py
+-rw-r--r--   0        0        0      141 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/motion.py
+-rw-r--r--   0        0        0      157 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/outdoor_plug.py
+-rw-r--r--   0        0        0      991 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ouimeaux_device/switch.py
+-rw-r--r--   0        0        0        0 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/py.typed
+-rw-r--r--   0        0        0    17280 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/ssdp.py
+-rw-r--r--   0        0        0    25195 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/subscribe.py
+-rw-r--r--   0        0        0     5522 2023-05-03 05:19:33.311345 pywemo-0.9.2/pywemo/util.py
+-rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 pywemo-0.9.2/PKG-INFO
```

### Comparing `pywemo-0.9.1/LICENSE` & `pywemo-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/README.rst` & `pywemo-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pyproject.toml` & `pywemo-0.9.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pywemo"
-version = "0.9.1"
+version = "0.9.2"
 description = "Lightweight Python module to discover and control WeMo devices"
 authors = ["Eric Severance <pywemo@esev.com>"]
 license = "MIT"
 
 readme = 'README.rst'
 
 repository = "https://github.com/pywemo/pywemo"
 homepage = "https://github.com/pywemo/pywemo"
 
 keywords = ['wemo', 'api']
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.7.2"
 ifaddr = ">=0.1.0"
 requests = ">=2.0"
 urllib3 = ">=1.26.0"
 lxml = "^4.6"
 
 [tool.poetry.dev-dependencies]
 # toml is used by multiple tools to read this pyproject.toml file
-toml = "^0.10"
+toml = ">=0.10"
 # formatters
-black = "21.10b0"
+black = "23.3.0"
 isort = "^5.6.4"
 # linters/code analysis
-flake8 = ">=3.6.0"
+flake8 = "^5.0.4"
 flake8-docstrings = ">=1.3.0"
-flake8-bugbear = "^20.11.1"
-pylint = "2.12.2"
+flake8-bugbear = ">=20.11.1"
+pylint = "^2.17.3"
 rstcheck = "^3.3.1"
-mypy = ">=0.900"
+mypy = "^1.2.0"
 # testing and code coverage
-pytest = "6.2.5"
+pytest = "^7.3.1"
 pytest-vcr = "1.0.2"
 types-requests = ">=2.0"
-coverage = "^5.4"
-coveralls = "^3.0.0"
+coverage = "^7.2.4"
 # version of generateDS used to create device.py and service.py in .../api/xsd
 generateDS = "2.37.11"
 # other
 pre-commit = "^2.10"
 
 [tool.coverage]
   [tool.coverage.run]
@@ -90,15 +89,15 @@
 [tool.isort]
 profile = "black"
 line_length = 79
 src_paths = ["pywemo", "tests"]
 skip_glob = "*/xsd/*"
 
 [tool.mypy]
-python_version = 3.8
+python_version = "3.10"
 show_error_codes = true
 ignore_missing_imports = true
 strict_equality = true
 warn_incomplete_stub = true
 warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = true
```

### Comparing `pywemo-0.9.1/pywemo/__init__.py` & `pywemo-0.9.2/pywemo/__init__.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/color.py` & `pywemo-0.9.2/pywemo/color.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/discovery.py` & `pywemo-0.9.2/pywemo/discovery.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/exceptions.py` & `pywemo-0.9.2/pywemo/exceptions.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/LICENSE` & `pywemo-0.9.2/pywemo/ouimeaux_device/LICENSE`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/__init__.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 )
                 continue
             return port
         except requests.exceptions.ConnectTimeout:
             # If we timed out connecting, then the wemo is gone,
             # no point in trying further.
             LOG.debug(
-                'Timed out connecting to %s on port %i, ' 'wemo is offline',
+                'Timed out connecting to %s on port %i, wemo is offline',
                 host,
                 port,
             )
             break
         except requests.exceptions.Timeout:
             # Apparently sometimes wemos get into a wedged state where
             # they still accept connections on an old port, but do not
@@ -115,15 +115,15 @@
                 "in a future release.",
                 DeprecationWarning,
             )
         self._state: int | None = None
         self.basic_state_params: dict[str, str] = {}
         self._reconnect_lock = threading.Lock()
         self.session = Session(url)
-        xml = self.session.get(url).content
+        xml = self.session.get(url).data
 
         try:
             super().__init__(**DeviceDescription.dict_from_xml(xml))
         except InvalidSchemaError:
             LOG.debug("Received invalid schema from %s: %r", url, xml)
             raise
 
@@ -367,33 +367,22 @@
                 input=password.encode('utf-8'),
             )
         except FileNotFoundError as exc:
             raise SetupException(
                 'openssl command failed (openssl not installed / not on path?)'
             ) from exc
         except subprocess.CalledProcessError as exc:
-            try:
-                stdout = openssl.stdout.decode(
-                    errors='backslashreplace'
-                ).strip()
-            except UnboundLocalError:
-                stdout = 'not available'
-            try:
-                stderr = openssl.stderr.decode(
-                    errors='backslashreplace'
-                ).strip()
-            except UnboundLocalError:
-                stderr = 'not available'
-            LOG.error('stdout:\n%s', stdout)
-            LOG.error('stderr:\n%s', stderr)
             raise SetupException('openssl command failed') from exc
 
-        # remove 16byte magic and salt prefix inserted by OpenSSL, which is of
-        # the form "Salted__XXXXXXXX" before the actual password
-        encrypted_password = base64.b64encode(openssl.stdout[16:]).decode()
+        output = openssl.stdout
+        if output.startswith(b'Salted__'):
+            # remove 16byte magic and salt prefix inserted by OpenSSL, which
+            # is of the form "Salted__XXXXXXXX" before the actual password
+            output = output[16:]
+        encrypted_password = base64.b64encode(output).decode()
 
         # the last 4 digits that wemo expects is xxyy, where:
         #     xx: length of the encrypted password as hexadecimal
         #     yy: length of the original password as hexadecimal
         n_encrypted = len(encrypted_password)
         n_password = len(password)
         LOG.debug('password length (before encryption): %s', n_password)
@@ -485,15 +474,15 @@
         """
         Connect Wemo to wifi network.
 
         See the setup method for details.
         """
         # a timeout of less than 20 is too short for many devices, so require
         # at least 20 seconds.
-        timeout = min(timeout, 15.0)
+        timeout = max(timeout, 20.0)
         status_delay = min(status_delay, timeout / 2.0)
         connection_attempts = int(max(1, connection_attempts))
 
         # find all access points that the device can see, and select the one
         # matching the desired SSID
         LOG.info('scanning for AP\'s...')
         wifisetup = self.get_service('WiFiSetup')
```

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/attributes.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/attributes.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/db_orm.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/db_orm.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/long_press.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/long_press.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     rules_db: RulesDb, device_name: str, device_udn: str
 ) -> RulesRow:
     """Ensure that a long press rule exists and is enabled for the device.
 
     Returns the long press rule.
     """
     current_rules = rules_db.rules_for_device(rule_type=RULE_TYPE_LONG_PRESS)
-    for (rule, _) in current_rules:
+    for rule, _ in current_rules:
         if rule.State != "1":
             LOG.info("Enabling long press rule for device %s", device_name)
             rule.State = "1"
             rule.update_db(rules_db.cursor())
         return rule
 
     LOG.info("Adding long press rule for device %s", device_name)
```

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/rules_db.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/rules_db.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/service.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,39 +64,39 @@
     takes longer than the timeout.
 
     Since much of pywemo is built atop the requests library, a `content`
     field on HTTPResponse is populated from the `data` field.
     """
 
     # Retry strategy for requests that fail.
-    retries = urllib3.Retry(
+    retries: int | urllib3.Retry | None = urllib3.Retry(
         total=6, backoff_factor=1.5, allowed_methods=['GET', 'POST']
     )
 
     # Seconds that a request can be idle before retrying.
     timeout = 3.0
 
     def __init__(
         self,
         url: str,
-        retries: int | None = None,
+        retries: int | urllib3.Retry | None = None,
         timeout: float | None = None,
     ) -> None:
         """Create a session with the specified default parameters."""
         self.url = url
         if retries is not None:
             self.retries = retries
         if timeout is not None:
             self.timeout = timeout
 
     def request(
         self,
         method: str,
         url: str,
-        retries: int | None = None,
+        retries: int | urllib3.Retry | None = None,
         timeout: float | None = None,
         **kwargs: Any,
     ) -> urllib3.HTTPResponse:
         """Send request and gather response.
 
         A non-200 response code will result in a HTTPException
         exception.
@@ -118,23 +118,25 @@
             timeout = self.timeout
 
         # Create and destroy the pool each time. WeMo devices do not support
         # http keep-alive. Forcing the pool to be destroyed ensures that the
         # http connection is also closed. This avoids tying up TCP sessions
         # on the device.
         with urllib3.PoolManager(retries=retries, timeout=timeout) as pool:
+            response: urllib3.HTTPResponse
             try:
                 response = pool.request(method=method, url=url, **kwargs)
                 if response.status != 200:
                     raise HTTPNotOkException(
                         f"Received status {response.status} for {url}"
                     )
             except urllib3.exceptions.HTTPError as err:
                 raise HTTPException(err) from err
-            response.content = response.data  # For `requests` compatibility.
+            # For `requests` compatibility.
+            response.content = response.data  # type: ignore
             return response
 
     def get(self, url: str, **kwargs: Any) -> urllib3.HTTPResponse:
         """HTTP GET request."""
         return self.request('GET', url, **kwargs)
 
     def post(self, url: str, **kwargs: Any) -> urllib3.HTTPResponse:
@@ -237,15 +239,15 @@
                     session.host,
                     session.port,
                     err,
                     attempt,
                 )
                 last_exception = err
             else:
-                envelope = et.fromstring(response.content)
+                envelope = et.fromstring(response.data)
                 body_element = list(envelope)[0]
                 response_element = list(body_element)[0]
                 if (
                     response_element.tag
                     == "{http://schemas.xmlsoap.org/soap/envelope/}Fault"
                 ):
                     raise SOAPFault(
@@ -278,15 +280,15 @@
         """Create an instance of a Service."""
         self.device = device
         self._config = service
         self.name = self.serviceType.split(':')[-2]
         self.actions = {}
 
         url = device.session.urljoin(service.description_url)
-        xml = device.session.get(url).content
+        xml = device.session.get(url).data
 
         try:
             scpd = ServiceDescription.from_xml(xml)
         except InvalidSchemaError:
             LOG.debug("Received invalid schema from %s: %r", url, xml)
             raise
```

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/wemo_services.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/wemo_services.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/wemo_services.pyi` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/wemo_services.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -111,14 +111,20 @@
     SetDataStores: UPnPMethod
     SetDeviceName: UPnPMethod
     SetDeviceNames: UPnPMethod
     SetDeviceStatus: UPnPMethod
     SetZigbeeMode: UPnPMethod
     UpgradeSubDeviceFirmware: UPnPMethod
 
+class Service_crockpotevent:
+    GetCrockpotState: UPnPMethod
+    GetJardenStatus: UPnPMethod
+    SetCrockpotState: UPnPMethod
+    SetJardenStatus: UPnPMethod
+
 class Service_deviceevent:
     GetAttributeList: UPnPMethod
     GetAttributes: UPnPMethod
     GetBlobStorage: UPnPMethod
     SetAttributes: UPnPMethod
     SetBlobStorage: UPnPMethod
 
@@ -151,14 +157,20 @@
     GetTodayONTime: UPnPMethod
     GetTodaySBYTime: UPnPMethod
     ResetPowerThreshold: UPnPMethod
     ScheduleDataExport: UPnPMethod
     SetAutoPowerThreshold: UPnPMethod
     SetPowerThreshold: UPnPMethod
 
+class Service_jardenevent:
+    GetCrockpotState: UPnPMethod
+    GetJardenStatus: UPnPMethod
+    SetCrockpotState: UPnPMethod
+    SetJardenStatus: UPnPMethod
+
 class Service_manufacture:
     GetManufactureData: UPnPMethod
 
 class Service_metainfo:
     GetExtMetaInfo: UPnPMethod
     GetMetaInfo: UPnPMethod
 
@@ -192,33 +204,37 @@
     GetTime: UPnPMethod
     TimeSync: UPnPMethod
 
 class WeMoServiceTypesMixin:
     WiFiSetup: Service_WiFiSetup
     basicevent: Service_basicevent
     bridge: Service_bridge
+    crockpotevent: Service_crockpotevent
     deviceevent: Service_deviceevent
     deviceinfo: Service_deviceinfo
     firmwareupdate: Service_firmwareupdate
     insight: Service_insight
+    jardenevent: Service_jardenevent
     manufacture: Service_manufacture
     metainfo: Service_metainfo
     remoteaccess: Service_remoteaccess
     rules: Service_rules
     smartsetup: Service_smartsetup
     timesync: Service_timesync
 
 class WeMoAllActionsMixin(
     Service_WiFiSetup,
     Service_basicevent,
     Service_bridge,
+    Service_crockpotevent,
     Service_deviceevent,
     Service_deviceinfo,
     Service_firmwareupdate,
     Service_insight,
+    Service_jardenevent,
     Service_manufacture,
     Service_metainfo,
     Service_remoteaccess,
     Service_rules,
     Service_smartsetup,
     Service_timesync,
 ):
```

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/device.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/device.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/device.xsd` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/device.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/service.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/service.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd/service.xsd` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd/service.xsd`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/api/xsd_types.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/api/xsd_types.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/bridge.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/bridge.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
         available: bool
         onoff: int
         level: int
         temperature_mireds: int
         temperature_kelvin: int
         color_xy: ColorXY
 
-
 else:
     from typing import Dict, Union
 
     DeviceState = Dict[str, Union[ColorXY, bool, int]]
 
 
 class LinkedDevice:
@@ -260,16 +259,15 @@
         # Update only the capability/value pair that changed.
         try:
             index = self.capabilities.index(name)
         except ValueError:
             # Should't receive updates for capabilities that were not
             # originally present.
             return False
-        else:
-            self._values[index] = value
+        self._values[index] = value
 
         # Don't call the subclass. It expects to have a list of all the
         # capability/value pairs. The subscription_update only receives a
         # single capability/value pair.
         LinkedDevice.update_state(self, {})
         return True
```

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/coffeemaker.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/coffeemaker.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/crockpot.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/crockpot.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/dimmer.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/dimmer.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/humidifier.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/humidifier.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/insight.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/insight.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
         ontotal: int
         todaymw: int
         totalmw: int
         currentpower: int
         wifipower: int
         powerthreshold: int
 
-
 else:
     from typing import Dict, Union
 
     InsightParams = Dict[str, Union[str, datetime, int]]
 
 
 class Insight(Switch):
```

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/maker.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/maker.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ouimeaux_device/switch.py` & `pywemo-0.9.2/pywemo/ouimeaux_device/switch.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/ssdp.py` & `pywemo-0.9.2/pywemo/ssdp.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
         """Scan for new uPnP devices and services."""
         with self._lock:
             if (
                 self.last_scan is None
                 or force_update
                 or datetime.now() - self.last_scan > MIN_TIME_BETWEEN_SCANS
             ):
-
                 self.remove_expired()
 
                 self.entries.extend(
                     entry
                     for entry in scan() + scan(ST)
                     if entry not in self.entries
                 )
```

### Comparing `pywemo-0.9.1/pywemo/subscribe.py` & `pywemo-0.9.2/pywemo/subscribe.py`

 * *Files identical despite different names*

### Comparing `pywemo-0.9.1/pywemo/util.py` & `pywemo-0.9.2/pywemo/util.py`

 * *Files 3% similar despite different names*

```diff
@@ -58,15 +58,17 @@
     Return local address of any network associated with a local interface
     that has broadcast (and probably multicast) capability.
     """
     addresses = []
 
     for iface in ifaddr.get_adapters():
         for addr in iface.ips:
-            if not addr.is_IPv4 or addr.ip == '127.0.0.1':
+            if not (addr.is_IPv4 and isinstance(addr.ip, str)):
+                continue
+            if addr.ip == '127.0.0.1':
                 continue
 
             addresses.append(addr.ip)
 
     return addresses
```

### Comparing `pywemo-0.9.1/setup.py` & `pywemo-0.9.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,180 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pywemo
+Version: 0.9.2
+Summary: Lightweight Python module to discover and control WeMo devices
+Home-page: https://github.com/pywemo/pywemo
+License: MIT
+Keywords: wemo,api
+Author: Eric Severance
+Author-email: pywemo@esev.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: ifaddr (>=0.1.0)
+Requires-Dist: lxml (>=4.6,<5.0)
+Requires-Dist: requests (>=2.0)
+Requires-Dist: urllib3 (>=1.26.0)
+Project-URL: Repository, https://github.com/pywemo/pywemo
+Description-Content-Type: text/x-rst
+
+pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge|
+===========================================================================
+Python 3 module to setup, discover and control WeMo devices.
+
+Dependencies
+------------
+pyWeMo depends on Python packages: requests, ifaddr, lxml, urllib3
+
+How to use
+----------
+
+.. code-block:: python
+
+    >>> import pywemo
+    >>> devices = pywemo.discover_devices()
+    >>> print(devices)
+    [<WeMo Insight "AC Insight">]
+
+    >>> devices[0].toggle()
+
+For advanced usage, the ``device.explain()`` method will print all known actions that the device reports to PyWeMo.
+
+If discovery doesn't work on your network
+-----------------------------------------
+Automatic discovery may not work reliably on some networks.
+In that case, you can use the device with an IP or hostname:
+
+.. code-block:: python
+
+    >>> import pywemo
+    >>> url = pywemo.setup_url_for_address("192.168.1.192")
+    >>> print(url)
+    http://192.168.1.192:49153/setup.xml
+    >>> device = pywemo.discovery.device_from_description(url)
+    >>> print(device)
+    <WeMo Maker "Hi Fi Systemline Sensor">
+
+Please note that ``discovery.device_from_description`` requires a ``url`` with an IP address, rather than a hostname.
+This is needed for the subscription update logic to work properly.
+In addition, recent versions of the WeMo firmware may not accept connections from hostnames and will return a 500 error.
+
+The ``setup_url_for_address`` function will lookup a hostname and provide a suitable ``url`` with an IP address.
+
+If the WeMo device is not on your network, you can also connect to it directly.
+After connecting, if the ``pywemo.discover_devices()`` doesn't work, you can get the IP Address by running an ``arp -a`` and use that in ``pywemo.setup_url_for_address``:
+
+.. code-block::
+
+    $ arp -a
+    _gateway (10.22.22.1) at [MAC ADDRESS REMOVED] [ether]
+    
+.. code-block:: python
+
+    >>> import pywemo
+    >>> url = pywemo.setup_url_for_address("10.22.22.1")
+    >>> device = pywemo.discovery.device_from_description(url)
+    >>> print(device)
+    <WeMo Switch "Wemo Mini">
+    >>> device.setup(ssid='MY SSID', password='MY NETWORK PASSWORD')
+    ('1', 'success')
+
+
+
+Testing new products
+--------------------
+If both methods above are not successful, then ``pywemo`` may not support your WeMo product yet.
+This may be particularly true if it is a new WeMo product.
+To test this, you can use a debug flag, ``pywemo.discover_devices(debug=True)`` or ``pywemo.discovery.device_from_description(url, debug=True)``.
+If an ``UnsupportedDevice`` is found, then it is highly likely that the product can be added to ``pywemo``.
+This ``UnsupportedDevice`` will allow manual interaction, but please open an issue to get first class support for the device.
+
+Device Reset and Setup
+----------------------
+PyWeMo includes the ability to reset and setup devices, without using the Belkin app or needing to create a Belkin account.
+This can be particularly useful if the intended use is fully local control, such as using Home Assistant.
+
+Reset
+~~~~~
+Reset can be performed with the ``reset`` method, which has 2 boolean input arguments, ``data`` and ``wifi``.
+WeMo devices contain a hardware reset procedure as well, so use of ``pywemo`` is for convenience or if physical access is not available.
+This ``reset`` method may not work on all devices.
+
+=======================================  =================  =======================
+Method in ``pywemo``                     Clears             Name in WeMo App
+=======================================  =================  =======================
+``device.reset(data=True, wifi=False)``  name, icon, rules  Clear Personalized Info
+``device.reset(data=False, wifi=True)``  wifi information   Change Wi-Fi
+``device.reset(data=True, wifi=True)``   everything         Factory Restore
+=======================================  =================  =======================
+
+Setup
+~~~~~
+
+Device setup is through the ``setup`` method, which has two required arguments: ``ssid`` and ``password``.
+The user must first connect to the devices locally broadcast access point, which typically starts with "WeMo.", and then discover the device there.
+Once done, pass the desired SSID and password (WPA2/AES encryption only) to the ``setup`` method to connect it to your wifi network.
+
+``device.setup(ssid='wifi_name', password='special_secret')``
+
+A few important notes:
+
+- Not all devices are currently supported for setup.
+- For a WeMo without internet access, see `this guide <https://github.com/pywemo/pywemo/wiki/WeMo-Cloud#disconnecting-from-the-cloud>`_ to stop any blinking lights.
+- If connecting to an open network, the password argument is ignored and you can provide anything, e.g. ``password=None``.
+- If connecting to a WPA2/AES-encrypted network, OpenSSL is used to encrypt the password by the ``pywemo`` library.
+  It must be installed and available on your ``PATH`` via calling ``openssl`` from a terminal or command prompt.
+
+Firmware Warning
+----------------
+Starting in May of 2020, Belkin started requiring users to create an account and login to the app (Android app version 1.25).
+In addition to the account, most of the app functionality now requires a connection to the cloud (internet access), even for simple actions such as toggling a switch.
+All of the commands that go through the cloud are encrypted and cannot be easily inspected.
+This raises the possibility that Belkin could, in the future, update WeMo device firmware and make breaking API changes that can no longer be deciphered.
+If this happens, ``pywemo`` may no longer function on that device.
+Thus it would be prudent to upgrade firmware cautiously and preferably only after confirming that breaking API changes have not been introduced.
+
+Developing
+----------
+Setup and builds are fully automated.
+You can run the build pipeline locally via:
+
+.. code-block::
+
+    # setup, install, format, lint, test and build:
+    ./scripts/build.sh
+
+Note that this will install a git ``pre-commit`` hook.
+For this hook to work correctly, ``poetry`` needs to be globally accessible on your ``PATH`` or the local virtual environment must be activated.
+This virtual environment can be activated with:
+
+.. code-block::
+
+    . .venv/bin/activate
+
+History
+-------
+This started as a stripped down version of `ouimeaux <https://github.com/iancmcc/ouimeaux>`_, copyright Ian McCracken, but has since taken its own path.
+
+License
+-------
+All contents of the pywemo/ouimeaux_device directory are licensed under a BSD 3-Clause license. The full text of that license is maintained within the pywemo/ouimeaux_device/LICENSE file.
+The rest of pyWeMo is released under the MIT license. See the top-level LICENSE file for more details.
+
+
+.. |Build Badge| image:: https://github.com/pywemo/pywemo/workflows/Build/badge.svg
+    :target: https://github.com/pywemo/pywemo/actions?query=workflow%3ABuild
+    :alt: GitHub build status
+.. |PyPI Version Badge| image:: https://img.shields.io/pypi/v/pywemo
+    :target: https://pypi.org/project/pywemo/
+    :alt: Latest PyPI version
+.. |Coverage| image:: https://coveralls.io/repos/github/pywemo/pywemo/badge.svg?branch=main
+    :target: https://coveralls.io/github/pywemo/pywemo?branch=main
+    :alt: Coveralls coverage
+.. |PyPI Downloads Badge| image:: https://img.shields.io/pypi/dm/pywemo
+    :target: https://pypi.org/project/pywemo/
+    :alt: Number of PyPI downloads
 
-packages = \
-['pywemo',
- 'pywemo.ouimeaux_device',
- 'pywemo.ouimeaux_device.api',
- 'pywemo.ouimeaux_device.api.xsd']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['ifaddr>=0.1.0', 'lxml>=4.6,<5.0', 'requests>=2.0', 'urllib3>=1.26.0']
-
-setup_kwargs = {
-    'name': 'pywemo',
-    'version': '0.9.1',
-    'description': 'Lightweight Python module to discover and control WeMo devices',
-    'long_description': 'pyWeMo |Build Badge| |PyPI Version Badge| |Coverage| |PyPI Downloads Badge|\n===========================================================================\nPython 3 module to setup, discover and control WeMo devices.\n\nDependencies\n------------\npyWeMo depends on Python packages: requests, ifaddr, lxml, urllib3\n\nHow to use\n----------\n\n.. code-block:: python\n\n    >>> import pywemo\n    >>> devices = pywemo.discover_devices()\n    >>> print(devices)\n    [<WeMo Insight "AC Insight">]\n\n    >>> devices[0].toggle()\n\nFor advanced usage, the ``device.explain()`` method will print all known actions that the device reports to PyWeMo.\n\nIf discovery doesn\'t work on your network\n-----------------------------------------\nAutomatic discovery may not work reliably on some networks.\nIn that case, you can use the device with an IP or hostname:\n\n.. code-block:: python\n\n    >>> import pywemo\n    >>> url = pywemo.setup_url_for_address("192.168.1.192")\n    >>> print(url)\n    http://192.168.1.192:49153/setup.xml\n    >>> device = pywemo.discovery.device_from_description(url)\n    >>> print(device)\n    <WeMo Maker "Hi Fi Systemline Sensor">\n\nPlease note that ``discovery.device_from_description`` requires a ``url`` with an IP address, rather than a hostname.\nThis is needed for the subscription update logic to work properly.\nIn addition, recent versions of the WeMo firmware may not accept connections from hostnames and will return a 500 error.\n\nThe ``setup_url_for_address`` function will lookup a hostname and provide a suitable ``url`` with an IP address.\n\nIf the WeMo device is not on your network, you can also connect to it directly.\nAfter connecting, if the ``pywemo.discover_devices()`` doesn\'t work, you can get the IP Address by running an ``arp -a`` and use that in ``pywemo.setup_url_for_address``:\n\n.. code-block::\n\n    $ arp -a\n    _gateway (10.22.22.1) at [MAC ADDRESS REMOVED] [ether]\n    \n.. code-block:: python\n\n    >>> import pywemo\n    >>> url = pywemo.setup_url_for_address("10.22.22.1")\n    >>> device = pywemo.discovery.device_from_description(url)\n    >>> print(device)\n    <WeMo Switch "Wemo Mini">\n    >>> device.setup(ssid=\'MY SSID\', password=\'MY NETWORK PASSWORD\')\n    (\'1\', \'success\')\n\n\n\nTesting new products\n--------------------\nIf both methods above are not successful, then ``pywemo`` may not support your WeMo product yet.\nThis may be particularly true if it is a new WeMo product.\nTo test this, you can use a debug flag, ``pywemo.discover_devices(debug=True)`` or ``pywemo.discovery.device_from_description(url, debug=True)``.\nIf an ``UnsupportedDevice`` is found, then it is highly likely that the product can be added to ``pywemo``.\nThis ``UnsupportedDevice`` will allow manual interaction, but please open an issue to get first class support for the device.\n\nDevice Reset and Setup\n----------------------\nPyWeMo includes the ability to reset and setup devices, without using the Belkin app or needing to create a Belkin account.\nThis can be particularly useful if the intended use is fully local control, such as using Home Assistant.\n\nReset\n~~~~~\nReset can be performed with the ``reset`` method, which has 2 boolean input arguments, ``data`` and ``wifi``.\nWeMo devices contain a hardware reset procedure as well, so use of ``pywemo`` is for convenience or if physical access is not available.\nThis ``reset`` method may not work on all devices.\n\n=======================================  =================  =======================\nMethod in ``pywemo``                     Clears             Name in WeMo App\n=======================================  =================  =======================\n``device.reset(data=True, wifi=False)``  name, icon, rules  Clear Personalized Info\n``device.reset(data=False, wifi=True)``  wifi information   Change Wi-Fi\n``device.reset(data=True, wifi=True)``   everything         Factory Restore\n=======================================  =================  =======================\n\nSetup\n~~~~~\n\nDevice setup is through the ``setup`` method, which has two required arguments: ``ssid`` and ``password``.\nThe user must first connect to the devices locally broadcast access point, which typically starts with "WeMo.", and then discover the device there.\nOnce done, pass the desired SSID and password (WPA2/AES encryption only) to the ``setup`` method to connect it to your wifi network.\n\n``device.setup(ssid=\'wifi_name\', password=\'special_secret\')``\n\nA few important notes:\n\n- Not all devices are currently supported for setup.\n- For a WeMo without internet access, see `this guide <https://github.com/pywemo/pywemo/wiki/WeMo-Cloud#disconnecting-from-the-cloud>`_ to stop any blinking lights.\n- If connecting to an open network, the password argument is ignored and you can provide anything, e.g. ``password=None``.\n- If connecting to a WPA2/AES-encrypted network, OpenSSL is used to encrypt the password by the ``pywemo`` library.\n  It must be installed and available on your ``PATH`` via calling ``openssl`` from a terminal or command prompt.\n\nFirmware Warning\n----------------\nStarting in May of 2020, Belkin started requiring users to create an account and login to the app (Android app version 1.25).\nIn addition to the account, most of the app functionality now requires a connection to the cloud (internet access), even for simple actions such as toggling a switch.\nAll of the commands that go through the cloud are encrypted and cannot be easily inspected.\nThis raises the possibility that Belkin could, in the future, update WeMo device firmware and make breaking API changes that can no longer be deciphered.\nIf this happens, ``pywemo`` may no longer function on that device.\nThus it would be prudent to upgrade firmware cautiously and preferably only after confirming that breaking API changes have not been introduced.\n\nDeveloping\n----------\nSetup and builds are fully automated.\nYou can run the build pipeline locally via:\n\n.. code-block::\n\n    # setup, install, format, lint, test and build:\n    ./scripts/build.sh\n\nNote that this will install a git ``pre-commit`` hook.\nFor this hook to work correctly, ``poetry`` needs to be globally accessible on your ``PATH`` or the local virtual environment must be activated.\nThis virtual environment can be activated with:\n\n.. code-block::\n\n    . .venv/bin/activate\n\nHistory\n-------\nThis started as a stripped down version of `ouimeaux <https://github.com/iancmcc/ouimeaux>`_, copyright Ian McCracken, but has since taken its own path.\n\nLicense\n-------\nAll contents of the pywemo/ouimeaux_device directory are licensed under a BSD 3-Clause license. The full text of that license is maintained within the pywemo/ouimeaux_device/LICENSE file.\nThe rest of pyWeMo is released under the MIT license. See the top-level LICENSE file for more details.\n\n\n.. |Build Badge| image:: https://github.com/pywemo/pywemo/workflows/Build/badge.svg\n    :target: https://github.com/pywemo/pywemo/actions?query=workflow%3ABuild\n    :alt: GitHub build status\n.. |PyPI Version Badge| image:: https://img.shields.io/pypi/v/pywemo\n    :target: https://pypi.org/project/pywemo/\n    :alt: Latest PyPI version\n.. |Coverage| image:: https://coveralls.io/repos/github/pywemo/pywemo/badge.svg?branch=main\n    :target: https://coveralls.io/github/pywemo/pywemo?branch=main\n    :alt: Coveralls coverage\n.. |PyPI Downloads Badge| image:: https://img.shields.io/pypi/dm/pywemo\n    :target: https://pypi.org/project/pywemo/\n    :alt: Number of PyPI downloads\n',
-    'author': 'Eric Severance',
-    'author_email': 'pywemo@esev.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/pywemo/pywemo',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

