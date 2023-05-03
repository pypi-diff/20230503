# Comparing `tmp/pyuftp-0.0.3.tar.gz` & `tmp/pyuftp-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuftp-0.0.3.tar", last modified: Fri Apr 28 13:21:48 2023, max compression
+gzip compressed data, was "pyuftp-0.0.4.tar", last modified: Wed May  3 10:53:04 2023, max compression
```

## Comparing `pyuftp-0.0.3.tar` & `pyuftp-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:21:48.222013 pyuftp-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-04-28 13:21:35.000000 pyuftp-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 13:21:48.222013 pyuftp-0.0.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)      170 2023-04-28 13:21:35.000000 pyuftp-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-28 13:21:35.000000 pyuftp-0.0.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:21:48.226013 pyuftp-0.0.3/pyuftp/
--rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-04-28 13:21:35.000000 pyuftp-0.0.3/pyuftp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 13:21:48.226013 pyuftp-0.0.3/pyuftp/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-28 13:21:35.000000 pyuftp-0.0.3/pyuftp/authenticate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-04-28 13:21:35.000000 pyuftp-0.0.3/pyuftp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-04-28 13:21:35.000000 pyuftp-0.0.3/pyuftp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6420 2023-04-28 13:21:35.000000 pyuftp-0.0.3/pyuftp/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-04-28 13:21:35.000000 pyuftp-0.0.3/pyuftp/uftp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-28 13:21:35.000000 pyuftp-0.0.3/pyuftp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 13:21:48.222013 pyuftp-0.0.3/pyuftp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-28 13:21:48.000000 pyuftp-0.0.3/pyuftp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-28 13:21:48.000000 pyuftp-0.0.3/pyuftp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 13:21:48.000000 pyuftp-0.0.3/pyuftp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-28 13:21:48.000000 pyuftp-0.0.3/pyuftp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 13:21:48.000000 pyuftp-0.0.3/pyuftp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-28 13:21:48.000000 pyuftp-0.0.3/pyuftp.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      190 2023-04-28 13:21:48.222013 pyuftp-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1867 2023-04-28 13:21:35.000000 pyuftp-0.0.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-28 13:21:35.000000 pyuftp-0.0.3/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:53:04.332293 pyuftp-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-03 10:52:53.000000 pyuftp-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-03 10:53:04.332293 pyuftp-0.0.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1108 2023-05-03 10:52:53.000000 pyuftp-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:53:04.332293 pyuftp-0.0.4/pyuftp/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       74 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyuftp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 10:53:04.332293 pyuftp-0.0.4/pyuftp/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyuftp/authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6770 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyuftp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyuftp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyuftp/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyuftp/share.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyuftp/uftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-05-03 10:52:53.000000 pyuftp-0.0.4/pyuftp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 10:53:04.332293 pyuftp-0.0.4/pyuftp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-03 10:53:04.000000 pyuftp-0.0.4/pyuftp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-03 10:53:04.000000 pyuftp-0.0.4/pyuftp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 10:53:04.000000 pyuftp-0.0.4/pyuftp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 10:53:04.000000 pyuftp-0.0.4/pyuftp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-03 10:53:04.000000 pyuftp-0.0.4/pyuftp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 10:53:04.000000 pyuftp-0.0.4/pyuftp.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      190 2023-05-03 10:53:04.332293 pyuftp-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1062 2023-05-03 10:52:53.000000 pyuftp-0.0.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-05-03 10:52:53.000000 pyuftp-0.0.4/versioneer.py
```

### Comparing `pyuftp-0.0.3/LICENSE` & `pyuftp-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuftp-0.0.3/pyuftp/authenticate.py` & `pyuftp-0.0.4/pyuftp/authenticate.py`

 * *Files 14% similar despite different names*

```diff
@@ -83,68 +83,14 @@
 
     def __repr__(self):
         return f"OIDC"
 
     __str__ = __repr__
 
 
