# Comparing `tmp/urlwatch-2.8.tar.gz` & `tmp/urlwatch-2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/urlwatch-2.8.tar", last modified: Sun Jan 28 19:48:41 2018, max compression
+gzip compressed data, was "dist/urlwatch-2.9.tar", last modified: Sat Mar 24 12:20:43 2018, max compression
```

## Comparing `urlwatch-2.8.tar` & `urlwatch-2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/
--rw-r--r--   0 thp        (501) staff       (20)      613 2018-01-28 19:48:41.000000 urlwatch-2.8/PKG-INFO
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/test/
--rw-r--r--   0 thp        (501) staff       (20)     4509 2018-01-28 19:38:07.000000 urlwatch-2.8/test/test_handler.py
--rw-r--r--   0 thp        (501) staff       (20)     1044 2017-11-08 22:10:36.000000 urlwatch-2.8/test/test_filters.py
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/test/data/
--rw-r--r--   0 thp        (501) staff       (20)      498 2016-10-31 09:54:09.000000 urlwatch-2.8/test/data/urlwatch.yaml
--rw-r--r--   0 thp        (501) staff       (20)     1004 2016-10-31 09:54:09.000000 urlwatch-2.8/test/data/urls.json
--rw-r--r--   0 thp        (501) staff       (20)      731 2016-10-31 09:54:09.000000 urlwatch-2.8/test/data/urlwatch.json
--rw-r--r--   0 thp        (501) staff       (20)     1218 2016-01-20 08:44:10.000000 urlwatch-2.8/test/data/urls.txt
--rw-r--r--   0 thp        (501) staff       (20)     8906 2018-01-28 19:47:22.000000 urlwatch-2.8/ChangeLog
--rw-r--r--   0 thp        (501) staff       (20)       92 2018-01-28 19:41:00.000000 urlwatch-2.8/MANIFEST.in
--rw-r--r--   0 thp        (501) staff       (20)     5475 2018-01-28 19:43:39.000000 urlwatch-2.8/README.md
--rw-r--r--   0 thp        (501) staff       (20)     1408 2018-01-28 19:42:07.000000 urlwatch-2.8/COPYING
--rw-r--r--   0 thp        (501) staff       (20)      920 2017-11-08 22:10:36.000000 urlwatch-2.8/setup.py
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/lib/
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/lib/urlwatch/
--rw-r--r--   0 thp        (501) staff       (20)     3359 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/worker.py
--rw-r--r--   0 thp        (501) staff       (20)     6407 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/command.py
--rw-r--r--   0 thp        (501) staff       (20)     5021 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/config.py
--rw-r--r--   0 thp        (501) staff       (20)     4690 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/handler.py
--rw-r--r--   0 thp        (501) staff       (20)     3596 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/util.py
--rw-r--r--   0 thp        (501) staff       (20)      598 2018-01-28 19:47:52.000000 urlwatch-2.8/lib/urlwatch/__init__.py
--rw-r--r--   0 thp        (501) staff       (20)     8839 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/jobs.py
--rw-r--r--   0 thp        (501) staff       (20)     4991 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/html2txt.py
--rw-r--r--   0 thp        (501) staff       (20)     2513 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/ical2txt.py
--rw-r--r--   0 thp        (501) staff       (20)    15357 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/storage.py
--rw-r--r--   0 thp        (501) staff       (20)    18441 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/reporters.py
--rw-r--r--   0 thp        (501) staff       (20)     3669 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/main.py
--rw-r--r--   0 thp        (501) staff       (20)     3353 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/migration.py
--rw-r--r--   0 thp        (501) staff       (20)     4309 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/mailer.py
--rw-r--r--   0 thp        (501) staff       (20)    11168 2018-01-28 19:42:07.000000 urlwatch-2.8/lib/urlwatch/filters.py
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/lib/urlwatch.egg-info/
--rw-r--r--   0 thp        (501) staff       (20)      613 2018-01-28 19:48:41.000000 urlwatch-2.8/lib/urlwatch.egg-info/PKG-INFO
--rw-r--r--   0 thp        (501) staff       (20)      839 2018-01-28 19:48:41.000000 urlwatch-2.8/lib/urlwatch.egg-info/SOURCES.txt
--rw-r--r--   0 thp        (501) staff       (20)       51 2018-01-28 19:48:41.000000 urlwatch-2.8/lib/urlwatch.egg-info/requires.txt
--rw-r--r--   0 thp        (501) staff       (20)        9 2018-01-28 19:48:41.000000 urlwatch-2.8/lib/urlwatch.egg-info/top_level.txt
--rw-r--r--   0 thp        (501) staff       (20)        1 2018-01-28 19:48:41.000000 urlwatch-2.8/lib/urlwatch.egg-info/dependency_links.txt
--rw-r--r--   0 thp        (501) staff       (20)       68 2018-01-28 19:48:41.000000 urlwatch-2.8/setup.cfg
--rwxr-xr-x   0 thp        (501) staff       (20)     3968 2018-01-28 19:42:07.000000 urlwatch-2.8/urlwatch
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/share/
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/share/man/
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/share/man/man1/
--rw-r--r--   0 thp        (501) staff       (20)     2007 2018-01-28 19:38:07.000000 urlwatch-2.8/share/man/man1/urlwatch.1
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/share/urlwatch/
-drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-01-28 19:48:41.000000 urlwatch-2.8/share/urlwatch/examples/
--rw-r--r--   0 thp        (501) staff       (20)     4014 2018-01-28 19:42:07.000000 urlwatch-2.8/share/urlwatch/examples/hooks.py.example
--rw-r--r--   0 thp        (501) staff       (20)     1488 2016-01-20 08:44:10.000000 urlwatch-2.8/share/urlwatch/examples/urls.yaml.example
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/
+-rw-r--r--   0 thp        (501) staff       (20)      615 2018-03-24 12:20:43.000000 urlwatch-2.9/PKG-INFO
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/test/
+-rw-r--r--   0 thp        (501) staff       (20)     4509 2018-01-28 19:38:07.000000 urlwatch-2.9/test/test_handler.py
+-rw-r--r--   0 thp        (501) staff       (20)     1044 2017-11-08 22:10:36.000000 urlwatch-2.9/test/test_filters.py
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/test/data/
+-rw-r--r--   0 thp        (501) staff       (20)      537 2018-02-21 10:53:59.000000 urlwatch-2.9/test/data/urlwatch.yaml
+-rw-r--r--   0 thp        (501) staff       (20)     1004 2016-10-31 09:54:09.000000 urlwatch-2.9/test/data/urls.json
+-rw-r--r--   0 thp        (501) staff       (20)      731 2016-10-31 09:54:09.000000 urlwatch-2.9/test/data/urlwatch.json
+-rw-r--r--   0 thp        (501) staff       (20)     1218 2016-01-20 08:44:10.000000 urlwatch-2.9/test/data/urls.txt
+-rw-r--r--   0 thp        (501) staff       (20)     9279 2018-03-24 12:17:42.000000 urlwatch-2.9/ChangeLog
+-rw-r--r--   0 thp        (501) staff       (20)       92 2018-01-28 19:41:00.000000 urlwatch-2.9/MANIFEST.in
+-rw-r--r--   0 thp        (501) staff       (20)     6410 2018-03-24 12:18:15.000000 urlwatch-2.9/README.md
+-rw-r--r--   0 thp        (501) staff       (20)     1408 2018-01-28 19:42:07.000000 urlwatch-2.9/COPYING
+-rw-r--r--   0 thp        (501) staff       (20)      939 2018-02-21 10:53:59.000000 urlwatch-2.9/setup.py
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/lib/
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/lib/urlwatch/
+-rw-r--r--   0 thp        (501) staff       (20)     3359 2018-01-28 19:42:07.000000 urlwatch-2.9/lib/urlwatch/worker.py
+-rw-r--r--   0 thp        (501) staff       (20)     8119 2018-03-24 12:14:58.000000 urlwatch-2.9/lib/urlwatch/command.py
+-rw-r--r--   0 thp        (501) staff       (20)     5197 2018-03-24 12:14:58.000000 urlwatch-2.9/lib/urlwatch/config.py
+-rw-r--r--   0 thp        (501) staff       (20)     4690 2018-01-28 19:42:07.000000 urlwatch-2.9/lib/urlwatch/handler.py
+-rw-r--r--   0 thp        (501) staff       (20)     3596 2018-01-28 19:42:07.000000 urlwatch-2.9/lib/urlwatch/util.py
+-rw-r--r--   0 thp        (501) staff       (20)      600 2018-03-24 12:17:54.000000 urlwatch-2.9/lib/urlwatch/__init__.py
+-rw-r--r--   0 thp        (501) staff       (20)     8839 2018-01-28 19:42:07.000000 urlwatch-2.9/lib/urlwatch/jobs.py
+-rw-r--r--   0 thp        (501) staff       (20)     4991 2018-01-28 19:42:07.000000 urlwatch-2.9/lib/urlwatch/html2txt.py
+-rw-r--r--   0 thp        (501) staff       (20)     2513 2018-01-28 19:42:07.000000 urlwatch-2.9/lib/urlwatch/ical2txt.py
+-rw-r--r--   0 thp        (501) staff       (20)    15418 2018-02-21 10:53:59.000000 urlwatch-2.9/lib/urlwatch/storage.py
+-rw-r--r--   0 thp        (501) staff       (20)    18456 2018-03-24 12:14:58.000000 urlwatch-2.9/lib/urlwatch/reporters.py
+-rw-r--r--   0 thp        (501) staff       (20)     3668 2018-02-21 10:53:59.000000 urlwatch-2.9/lib/urlwatch/main.py
+-rw-r--r--   0 thp        (501) staff       (20)     3323 2018-02-21 11:00:29.000000 urlwatch-2.9/lib/urlwatch/migration.py
+-rw-r--r--   0 thp        (501) staff       (20)     4424 2018-03-24 12:14:58.000000 urlwatch-2.9/lib/urlwatch/mailer.py
+-rw-r--r--   0 thp        (501) staff       (20)    11168 2018-01-28 19:42:07.000000 urlwatch-2.9/lib/urlwatch/filters.py
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/lib/urlwatch.egg-info/
+-rw-r--r--   0 thp        (501) staff       (20)      615 2018-03-24 12:20:43.000000 urlwatch-2.9/lib/urlwatch.egg-info/PKG-INFO
+-rw-r--r--   0 thp        (501) staff       (20)      839 2018-03-24 12:20:43.000000 urlwatch-2.9/lib/urlwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 thp        (501) staff       (20)       51 2018-03-24 12:20:43.000000 urlwatch-2.9/lib/urlwatch.egg-info/requires.txt
+-rw-r--r--   0 thp        (501) staff       (20)        9 2018-03-24 12:20:43.000000 urlwatch-2.9/lib/urlwatch.egg-info/top_level.txt
+-rw-r--r--   0 thp        (501) staff       (20)        1 2018-03-24 12:20:43.000000 urlwatch-2.9/lib/urlwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 thp        (501) staff       (20)       68 2018-03-24 12:20:43.000000 urlwatch-2.9/setup.cfg
+-rwxr-xr-x   0 thp        (501) staff       (20)     4237 2018-03-24 12:14:58.000000 urlwatch-2.9/urlwatch
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/share/
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/share/man/
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/share/man/man1/
+-rw-r--r--   0 thp        (501) staff       (20)     2007 2018-03-24 12:14:58.000000 urlwatch-2.9/share/man/man1/urlwatch.1
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/share/urlwatch/
+drwxr-xr-x   0 thp        (501) staff       (20)        0 2018-03-24 12:20:43.000000 urlwatch-2.9/share/urlwatch/examples/
+-rw-r--r--   0 thp        (501) staff       (20)     4014 2018-01-28 19:42:07.000000 urlwatch-2.9/share/urlwatch/examples/hooks.py.example
+-rw-r--r--   0 thp        (501) staff       (20)     1488 2016-01-20 08:44:10.000000 urlwatch-2.9/share/urlwatch/examples/urls.yaml.example
```

### Comparing `urlwatch-2.8/test/test_handler.py` & `urlwatch-2.9/test/test_handler.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/test/test_filters.py` & `urlwatch-2.9/test/test_filters.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/test/data/urls.json` & `urlwatch-2.9/test/data/urls.json`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/test/data/urlwatch.json` & `urlwatch-2.9/test/data/urlwatch.json`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/test/data/urls.txt` & `urlwatch-2.9/test/data/urls.txt`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/ChangeLog` & `urlwatch-2.9/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -215,7 +215,14 @@
 	* New reporter: Telegram support (by gvandenbroucke)
 
 2018-01-28 Thomas Perl <m@thp.io>
 	* Documentation: Mention appdirs (by e-dschungel)
 	* SMTP: Fix handling of missing user field (by e-dschungel)
 	* Manpage: Fix documentation of XDG environment variables (by Jelle van der Waa)
 	* Unit tests: Fix imports for out-of-source-tree tests (by Maxime Werlen)
+
+2018-03-24 Thomas Perl <m@thp.io>
+	* Pushover: Device and sound attribute (by Tobias Haupenthal)
+	* XDG: Move cache file to XDG_CACHE_DIR (by Maxime Werlen)
+	* E-Mail: Add support for --smtp-login and document GMail SMTP usage
+	* Cleanups: Fix out-of-date debug message, use https (by Jakub Wilk)
+	* Migration: Unconditionally migrate urlwatch 1.x cache dirs (Fixes #206)
```

