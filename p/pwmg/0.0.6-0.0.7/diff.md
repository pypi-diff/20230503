# Comparing `tmp/pwmg-0.0.6.tar.gz` & `tmp/pwmg-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwmg-0.0.6.tar", last modified: Tue Dec 14 18:59:36 2021, max compression
+gzip compressed data, was "pwmg-0.0.7.tar", last modified: Tue May  2 22:50:55 2023, max compression
```

## Comparing `pwmg-0.0.6.tar` & `pwmg-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 fxia     (197610) None     (197121)        0 2021-12-14 18:59:36.825372 pwmg-0.0.6/
--rw-r--r--   0 fxia     (197610) None     (197121)     6207 2021-12-14 18:59:36.824403 pwmg-0.0.6/PKG-INFO
--rw-r--r--   0 fxia     (197610) None     (197121)     4633 2021-12-14 18:46:21.000000 pwmg-0.0.6/README.md
-drwxr-xr-x   0 fxia     (197610) None     (197121)        0 2021-12-14 18:59:36.806821 pwmg-0.0.6/pwmg/
--rw-r--r--   0 fxia     (197610) None     (197121)       18 2021-12-14 18:46:21.000000 pwmg-0.0.6/pwmg/__init__.py
--rwxr-xr-x   0 fxia     (197610) None     (197121)    13146 2021-12-14 18:54:49.000000 pwmg-0.0.6/pwmg/pwmg.py
-drwxr-xr-x   0 fxia     (197610) None     (197121)        0 2021-12-14 18:59:36.821470 pwmg-0.0.6/pwmg.egg-info/
--rw-r--r--   0 fxia     (197610) None     (197121)     6207 2021-12-14 18:59:36.000000 pwmg-0.0.6/pwmg.egg-info/PKG-INFO
--rw-r--r--   0 fxia     (197610) None     (197121)      206 2021-12-14 18:59:36.000000 pwmg-0.0.6/pwmg.egg-info/SOURCES.txt
--rw-r--r--   0 fxia     (197610) None     (197121)        1 2021-12-14 18:59:36.000000 pwmg-0.0.6/pwmg.egg-info/dependency_links.txt
--rw-r--r--   0 fxia     (197610) None     (197121)       41 2021-12-14 18:59:36.000000 pwmg-0.0.6/pwmg.egg-info/entry_points.txt
--rw-r--r--   0 fxia     (197610) None     (197121)        5 2021-12-14 18:59:36.000000 pwmg-0.0.6/pwmg.egg-info/top_level.txt
--rw-r--r--   0 fxia     (197610) None     (197121)      104 2021-12-14 18:46:21.000000 pwmg-0.0.6/pyproject.toml
--rw-r--r--   0 fxia     (197610) None     (197121)       38 2021-12-14 18:59:36.826351 pwmg-0.0.6/setup.cfg
--rw-r--r--   0 fxia     (197610) None     (197121)      788 2021-12-14 18:59:30.000000 pwmg-0.0.6/setup.py
+drwxrwxrwx   0 fxia      (1000) fxia      (1000)        0 2023-05-02 22:50:55.135253 pwmg-0.0.7/
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)     1089 2023-05-02 17:07:57.000000 pwmg-0.0.7/LICENSE
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)     5045 2023-05-02 22:50:55.119620 pwmg-0.0.7/PKG-INFO
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)     4633 2023-05-02 17:07:57.000000 pwmg-0.0.7/README.md
+drwxrwxrwx   0 fxia      (1000) fxia      (1000)        0 2023-05-02 22:50:55.005337 pwmg-0.0.7/pwmg/
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)       18 2023-05-02 17:07:57.000000 pwmg-0.0.7/pwmg/__init__.py
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)    13192 2023-05-02 22:32:55.000000 pwmg-0.0.7/pwmg/pwmg.py
+drwxrwxrwx   0 fxia      (1000) fxia      (1000)        0 2023-05-02 22:50:55.097482 pwmg-0.0.7/pwmg.egg-info/
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)     5045 2023-05-02 22:50:54.000000 pwmg-0.0.7/pwmg.egg-info/PKG-INFO
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)      214 2023-05-02 22:50:54.000000 pwmg-0.0.7/pwmg.egg-info/SOURCES.txt
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)        1 2023-05-02 22:50:54.000000 pwmg-0.0.7/pwmg.egg-info/dependency_links.txt
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)       40 2023-05-02 22:50:54.000000 pwmg-0.0.7/pwmg.egg-info/entry_points.txt
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)        5 2023-05-02 22:50:54.000000 pwmg-0.0.7/pwmg.egg-info/top_level.txt
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)      104 2023-05-02 17:07:57.000000 pwmg-0.0.7/pyproject.toml
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)       38 2023-05-02 22:50:55.135253 pwmg-0.0.7/setup.cfg
+-rwxrwxrwx   0 fxia      (1000) fxia      (1000)      788 2023-05-02 22:48:00.000000 pwmg-0.0.7/setup.py
```

### Comparing `pwmg-0.0.6/PKG-INFO` & `pwmg-0.0.7/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,157 +1,156 @@
 Metadata-Version: 2.1
 Name: pwmg
