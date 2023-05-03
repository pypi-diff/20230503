# Comparing `tmp/file-io-cli-tddschn-0.1.1.tar.gz` & `tmp/file_io_cli_tddschn-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-io-cli-tddschn-0.1.1.tar", max compression
+gzip compressed data, was "file_io_cli_tddschn-1.0.5.tar", max compression
```

## Comparing `file-io-cli-tddschn-0.1.1.tar` & `file_io_cli_tddschn-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1084 2022-05-04 13:33:08.470330 file-io-cli-tddschn-0.1.1/LICENSE.txt
--rw-r--r--   0        0        0     1857 2022-05-04 13:33:08.470997 file-io-cli-tddschn-0.1.1/README.md
--rw-r--r--   0        0        0       94 2022-05-06 05:37:25.160714 file-io-cli-tddschn-0.1.1/file_io_cli_tddschn/__init__.py
--rw-r--r--   0        0        0     9956 2022-05-06 05:33:41.387013 file-io-cli-tddschn-0.1.1/file_io_cli_tddschn/file_io_cli.py
--rw-r--r--   0        0        0      920 2022-05-06 05:37:25.160285 file-io-cli-tddschn-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2822 2022-05-06 05:37:40.570284 file-io-cli-tddschn-0.1.1/setup.py
--rw-r--r--   0        0        0     2656 2022-05-06 05:37:40.570668 file-io-cli-tddschn-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1084 2023-05-03 13:52:47.818681 file_io_cli_tddschn-1.0.5/LICENSE.txt
+-rw-r--r--   0        0        0     1857 2023-05-03 13:52:47.819053 file_io_cli_tddschn-1.0.5/README.md
+-rw-r--r--   0        0        0    10270 2023-05-03 14:27:00.514038 file_io_cli_tddschn-1.0.5/file_io_cli.py
+-rw-r--r--   0        0        0      932 2023-05-03 14:27:00.512913 file_io_cli_tddschn-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     2663 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.0.5/PKG-INFO
```

### Comparing `file-io-cli-tddschn-0.1.1/LICENSE.txt` & `file_io_cli_tddschn-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file-io-cli-tddschn-0.1.1/README.md` & `file_io_cli_tddschn-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `file-io-cli-tddschn-0.1.1/file_io_cli_tddschn/file_io_cli.py` & `file_io_cli_tddschn-1.0.5/file_io_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) 2018 Niklas Rosenstein
-# Copyright (c) 2022 Xinyuan Chen
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to
 # deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -16,28 +15,30 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
 # FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS
 # IN THE SOFTWARE.
 
 from __future__ import division, print_function
-from . import __author__, __version__
 
 import argparse
-import clipboard
+from typing import Literal
+import json
 import os
 import subprocess
 import sys
 import threading
 import time
 import uuid
 
+__author__ = 'Niklas Rosenstein <rosensteinniklas@gmail.com> Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>'
+__version__ = '1.0.5'
 
-class MultipartFileEncoder(object):
 
+class MultipartFileEncoder(object):
     def __init__(self, field, fp, filename=None, boundary=None, headers=None):
         self.field = field
         self.fp = fp
         self.filename = filename
         self.boundary = (boundary or uuid.uuid4().hex).encode('ascii')
         self.content_type = b'multipart/form-data; boundary=' + self.boundary
 
@@ -48,16 +49,17 @@
             if self.filename:
                 disposition += '; filename="{}"'.format(self.filename)
             headers['Content-Disposition'] = disposition
 
         if 'Content-Type' not in headers:
             headers['Content-Type'] = 'application/octet-stream'
 
-        self.headers = b'\r\n'.join('{}: {}'.format(k, v).encode('ascii')
-                                    for k, v in headers.items())
+        self.headers = b'\r\n'.join(
+            '{}: {}'.format(k, v).encode('ascii') for k, v in headers.items()
+        )
 
     def compute_size(self, include_final_boundary=True):
         pos = self.fp.tell()
         self.fp.seek(0, os.SEEK_END)
         size = self.fp.tell()
         self.fp.seek(pos)
         size += len(self.boundary) + 4 + 4 + len(self.headers) + 2
@@ -73,27 +75,27 @@
         yield self.headers
         yield b'\r\n'
         yield b'\r\n'
 
         # TODO: Check if boundary value occurs in data body.
         while True:
             data = self.fp.read(chunksize)
-            if not data: break
+            if not data:
+                break
             yield data
 
         yield b'\r\n'
 
         if include_final_boundary:
             yield b'--'
             yield self.boundary
             yield b'--\r\n'
 
 
 class GeneratorFileReader(object):
-
     def __init__(self, gen):
         self.gen = gen
         self.buffer = b''
 
     def readable(self):
         return True
 
@@ -119,15 +121,14 @@
                         break
                 else:
                     break
             return res
 
 
 class FileMonitor(object):
-
     def __init__(self, fp, callback=None):
         self.fp = fp
         self.bytes_read = 0
         self.callback = callback
 
     def __getattr__(self, key):
         return getattr(self.fp, key)
@@ -137,134 +138,152 @@
         self.bytes_read += len(res)
         if self.callback:
             self.callback(self)
         return res
 
 
 class ProgressDisplay(object):
-
     SPINCHARS = '\\|/-'
 
     def __init__(self, n_max=None):
         self.n_max = n_max
         self.alteration = 0
         self.last_print = None
 
     def update(self, n_read, force=False):
-        if not force and self.last_print is not None and time.perf_counter(
-        ) - self.last_print < 0.25:
+        if (
+            not force
+            and self.last_print is not None
+            and time.perf_counter() - self.last_print < 0.25
+        ):
             return
         self.last_print = time.perf_counter()
         self.__clear_line(file=sys.stderr)
         if self.n_max is None:
             c = self.SPINCHARS[self.alteration % len(self.SPINCHARS)]
-            print('\r{} ({})'.format(c, self.human_size(n_read)),
-                  end='',
-                  file=sys.stderr)
+            print(
+                '\r{} ({})'.format(c, self.human_size(n_read)), end='', file=sys.stderr
+            )
         else:
             w = 60
             p = n_read / self.n_max
             l = int(w * p)
 
             bar = '[' + '=' * l + ' ' * (w - l) + ']'
-            print('\r{} {}% ({} / {})'.format(bar, int(p * 100),
-                                              self.human_size(n_read),
-                                              self.human_size(self.n_max)),
-                  end='',
-                  file=sys.stderr)
+            print(
+                '\r{} {}% ({} / {})'.format(
+                    bar,
+                    int(p * 100),
+                    self.human_size(n_read),
+                    self.human_size(self.n_max),
+                ),
+                end='',
+                file=sys.stderr,
+            )
         sys.stderr.flush()
         self.alteration += 1
 
     def finish(self):
         print(file=sys.stderr)
 
     @staticmethod
     def __clear_line(file=None):
         print('\r\33[K', end='', file=file)
 
     @staticmethod
-    def human_size(n_bytes,
-                   units=[' bytes', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB']):
+    def human_size(n_bytes, units=[' bytes', 'KB', 'MB', 'GB', 'TB', 'PB', 'EB']):
         # https://stackoverflow.com/a/43750422/791713
-        return str(n_bytes) + units[
-            0] if n_bytes < 1024 else ProgressDisplay.human_size(
-                n_bytes >> 10, units[1:])
+        return (
+            str(n_bytes) + units[0]
+            if n_bytes < 1024
+            else ProgressDisplay.human_size(n_bytes >> 10, units[1:])
+        )
 
 
 def stream_file(fp, chunksize=8192):
     while True:
         data = fp.read(chunksize)
-        if data: yield data
-        else: break
+        if data:
+            yield data
+        else:
+            break
 
 
 def spawn_process(*args, **kwargs):
     on_exit = kwargs.pop('on_exit', None)
 
     def worker():
         subprocess.call(*args, **kwargs)
         if on_exit is not None:
             on_exit()
 
     threading.Thread(target=worker).start()
 
 
-def main(prog=None, argv=None):
+def get_args(prog=None) -> argparse.Namespace | Literal[0]:
     parser = argparse.ArgumentParser(
         prog=prog,
-        description=
-        'Upload a file to file.io and print the download link. Supports stdin.'
+        description='Upload a file to file.io and print the download link. Supports stdin.',
     )
     parser.add_argument('--version', action='version', version=__version__)
-    parser.add_argument('-e',
-                        '--expires',
-                        metavar='E',
-                        help='set the expiration time for the uploaded file')
-    parser.add_argument('-n',
-                        '--name',
-                        help='specify or override the filename')
-    parser.add_argument('-q',
-                        '--quiet',
-                        action='store_true',
-                        help='hide the progress bar')
-    parser.add_argument('-c',
-                        '--clip',
-                        action='store_true',
-                        help='copy the URL to your clipboard')
+    parser.add_argument(
+        '-e',
+        '--expires',
+        metavar='E',
+        help='set the expiration time for the uploaded file',
+    )
+    parser.add_argument('-n', '--name', help='specify or override the filename')
+    parser.add_argument(
+        '-q', '--quiet', action='store_true', help='hide the progress bar'
+    )
+    parser.add_argument(
+        '-c', '--clip', action='store_true', help='copy the URL to your clipboard'
+    )
     parser.add_argument(
         '-t',
         '--tar',
         metavar='PATH',
-        help='create a TAR archive from the specified file or directory')
+        help='create a TAR archive from the specified file or directory',
+    )
     parser.add_argument(
         '-z',
         '--gzip',
         action='store_true',
-        help='filter the TAR archive through gzip (only with -t, --tar)')
+        help='filter the TAR archive through gzip (only with -t, --tar)',
+    )
+    parser.add_argument(
+        '-v', '--verbose', action='store_true', help='print the server response'
+    )
     parser.add_argument('file', nargs='?', help='the file to upload')
     args = parser.parse_args()
 
     if not args.file and not args.tar and sys.stdin.isatty():
         parser.print_usage()
         return 0
     if args.file and args.tar:
         parser.error('conflicting options: file and -t, --tar')
+    return args
+
 
+def main(prog=None, argv=None):
+    args = get_args(prog=prog)
+    import clipboard
+    import requests
+
+    if args == 0:
+        return
     if not args.name and args.file:
         args.name = os.path.basename(args.file)
     elif not args.name and args.tar:
-        args.name = os.path.basename(
-            args.tar) + ('.tgz' if args.gzip else '.tar')
+        args.name = os.path.basename(args.tar) + ('.tgz' if args.gzip else '.tar')
 
     if args.tar:
         r, w = os.pipe()
         flags = '-czf-' if args.gzip else '-cf-'
-        spawn_process(['tar', flags, args.tar],
-                      stdout=w,
-                      on_exit=lambda: os.close(w))
+        spawn_process(['tar', flags, args.tar], stdout=w, on_exit=lambda: os.close(w))
         file_size = None
         fp = os.fdopen(r, 'rb')
     elif args.file:
         file_size = os.stat(args.file).st_size
         fp = open(args.file, 'rb')
     else:
         file_size = None
@@ -280,36 +299,38 @@
     headers = {'Content-Type': encoder.content_type}
     params = {}
     if args.expires:
         params['expires'] = args.expiry
 
     url = 'http://file.io'
     if params:
+        from urllib.parse import urlencode
+
         url += '?' + urlencode(params)
 
     try:
-        import requests
-        response = requests.post(url,
-                                 params=params,
-                                 data=stream_file(stream),
-                                 headers=headers)
+        response = requests.post(
+            url, params=params, data=stream_file(stream), headers=headers
+        )
         response.raise_for_status()
     except BaseException as exc:
         if not args.quiet:
-            progress.finish()
+            progress.finish()  # type: ignore
         if isinstance(exc, KeyboardInterrupt):
             print('aborted.', file=sys.stderr)
             return 1
         raise
     else:
         if not args.quiet:
-            progress.update(fp.bytes_read, force=True)
-            progress.finish()
+            progress.update(fp.bytes_read, force=True)  # type: ignore
+            progress.finish()  # type: ignore
 
-    link = response.json()['link']
+    link = (res_d := response.json())['link']
+    if args.verbose:
+        print(json.dumps(res_d, indent=2), file=sys.stderr)
 
     if args.clip:
         print(link, '(copied to clipboard)')
         clipboard.copy(link)
     else:
         print(link)
```

### Comparing `file-io-cli-tddschn-0.1.1/PKG-INFO` & `file_io_cli_tddschn-1.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: file-io-cli-tddschn
-Version: 0.1.1
+Version: 1.0.5
 Summary: Command-line tool to upload files to https://file.io
 Home-page: https://github.com/tddschn/file.io-cli-tddschn
 License: MIT
-Keywords: file.io,cli,upload,download
-Author: Xinyuan Chen
+Keywords: file.io,utility,uploader,CLI
+Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Dist: clipboard (>=0.0.4,<0.0.5)
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: clipboard (>=0.0.4,<1.0.0)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/tddschn/file.io-cli-tddschn/issues
 Project-URL: Repository, https://github.com/tddschn/file.io-cli-tddschn
 Description-Content-Type: text/markdown
 
 # file.io-cli
 
     $ pip install file.io-cli
```