### Comparing `urlwatch-2.8/README.md` & `urlwatch-2.9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -98,24 +98,24 @@
 filter: element-by-id:something,html2text
 ```
 
 The example urls.yaml file also demonstrates the use of built-in
 filters, here 3 filters are used: html2text, line-grep and whitespace
 removal to get just a certain info field from a webpage:
 ```yaml
-url: http://thp.io/2008/urlwatch/
+url: https://thp.io/2008/urlwatch/
 filter: html2text,grep:Current.*version,strip
 ```
 For most cases, this means that you can specify a filter chain in
 your urls.yaml page without requiring a custom hook where previously
 you would have needed to write custom filtering code in Python.
 
 If you want to extract only the body tag you can use this filer:
 ```yaml
-url: http://thp.io/2008/urlwatch/
+url: https://thp.io/2008/urlwatch/
 filter: element-by-tag:body
 ```
 
 PUSHOVER
 --------
 
 You can configure urlwatch to send real time notifications about changes
@@ -142,13 +142,42 @@
 ```yaml
 telegram:
   bot_token: '999999999:3tOhy2CuZE0pTaCtszRfKpnagOG8IQbP5gf' # your bot api token
   chat_id: '88888888' # the chat id where the messages should be sent
   enabled: true
 ```
 
+
+E-MAIL VIA GMAIL SMTP
+---------------------
+
+You need to configure your GMail account to allow for "less secure" (password-based)
+apps to login:
+
+1. Go to https://myaccount.google.com/
+2. Click on "Sign-in & security"
+3. Scroll all the way down to "Allow less secure apps" and enable it
+
+Now, start the configuration editor: `urlwatch --edit-config`
+
+These are the keys you need to configure (see #158):
+
+- `report/email/enabled`: `true`
+- `report/email/from`: `your.username@gmail.com` (edit accordingly)
+- `report/email/method`: `smtp`
+- `report/email/smtp/host`: `smtp.gmail.com`
+- `report/email/smtp/keyring`: `true`
+- `report/email/smtp/port`: `587`
+- `report/email/smtp/starttls`: `true`
+- `report/email/to`: The e-mail address you want to send reports to
+
+Now, for setting the password, it's not stored in the config file, but in your
+keychain. To store the password, run: `urlwatch --smtp-login` and enter your
+password.
+
+
 CONTACT
 -------
 
-Website: http://thp.io/2008/urlwatch/
+Website: https://thp.io/2008/urlwatch/
 
 E-Mail: m@thp.io
```

