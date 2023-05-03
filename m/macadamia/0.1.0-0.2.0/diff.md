# Comparing `tmp/macadamia-0.1.0.tar.gz` & `tmp/macadamia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macadamia-0.1.0.tar", last modified: Fri Mar 17 22:44:06 2023, max compression
+gzip compressed data, was "macadamia-0.2.0.tar", last modified: Wed May  3 16:41:21 2023, max compression
```

## Comparing `macadamia-0.1.0.tar` & `macadamia-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-03-17 22:44:06.654341 macadamia-0.1.0/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      533 2023-03-17 22:44:06.654341 macadamia-0.1.0/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)     6344 2023-03-17 22:42:52.000000 macadamia-0.1.0/README.md
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-03-17 22:44:06.654341 macadamia-0.1.0/macadamia/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1040 2023-03-17 22:42:52.000000 macadamia-0.1.0/macadamia/__init__.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-03-17 22:44:06.654341 macadamia-0.1.0/macadamia.egg-info/
--rw-r--r--   0 kevin     (1000) kevin     (1000)      533 2023-03-17 22:44:06.000000 macadamia-0.1.0/macadamia.egg-info/PKG-INFO
--rw-r--r--   0 kevin     (1000) kevin     (1000)      212 2023-03-17 22:44:06.000000 macadamia-0.1.0/macadamia.egg-info/SOURCES.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)        1 2023-03-17 22:44:06.000000 macadamia-0.1.0/macadamia.egg-info/dependency_links.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)       10 2023-03-17 22:44:06.000000 macadamia-0.1.0/macadamia.egg-info/top_level.txt
--rw-r--r--   0 kevin     (1000) kevin     (1000)       38 2023-03-17 22:44:06.654341 macadamia-0.1.0/setup.cfg
--rw-r--r--   0 kevin     (1000) kevin     (1000)     1184 2023-03-17 22:42:52.000000 macadamia-0.1.0/setup.py
-drwxr-xr-x   0 kevin     (1000) kevin     (1000)        0 2023-03-17 22:44:06.654341 macadamia-0.1.0/tests/
--rw-r--r--   0 kevin     (1000) kevin     (1000)     3396 2023-03-17 22:42:52.000000 macadamia-0.1.0/tests/test_fiztmz.py
--rw-r--r--   0 kevin     (1000) kevin     (1000)     2694 2023-03-17 22:42:52.000000 macadamia-0.1.0/tests/test_utmz.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-03 16:41:21.404996 macadamia-0.2.0/
+-rw-r--r--   0 kevin      (501) staff       (20)      533 2023-05-03 16:41:21.404863 macadamia-0.2.0/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     6833 2023-05-03 16:38:47.000000 macadamia-0.2.0/README.md
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-03 16:41:21.404014 macadamia-0.2.0/macadamia/
+-rw-r--r--   0 kevin      (501) staff       (20)     1178 2023-05-03 16:38:47.000000 macadamia-0.2.0/macadamia/__init__.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-03 16:41:21.404460 macadamia-0.2.0/macadamia.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)      533 2023-05-03 16:41:21.000000 macadamia-0.2.0/macadamia.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)      212 2023-05-03 16:41:21.000000 macadamia-0.2.0/macadamia.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-05-03 16:41:21.000000 macadamia-0.2.0/macadamia.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       10 2023-05-03 16:41:21.000000 macadamia-0.2.0/macadamia.egg-info/top_level.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       38 2023-05-03 16:41:21.405031 macadamia-0.2.0/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)     1184 2023-05-03 16:40:17.000000 macadamia-0.2.0/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-05-03 16:41:21.404696 macadamia-0.2.0/tests/
+-rw-r--r--   0 kevin      (501) staff       (20)     4027 2023-05-03 16:38:47.000000 macadamia-0.2.0/tests/test_fiztmz.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2694 2023-05-03 16:38:47.000000 macadamia-0.2.0/tests/test_utmz.py
```

### Comparing `macadamia-0.1.0/PKG-INFO` & `macadamia-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macadamia
-Version: 0.1.0
+Version: 0.2.0
 Summary: A parser for Google Analytics Cookies
 Home-page: https://github.com/realgeeks/macadamia
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `macadamia-0.1.0/README.md` & `macadamia-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -24,42 +24,46 @@
 ```python
 >>> from macadamia import parse_cookie
 >>> cookie_to_parse = "208940939.1365186784.1.1.fiztmcsr=(direct)|fiztmccn=(direct)|fiztmcmd=(none)"
 >>> parsed_cookie = parse_cookie(cookie_to_parse, prefix="fiztm")
 >>> {'domain_hash': '208940939', 'campaign_number': '1', 'campaign_data': {'source': '(direct)', 'campaign_name': '(direct)', 'medium': '(none)'}, 'timestamp': datetime.datetime(2013, 4, 5, 8, 33, 4), 'session_counter': '1'}
 ```
 
+## The future of google analytics cookies
+
+Google has deprecated this cookie format and now GA4 stores a cookie incompatible with Macadamia.  If you would like to continue using Macadamia, version `0.2.0` adds support for parsing cookies created by [the included utmz cookie replicator javascript](https://github.com/RealGeeks/macadamia/blob/master/utmz-cookie.js)
+
 ###__utma Visitor Cookie (lasts 2 years)
 Used to distinguish users and sessions. The cookie is created when the javascript library executes and no existing __utma cookies exists. The cookie is updated every time data is sent to Google Analytics.
 
 Each group is separated by a period character. All times stored are UNIX timest­amps. For new visits the three times in this cookie will all be the same.
 
 Has the following info:
   * domain_hash
   * random_id
   * first_visit_at
   * previous_visit_at
   * current_visit_at
   * session_counter
 
-###__utmb Session Cookie (lasts 30 minutes)
+### `__utmb` Session Cookie (lasts 30 minutes)
 Used to determine new sessions/visits. The cookie is created when the javascript library executes and no existing __utmb cookies exists. The cookie is updated every time data is sent to Google Analytics.
 
 Has the following fields:
   * domain_hash
   * pageviews
   * tokens_available
   * time_of_session
 
 Each group is separated by a period character. All times stored are UNIX timestamps. The token bucket stores how many requests are being made to GA at once. This number will decrease for each request, any requests sent while the bucket is empty will be discarded.
 
-###__utmc (lasts until browser is closed)
+### `__utmc` (lasts until browser is closed)
 Deprecated.  Still set for backwards compability sometimes.
 
-###__utmz (lasts 6 months)
+### `__utmz` (lasts 6 months)
 Stores the traffic source or campaign that explains how the user reached your site. The cookie is created when the javascript library executes and is updated every time data is sent to Google Analytics.
 
 Has the following fields:
 
 * domain_hash
 * timestamp
 * session_counter
@@ -77,26 +81,26 @@
 | utmcct  | campaign content | the relative page URL of the referring site if a referral |
 | utmgclid | google click ID | ? |
 
 `utmgclid` will only be set for AutoTagged AdWords visits. If set, other parameters will be unset, as utmgclid is a hash of the campaign values and is used instead.
 
 ## Rare variables
 
-###__utmv (lasts 2 years)
+### `__utmv` (lasts 2 years)
 Used to store visitor-level custom variable data. 
 
   * domain_hash
   * custom variable value
 
 Each group is separated by a period character. This cookie can only be created by using Google Analytics' deprecated _setVar() method. Calling this method sets this cookie and automa­tically sends the data to Google Analytics via a __utm.gif request.  Values sent in this manner appear in the "User Define­d" report, unless otherwise interc­epted with profile filters.
 
-###__utmx
+### `__utmx`
 Used by Website Optimizer.  Now used by "Content Experiments?"
 
-###__utmk
+### `__utmk`
 Digest hashes of utm values
 
 Sources:
   * [Google Analytics v2 cheatsheet](http://www.cheatography.com/jay-taylor/cheat-sheets/google-analytics-cookies-v2/)
   * [Google UTMZ Cookie Parser](http://daleconboy.com/portfolio/code/google-utmz-cookie-parser)
   * [Python GA Cookie Parser](https://github.com/ryonlife/Python-Google-Analytics-Cookie-Parser)
   * [Official GA Cookie Documentation](https://developers.google.com/analytics/devguides/collection/analyticsjs/cookie-usage)
@@ -104,27 +108,28 @@
 ## Running tests via tox and docker
 ```bash
 make test
 ```
 
 ## Changelog
 
+* 0.2.0: Support cookies missing the leading fields, as created by some `_utmz` replicator scripts.
 * 0.1.0: Support cookies shaped like `_utmz` but with a different name
 * 0.0.7: Actually add Python 3 compatibility and upgrade Dockerfile base image to test against Python 3.7
 * 0.0.6: Python 3 compatibility and add Dockerfile for development
 * 0.0.5: Fix typo parsing `utmgclid` cookie value
 * 0.0.4: URLDecode cookie information
 * 0.0.3: Fix bug where the . in a referring domain name was causing the `campaign_data` field to be cut off
 * 0.0.2: Remove accidential PyYAML dependency
 * 0.0.1: initial release
 
 ## License (MIT)
 The MIT License (MIT)
 
-Copyright (c) 2013 Kevin McCarthy
+Copyright (c) 2013-2023 Kevin McCarthy
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `macadamia-0.1.0/macadamia/__init__.py` & `macadamia-0.2.0/macadamia/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import re
 
 try:
     from urllib2 import unquote
 except ImportError:
     from urllib.parse import unquote
 
 
