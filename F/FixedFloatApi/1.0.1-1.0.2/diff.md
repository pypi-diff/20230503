# Comparing `tmp/FixedFloatApi-1.0.1.tar.gz` & `tmp/FixedFloatApi-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/FixedFloatApi-1.0.1.tar", last modified: Tue May  2 21:55:05 2023, max compression
+gzip compressed data, was "dist/FixedFloatApi-1.0.2.tar", last modified: Tue May  2 22:50:38 2023, max compression
```

## Comparing `FixedFloatApi-1.0.1.tar` & `FixedFloatApi-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/
--rw-rw-r--   0 root         (0) root         (0)     3250 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      293 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)       14 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/FixedFloatApi.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)     1060 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/LICENSE.txt
--rw-rw-r--   0 root         (0) root         (0)       38 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)     3250 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1848 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/README.md
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/fixedfloatapi/
--rw-rw-r--   0 root         (0) root         (0)     1522 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/fixedfloatapi/FixedFloatAPI.py
--rw-rw-r--   0 root         (0) root         (0)       38 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/fixedfloatapi/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       79 2023-05-02 21:55:05.000000 FixedFloatApi-1.0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1017 2023-05-02 21:50:09.000000 FixedFloatApi-1.0.1/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)     2834 2023-05-02 22:50:37.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      293 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2023-05-02 22:50:37.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2023-05-02 22:50:37.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)       14 2023-05-02 22:50:37.000000 FixedFloatApi-1.0.2/FixedFloatApi.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)     1060 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/LICENSE.txt
+-rw-rw-r--   0 root         (0) root         (0)       38 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)     2834 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1488 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/README.md
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/fixedfloatapi/
+-rw-rw-r--   0 root         (0) root         (0)     1522 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/fixedfloatapi/FixedFloatAPI.py
+-rw-rw-r--   0 root         (0) root         (0)       54 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/fixedfloatapi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)       79 2023-05-02 22:50:38.000000 FixedFloatApi-1.0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1017 2023-05-02 22:47:11.000000 FixedFloatApi-1.0.2/setup.py
```

### Comparing `FixedFloatApi-1.0.1/FixedFloatApi.egg-info/PKG-INFO` & `FixedFloatApi-1.0.2/FixedFloatApi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,93 +1,86 @@
 Metadata-Version: 2.1
 Name: FixedFloatApi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.
 Home-page: https://github.com/Jobians/FixedFloatApi
 Author: JobiansTechie
 Author-email: jobianstechie@gmail.com
 License: MIT
-Description: FixedFloatApi
-        =============
+Description: ## Installation
         
-        A Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.
+        ```bash
+        pip install FixedFloatApi
+        ```
+        
+        ## Usage
+        
+        ```python
+        from fixedfloatapi import FixedFloatApi
+        
+        # create a new API client
+        api = FixedFloatApi(key='YOUR_API_KEY', secret='YOUR_API_SECRET')
+        
+        # Get a list of supported currencies
+        ccies = api.ccies()
+        print(ccies)
+        
+        # Get the current price for an exchange
+        price = api.price({
+            'fromCcy': 'BTC',
+            'toCcy': 'ETH',
+            'amount': 1.0,
+            'direction': 'from',
+            'type': 'fixed' # or 'float'
+        })
+        print(price)
+        
+        # Create a new exchange order
+        order = api.create({
+            'fromCcy': 'BTC',
+            'toCcy': 'ETH',
+            'amount': 1.0,
+            'direction': 'from',
+            'type': 'fixed', # or 'float'
+            'toAddress': '0x123...'
+        })
+        print(order)
+        
+        # Place an order for an existing exchange
+        order_status = api.order({
+            'id': '12345',
+            'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7'
+        })
+        print(order_status)
+        
+        # Request emergency assistance for an exchange
+        emergency = api.emergency({
+            'id': '12345',
+            'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+            'choice': 'EXCHANGE'
+        })
+        print(emergency)
+        
+        # set email address for order notifications
+        set_email = api.setEmail({
+            'id': 'TESTID',
+            'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+            'email': 'notifyme@gmail.com',
+        })
+        print(set_email)
+        
+        # get a QR code for a trade
+        qr_code = api.qr({
+            'id': 'TESTID',
+            'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+        })
+        print(qr_code)
+        ```
         
