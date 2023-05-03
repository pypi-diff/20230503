# Comparing `tmp/MHTMLconverter-0.2.tar.gz` & `tmp/MHTMLconverter-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MHTMLconverter-0.2.tar", last modified: Mon May  1 12:05:04 2023, max compression
+gzip compressed data, was "MHTMLconverter-0.3.tar", last modified: Wed May  3 11:29:32 2023, max compression
```

## Comparing `MHTMLconverter-0.2.tar` & `MHTMLconverter-0.3.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 12:05:04.008056 MHTMLconverter-0.2/
-drwxrwxrwx   0        0        0        0 2023-05-01 12:05:03.988381 MHTMLconverter-0.2/MHTMLconverter.egg-info/
--rw-rw-rw-   0        0        0     1073 2023-05-01 12:05:03.000000 MHTMLconverter-0.2/MHTMLconverter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-05-01 12:05:03.000000 MHTMLconverter-0.2/MHTMLconverter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 12:05:03.000000 MHTMLconverter-0.2/MHTMLconverter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2023-05-01 12:05:03.000000 MHTMLconverter-0.2/MHTMLconverter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-01 12:05:03.000000 MHTMLconverter-0.2/MHTMLconverter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1073 2023-05-01 12:05:04.009053 MHTMLconverter-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      726 2023-05-01 11:59:11.000000 MHTMLconverter-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 12:05:03.997532 MHTMLconverter-0.2/mhtmlconverter/
--rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.2/mhtmlconverter/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 12:05:04.007056 MHTMLconverter-0.2/mhtmlconverter/cli/
--rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.2/mhtmlconverter/cli/__init__.py
--rw-rw-rw-   0        0        0      798 2023-04-30 15:11:33.000000 MHTMLconverter-0.2/mhtmlconverter/cli/html2mhtml.py
--rw-rw-rw-   0        0        0      772 2023-04-30 15:11:55.000000 MHTMLconverter-0.2/mhtmlconverter/cli/md2mhtml.py
--rw-rw-rw-   0        0        0      739 2023-04-30 14:18:11.000000 MHTMLconverter-0.2/mhtmlconverter/fileutility.py
--rw-rw-rw-   0        0        0     2758 2023-04-29 18:40:26.000000 MHTMLconverter-0.2/mhtmlconverter/htmlutility.py
--rw-rw-rw-   0        0        0     3803 2023-04-30 14:19:03.000000 MHTMLconverter-0.2/mhtmlconverter/mhtml.py
--rw-rw-rw-   0        0        0       92 2023-04-30 14:53:31.000000 MHTMLconverter-0.2/pyproject.toml
--rw-rw-rw-   0        0        0      515 2023-05-01 12:05:04.010056 MHTMLconverter-0.2/setup.cfg
--rw-rw-rw-   0        0        0      293 2023-04-30 16:01:35.000000 MHTMLconverter-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.336892 MHTMLconverter-0.3/
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.319806 MHTMLconverter-0.3/MHTMLconverter.egg-info/
+-rw-rw-rw-   0        0        0     1081 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      663 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-03 11:29:32.000000 MHTMLconverter-0.3/MHTMLconverter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1081 2023-05-03 11:29:32.337912 MHTMLconverter-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.328360 MHTMLconverter-0.3/mhtmlconverter/
+-rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.3/mhtmlconverter/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.333372 MHTMLconverter-0.3/mhtmlconverter/cli/
+-rw-rw-rw-   0        0        0        0 2023-04-30 14:14:46.000000 MHTMLconverter-0.3/mhtmlconverter/cli/__init__.py
+-rw-rw-rw-   0        0        0      845 2023-05-02 17:55:24.000000 MHTMLconverter-0.3/mhtmlconverter/cli/html2mhtml.py
+-rw-rw-rw-   0        0        0      945 2023-05-02 17:57:20.000000 MHTMLconverter-0.3/mhtmlconverter/cli/md2mhtml.py
+-rw-rw-rw-   0        0        0     1033 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/mhtmlconverter/fileutility.py
+-rw-rw-rw-   0        0        0     5029 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/mhtmlconverter/htmlutility.py
+-rw-rw-rw-   0        0        0     5260 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/mhtmlconverter/mhtml.py
+-rw-rw-rw-   0        0        0       92 2023-04-30 14:53:31.000000 MHTMLconverter-0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      515 2023-05-03 11:29:32.338904 MHTMLconverter-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      293 2023-04-30 16:01:35.000000 MHTMLconverter-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:29:32.336892 MHTMLconverter-0.3/tests/
+-rw-rw-rw-   0        0        0     1036 2023-05-03 11:20:43.000000 MHTMLconverter-0.3/tests/test_html.py
+-rw-rw-rw-   0        0        0      988 2023-05-02 19:55:58.000000 MHTMLconverter-0.3/tests/test_md.py
```

### Comparing `MHTMLconverter-0.2/MHTMLconverter.egg-info/PKG-INFO` & `MHTMLconverter-0.3/MHTMLconverter.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MHTMLconverter
-Version: 0.2
+Version: 0.3
 Summary: Tools to convert markdown or html files including images to a single MHTML self-content file
 Home-page: https://github.com/arnaudrevel/MHTMLconverter
 Author: Arnaud Revel
 Author-email: revel.arnaud@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
@@ -29,10 +29,10 @@
 Converts markdown files (either local or remote) to mhtml, including referenced images.
 
 ```
 >> python -m mhtmlconverter.cli.md2mhtml -i README.md -o my_output.mhtml
 
 ```
 
-### TODO
+### ~~TODO~~
 