### Comparing `urlwatch-2.8/COPYING` & `urlwatch-2.9/COPYING`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/setup.py` & `urlwatch-2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,8 +21,9 @@
     ('share/man/man1', ['share/man/man1/urlwatch.1']),
     ('share/urlwatch/examples', [
         'share/urlwatch/examples/hooks.py.example',
         'share/urlwatch/examples/urls.yaml.example',
     ]),
 ]
 
+del m['copyright']
 setup(**m)
```

### Comparing `urlwatch-2.8/lib/urlwatch/worker.py` & `urlwatch-2.9/lib/urlwatch/worker.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/lib/urlwatch/command.py` & `urlwatch-2.9/lib/urlwatch/command.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 import subprocess
 import sys
 
 from .filters import FilterBase
 from .jobs import JobBase
 from .reporters import ReporterBase
 from .util import atomic_rename
+from .mailer import set_password, have_password
 
 logger = logging.getLogger(__name__)
 
 
 class UrlwatchCommand:
     def __init__(self, urlwatcher):
 
@@ -155,13 +156,57 @@
         if self.urlwatch_config.add is not None or self.urlwatch_config.delete is not None:
             sys.exit(self.modify_urls())
 
     def check_edit_config(self):
         if self.urlwatch_config.edit_config:
             sys.exit(self.urlwatcher.config_storage.edit())
 