-class RefreshHandler:
-    """helper to refresh an OAuth token"""
-
-    def __init__(self, refresh_config, token=None):
-        """
-        token: initial access token (can be None)
-        refresh_config: a dict containing url, client_id, client_secret, refresh_token
-        """
-        self.refresh_config = refresh_config
-        self.token = token
-        if not token:
-            self.refresh()
-
-    def is_valid_token(self):
-        """
-        check if the given token is still valid
-        TODO check whether token was revoked
-        """
-        try:
-            jwt_decode(
-                self.token,
-                options={
-                    "verify_signature": False,
-                    "verify_nbf": False,
-                    "verify_exp": True,
-                    "verify_aud": False,
-                },
-            )
-            return True
-        except ExpiredSignatureError:
-            return False
-
-    def refresh(self):
-        """refresh the token"""
-        params = dict(
-            client_id=self.refresh_config["client_id"],
-            client_secret=self.refresh_config["client_secret"],
-            refresh_token=self.refresh_config["refresh_token"],
-            grant_type="refresh_token",
-        )
-        url = "%stoken" % self.refresh_config["url"]
-
-        res = requests.post(url, headers={"Accept": "application/json"}, data=params)
-        res.raise_for_status()
-        self.token = res.json()["access_token"]
-        return self.token
-
-    def get_token(self):
-        """get a valid access token. If necessary, refresh it."""
-        if not self.is_valid_token():
-            self.refresh()
-        return self.token
-
-
 class JWTToken(Credential):
     """
     Produces a signed JWT token ("Bearer <auth_token>")
     uses pyjwt
 
     Args:
         subject - the subject user name or user X.500 DN
@@ -188,14 +134,26 @@
         return "Bearer " + self.create_token()
 
     def __repr__(self):
         return f"JWT"
 
     __str__ = __repr__
 
+class Anonymous(Credential):
+    """
+    Anonymous access - no auth header at all
+    """
+
+    def get_auth_header(self):
+        return None
+    
+    def __repr__(self):
+        return f"ANONYMOUS"
+
+    __str__ = __repr__
 
 def create_credential(username=None, password=None, token=None, identity=None):
     """Helper to create the most common types of credentials
 
     Requires one of the following combinations of arguments
 
     username + password : create a UsernamePassword credential