@@ -19,22 +20,26 @@
     fields = [d.split("=") for d in data.split("|")]
     info = dict((human_names[d[0]], unquote(d[1])) for d in fields)
 
     return info
 
 
 def parse_cookie(cookie, prefix="utm"):
-    fields = cookie.split(".")
+    fields = re.search(r"^(?:(\d*)\.(\d*)\.(\d*)\.(\d*).)?(.+)$", cookie).groups()
+    fields = [field or "" for field in fields]
 
-    campaign_data = parse_campaign_data(".".join(fields[4:]), prefix=prefix)
+    if fields[1]:
+        timestamp = datetime.datetime.fromtimestamp(int(fields[1]))
+    else:
+        timestamp = ""
 
     return {
         "domain_hash": fields[0],
-        "timestamp": datetime.datetime.fromtimestamp(int(fields[1])),
+        "timestamp": timestamp,
         "session_counter": fields[2],
         "campaign_number": fields[3],
-        "campaign_data": campaign_data,
+        "campaign_data": parse_campaign_data(fields[4], prefix),
     }
 
 
 def parse_utmz(cookie):
     return parse_cookie(cookie, prefix="utm")
```

### Comparing `macadamia-0.1.0/macadamia.egg-info/PKG-INFO` & `macadamia-0.2.0/macadamia.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macadamia
-Version: 0.1.0
+Version: 0.2.0
 Summary: A parser for Google Analytics Cookies
 Home-page: https://github.com/realgeeks/macadamia
 Author: Kevin McCarthy
 Author-email: me@kevinmccarthy.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `macadamia-0.1.0/setup.py` & `macadamia-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     def run_tests(self):
         #import here, cause outside the eggs aren't loaded
         import pytest
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 setup(name='macadamia',
-      version='0.1.0',
+      version='0.2.0',
       description="A parser for Google Analytics Cookies",
       author='Kevin McCarthy',
       author_email='me@kevinmccarthy.org',
       url='https://github.com/realgeeks/macadamia',
       packages=['macadamia'],
       install_requires=[],
       license='MIT',
```