-    def run(self):
+    def check_smtp_login(self):
+        if self.urlwatch_config.smtp_login:
+            config = self.urlwatcher.config_storage.config['report']['email']
+            smtp_config = config['smtp']
+
+            success = True
+
+            if not config['enabled']:
+                print('Please enable e-mail reporting in the config first.')
+                success = False
+
+            if config['method'] != 'smtp':
+                print('Please set the method to SMTP for the e-mail reporter.')
+                success = False
+
+            if not smtp_config['keyring']:
+                print('Keyring authentication must be enabled for SMTP.')
+                success = False
+
+            smtp_hostname = smtp_config['host']
+            if not smtp_hostname:
+                print('Please configure the SMTP hostname in the config first.')
+                success = False
+
+            smtp_username = smtp_config.get('user', config['from'])
+            if not smtp_username:
+                print('Please configure the SMTP username in the config first.')
+                success = False
+
+            if not success:
+                sys.exit(1)
+
+            if have_password(smtp_hostname, smtp_username):
+                message = 'Password for %s / %s already set, update? [y/N] ' % (smtp_username, smtp_hostname)
+                if input(message).lower() != 'y':
+                    print('Password unchanged.')
+                    sys.exit(0)
+
+            if success:
+                set_password(smtp_hostname, smtp_username)
+                # TODO: Actually verify that the login to the server works
+
+            sys.exit(0)
 
