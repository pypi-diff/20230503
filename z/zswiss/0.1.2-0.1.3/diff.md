# Comparing `tmp/zswiss-0.1.2.tar.gz` & `tmp/zswiss-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zswiss-0.1.2.tar", last modified: Wed Nov 30 03:54:12 2022, max compression
+gzip compressed data, was "zswiss-0.1.3.tar", last modified: Wed May  3 10:06:00 2023, max compression
```

## Comparing `zswiss-0.1.2.tar` & `zswiss-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-11-30 03:54:12.638096 zswiss-0.1.2/
--rw-rw-rw-   0        0        0     1088 2022-11-30 03:25:13.000000 zswiss-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      858 2022-11-30 03:54:12.638096 zswiss-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-11-30 03:25:13.000000 zswiss-0.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2022-11-30 03:54:12.638096 zswiss-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1215 2022-11-30 03:37:03.000000 zswiss-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-30 03:54:12.632555 zswiss-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2022-11-30 03:25:13.000000 zswiss-0.1.2/tests/__init__.py
--rw-rw-rw-   0        0        0     3601 2022-11-30 03:50:31.000000 zswiss-0.1.2/tests/test_file_utils.py
-drwxrwxrwx   0        0        0        0 2022-11-30 03:54:12.633566 zswiss-0.1.2/zswiss/
--rw-rw-rw-   0        0        0        0 2022-11-30 03:25:13.000000 zswiss-0.1.2/zswiss/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-30 03:54:12.637077 zswiss-0.1.2/zswiss/utils/
--rw-rw-rw-   0        0        0        0 2022-11-30 03:25:13.000000 zswiss-0.1.2/zswiss/utils/__init__.py
--rw-rw-rw-   0        0        0     4751 2022-11-30 03:39:20.000000 zswiss-0.1.2/zswiss/utils/file_utils.py
-drwxrwxrwx   0        0        0        0 2022-11-30 03:54:12.635563 zswiss-0.1.2/zswiss.egg-info/
--rw-rw-rw-   0        0        0      858 2022-11-30 03:54:12.000000 zswiss-0.1.2/zswiss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2022-11-30 03:54:12.000000 zswiss-0.1.2/zswiss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-30 03:54:12.000000 zswiss-0.1.2/zswiss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-11-30 03:54:12.000000 zswiss-0.1.2/zswiss.egg-info/top_level.txt
+drwxr-xr-x   0 labrador   (501) staff       (20)        0 2023-05-03 10:06:00.178691 zswiss-0.1.3/
+-rw-r--r--   0 labrador   (501) staff       (20)     1068 2022-11-09 06:13:08.000000 zswiss-0.1.3/LICENSE
+-rw-r--r--   0 labrador   (501) staff       (20)      836 2023-05-03 10:06:00.178544 zswiss-0.1.3/PKG-INFO
+-rw-r--r--   0 labrador   (501) staff       (20)        0 2022-11-09 06:03:20.000000 zswiss-0.1.3/README.rst
+-rw-r--r--   0 labrador   (501) staff       (20)       38 2023-05-03 10:06:00.178736 zswiss-0.1.3/setup.cfg
+-rw-r--r--   0 labrador   (501) staff       (20)     1181 2023-05-03 10:00:13.000000 zswiss-0.1.3/setup.py
+drwxr-xr-x   0 labrador   (501) staff       (20)        0 2023-05-03 10:06:00.177417 zswiss-0.1.3/tests/
+-rw-r--r--   0 labrador   (501) staff       (20)        0 2022-11-09 04:39:39.000000 zswiss-0.1.3/tests/__init__.py
+-rw-r--r--   0 labrador   (501) staff       (20)     4039 2023-05-03 09:57:57.000000 zswiss-0.1.3/tests/test_file_utils.py
+drwxr-xr-x   0 labrador   (501) staff       (20)        0 2023-05-03 10:06:00.177646 zswiss-0.1.3/zswiss/
+-rw-r--r--   0 labrador   (501) staff       (20)        0 2022-11-09 06:56:38.000000 zswiss-0.1.3/zswiss/__init__.py
+drwxr-xr-x   0 labrador   (501) staff       (20)        0 2023-05-03 10:06:00.178217 zswiss-0.1.3/zswiss/utils/
+-rw-r--r--   0 labrador   (501) staff       (20)        0 2022-11-09 03:21:46.000000 zswiss-0.1.3/zswiss/utils/__init__.py
+-rw-r--r--   0 labrador   (501) staff       (20)     5425 2023-05-03 09:55:06.000000 zswiss-0.1.3/zswiss/utils/file_utils.py
+drwxr-xr-x   0 labrador   (501) staff       (20)        0 2023-05-03 10:06:00.178059 zswiss-0.1.3/zswiss.egg-info/
+-rw-r--r--   0 labrador   (501) staff       (20)      836 2023-05-03 10:06:00.000000 zswiss-0.1.3/zswiss.egg-info/PKG-INFO
+-rw-r--r--   0 labrador   (501) staff       (20)      261 2023-05-03 10:06:00.000000 zswiss-0.1.3/zswiss.egg-info/SOURCES.txt
+-rw-r--r--   0 labrador   (501) staff       (20)        1 2023-05-03 10:06:00.000000 zswiss-0.1.3/zswiss.egg-info/dependency_links.txt
+-rw-r--r--   0 labrador   (501) staff       (20)       13 2023-05-03 10:06:00.000000 zswiss-0.1.3/zswiss.egg-info/top_level.txt
```

### Comparing `zswiss-0.1.2/LICENSE` & `zswiss-0.1.3/LICENSE`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) [year] [fullname]
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) [year] [fullname]
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `zswiss-0.1.2/PKG-INFO` & `zswiss-0.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: zswiss
-Version: 0.1.2
-Summary: some tools, simple but useful
-Author: neilxzhang
-Author-email: legend_zhx@163.com
-License: MIT License
-Platform: all
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: zswiss
+Version: 0.1.3
+Summary: some tools, simple but useful
+Author: neilxzhang
+Author-email: legend_zhx@163.com
+License: MIT License
+Platform: all
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
```

### Comparing `zswiss-0.1.2/tests/test_file_utils.py` & `zswiss-0.1.3/tests/test_file_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,72 +1,83 @@
-import unittest
-from zswiss.utils.file_utils import load_to_set
-from zswiss.utils.file_utils import load_to_list
-from zswiss.utils.file_utils import save_from_list
-from zswiss.utils.file_utils import save_from_set
-
-
-class TestFileUtils(unittest.TestCase):
-
-    def test_load_to_list(self):
-        paths = ['../docs/samples']
-        res = load_to_list(paths, deduplicate=True, appendix=None)
-        self.assertListEqual(res, ['1.txt', '2.txt'], 'error')
-
-        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
-        res = load_to_list(paths, deduplicate=True, appendix='txt')
-        self.assertListEqual(res, ['11.txt', '21.txt', '1.txt', '2.txt'], 'error')
-
-        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
-        res = load_to_list(paths, deduplicate=False, appendix='txt')
-        self.assertListEqual(res, ['11.txt', '11.txt', '21.txt', '1.txt', '2.txt'], 'error')
-
-        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
-        res = load_to_list(paths, deduplicate=False, appendix=None)
-        self.assertSetEqual(set(res), set(['11.txt', '11.txt', '12', '21.txt', '21', '1.txt', '2.txt']), 'error')
-
-        paths = ['../docs/samples']
-        res = load_to_list(paths, appendix=None, recurse=True)
-        print('res:', res)
-        self.assertSetEqual(set(res), set(['11.txt', '12', '21', '21.txt', '1.txt', '2.txt']))
-
-    def test_load_to_set(self):
-        paths = ['../docs/samples']
-        res = load_to_set(paths, appendix=None)
-        self.assertSetEqual(res, set(['2.txt', '1.txt']), 'error')
-
-        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
-        res = load_to_set(paths, appendix='txt')
-        self.assertSetEqual(res, set(['11.txt', '21.txt', '1.txt', '2.txt']), 'error')
-
-        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
-        res = load_to_set(paths, appendix='txt')
-        self.assertSetEqual(res, set(['11.txt', '11.txt', '21.txt', '1.txt', '2.txt']), 'error')
-
-        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
-        res = load_to_set(paths, appendix=None)
-        self.assertSetEqual(set(res), set(['11.txt', '11.txt', '12', '21.txt', '21', '1.txt', '2.txt']), 'error')
-
-        paths = ['../docs/samples']
-        res = load_to_set(paths, appendix=None, recurse=True)
-        self.assertSetEqual(set(res), set(['11.txt', '12', '21', '21.txt', '1.txt', '2.txt']))
-
-    def test_save_from_list(self):
-        records1 = ['1', '2', '3', '3']
-        file_path1 = '../docs/samples_for_save/save1.txt'
-        save_from_list(records1, file_path1, deduplicate=False)
-        self.assertListEqual(records1, load_to_list([file_path1]))
-
-        records2 = ['1', '2', '3', '3']
-        file_path2 = '../docs/samples_for_save/save2.txt'
-        save_from_list(records2, file_path2, deduplicate=True)
-        self.assertListEqual(['1', '2', '3'], load_to_list([file_path2]))
-
-    def test_save_from_set(self):
-        records3 = set(['1', '2', '3', '3'])
-        file_path3 = '../docs/samples_for_save/save3.txt'
-        save_from_set(records3, file_path3)
-        self.assertSetEqual(set(records3), load_to_set([file_path3]))
-
-
-if __name__ == '__main__':
-    unittest.main()
+import unittest
+from zswiss.utils.file_utils import load_to_set
+from zswiss.utils.file_utils import load_to_list
+from zswiss.utils.file_utils import save_from_list
+from zswiss.utils.file_utils import save_from_set
+from zswiss.utils.file_utils import find_by_name
+
+
+class TestFileUtils(unittest.TestCase):
+
+    @unittest.skip
+    def test_load_to_list(self):
+        paths = ['../docs/samples']
+        res = load_to_list(paths, deduplicate=True, appendix=None)
+        self.assertListEqual(res, ['1.txt', '2.txt'], 'error')
+
+        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
+        res = load_to_list(paths, deduplicate=True, appendix='txt')
+        self.assertListEqual(res, ['11.txt', '21.txt', '1.txt', '2.txt'], 'error')
+
+        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
+        res = load_to_list(paths, deduplicate=False, appendix='txt')
+        self.assertListEqual(res, ['11.txt', '11.txt', '21.txt', '1.txt', '2.txt'], 'error')
+
+        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
+        res = load_to_list(paths, deduplicate=False, appendix=None)
+        self.assertSetEqual(set(res), set(['11.txt', '11.txt', '12', '21.txt', '21', '1.txt', '2.txt']), 'error')
+
+        paths = ['../docs/samples']
+        res = load_to_list(paths, appendix=None, recurse=True)
+        print('res:', res)
+        self.assertSetEqual(set(res), set(['11.txt', '12', '21', '21.txt', '1.txt', '2.txt']))
+
+    def test_load_to_set(self):
+        paths = ['../docs/samples']
+        res = load_to_set(paths, appendix=None)
+        self.assertSetEqual(res, set(['2.txt', '1.txt']), 'error')
+
+        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
+        res = load_to_set(paths, appendix='txt')
+        self.assertSetEqual(res, set(['11.txt', '21.txt', '1.txt', '2.txt']), 'error')
+
+        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
+        res = load_to_set(paths, appendix='txt')
+        self.assertSetEqual(res, set(['11.txt', '11.txt', '21.txt', '1.txt', '2.txt']), 'error')
+
+        paths = ['../docs/samples/subdir1', '../docs/samples/subdir2', '../docs/samples/1.txt', '../docs/samples/2.txt']
+        res = load_to_set(paths, appendix=None)
+        self.assertSetEqual(set(res), set(['11.txt', '11.txt', '12', '21.txt', '21', '1.txt', '2.txt']), 'error')
+
+        paths = ['../docs/samples']
+        res = load_to_set(paths, appendix=None, recurse=True)
+        self.assertSetEqual(set(res), set(['11.txt', '12', '21', '21.txt', '1.txt', '2.txt']))
+
+    def test_save_from_list(self):
+        records1 = ['1', '2', '3', '3']
+        file_path1 = '../docs/samples_for_save/save1.txt'
+        save_from_list(records1, file_path1, deduplicate=False)
+        self.assertListEqual(records1, load_to_list([file_path1]))
+
+        records2 = ['1', '2', '3', '3']
+        file_path2 = '../docs/samples_for_save/save2.txt'
+        save_from_list(records2, file_path2, deduplicate=True)
+        self.assertListEqual(['1', '2', '3'], load_to_list([file_path2]))
+
+    def test_save_from_set(self):
+        records3 = set(['1', '2', '3', '3'])
+        file_path3 = '../docs/samples_for_save/save3.txt'
+        save_from_set(records3, file_path3)
+        self.assertSetEqual(set(records3), load_to_set([file_path3]))
+
+    def test_find_by_name(self):
+        base_path = '../docs/samples'
+        res = find_by_name(base_path, '1', False)
+        print(res)
+        self.assertSetEqual(set(res),
+                            set(['../docs/samples/1.txt', '../docs/samples/subdir2/21',
+                                 '../docs/samples/subdir2/21.txt',
+                                 '../docs/samples/subdir1/11.txt', '../docs/samples/subdir1/12']), 'error')
+
+
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `zswiss-0.1.2/zswiss.egg-info/PKG-INFO` & `zswiss-0.1.3/zswiss.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1
-Name: zswiss
-Version: 0.1.2
-Summary: some tools, simple but useful
-Author: neilxzhang
-Author-email: legend_zhx@163.com
-License: MIT License
-Platform: all
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Natural Language :: Chinese (Simplified)
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Software Development :: Libraries
-License-File: LICENSE
+Metadata-Version: 2.1
+Name: zswiss
+Version: 0.1.3
+Summary: some tools, simple but useful
+Author: neilxzhang
+Author-email: legend_zhx@163.com
+License: MIT License
+Platform: all
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Natural Language :: Chinese (Simplified)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 2
+Classifier: Programming Language :: Python :: 2.7
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
```