-Version: 0.0.6
+Version: 0.0.7
 Summary: A password management tool
 Home-page: https://github.com/fredxia/pwmg
 Author: Fred Xia
 Author-email: fredxia2011@gmail.com
-License: UNKNOWN
-Description: # pwmg
-        A password management tool
-        
-        `pwmg` is a standalone python3 script to manage a collection of password
-        entries. Each entry consists of a site name, an user account name,
-        and the password. `pwmg` will add a timestamp when it encrypts and stores
-        the password entry. The encrypted entries are stored in a local file.
-        
-        A master secrete key is used to encrypt and decrypt password entries.
-        
-        The algorithm for encryption is XTEA, with 64 rounds of computation.
-        See https://en.wikipedia.org/wiki/XTEA for more information. Each entry
-        is padded to 256 bytes, prepended and appended with randomly generated
-        printable characters. A '\0' is inserted to mark the start and/or end
-        of the password entry. The entire string is then encrypted, 8-byte
-        per block, with CBC.
-        
-        The master secrete key must be more than 8 characters long. It is advised,
-        but not enforced, to use mixed characters, special characters, and digits.
-        
-        Perhaps what's interesting about this program is that it is a single file,
-        uses only standard Python3 libraries, and does not require or download any
-        additional modules from PyPi repository or any other source. Hence the
-        user can be assured there is no possible malicious injection of Python
-        code. You can download just the `pwmg.py` and it is ready to use.
-        
-        You can install it with the `pip` command
-        
-        ```
-        # python3 -m pip install pwmg
-        ```
-        
-        Github link: https://github.com/fredxia/pwmg
-        
-        ## Usage
-        
-        The default file to store encrypted passwords is `~/.pwmg_db`. There is a
-        command line option `-f` to use a different file.
-        
-        To avoid potential leak of passwords in the shell `.history` file master secrete
-        key or password is only typed in at prompt, not with command line option.
-        
-        Below is an example to save a password. Notice the master secrete key is
-        not printed to the terminal (per Python3's `getpass` module).
-        
-        ```text
-        $ pwmg update 'fred walmart account' testuser2gmail@gmail.com
-        Secrete key:
-        Password for fred walmart account:Test&simple2
-        Site 'fred walmart account' password updated
-        
-        $ pwmg show
-        Secrete key:
-        
-            --------------------------------------------------------------------------
-            | SITE                 | USER NAME           | PASSWORD     | TIMESTAMP  |
-            --------------------------------------------------------------------------
-            | fred walmart account | testuser2@gmail.com | Test&simple2 | 2021-08-09 |
-            --------------------------------------------------------------------------
-        ```
-        
-        This is what the encrypted file looks like
-        
-        ```text
-        % cat ~/.pwmg_db
-        # password file created 2021-08-09
-        ziNbM2q+FHn7iD4UXWg8tx48DC38eEh+pg+0MxfJogMjsi3H0L3iOC09bISNABMWi4g3UttuMNmF3O7t89/ww7wv7hh1+D98fZ8g/WUkgk3FslRDdJLeGk34BFrP1nIzyQD5adrYRVXtBkFv5pBwBr/lQfWQjsLyP8hMuCJ1DzOFiMAjLRwnIUhitwAqXcQwjo06EHmoi9NllW7W2NAWZQWnMRHHzURt+uBtUvFY9JSAWdLGRDdo2FhfbSeLwfc5ZIbBneMJc0Ye3alP8J9rODwXnoLSHaMY9iLzowHWR72fVP0nZa23ZLsKuZ937EkCX1FJP85IPL+hdSdwS/Y1Yg==
-        ```
-        
-        You can also remove a site. export passwords to a CSV file, or import passwords
-        from an exported CSV file. For export and import the delimiter is assumed by
-        default to be TAB character (can be changed with `-d` option).
-        
-        Each functionality is a sub command. All sub commands can be listed by the
-        help option. Without any command line sub command specified the default is
-        "show" command.
-        
-        By convention arguments in square brackets are optional in the following "-h"
-        output.
-        
-        ```text
-        % pwmg -h
-        usage: pwmg [-h] [-f <FILENAME>] {show,rm,update,pw,import,export} ...
-        
-        A password management tool
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -f <FILENAME>, --file <FILENAME>
-                                Password file. Default is ~/.pwmg_db
-        
-        command:
-          {show,rm,update,pw,import,export}
-            show                show or search password entries
-            update              update or add password entry    
-            rm                  remove entry
-            pw                  change master secrete key
-            import              import from csv file
-            export              export to csv file
-        ```
-        
-        ```text
-        % pwmg update -h
-        usage: pwmg update [-h] <SITE> <USER NAME>
-        
-        positional arguments:
-          <SITE>       site to delete
-          <USER NAME>  user name
-        ```
-        
-        ```text
-        % pwmg show -h
-        usage: pwmg show [-h] [<NAME>]
-        
-        positional arguments:
-          <NAME>      site or user name
-        ```
-        
-        ```text
-        % pwmg rm -h
-        usage: pwmg rm [-h] <SITE>
-        
-        positional arguments:
-          <SITE>      site to delete
-        ```
-        
-        ```text
-        % pwmg import -h
-        usage: pwmg import [-h] [-d <DELIMITER>] <FILE>
-        
-        positional arguments:
-          <FILE>          file to import from
-        ```
-        
-        ```text
-        % pwmg export -h
-        usage: pwmg export [-h] [-d <DELIMITER>] <FILE>
-        
-        positional arguments:
-          <FILE>          file to export to
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pwmg
+A password management tool
+
+`pwmg` is a standalone python3 script to manage a collection of password
+entries. Each entry consists of a site name, an user account name,
+and the password. `pwmg` will add a timestamp when it encrypts and stores
+the password entry. The encrypted entries are stored in a local file.
+
+A master secrete key is used to encrypt and decrypt password entries.
+
+The algorithm for encryption is XTEA, with 64 rounds of computation.
+See https://en.wikipedia.org/wiki/XTEA for more information. Each entry
+is padded to 256 bytes, prepended and appended with randomly generated
+printable characters. A '\0' is inserted to mark the start and/or end
+of the password entry. The entire string is then encrypted, 8-byte
+per block, with CBC.
+
+The master secrete key must be more than 8 characters long. It is advised,
+but not enforced, to use mixed characters, special characters, and digits.
+
+Perhaps what's interesting about this program is that it is a single file,
+uses only standard Python3 libraries, and does not require or download any
+additional modules from PyPi repository or any other source. Hence the
+user can be assured there is no possible malicious injection of Python
+code. You can download just the `pwmg.py` and it is ready to use.
+
+You can install it with the `pip` command
+
+```
+# python3 -m pip install pwmg
+```
+
+Github link: https://github.com/fredxia/pwmg
+
+## Usage
+
+The default file to store encrypted passwords is `~/.pwmg_db`. There is a
+command line option `-f` to use a different file.
+
+To avoid potential leak of passwords in the shell `.history` file master secrete
+key or password is only typed in at prompt, not with command line option.
+
+Below is an example to save a password. Notice the master secrete key is
+not printed to the terminal (per Python3's `getpass` module).
+
+```text
+$ pwmg update 'fred walmart account' testuser2gmail@gmail.com
+Secrete key:
+Password for fred walmart account:Test&simple2
+Site 'fred walmart account' password updated
+
+$ pwmg show
+Secrete key:
+
+    --------------------------------------------------------------------------
+    | SITE                 | USER NAME           | PASSWORD     | TIMESTAMP  |
+    --------------------------------------------------------------------------
+    | fred walmart account | testuser2@gmail.com | Test&simple2 | 2021-08-09 |
+    --------------------------------------------------------------------------
+```
+
+This is what the encrypted file looks like
+
+```text
+% cat ~/.pwmg_db
+# password file created 2021-08-09
+ziNbM2q+FHn7iD4UXWg8tx48DC38eEh+pg+0MxfJogMjsi3H0L3iOC09bISNABMWi4g3UttuMNmF3O7t89/ww7wv7hh1+D98fZ8g/WUkgk3FslRDdJLeGk34BFrP1nIzyQD5adrYRVXtBkFv5pBwBr/lQfWQjsLyP8hMuCJ1DzOFiMAjLRwnIUhitwAqXcQwjo06EHmoi9NllW7W2NAWZQWnMRHHzURt+uBtUvFY9JSAWdLGRDdo2FhfbSeLwfc5ZIbBneMJc0Ye3alP8J9rODwXnoLSHaMY9iLzowHWR72fVP0nZa23ZLsKuZ937EkCX1FJP85IPL+hdSdwS/Y1Yg==
+```
+
+You can also remove a site. export passwords to a CSV file, or import passwords
+from an exported CSV file. For export and import the delimiter is assumed by
+default to be TAB character (can be changed with `-d` option).
+
+Each functionality is a sub command. All sub commands can be listed by the
+help option. Without any command line sub command specified the default is
+"show" command.
+
+By convention arguments in square brackets are optional in the following "-h"
+output.
+
+```text
+% pwmg -h
+usage: pwmg [-h] [-f <FILENAME>] {show,rm,update,pw,import,export} ...
+
+A password management tool
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f <FILENAME>, --file <FILENAME>
+                        Password file. Default is ~/.pwmg_db
+
+command:
+  {show,rm,update,pw,import,export}
+    show                show or search password entries
+    update              update or add password entry    
+    rm                  remove entry
+    pw                  change master secrete key
+    import              import from csv file
+    export              export to csv file
+```
+
+```text
+% pwmg update -h
+usage: pwmg update [-h] <SITE> <USER NAME>
+
+positional arguments:
+  <SITE>       site to delete
+  <USER NAME>  user name
+```
+
+```text
+% pwmg show -h
+usage: pwmg show [-h] [<NAME>]
+
+positional arguments:
+  <NAME>      site or user name
+```
+
+```text
+% pwmg rm -h
+usage: pwmg rm [-h] <SITE>
+
+positional arguments:
+  <SITE>      site to delete
+```
+
+```text
+% pwmg import -h
+usage: pwmg import [-h] [-d <DELIMITER>] <FILE>
+
+positional arguments:
+  <FILE>          file to import from
+```
+
+```text
+% pwmg export -h
+usage: pwmg export [-h] [-d <DELIMITER>] <FILE>
+
+positional arguments:
+  <FILE>          file to export to
+
+```
```

### Comparing `pwmg-0.0.6/README.md` & `pwmg-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pwmg-0.0.6/pwmg/pwmg.py` & `pwmg-0.0.7/pwmg/pwmg.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,17 @@
     if m == 0:
         return bv
     pad_len = block_sz - m - 2
     p = [ ord(random.choice(string.printable)) for _ in range(pad_len) ]
     split = random.randint(0, pad_len)
     bv2 = bytes(p[:split]) + bytes([0]) + bv
     if split < pad_len:
-        bv2 += bytes([0]) + bytes(p[split:])
+        bv2 = bv2 + bytes([0]) + bytes(p[split:])
+    else:
+        bv2 = bv2 + bytes([0])
     assert len(bv2) % block_sz == 0
     return bv2
 
 def unpad_str(value):
     idx = value.find("\x00")
     if idx < 0:
         return value
```

### Comparing `pwmg-0.0.6/pwmg.egg-info/PKG-INFO` & `pwmg-0.0.7/pwmg.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,157 +1,156 @@
 Metadata-Version: 2.1
 Name: pwmg
-Version: 0.0.6
+Version: 0.0.7
 Summary: A password management tool
 Home-page: https://github.com/fredxia/pwmg
 Author: Fred Xia
 Author-email: fredxia2011@gmail.com
-License: UNKNOWN
-Description: # pwmg
-        A password management tool
-        
-        `pwmg` is a standalone python3 script to manage a collection of password
-        entries. Each entry consists of a site name, an user account name,
-        and the password. `pwmg` will add a timestamp when it encrypts and stores
-        the password entry. The encrypted entries are stored in a local file.
-        
-        A master secrete key is used to encrypt and decrypt password entries.
-        
-        The algorithm for encryption is XTEA, with 64 rounds of computation.
-        See https://en.wikipedia.org/wiki/XTEA for more information. Each entry
-        is padded to 256 bytes, prepended and appended with randomly generated
-        printable characters. A '\0' is inserted to mark the start and/or end
-        of the password entry. The entire string is then encrypted, 8-byte
-        per block, with CBC.
-        
-        The master secrete key must be more than 8 characters long. It is advised,
-        but not enforced, to use mixed characters, special characters, and digits.
-        
-        Perhaps what's interesting about this program is that it is a single file,
-        uses only standard Python3 libraries, and does not require or download any
-        additional modules from PyPi repository or any other source. Hence the
-        user can be assured there is no possible malicious injection of Python
-        code. You can download just the `pwmg.py` and it is ready to use.
-        
-        You can install it with the `pip` command
-        
-        ```
-        # python3 -m pip install pwmg
-        ```
-        
-        Github link: https://github.com/fredxia/pwmg
-        
-        ## Usage
-        
-        The default file to store encrypted passwords is `~/.pwmg_db`. There is a
-        command line option `-f` to use a different file.
-        
-        To avoid potential leak of passwords in the shell `.history` file master secrete
-        key or password is only typed in at prompt, not with command line option.
-        
-        Below is an example to save a password. Notice the master secrete key is
-        not printed to the terminal (per Python3's `getpass` module).
-        
-        ```text
-        $ pwmg update 'fred walmart account' testuser2gmail@gmail.com
-        Secrete key:
-        Password for fred walmart account:Test&simple2
-        Site 'fred walmart account' password updated
-        
-        $ pwmg show
-        Secrete key:
-        
-            --------------------------------------------------------------------------
-            | SITE                 | USER NAME           | PASSWORD     | TIMESTAMP  |
-            --------------------------------------------------------------------------
-            | fred walmart account | testuser2@gmail.com | Test&simple2 | 2021-08-09 |
-            --------------------------------------------------------------------------
-        ```
-        
-        This is what the encrypted file looks like
-        
-        ```text
-        % cat ~/.pwmg_db
-        # password file created 2021-08-09
-        ziNbM2q+FHn7iD4UXWg8tx48DC38eEh+pg+0MxfJogMjsi3H0L3iOC09bISNABMWi4g3UttuMNmF3O7t89/ww7wv7hh1+D98fZ8g/WUkgk3FslRDdJLeGk34BFrP1nIzyQD5adrYRVXtBkFv5pBwBr/lQfWQjsLyP8hMuCJ1DzOFiMAjLRwnIUhitwAqXcQwjo06EHmoi9NllW7W2NAWZQWnMRHHzURt+uBtUvFY9JSAWdLGRDdo2FhfbSeLwfc5ZIbBneMJc0Ye3alP8J9rODwXnoLSHaMY9iLzowHWR72fVP0nZa23ZLsKuZ937EkCX1FJP85IPL+hdSdwS/Y1Yg==
-        ```
-        
-        You can also remove a site. export passwords to a CSV file, or import passwords
-        from an exported CSV file. For export and import the delimiter is assumed by
-        default to be TAB character (can be changed with `-d` option).
-        
-        Each functionality is a sub command. All sub commands can be listed by the
-        help option. Without any command line sub command specified the default is
-        "show" command.
-        
-        By convention arguments in square brackets are optional in the following "-h"
-        output.
-        
-        ```text
-        % pwmg -h
-        usage: pwmg [-h] [-f <FILENAME>] {show,rm,update,pw,import,export} ...
-        
-        A password management tool
-        
-        optional arguments:
-          -h, --help            show this help message and exit
-          -f <FILENAME>, --file <FILENAME>
-                                Password file. Default is ~/.pwmg_db
-        
-        command:
-          {show,rm,update,pw,import,export}
-            show                show or search password entries
-            update              update or add password entry    
-            rm                  remove entry
-            pw                  change master secrete key
-            import              import from csv file
-            export              export to csv file
-        ```
-        
-        ```text
-        % pwmg update -h
-        usage: pwmg update [-h] <SITE> <USER NAME>
-        
-        positional arguments:
-          <SITE>       site to delete
-          <USER NAME>  user name
-        ```
-        
-        ```text
-        % pwmg show -h
-        usage: pwmg show [-h] [<NAME>]
-        
-        positional arguments:
-          <NAME>      site or user name
-        ```
-        
-        ```text
-        % pwmg rm -h
-        usage: pwmg rm [-h] <SITE>
-        
-        positional arguments:
-          <SITE>      site to delete
-        ```
-        
-        ```text
-        % pwmg import -h
-        usage: pwmg import [-h] [-d <DELIMITER>] <FILE>
-        
-        positional arguments:
-          <FILE>          file to import from
-        ```
-        
-        ```text
-        % pwmg export -h
-        usage: pwmg export [-h] [-d <DELIMITER>] <FILE>
-        
-        positional arguments:
-          <FILE>          file to export to
-        
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# pwmg
+A password management tool
+
+`pwmg` is a standalone python3 script to manage a collection of password
+entries. Each entry consists of a site name, an user account name,
+and the password. `pwmg` will add a timestamp when it encrypts and stores
+the password entry. The encrypted entries are stored in a local file.
+
+A master secrete key is used to encrypt and decrypt password entries.
+
+The algorithm for encryption is XTEA, with 64 rounds of computation.
+See https://en.wikipedia.org/wiki/XTEA for more information. Each entry
+is padded to 256 bytes, prepended and appended with randomly generated
+printable characters. A '\0' is inserted to mark the start and/or end
+of the password entry. The entire string is then encrypted, 8-byte
+per block, with CBC.
+
+The master secrete key must be more than 8 characters long. It is advised,
+but not enforced, to use mixed characters, special characters, and digits.
+
+Perhaps what's interesting about this program is that it is a single file,
+uses only standard Python3 libraries, and does not require or download any
+additional modules from PyPi repository or any other source. Hence the
+user can be assured there is no possible malicious injection of Python
+code. You can download just the `pwmg.py` and it is ready to use.
+
+You can install it with the `pip` command
+
+```
+# python3 -m pip install pwmg
+```
+
+Github link: https://github.com/fredxia/pwmg
+
+## Usage
+
+The default file to store encrypted passwords is `~/.pwmg_db`. There is a
+command line option `-f` to use a different file.
+
+To avoid potential leak of passwords in the shell `.history` file master secrete
+key or password is only typed in at prompt, not with command line option.
+
+Below is an example to save a password. Notice the master secrete key is
+not printed to the terminal (per Python3's `getpass` module).
+
+```text
+$ pwmg update 'fred walmart account' testuser2gmail@gmail.com
+Secrete key:
+Password for fred walmart account:Test&simple2
+Site 'fred walmart account' password updated
+
+$ pwmg show
+Secrete key:
+
+    --------------------------------------------------------------------------
+    | SITE                 | USER NAME           | PASSWORD     | TIMESTAMP  |
+    --------------------------------------------------------------------------
+    | fred walmart account | testuser2@gmail.com | Test&simple2 | 2021-08-09 |
+    --------------------------------------------------------------------------
+```
+
+This is what the encrypted file looks like
+
+```text
+% cat ~/.pwmg_db
+# password file created 2021-08-09
+ziNbM2q+FHn7iD4UXWg8tx48DC38eEh+pg+0MxfJogMjsi3H0L3iOC09bISNABMWi4g3UttuMNmF3O7t89/ww7wv7hh1+D98fZ8g/WUkgk3FslRDdJLeGk34BFrP1nIzyQD5adrYRVXtBkFv5pBwBr/lQfWQjsLyP8hMuCJ1DzOFiMAjLRwnIUhitwAqXcQwjo06EHmoi9NllW7W2NAWZQWnMRHHzURt+uBtUvFY9JSAWdLGRDdo2FhfbSeLwfc5ZIbBneMJc0Ye3alP8J9rODwXnoLSHaMY9iLzowHWR72fVP0nZa23ZLsKuZ937EkCX1FJP85IPL+hdSdwS/Y1Yg==
+```
+
+You can also remove a site. export passwords to a CSV file, or import passwords
+from an exported CSV file. For export and import the delimiter is assumed by
+default to be TAB character (can be changed with `-d` option).
+
+Each functionality is a sub command. All sub commands can be listed by the
+help option. Without any command line sub command specified the default is
+"show" command.
+
+By convention arguments in square brackets are optional in the following "-h"
+output.
+
+```text
+% pwmg -h
+usage: pwmg [-h] [-f <FILENAME>] {show,rm,update,pw,import,export} ...
+
+A password management tool
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -f <FILENAME>, --file <FILENAME>
+                        Password file. Default is ~/.pwmg_db
+
+command:
+  {show,rm,update,pw,import,export}
+    show                show or search password entries
+    update              update or add password entry    
+    rm                  remove entry
+    pw                  change master secrete key
+    import              import from csv file
+    export              export to csv file
+```
+
+```text
+% pwmg update -h
+usage: pwmg update [-h] <SITE> <USER NAME>
+
+positional arguments:
+  <SITE>       site to delete
+  <USER NAME>  user name
+```
+
+```text
+% pwmg show -h
+usage: pwmg show [-h] [<NAME>]
+
+positional arguments:
+  <NAME>      site or user name
+```
+
+```text
+% pwmg rm -h
+usage: pwmg rm [-h] <SITE>
+
+positional arguments:
+  <SITE>      site to delete
+```
+
+```text
+% pwmg import -h
+usage: pwmg import [-h] [-d <DELIMITER>] <FILE>
+
+positional arguments:
+  <FILE>          file to import from
+```
+
+```text
+% pwmg export -h
+usage: pwmg export [-h] [-d <DELIMITER>] <FILE>
+
+positional arguments:
+  <FILE>          file to export to
+
+```
```

### Comparing `pwmg-0.0.6/setup.py` & `pwmg-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 packages = ["pwmg"]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pwmg",
-    version="0.0.6",
+    version="0.0.7",
     author="Fred Xia",
     author_email="fredxia2011@gmail.com",
     description="A password management tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fredxia/pwmg",
     classifiers=[
```