+    def run(self):
         self.check_edit_config()
+        self.check_smtp_login()
         self.handle_actions()
         self.urlwatcher.run_jobs()
         self.urlwatcher.close()
```

### Comparing `urlwatch-2.8/lib/urlwatch/config.py` & `urlwatch-2.9/lib/urlwatch/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,17 @@
         group.add_argument('--config', metavar='FILE', help='read configuration from FILE',
                            default=self.config)
         group.add_argument('--hooks', metavar='FILE', help='use FILE as hooks.py module',
                            default=self.hooks)
         group.add_argument('--cache', metavar='FILE', help='use FILE as cache database',
                            default=self.cache)
 
+        group = parser.add_argument_group('Authentication')
+        group.add_argument('--smtp-login', action='store_true', help='Enter password for SMTP (store in keyring)')
+
         group = parser.add_argument_group('job list management')
         group.add_argument('--list', action='store_true', help='list jobs')
         group.add_argument('--add', metavar='JOB', help='add job (key1=value1,key2=value2,...)')
         group.add_argument('--delete', metavar='JOB', help='delete job by location or index')
         group = parser.add_argument_group('interactive commands ($EDITOR/$VISUAL)')
         group.add_argument('--edit', action='store_true', help='edit URL/job list')
         group.add_argument('--edit-config', action='store_true', help='edit configuration file')