@@ -203,15 +161,18 @@
     username + identity : create a JWTToken credential which will be signed
                           with the given private key (ssh key or PEM)
     """
 
     if token is not None:
         return OIDCToken(token)
     if token is None and identity is None:
-        return UsernamePassword(username, password)
+        if username=="anonymous":
+            return Anonymous()
+        else:
+            return UsernamePassword(username, password)
     if identity is None:
         raise AuthenticationFailedException("Not enough info to create user credential")
     try:
         from cryptography.hazmat.primitives import serialization
         pem = open(identity).read()
         pem_bytes = bytes(pem, "UTF-8")
         if password is not None and len(password) > 0:
@@ -259,25 +220,27 @@
         "Accept": "application/json",
     }
     with requests.get(headers=_headers, url=url, verify=False) as res:
         check_error(res)
         js = res.json()
     return js
 
-def post_json(url, credential, json_data):
+def post_json(url, credential, json_data, as_json = True):
     _headers = {
         "Authorization": credential.get_auth_header(),
         "Accept": "application/json",
         "Content-Type": "application/json"
     }
     with requests.post(headers=_headers, url=url, json=json_data, verify=False) as res:
         check_error(res)
-        js = res.json()
-    return js
-
+        if res.status_code==201:
+            return res.headers['Location']
+        elif as_json:
+            return res.json()
+    
 def check_error(res):
     """checks for error and extracts any error info sent by the server"""
     if 400 <= res.status_code < 600:
         reason = res.reason
         try:
             reason = res.json().get("errorMessage", "n/a")
         except ValueError:
```

### Comparing `pyuftp-0.0.3/pyuftp/base.py` & `pyuftp-0.0.4/pyuftp/base.py`

 * *Files identical despite different names*

### Comparing `pyuftp-0.0.3/pyuftp/client.py` & `pyuftp-0.0.4/pyuftp/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 """ Main client class """
 
-import pyuftp.base, pyuftp.cp, pyuftp.utils, pyuftp._version
+import pyuftp.base, pyuftp.cp, pyuftp.share, pyuftp.utils, pyuftp._version
 
-import sys
+import platform, sys
 
 _commands = {
             "authenticate": pyuftp.base.Auth(),
             "checksum": pyuftp.utils.Checksum(),
             "cp": pyuftp.cp.Copy(),
             "find": pyuftp.utils.Find(),
             "info": pyuftp.base.Info(),
             "ls": pyuftp.utils.Ls(),
-            "mkdir": pyuftp.utils.Mkdir(),  
-            "rm": pyuftp.utils.Rm(),  
+            "mkdir": pyuftp.utils.Mkdir(),
+            "rm": pyuftp.utils.Rm(),
+            "share": pyuftp.share.Share(),
         }
 
 def show_version():
     print("PyUFTP commandline client for UFTP (UNICORE FTP) "
           "%s, https://www.unicore.eu" % pyuftp._version.get_versions().get('version', "n/a"))
     print("Python %s" % sys.version)
+    print("OS: %s" % platform.platform())
+
 
 def help():
     s = """PyUFTP commandline client for UFTP (UNICORE FTP) %s, https://www.unicore.eu
 Usage: pyuftp <command> [OPTIONS] <args>
 The following commands are available:""" % pyuftp._version.get_versions().get('version', "n/a")
     print(s)
     for cmd in _commands:
         print (f" {cmd:20} - {_commands[cmd].get_synopsis()}")
     print("Enter 'pyuftp <command> -h' for help on a particular command.")
 
 def run(args):
-
     _help = ["help", "-h", "--help"]
-
     if len(args)<1 or args[0] in _help:
         help()
         return
-
     _version = ["version", "-V", "--version"]
-    
     if args[0] in _version:
         show_version()
         return
-        
+
     command = None
     cmd = args[0]
     for k in _commands:
         if k.startswith(cmd):
             command = _commands[k]
             break
     if command is None:
```

### Comparing `pyuftp-0.0.3/pyuftp/cp.py` & `pyuftp-0.0.4/pyuftp/cp.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,21 +9,24 @@
         self.parser.prog = "pyuftp cp"
         self.parser.description = self.get_synopsis()
         self.parser.add_argument("source", nargs="+", help="Source(s)")
         self.parser.add_argument("target", help="Target")
         self.parser.add_argument("-r", "--recurse", required=False, action="store_true",
                             help="recurse into subdirectories, if applicable")
         self.parser.add_argument("-B", "--bytes", help="Byte range", required=False)
+        self.parser.add_argument("-a", "--archive", action="store_true", required=False,
+                                 help="Tell server to interpret data as tar/zip stream and unpack it")
         
     def get_synopsis(self):
         return """Copy file(s)"""
 
     def run(self, args):
         super().run(args)
         self.init_range()
+        self.archive_mode = self.args.archive
         for s in self.args.source:
             self.verbose(f"Copy {s} --> {self.args.target}")
             endpoint, _, _ = self.parse_url(self.args.target)
             if not endpoint:
                 self.do_download(s, self.args.target)
             else:
                 self.do_upload(s, self.args.target)
@@ -87,14 +90,16 @@
 
     def do_upload(self, local, remote):
         """ upload local source (which can specify wildcards) to a remote location """
         endpoint, base_dir, remote_file_name  = self.parse_url(remote)
         uftp = pyuftp.uftp.UFTP()
         host, port, onetime_pwd = self.authenticate(endpoint, base_dir)
         with pyuftp.uftp.open(host, port, onetime_pwd) as uftp:
+            if self.archive_mode:
+                uftp.set_archive_mode()
             if "-"==local:
                 offset, length = self._get_range()
                 writer = uftp.get_write_socket(remote_file_name, 0, length).makefile("wb")
                 total, duration = uftp.copy_data(sys.stdin.buffer, writer, length)
                 self.log_usage(True, "stdin", remote_file_name, total, duration)
                 writer.close()
                 uftp.finish_transfer()
```

### Comparing `pyuftp-0.0.3/pyuftp/uftp.py` & `pyuftp-0.0.4/pyuftp/uftp.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,17 @@
         try:
             reply = self.ftp.sendcmd(f"MFMT {stime} {path}")
             if not reply.startswith("213"):
                 raise OSError("Could not set time: " % reply)
         except ftplib.Error as e:
             raise OSError(e)
 
+    def set_archive_mode(self):
+        self.ftp.sendcmd("TYPE ARCHIVE")
+
     def checksum(self, path, algo=None):
         """ get a checksum """
         path = self.normalize(path)
         try:
             if algo:
                 reply = self.ftp.sendcmd("OPTS HASH %s" % algo)
                 if not reply.startswith("200"):
```

### Comparing `pyuftp-0.0.3/pyuftp/utils.py` & `pyuftp-0.0.4/pyuftp/utils.py`

 * *Files identical despite different names*

### Comparing `pyuftp-0.0.3/versioneer.py` & `pyuftp-0.0.4/versioneer.py`

 * *Files identical despite different names*