-css are not yet managed :/
+~~css are not yet managed :/~~
```

### Comparing `MHTMLconverter-0.2/MHTMLconverter.egg-info/SOURCES.txt` & `MHTMLconverter-0.3/MHTMLconverter.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -14,8 +14,10 @@
 mhtmlconverter.egg-info/PKG-INFO
 mhtmlconverter.egg-info/SOURCES.txt
 mhtmlconverter.egg-info/dependency_links.txt
 mhtmlconverter.egg-info/requires.txt
 mhtmlconverter.egg-info/top_level.txt
 mhtmlconverter/cli/__init__.py
 mhtmlconverter/cli/html2mhtml.py
-mhtmlconverter/cli/md2mhtml.py
+mhtmlconverter/cli/md2mhtml.py
+tests/test_html.py
+tests/test_md.py
```

### Comparing `MHTMLconverter-0.2/PKG-INFO` & `MHTMLconverter-0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MHTMLconverter
-Version: 0.2
+Version: 0.3
 Summary: Tools to convert markdown or html files including images to a single MHTML self-content file
 Home-page: https://github.com/arnaudrevel/MHTMLconverter
 Author: Arnaud Revel
 Author-email: revel.arnaud@gmail.com
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
@@ -29,10 +29,10 @@
 Converts markdown files (either local or remote) to mhtml, including referenced images.
 
 ```
 >> python -m mhtmlconverter.cli.md2mhtml -i README.md -o my_output.mhtml
 
 ```
 
-### TODO
+### ~~TODO~~
 
-css are not yet managed :/
+~~css are not yet managed :/~~
```

### Comparing `MHTMLconverter-0.2/README.md` & `MHTMLconverter-0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -19,10 +19,10 @@
 Converts markdown files (either local or remote) to mhtml, including referenced images.
 
 ```
 >> python -m mhtmlconverter.cli.md2mhtml -i README.md -o my_output.mhtml
 
 ```
 
-### TODO
+### ~~TODO~~
 
-css are not yet managed :/
+~~css are not yet managed :/~~
```

### Comparing `MHTMLconverter-0.2/mhtmlconverter/cli/html2mhtml.py` & `MHTMLconverter-0.3/mhtmlconverter/cli/html2mhtml.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 logging.basicConfig(level=logging.INFO,format="\x1b[32;20m %(filename)s > \x1b[34;20m %(funcName)s : \x1b[0m %(message)s")
 
 
 @click.command(help="HTML to MHTML converter")
 @click.option("-i","--input","htmlfile",required=True, help="html input filename")
 @click.option("-o","--output","outputfile",default="output.mhtml",help="mhtml output filename")
-def main(htmlfile,outputfile):
+def main(htmlfile:str = "index.html",outputfile:str = "output.mhtml")-> None:
     """
     Main program
     Converts the 'htmlfile' with references to images into an mhtml single file
     """
     mhtml.url_to_mhtml(htmlfile,outputfile)
 
  # Main entry point
```

### Comparing `MHTMLconverter-0.2/mhtmlconverter/cli/md2mhtml.py` & `MHTMLconverter-0.3/mhtmlconverter/cli/md2mhtml.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 This package intends to provide a tool to convert markdown files including
 images to a single MHTML self-content file
 """
 import logging
-from .. import mhtml
 import click
 import markdown
-
+from .. import mhtml
 
 logging.basicConfig(level=logging.INFO,format="%(filename)s - %(funcName)s - %(message)s")
 
 
 @click.command(help="MD to MHTML converter")
 @click.option("-i","--input","mdfile", required=True,help="md input filename")
 @click.option("-o","--output","outputfile",default="output.mhtml",help="mhtml output filename")
-def main(mdfile,outputfile):
-    with open(mdfile,"r") as f:
-        htmlcontent = markdown.markdown(f.read())
+def main(mdfile:str = "README.md",outputfile: str = "output.mhtml") -> None:
+    """
+    Main program
+    Converts the 'mdfile' with references to images into an mhtml single file
+    """
+    with open(mdfile,"r") as md_file:
+        htmlcontent = markdown.markdown(md_file.read())
         mhtml.html_content_to_mhtml(htmlcontent,outputfile, mdfile)
 
  # Main entry point
 if __name__ == "__main__":
     main()
```

### Comparing `MHTMLconverter-0.2/setup.cfg` & `MHTMLconverter-0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6874 6d6c 636f 6e76 6572 7465   = mhtmlconverte
 00000020: 720d 0a61 7574 686f 7220 3d20 4172 6e61  r..author = Arna
 00000030: 7564 2052 6576 656c 0d0a 6175 7468 6f72  ud Revel..author
 00000040: 5f65 6d61 696c 203d 2072 6576 656c 2e61  _email = revel.a
 00000050: 726e 6175 6440 676d 6169 6c2e 636f 6d0d  rnaud@gmail.com.
-00000060: 0a76 6572 7369 6f6e 203d 2030 2e32 0d0a  .version = 0.2..
+00000060: 0a76 6572 7369 6f6e 203d 2030 2e33 0d0a  .version = 0.3..
 00000070: 6c69 6365 6e73 655f 6669 6c65 7320 3d20  license_files = 
 00000080: 4c49 4345 4e43 450d 0a75 726c 203d 2068  LICENCE..url = h
 00000090: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 000000a0: 6d2f 6172 6e61 7564 7265 7665 6c2f 4d48  m/arnaudrevel/MH
 000000b0: 544d 4c63 6f6e 7665 7274 6572 0d0a 6465  TMLconverter..de
 000000c0: 7363 7269 7074 696f 6e20 3d20 546f 6f6c  scription = Tool
 000000d0: 7320 746f 2063 6f6e 7665 7274 206d 6172  s to convert mar
```