-        Installation
-        ------------
-        
-        .. code-block:: bash
-        
-            pip install FixedFloatApi
-        
-        Usage
-        -----
-        
-        .. code-block:: python
-        
-            from fixedfloatapi import FixedFloatApi
-        
-            # create a new API client
-            api = FixedFloatApi(key='YOUR_API_KEY', secret='YOUR_API_SECRET')
-        
-            # Get a list of supported currencies
-            ccies = api.ccies()
-            print(ccies)
-        
-            # Get the current price for an exchange
-            price = api.price({
-                'fromCcy': 'BTC',
-                'toCcy': 'ETH',
-                'amount': 1.0,
-                'direction': 'from',
-                'type': 'fixed' # or 'float'
-            })
-            print(price)
-        
-            # Create a new exchange order
-            order = api.create({
-                'fromCcy': 'BTC',
-                'toCcy': 'ETH',
-                'amount': 1.0,
-                'direction': 'from',
-                'type': 'fixed', # or 'float'
-                'toAddress': '0x123...'
-            })
-            print(order)
-        
-            # Place an order for an existing exchange
-            order_status = api.order({
-                'id': '12345',
-                'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7'
-            })
-            print(order_status)
-        
-            # Request emergency assistance for an exchange
-            emergency = api.emergency({
-                'id': '12345',
-                'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-                'choice': 'EXCHANGE'
-            })
-            print(emergency)
-        
-            # set email address for order notifications
-            set_email = api.setEmail({
-                'id': 'TESTID',
-                'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-                'email': 'notifyme@gmail.com',
-            })
-            print(set_email)
-        
-            # get a QR code for a trade
-            qr_code = api.qr({
-                'id': 'TESTID',
-                'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-            })
-            print(qr_code)
-        
-        For more information, see the `API documentation <https://fixedfloat.com/api>`_.
+        For more information, see the [API documentation](https://fixedfloat.com/api).
         
 Keywords: FixedFloat,Api,FixedFloat Python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FixedFloatApi-1.0.1/LICENSE.txt` & `FixedFloatApi-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FixedFloatApi-1.0.1/PKG-INFO` & `FixedFloatApi-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,93 +1,86 @@
 Metadata-Version: 2.1
 Name: FixedFloatApi
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.
 Home-page: https://github.com/Jobians/FixedFloatApi
 Author: JobiansTechie
 Author-email: jobianstechie@gmail.com
 License: MIT
-Description: FixedFloatApi
-        =============
+Description: ## Installation
         
-        A Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.
+        ```bash
+        pip install FixedFloatApi
+        ```
+        
+        ## Usage
+        
+        ```python
+        from fixedfloatapi import FixedFloatApi
+        
+        # create a new API client
+        api = FixedFloatApi(key='YOUR_API_KEY', secret='YOUR_API_SECRET')
+        
+        # Get a list of supported currencies
+        ccies = api.ccies()
+        print(ccies)
+        
+        # Get the current price for an exchange
+        price = api.price({
+            'fromCcy': 'BTC',
+            'toCcy': 'ETH',
+            'amount': 1.0,
+            'direction': 'from',
+            'type': 'fixed' # or 'float'
+        })
+        print(price)
+        
+        # Create a new exchange order
+        order = api.create({
+            'fromCcy': 'BTC',
+            'toCcy': 'ETH',
+            'amount': 1.0,
+            'direction': 'from',
+            'type': 'fixed', # or 'float'
+            'toAddress': '0x123...'
+        })
+        print(order)
+        
+        # Place an order for an existing exchange
+        order_status = api.order({
+            'id': '12345',
+            'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7'
+        })
+        print(order_status)
+        
+        # Request emergency assistance for an exchange
+        emergency = api.emergency({
+            'id': '12345',
+            'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+            'choice': 'EXCHANGE'
+        })
+        print(emergency)
+        
+        # set email address for order notifications
+        set_email = api.setEmail({
+            'id': 'TESTID',
+            'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+            'email': 'notifyme@gmail.com',
+        })
+        print(set_email)
+        
+        # get a QR code for a trade
+        qr_code = api.qr({
+            'id': 'TESTID',
+            'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+        })
+        print(qr_code)
+        ```
         
-        Installation
-        ------------
-        
-        .. code-block:: bash
-        
-            pip install FixedFloatApi
-        
-        Usage
-        -----
-        
-        .. code-block:: python
-        
-            from fixedfloatapi import FixedFloatApi
-        
-            # create a new API client
-            api = FixedFloatApi(key='YOUR_API_KEY', secret='YOUR_API_SECRET')
-        
-            # Get a list of supported currencies
-            ccies = api.ccies()
-            print(ccies)
-        
-            # Get the current price for an exchange
-            price = api.price({
-                'fromCcy': 'BTC',
-                'toCcy': 'ETH',
-                'amount': 1.0,
-                'direction': 'from',
-                'type': 'fixed' # or 'float'
-            })
-            print(price)
-        
-            # Create a new exchange order
-            order = api.create({
-                'fromCcy': 'BTC',
-                'toCcy': 'ETH',
-                'amount': 1.0,
-                'direction': 'from',
-                'type': 'fixed', # or 'float'
-                'toAddress': '0x123...'
-            })
-            print(order)
-        
-            # Place an order for an existing exchange
-            order_status = api.order({
-                'id': '12345',
-                'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7'
-            })
-            print(order_status)
-        
-            # Request emergency assistance for an exchange
-            emergency = api.emergency({
-                'id': '12345',
-                'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-                'choice': 'EXCHANGE'
-            })
-            print(emergency)
-        
-            # set email address for order notifications
-            set_email = api.setEmail({
-                'id': 'TESTID',
-                'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-                'email': 'notifyme@gmail.com',
-            })
-            print(set_email)
-        
-            # get a QR code for a trade
-            qr_code = api.qr({
-                'id': 'TESTID',
-                'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-            })
-            print(qr_code)
-        
-        For more information, see the `API documentation <https://fixedfloat.com/api>`_.
+        For more information, see the [API documentation](https://fixedfloat.com/api).
         
 Keywords: FixedFloat,Api,FixedFloat Python
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FixedFloatApi-1.0.1/README.md` & `FixedFloatApi-1.0.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,71 @@
-FixedFloatApi
-=============
+## Installation
 
-A Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.
+```bash
+pip install FixedFloatApi
+```
+
+## Usage
+
+```python
+from fixedfloatapi import FixedFloatApi
+
+# create a new API client
+api = FixedFloatApi(key='YOUR_API_KEY', secret='YOUR_API_SECRET')
+
+# Get a list of supported currencies
+ccies = api.ccies()
+print(ccies)
+
+# Get the current price for an exchange
+price = api.price({
+    'fromCcy': 'BTC',
+    'toCcy': 'ETH',
+    'amount': 1.0,
+    'direction': 'from',
+    'type': 'fixed' # or 'float'
+})
+print(price)
+
+# Create a new exchange order
+order = api.create({
+    'fromCcy': 'BTC',
+    'toCcy': 'ETH',
+    'amount': 1.0,
+    'direction': 'from',
+    'type': 'fixed', # or 'float'
+    'toAddress': '0x123...'
+})
+print(order)
+
+# Place an order for an existing exchange
+order_status = api.order({
+    'id': '12345',
+    'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7'
+})
+print(order_status)
+
+# Request emergency assistance for an exchange
+emergency = api.emergency({
+    'id': '12345',
+    'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+    'choice': 'EXCHANGE'
+})
+print(emergency)
+
+# set email address for order notifications
+set_email = api.setEmail({
+    'id': 'TESTID',
+    'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+    'email': 'notifyme@gmail.com',
+})
+print(set_email)
+
+# get a QR code for a trade
+qr_code = api.qr({
+    'id': 'TESTID',
+    'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
+})
+print(qr_code)
+```
 
-Installation
-------------
-
-.. code-block:: bash
-
-    pip install FixedFloatApi
-
-Usage
------
-
-.. code-block:: python
-
-    from fixedfloatapi import FixedFloatApi
-
-    # create a new API client
-    api = FixedFloatApi(key='YOUR_API_KEY', secret='YOUR_API_SECRET')
-
-    # Get a list of supported currencies
-    ccies = api.ccies()
-    print(ccies)
-
-    # Get the current price for an exchange
-    price = api.price({
-        'fromCcy': 'BTC',
-        'toCcy': 'ETH',
-        'amount': 1.0,
-        'direction': 'from',
-        'type': 'fixed' # or 'float'
-    })
-    print(price)
-
-    # Create a new exchange order
-    order = api.create({
-        'fromCcy': 'BTC',
-        'toCcy': 'ETH',
-        'amount': 1.0,
-        'direction': 'from',
-        'type': 'fixed', # or 'float'
-        'toAddress': '0x123...'
-    })
-    print(order)
-
-    # Place an order for an existing exchange
-    order_status = api.order({
-        'id': '12345',
-        'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7'
-    })
-    print(order_status)
-
-    # Request emergency assistance for an exchange
-    emergency = api.emergency({
-        'id': '12345',
-        'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-        'choice': 'EXCHANGE'
-    })
-    print(emergency)
-
-    # set email address for order notifications
-    set_email = api.setEmail({
-        'id': 'TESTID',
-        'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-        'email': 'notifyme@gmail.com',
-    })
-    print(set_email)
-
-    # get a QR code for a trade
-    qr_code = api.qr({
-        'id': 'TESTID',
-        'token': 'TESTTOKENvRB90NOtr397kHY3PJ1VRy2p29HHaN7',
-    })
-    print(qr_code)
-
-For more information, see the `API documentation <https://fixedfloat.com/api>`_.
+For more information, see the [API documentation](https://fixedfloat.com/api).
```

### Comparing `FixedFloatApi-1.0.1/fixedfloatapi/FixedFloatAPI.py` & `FixedFloatApi-1.0.2/fixedfloatapi/FixedFloatAPI.py`

 * *Files identical despite different names*

### Comparing `FixedFloatApi-1.0.1/setup.py` & `FixedFloatApi-1.0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FixedFloatApi',
     packages=find_packages(),
     include_package_data=True,
-    version='1.0.1',
+    version='1.0.2',
     license='MIT',
     description='Python wrapper for interacting with the FixedFloat API to exchange cryptocurrencies.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='JobiansTechie',
     author_email='jobianstechie@gmail.com',
     url='https://github.com/Jobians/FixedFloatApi',
```