### Comparing `macadamia-0.1.0/tests/test_fiztmz.py` & `macadamia-0.2.0/tests/test_fiztmz.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,12 +76,27 @@
                     "campaign_keyword": "real estate for sale in wilmington nc",
                     "campaign_name": "(not set)",
                     "google_click_id": "CMbMrdi_ybgCFWho7AodDyAAvQ",
                     "medium": "(not set)",
                 },
             },
         ),
+        (
+            "fiztmgclid=CMbMrdi_ybgCFWho7AodDyAAvQ|fiztmccn=(not set)|fiztmcmd=(not set)|fiztmctr=real estate for sale in wilmington nc",
+            {
+                "campaign_number": "",
+                "domain_hash": "",
+                "session_counter": "",
+                "timestamp": "",
+                "campaign_data": {
+                    "campaign_keyword": "real estate for sale in wilmington nc",
+                    "campaign_name": "(not set)",
+                    "google_click_id": "CMbMrdi_ybgCFWho7AodDyAAvQ",
+                    "medium": "(not set)",
+                },
+            },
+        ),
     ],
 )
 def test_cookie_split_and_parse(cookie, expected):
     info = parse_cookie(cookie, prefix="fiztm")
     assert info == expected
```

### Comparing `macadamia-0.1.0/tests/test_utmz.py` & `macadamia-0.2.0/tests/test_utmz.py`

 * *Files identical despite different names*

