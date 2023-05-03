# Comparing `tmp/dumb_pypi-1.8.0.tar.gz` & `tmp/dumb_pypi-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumb_pypi-1.8.0.tar", last modified: Fri Dec  3 06:13:09 2021, max compression
+gzip compressed data, was "dist/dumb_pypi-1.9.0.tar", last modified: Wed Mar 16 22:19:43 2022, max compression
```

## Comparing `dumb_pypi-1.8.0.tar` & `dumb_pypi-1.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2021-12-03 06:13:09.274098 dumb_pypi-1.8.0/
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      557 2021-12-03 06:07:36.000000 dumb_pypi-1.8.0/LICENSE
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     7841 2021-12-03 06:13:09.274098 dumb_pypi-1.8.0/PKG-INFO
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     7169 2021-12-03 06:12:36.000000 dumb_pypi-1.8.0/README.md
-drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2021-12-03 06:13:09.274098 dumb_pypi-1.8.0/dumb_pypi/
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)        0 2021-12-03 06:07:36.000000 dumb_pypi-1.8.0/dumb_pypi/__init__.py
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)    15369 2021-12-03 06:12:36.000000 dumb_pypi-1.8.0/dumb_pypi/main.py
-drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2021-12-03 06:13:09.274098 dumb_pypi-1.8.0/dumb_pypi/templates/
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     4190 2021-12-03 06:07:36.000000 dumb_pypi-1.8.0/dumb_pypi/templates/_base.html
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     2117 2021-12-03 06:07:36.000000 dumb_pypi-1.8.0/dumb_pypi/templates/changelog.html
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     2897 2021-12-03 06:07:36.000000 dumb_pypi-1.8.0/dumb_pypi/templates/index.html
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     1172 2021-12-03 06:07:36.000000 dumb_pypi-1.8.0/dumb_pypi/templates/package.html
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      435 2021-12-03 06:07:36.000000 dumb_pypi-1.8.0/dumb_pypi/templates/simple.html
-drwxr-xr-x   0 ckuehl    (1000) ckuehl    (1000)        0 2021-12-03 06:13:09.274098 dumb_pypi-1.8.0/dumb_pypi.egg-info/
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     7841 2021-12-03 06:13:09.000000 dumb_pypi-1.8.0/dumb_pypi.egg-info/PKG-INFO
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)      438 2021-12-03 06:13:09.000000 dumb_pypi-1.8.0/dumb_pypi.egg-info/SOURCES.txt
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)        1 2021-12-03 06:13:09.000000 dumb_pypi-1.8.0/dumb_pypi.egg-info/dependency_links.txt
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       51 2021-12-03 06:13:09.000000 dumb_pypi-1.8.0/dumb_pypi.egg-info/entry_points.txt
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       25 2021-12-03 06:13:09.000000 dumb_pypi-1.8.0/dumb_pypi.egg-info/requires.txt
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       10 2021-12-03 06:13:09.000000 dumb_pypi-1.8.0/dumb_pypi.egg-info/top_level.txt
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)     1158 2021-12-03 06:13:09.274098 dumb_pypi-1.8.0/setup.cfg
--rw-r--r--   0 ckuehl    (1000) ckuehl    (1000)       37 2021-12-03 06:07:36.000000 dumb_pypi-1.8.0/setup.py
+drwxr-xr-x   0 ckuehl    (3557) users      (100)        0 2022-03-16 22:19:43.739321 dumb_pypi-1.9.0/
+-rw-r--r--   0 ckuehl    (3557) users      (100)      557 2017-04-22 23:40:51.000000 dumb_pypi-1.9.0/LICENSE
+-rw-r--r--   0 ckuehl    (3557) users      (100)    10606 2022-03-16 22:19:43.739321 dumb_pypi-1.9.0/PKG-INFO
+-rw-r--r--   0 ckuehl    (3557) users      (100)     8215 2022-03-16 22:12:34.000000 dumb_pypi-1.9.0/README.md
+drwxr-xr-x   0 ckuehl    (3557) users      (100)        0 2022-03-16 22:19:43.739321 dumb_pypi-1.9.0/dumb_pypi/
+-rw-r--r--   0 ckuehl    (3557) users      (100)        0 2017-04-22 23:40:51.000000 dumb_pypi-1.9.0/dumb_pypi/__init__.py
+-rw-r--r--   0 ckuehl    (3557) users      (100)    17617 2022-03-16 22:12:34.000000 dumb_pypi-1.9.0/dumb_pypi/main.py
+drwxr-xr-x   0 ckuehl    (3557) users      (100)        0 2022-03-16 22:19:43.739321 dumb_pypi-1.9.0/dumb_pypi/templates/
+-rw-r--r--   0 ckuehl    (3557) users      (100)     4190 2021-07-06 20:41:41.000000 dumb_pypi-1.9.0/dumb_pypi/templates/_base.html
+-rw-r--r--   0 ckuehl    (3557) users      (100)     2117 2021-07-06 20:41:41.000000 dumb_pypi-1.9.0/dumb_pypi/templates/changelog.html
+-rw-r--r--   0 ckuehl    (3557) users      (100)     2897 2021-10-26 19:33:38.000000 dumb_pypi-1.9.0/dumb_pypi/templates/index.html
+-rw-r--r--   0 ckuehl    (3557) users      (100)     1172 2021-12-02 21:13:22.000000 dumb_pypi-1.9.0/dumb_pypi/templates/package.html
+-rw-r--r--   0 ckuehl    (3557) users      (100)      435 2021-10-26 19:33:38.000000 dumb_pypi-1.9.0/dumb_pypi/templates/simple.html
+drwxr-xr-x   0 ckuehl    (3557) users      (100)        0 2022-03-16 22:19:43.739321 dumb_pypi-1.9.0/dumb_pypi.egg-info/
+-rw-r--r--   0 ckuehl    (3557) users      (100)    10606 2022-03-16 22:19:43.000000 dumb_pypi-1.9.0/dumb_pypi.egg-info/PKG-INFO
+-rw-r--r--   0 ckuehl    (3557) users      (100)      438 2022-03-16 22:19:43.000000 dumb_pypi-1.9.0/dumb_pypi.egg-info/SOURCES.txt
+-rw-r--r--   0 ckuehl    (3557) users      (100)        1 2022-03-16 22:19:43.000000 dumb_pypi-1.9.0/dumb_pypi.egg-info/dependency_links.txt
+-rw-r--r--   0 ckuehl    (3557) users      (100)       51 2022-03-16 22:19:43.000000 dumb_pypi-1.9.0/dumb_pypi.egg-info/entry_points.txt
+-rw-r--r--   0 ckuehl    (3557) users      (100)       25 2022-03-16 22:19:43.000000 dumb_pypi-1.9.0/dumb_pypi.egg-info/requires.txt
+-rw-r--r--   0 ckuehl    (3557) users      (100)       10 2022-03-16 22:19:43.000000 dumb_pypi-1.9.0/dumb_pypi.egg-info/top_level.txt
+-rw-r--r--   0 ckuehl    (3557) users      (100)     1239 2022-03-16 22:19:43.739321 dumb_pypi-1.9.0/setup.cfg
+-rw-r--r--   0 ckuehl    (3557) users      (100)       37 2019-12-02 18:28:57.000000 dumb_pypi-1.9.0/setup.py
```

### Comparing `dumb_pypi-1.8.0/LICENSE` & `dumb_pypi-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dumb_pypi-1.8.0/PKG-INFO` & `dumb_pypi-1.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: dumb_pypi
-Version: 1.8.0
-Summary: UNKNOWN
-Home-page: https://github.com/chriskuehl/dumb-pypi
-Author: Chris Kuehl
-Author-email: ckuehl@ckuehl.me
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 dumb-pypi
 ---------
 
 [![Build Status](https://travis-ci.org/chriskuehl/dumb-pypi.svg?branch=master)](https://travis-ci.org/chriskuehl/dumb-pypi)
 [![Coverage Status](https://coveralls.io/repos/github/chriskuehl/dumb-pypi/badge.svg?branch=master)](https://coveralls.io/github/chriskuehl/dumb-pypi?branch=master)
 [![PyPI version](https://badge.fury.io/py/dumb-pypi.svg)](https://pypi.python.org/pypi/dumb-pypi)
 
@@ -187,22 +167,41 @@
 
 ### Using your deployed index server with pip
 
 When running pip, pass `-i https://my-pypi-server/simple` or set the
 environment variable `PIP_INDEX_URL=https://my-pypi-server/simple`.
 
 
+### Known incompatibilities with public PyPI
+
+We try to maintain compatibility with the standard PyPI interface, but there
+are some incompatibilities currently which are hard to fix due to dumb-pypi's
+design:
+
+* While [both JSON API endpoints][json-api] are supported, many keys in the
+  JSON API are not present since they require inspecting packages which
+  dumb-pypi can't do. Some of these, like `requires_python` and
+  `requires_dist`, can be passed in as JSON.
+
+* The [per-version JSON API endpoint][per-version-api] only includes data about
+  the current requested version and not _all_ versions, unlike public PyPI. In
+  other words, if you access `/pypi/<package>/1.0.0/json`, you will only see
+  the `1.0.0` release under the `releases` key and not every release ever made.
+  The regular non-versioned API route (`/pypi/<package>/json`) will have all
+  releases.
+
+
 ## Contributing
 
 Thanks for contributing! To get started, run `make venv` and then `.
 venv/bin/activate` to source the virtualenv. You should now have a `dumb-pypi`
 command on your path using your checked-out version of the code.
 
 To run the tests, call `make test`. To run an individual test, you can do
 `py.test -k name_of_test tests` (with the virtualenv activated).
 
 
 [rationale]: https://github.com/chriskuehl/dumb-pypi/blob/master/RATIONALE.md
 [pep503]: https://www.python.org/dev/peps/pep-0503/#normalized-names
 [s3-metadata]: https://docs.aws.amazon.com/AmazonS3/latest/dev/UsingMetadata.html#UserMetadata
-
-
+[json-api]: https://warehouse.pypa.io/api-reference/json.html
+[per-version-api]: https://warehouse.pypa.io/api-reference/json.html#get--pypi--project_name---version--json
```

### Comparing `dumb_pypi-1.8.0/dumb_pypi/main.py` & `dumb_pypi-1.9.0/dumb_pypi/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
 class Package(NamedTuple):
     filename: str
     name: str
     version: Optional[str]
     parsed_version: packaging.version.Version
     hash: Optional[str]
+    requires_dist: Optional[Tuple[str, ...]]
     requires_python: Optional[str]
     upload_timestamp: Optional[int]
     uploaded_by: Optional[str]
 
     def __lt__(self, other: Tuple[Any, ...]) -> bool:
         assert isinstance(other, Package), type(other)
         return self.sort_key < other.sort_key
@@ -133,47 +134,59 @@
             info += f', {self.uploaded_by}'
         return info
 
     def url(self, base_url: str, *, include_hash: bool = True) -> str:
         hash_part = f'#{self.hash}' if self.hash and include_hash else ''
         return f'{base_url.rstrip("/")}/{self.filename}{hash_part}'
 
+    @property
+    def packagetype(self) -> str:
+        if self.filename.endswith('.whl'):
+            return 'bdist_wheel'
+        elif self.filename.endswith('.egg'):
+            return 'bdist_egg'
+        else:
+            return 'sdist'
+
     def json_info(self, base_url: str) -> Dict[str, Any]:
         ret: Dict[str, Any] = {
             'filename': self.filename,
             'url': self.url(base_url, include_hash=False),
             'requires_python': self.requires_python,
+            'packagetype': self.packagetype,
         }
         if self.upload_timestamp is not None:
             ret['upload_time'] = self.formatted_upload_time
         if self.hash is not None:
             algo, h = self.hash.split('=')
             ret['digests'] = {algo: h}
         return ret
 
     @classmethod
     def create(
             cls,
             *,
             filename: str,
             hash: Optional[str] = None,
+            requires_dist: Optional[Sequence[str]] = None,
             requires_python: Optional[str] = None,
             upload_timestamp: Optional[int] = None,
             uploaded_by: Optional[str] = None,
     ) -> 'Package':
         if not re.match(r'[a-zA-Z0-9_\-\.\+]+$', filename) or '..' in filename:
             raise ValueError(f'Unsafe package name: {filename}')
 
         name, version = guess_name_version_from_filename(filename)
         return cls(
             filename=filename,
             name=packaging.utils.canonicalize_name(name),
             version=version,
             parsed_version=packaging.version.parse(version or '0'),
             hash=hash,
+            requires_dist=tuple(requires_dist) if requires_dist is not None else None,
             requires_python=requires_python,
             upload_timestamp=upload_timestamp,
             uploaded_by=uploaded_by,
         )
 
 
 @contextlib.contextmanager
@@ -192,26 +205,58 @@
         os.replace(tmp, path)
 
 
 def _format_datetime(dt: datetime) -> str:
     return dt.strftime('%Y-%m-%d %H:%M:%S')
 
 
-def _package_json(files: List[Package], base_url: str) -> Dict[str, Any]:
+IMPORTANT_METADATA_FOR_INFO = frozenset((
+    'name',
+    'version',
+    'requires_dist',
+    'requires_python',
+))
+
+
+def _package_json(sorted_files: List[Package], base_url: str) -> Dict[str, Any]:
     # https://warehouse.pypa.io/api-reference/json.html
     # note: the full api contains much more, we only output the info we have
-    by_version: Dict[str, List[Dict[str, Any]]] = collections.defaultdict(list)
-    for file in files:
+    by_version: Dict[str, List[Package]] = collections.defaultdict(list)
+    for file in sorted_files:
         if file.version is not None:
-            by_version[file.version].append(file.json_info(base_url))
+            by_version[file.version].append(file)
+
+    # Find a file from the latest release to use for "info". We don't want to
+    # mix-and-match the metadata across releases since tools like Poetry rely
+    # on this, but we do want to pick the file in the release with the most
+    # populated metadata.
+    latest_file = sorted_files[-1]
+    if sorted_files[-1].version is not None:
+        latest_file = max(
+            by_version[sorted_files[-1].version],
+            key=lambda f: sum(bool(getattr(f, v)) for v in IMPORTANT_METADATA_FOR_INFO),
+        )
 
     return {
-        'info': {'name': files[0].name, 'version': files[0].version},
-        'releases': by_version,
-        'urls': by_version[files[0].version] if files[0].version else [],
+        'info': {
+            'name': latest_file.name,
+            'version': latest_file.version,
+            'requires_dist': latest_file.requires_dist,
+            'requires_python': latest_file.requires_python,
+            'platform': "UNKNOWN",
+            'summary': None,
+        },
+        'releases': {
+            version: [file_.json_info(base_url) for file_ in files]
+            for version, files in by_version.items()
+        },
+        'urls': [
+            file_.json_info(base_url)
+            for file_ in by_version[latest_file.version]
+        ] if latest_file and latest_file.version is not None else [],
     }
 
 
 class Settings(NamedTuple):
     output_dir: str
     packages_url: str
     title: str
@@ -277,14 +322,27 @@
 
             # /pypi/{package}/json
             pypi_package_dir = os.path.join(pypi, package_name)
             os.makedirs(pypi_package_dir, exist_ok=True)
             with atomic_write(os.path.join(pypi_package_dir, 'json')) as f:
                 json.dump(_package_json(sorted_files, settings.packages_url), f)
 
+            # /pypi/{package}/{version}/json
+            # TODO: Consider making this only generate JSON for the changed versions.
+            version_to_files = collections.defaultdict(list)
+            for file_ in sorted_files:
+                version_to_files[file_.version].append(file_)
+            for version, files in version_to_files.items():
+                if version is None:
+                    continue
+                version_dir = os.path.join(pypi_package_dir, version)
+                os.makedirs(version_dir, exist_ok=True)
+                with atomic_write(os.path.join(version_dir, 'json')) as f:
+                    json.dump(_package_json(files, settings.packages_url), f)
+
     # /changelog
     # Always rebuild (we would have short circuited already if nothing changed).
     changelog = os.path.join(settings.output_dir, 'changelog')
     os.makedirs(changelog, exist_ok=True)
     files_newest_first = sorted(
         itertools.chain.from_iterable(packages.values()),
         key=lambda package: (package.upload_timestamp or 0, package.filename),
```

### Comparing `dumb_pypi-1.8.0/dumb_pypi/templates/_base.html` & `dumb_pypi-1.9.0/dumb_pypi/templates/_base.html`

 * *Files identical despite different names*

### Comparing `dumb_pypi-1.8.0/dumb_pypi/templates/changelog.html` & `dumb_pypi-1.9.0/dumb_pypi/templates/changelog.html`

 * *Files identical despite different names*

### Comparing `dumb_pypi-1.8.0/dumb_pypi/templates/index.html` & `dumb_pypi-1.9.0/dumb_pypi/templates/index.html`

 * *Files identical despite different names*

### Comparing `dumb_pypi-1.8.0/dumb_pypi/templates/package.html` & `dumb_pypi-1.9.0/dumb_pypi/templates/package.html`

 * *Files identical despite different names*

### Comparing `dumb_pypi-1.8.0/setup.cfg` & `dumb_pypi-1.9.0/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [metadata]
 name = dumb_pypi
-version = 1.8.0
+version = 1.9.0
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/chriskuehl/dumb-pypi
 author = Chris Kuehl
 author_email = ckuehl@ckuehl.me
+license = Apache License 2.0
 license_file = LICENSE
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
+	License :: OSI Approved :: Apache Software License
 
 [options]
 packages = dumb_pypi
 install_requires = 
 	distlib
 	jinja2
 	packaging
```