```

### Comparing `urlwatch-2.8/lib/urlwatch/handler.py` & `urlwatch-2.9/lib/urlwatch/handler.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/lib/urlwatch/util.py` & `urlwatch-2.9/lib/urlwatch/util.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/lib/urlwatch/__init__.py` & `urlwatch-2.9/lib/urlwatch/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 """
 
 pkgname = 'urlwatch'
 
 __copyright__ = 'Copyright 2008-2018 Thomas Perl'
 __author__ = 'Thomas Perl <m@thp.io>'
 __license__ = 'BSD'
-__url__ = 'http://thp.io/2008/urlwatch/'
-__version__ = '2.8'
-__user_agent__ = '%s/%s (+http://thp.io/2008/urlwatch/info.html)' % (pkgname, __version__)
+__url__ = 'https://thp.io/2008/urlwatch/'
+__version__ = '2.9'
+__user_agent__ = '%s/%s (+https://thp.io/2008/urlwatch/info.html)' % (pkgname, __version__)
```

### Comparing `urlwatch-2.8/lib/urlwatch/jobs.py` & `urlwatch-2.9/lib/urlwatch/jobs.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/lib/urlwatch/html2txt.py` & `urlwatch-2.9/lib/urlwatch/html2txt.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/lib/urlwatch/ical2txt.py` & `urlwatch-2.9/lib/urlwatch/ical2txt.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/lib/urlwatch/storage.py` & `urlwatch-2.9/lib/urlwatch/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,16 @@
             'sendmail': {
                 'path': 'sendmail',
             }
         },
         'pushover': {
             'enabled': False,
             'app': '',
+            'device': '',
+            'sound': 'spacealarm',
             'user': '',
         },
         'pushbullet': {
             'enabled': False,
             'api_key': '',
         },
         'mailgun': {
```

### Comparing `urlwatch-2.8/lib/urlwatch/reporters.py` & `urlwatch-2.9/lib/urlwatch/reporters.py`

 * *Files 2% similar despite different names*

```diff
@@ -347,16 +347,14 @@
             mailer = SMTPMailer(smtp_user, self.config['smtp']['host'], self.config['smtp']['port'],
                                 self.config['smtp']['starttls'], self.config['smtp']['keyring'])
         elif self.config['method'] == "sendmail":
             mailer = SendmailMailer(self.config['sendmail']['path'])
         else:
             logger.error('Invalid entry for method {method}'.format(method=self.config['method']))
 
-        # TODO set_password(options.email_smtp, options.email_from)
-
         if self.config['html']:
             body_html = '\n'.join(self.convert(HtmlReporter).submit())
 
             msg = mailer.msg_html(self.config['from'], self.config['to'], subject, body_text, body_html)
         else:
             msg = mailer.msg_plain(self.config['from'], self.config['to'], subject, body_text)
 
@@ -398,15 +396,17 @@
     __kind__ = 'pushover'
 
     def web_service_get(self):
         app = chump.Application(self.config['app'])
         return app.get_user(self.config['user'])
 
     def web_service_submit(self, service, title, body):
-        msg = service.create_message(title=title, message=body, html=True, sound='spacealarm')
+        sound = self.config['sound']
+        device = self.config['device']
+        msg = service.create_message(title=title, message=body, html=True, sound=sound, device=device)
         msg.send()
 
 
 class PushbulletReport(WebServiceReporter):
     """Send summary via pushbullet.com"""
 
     __kind__ = 'pushbullet'
```

### Comparing `urlwatch-2.8/lib/urlwatch/main.py` & `urlwatch-2.9/lib/urlwatch/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 class Urlwatch(object):
     def __init__(self, urlwatch_config, config_storage, cache_storage, urls_storage):
 
         self.urlwatch_config = urlwatch_config
 
         logger.info('Using %s as URLs file', self.urlwatch_config.urls)
         logger.info('Using %s for hooks', self.urlwatch_config.hooks)
-        logger.info('Using %s as cache directory', self.urlwatch_config.cache)
+        logger.info('Using %s as cache database', self.urlwatch_config.cache)
 
         self.config_storage = config_storage
         self.cache_storage = cache_storage
         self.urls_storage = urls_storage
 
         self.report = Report(self)
         self.jobs = None
```

### Comparing `urlwatch-2.8/lib/urlwatch/migration.py` & `urlwatch-2.9/lib/urlwatch/migration.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 def migrate_cache(urlwatcher):
     # Migrate urlwatch 1.x cache to urlwatch 2.x
 
     urlwatch_config = urlwatcher.urlwatch_config
     cache = urlwatch_config.cache
     cache_dir = os.path.join(urlwatch_config.urlwatch_dir, 'cache')
 
-    if not os.path.isfile(cache) and os.path.isdir(cache_dir):
+    if os.path.isdir(cache_dir):
         print("""
     Migrating cache: {cache_dir} -> {cache_db}
     """.format(cache_dir=cache_dir, cache_db=cache))
 
         old_cache_storage = CacheDirStorage(cache_dir)
         urlwatcher.cache_storage.restore(old_cache_storage.backup())
         urlwatcher.cache_storage.gc([job.get_guid() for job in urlwatcher.jobs])
```

### Comparing `urlwatch-2.8/lib/urlwatch/mailer.py` & `urlwatch-2.9/lib/urlwatch/mailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,18 @@
                              stderr=subprocess.PIPE,
                              universal_newlines=True)
         result = p.communicate(msg.as_string())
         if p.returncode:
             logger.error('Sendmail failed with {result}'.format(result=result))
 
 
+def have_password(smtp_server, from_email):
+    return keyring.get_password(smtp_server, from_email) is not None
+
+
 def set_password(smtp_server, from_email):
     ''' Set the keyring password for the mail connection. Interactive.'''
     if keyring is None:
         raise ImportError('keyring module missing - service unsupported')
 
     password = getpass.getpass(prompt='Enter password for {} using {}: '.format(from_email, smtp_server))
     keyring.set_password(smtp_server, from_email, password)
```

### Comparing `urlwatch-2.8/lib/urlwatch/filters.py` & `urlwatch-2.9/lib/urlwatch/filters.py`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/lib/urlwatch.egg-info/SOURCES.txt` & `urlwatch-2.9/lib/urlwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/urlwatch` & `urlwatch-2.9/urlwatch`

 * *Files 9% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 import socket
 import sys
 
 from appdirs import AppDirs
 
 pkgname = 'urlwatch'
 urlwatch_dir = os.path.expanduser(os.path.join('~', '.' + pkgname))
+urlwatch_cache_dir = AppDirs(pkgname).user_cache_dir
 
 if not os.path.exists(urlwatch_dir):
     urlwatch_dir = AppDirs(pkgname).user_config_dir
 
 # Check if we are installed in the system already
 (prefix, bindir) = os.path.split(os.path.dirname(os.path.abspath(sys.argv[0])))
 
@@ -82,16 +83,20 @@
         root_logger.setLevel(logging.DEBUG)
         root_logger.info('turning on verbose logging mode')
 
 
 if __name__ == '__main__':
     config_file = os.path.join(urlwatch_dir, CONFIG_FILE)
     urls_file = os.path.join(urlwatch_dir, URLS_FILE)
-    cache_file = os.path.join(urlwatch_dir, CACHE_FILE)
     hooks_file = os.path.join(urlwatch_dir, HOOKS_FILE)
+    new_cache_file = os.path.join(urlwatch_cache_dir, CACHE_FILE)
+    old_cache_file = os.path.join(urlwatch_dir, CACHE_FILE)
+    cache_file = new_cache_file
+    if os.path.exists(old_cache_file) and not os.path.exists(new_cache_file):
+        cache_file = old_cache_file
 
     command_config = CommandConfig(pkgname, urlwatch_dir, bindir, prefix,
                                    config_file, urls_file, hooks_file, cache_file, False)
     setup_logger(command_config.verbose)
 
     # setup storage API
     config_storage = YamlConfigStorage(command_config.config)
```

### Comparing `urlwatch-2.8/share/man/man1/urlwatch.1` & `urlwatch-2.9/share/man/man1/urlwatch.1`

 * *Files 10% similar despite different names*

```diff
@@ -73,13 +73,13 @@
 .TP
 .B $XDG_CONFIG_HOME/urlwatch/urls.yaml
 A list of URLs, commands and other jobs to watch
 .TP
 .B $XDG_CONFIG_HOME/urlwatch/hooks.py
 A Python module that can implement new job types, filters and reporters
 .TP
-.B $XDG_CONFIG_HOME/urlwatch/cache.db
+.B $XDG_CACHE_HOME/urlwatch/cache.db
 A SQLite 3 database that contains the state history of jobs (for diffing)
 .SH AUTHOR
 Thomas Perl <thp.io/about>
 .SH WEBSITE
-http://thp.io/2008/urlwatch/
+https://thp.io/2008/urlwatch/
```

### Comparing `urlwatch-2.8/share/urlwatch/examples/hooks.py.example` & `urlwatch-2.9/share/urlwatch/examples/hooks.py.example`

 * *Files identical despite different names*

### Comparing `urlwatch-2.8/share/urlwatch/examples/urls.yaml.example` & `urlwatch-2.9/share/urlwatch/examples/urls.yaml.example`

 * *Files identical despite different names*

