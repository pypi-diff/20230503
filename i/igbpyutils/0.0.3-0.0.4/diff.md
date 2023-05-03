# Comparing `tmp/igbpyutils-0.0.3.tar.gz` & `tmp/igbpyutils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igbpyutils-0.0.3.tar", last modified: Sun Apr 16 11:34:01 2023, max compression
+gzip compressed data, was "igbpyutils-0.0.4.tar", last modified: Wed May  3 16:59:53 2023, max compression
```

## Comparing `igbpyutils-0.0.3.tar` & `igbpyutils-0.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/
--rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.3/LICENSE.txt
--rw-------   0 haukex    (1000) haukex    (1000)     2374 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)     1496 2023-04-15 09:00:42.000000 igbpyutils-0.0.3/README.md
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-16 11:34:01.809254 igbpyutils-0.0.3/igbpyutils/
--rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.3/igbpyutils/__init__.py
--rw-------   0 haukex    (1000) haukex    (1000)     1528 2023-04-16 11:28:55.000000 igbpyutils-0.0.3/igbpyutils/dt.py
--rw-------   0 haukex    (1000) haukex    (1000)     5263 2023-04-15 08:15:49.000000 igbpyutils-0.0.3/igbpyutils/error.py
--rw-------   0 haukex    (1000) haukex    (1000)     9181 2023-04-15 10:48:14.000000 igbpyutils-0.0.3/igbpyutils/file.py
--rw-------   0 haukex    (1000) haukex    (1000)     5432 2023-04-15 10:48:14.000000 igbpyutils-0.0.3/igbpyutils/iter.py
--rw-------   0 haukex    (1000) haukex    (1000)     1429 2023-04-14 19:21:32.000000 igbpyutils-0.0.3/igbpyutils/test.py
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/igbpyutils.egg-info/
--rw-------   0 haukex    (1000) haukex    (1000)     2374 2023-04-16 11:34:01.000000 igbpyutils-0.0.3/igbpyutils.egg-info/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)      383 2023-04-16 11:34:01.000000 igbpyutils-0.0.3/igbpyutils.egg-info/SOURCES.txt
--rw-------   0 haukex    (1000) haukex    (1000)        1 2023-04-16 11:34:01.000000 igbpyutils-0.0.3/igbpyutils.egg-info/dependency_links.txt
--rw-------   0 haukex    (1000) haukex    (1000)       11 2023-04-16 11:34:01.000000 igbpyutils-0.0.3/igbpyutils.egg-info/top_level.txt
--rw-------   0 haukex    (1000) haukex    (1000)      904 2023-04-16 11:23:07.000000 igbpyutils-0.0.3/pyproject.toml
--rw-------   0 haukex    (1000) haukex    (1000)       38 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/setup.cfg
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-04-16 11:34:01.813254 igbpyutils-0.0.3/tests/
--rwxr-xr-x   0 haukex    (1000) haukex    (1000)     2023 2023-04-16 11:23:30.000000 igbpyutils-0.0.3/tests/test_dt.py
--rwx------   0 haukex    (1000) haukex    (1000)     6413 2023-04-15 08:58:04.000000 igbpyutils-0.0.3/tests/test_error.py
--rwx------   0 haukex    (1000) haukex    (1000)    11396 2023-04-15 10:48:14.000000 igbpyutils-0.0.3/tests/test_file.py
--rwx------   0 haukex    (1000) haukex    (1000)     9018 2023-04-16 11:21:31.000000 igbpyutils-0.0.3/tests/test_iter.py
--rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.3/tests/test_test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/
+-rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.4/LICENSE.txt
+-rw-------   0 haukex    (1000) haukex    (1000)     2427 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)     1549 2023-05-03 16:06:37.000000 igbpyutils-0.0.4/README.md
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/igbpyutils/
+-rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.4/igbpyutils/__init__.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1528 2023-04-16 11:28:55.000000 igbpyutils-0.0.4/igbpyutils/dt.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5730 2023-05-03 16:39:35.000000 igbpyutils-0.0.4/igbpyutils/error.py
+-rw-------   0 haukex    (1000) haukex    (1000)     9717 2023-05-03 16:48:00.000000 igbpyutils-0.0.4/igbpyutils/file.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5442 2023-05-03 16:48:35.000000 igbpyutils-0.0.4/igbpyutils/iter.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1429 2023-04-14 19:21:32.000000 igbpyutils-0.0.4/igbpyutils/test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/igbpyutils.egg-info/
+-rw-------   0 haukex    (1000) haukex    (1000)     2427 2023-05-03 16:59:53.000000 igbpyutils-0.0.4/igbpyutils.egg-info/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)      383 2023-05-03 16:59:53.000000 igbpyutils-0.0.4/igbpyutils.egg-info/SOURCES.txt
+-rw-------   0 haukex    (1000) haukex    (1000)        1 2023-05-03 16:59:53.000000 igbpyutils-0.0.4/igbpyutils.egg-info/dependency_links.txt
+-rw-------   0 haukex    (1000) haukex    (1000)       11 2023-05-03 16:59:53.000000 igbpyutils-0.0.4/igbpyutils.egg-info/top_level.txt
+-rw-------   0 haukex    (1000) haukex    (1000)      904 2023-05-03 16:51:32.000000 igbpyutils-0.0.4/pyproject.toml
+-rw-------   0 haukex    (1000) haukex    (1000)       38 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/setup.cfg
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/tests/
+-rwxr-xr-x   0 haukex    (1000) haukex    (1000)     2023 2023-04-16 11:23:30.000000 igbpyutils-0.0.4/tests/test_dt.py
+-rwx------   0 haukex    (1000) haukex    (1000)     6923 2023-05-03 16:39:39.000000 igbpyutils-0.0.4/tests/test_error.py
+-rwx------   0 haukex    (1000) haukex    (1000)    11434 2023-05-03 16:24:28.000000 igbpyutils-0.0.4/tests/test_file.py
+-rwx------   0 haukex    (1000) haukex    (1000)     9018 2023-04-16 11:21:31.000000 igbpyutils-0.0.4/tests/test_iter.py
+-rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.4/tests/test_test.py
```

### Comparing `igbpyutils-0.0.3/LICENSE.txt` & `igbpyutils-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.3/PKG-INFO` & `igbpyutils-0.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igbpyutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Various Python Utilities
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Homepage, https://github.com/haukex/igbpyutils
 Project-URL: Bug Tracker, https://github.com/haukex/igbpyutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,14 +23,15 @@
 ====================
 
 This is a collection of various Python tools, libraries, and utilities
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
 (IGB) in the Forschungsverbund Berlin e.V. (<https://www.igb-berlin.de/en>).
 
 Please see the individual files in this project for documentation.
+(TODO: Check and generate documentation with Sphinx)
 
 This is a companion library to the `igbdatatools` library
 (<https://github.com/haukex/igbdatatools>) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
 cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
```

### Comparing `igbpyutils-0.0.3/README.md` & `igbpyutils-0.0.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 ====================
 
 This is a collection of various Python tools, libraries, and utilities
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
 (IGB) in the Forschungsverbund Berlin e.V. (<https://www.igb-berlin.de/en>).
 
 Please see the individual files in this project for documentation.
+(TODO: Check and generate documentation with Sphinx)
 
 This is a companion library to the `igbdatatools` library
 (<https://github.com/haukex/igbdatatools>) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
 cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
```

### Comparing `igbpyutils-0.0.3/igbpyutils/dt.py` & `igbpyutils-0.0.4/igbpyutils/dt.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.3/igbpyutils/error.py` & `igbpyutils-0.0.4/igbpyutils/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,33 +38,35 @@
         Path(stack_frame.frame.f_code.co_filename).parts[-2:] == ('unittest','main.py')
         for stack_frame in inspect.stack() )
 
 _basepath = Path(__main__.__file__).parent.resolve(strict=True) \
     if hasattr(__main__, '__file__') and not running_in_unittest() \
     else Path().resolve(strict=True)  # just the CWD
 
-def _extype_fullname(ex: type) -> str:
+def extype_fullname(ex: type) -> str:
+    """Return the name of an exception together with its module name, if any."""
     if ex.__module__ in ('builtins','__main__'): return ex.__name__
     else: return ex.__module__ + "." + ex.__name__
 
-def _ex_repr(ex: BaseException) -> str:
-    return _extype_fullname(type(ex)) + '(' + ', '.join(map(repr, ex.args)) + ')'
+def ex_repr(ex: BaseException) -> str:
+    """Return a representation of the exception including its full name and ``.args``."""
+    return extype_fullname(type(ex)) + '(' + ', '.join(map(repr, ex.args)) + ')'
 
 # Equivalent to Lib/warnings.py, but customize UserWarning messages to be shorter.
 def _showwarning(message, category, filename, lineno, file=None, line=None):
     if file is None:  # pragma: no cover
         file = sys.stderr
         if file is None: return
     if issubclass(category, UserWarning):
         try:
             fn = Path(filename).resolve(strict=True)
         except OSError:  # pragma: no cover
             fn = Path(filename)
         if fn.is_relative_to(_basepath): fn = fn.relative_to(_basepath)
-        text = f"{_extype_fullname(category)}: {message} at {fn}:{lineno}\n"
+        text = f"{extype_fullname(category)}: {message} at {fn}:{lineno}\n"
     else:
         text = warnings.formatwarning(message, category, filename, lineno, line)
     try: file.write(text)
     except OSError: pass  # pragma: no cover
 
 def _excepthook(_type, value, _traceback):  # pragma: no cover
     for s in javaishstacktrace(value): print(s)
@@ -103,18 +105,23 @@
     """
     causes = [ex]
     while ex.__cause__:
         ex = ex.__cause__
         causes.append(ex)
     first = True
     for e in reversed(causes):
-        r = _ex_repr(e)
+        r = ex_repr(e)
         if isinstance(e, AssertionError):  # for "assert"s we'd like to see the source that caused it
-            lines = inspect.getinnerframes(e.__traceback__)[-1].code_context
-            r += f" [{ lines[0].strip() if len(lines)==1 else ''.join(lines) !r}]"
+            assert e.__traceback__  # for some reason, the coverage tool is reporting the following `if` is false on 3.9?
+            if e.__traceback__:  # cover-not-le3.9
+                lines = inspect.getinnerframes(e.__traceback__)[-1].code_context
+                if lines:
+                    r += f" [{ lines[0].strip() if len(lines)==1 else ''.join(lines) !r}]"
+                else: pass  # pragma: no cover
+            else: pass  # cover-not-ge3.10
         yield r if first else "which caused: " + r
         for item in reversed( extract_tb(e.__traceback__) ):
             try:
                 fn = Path(item.filename).resolve(strict=True)
             except OSError:  # pragma: no cover
                 fn = Path(item.filename)
             if fn.is_relative_to(_basepath): fn = fn.relative_to(_basepath)
```

### Comparing `igbpyutils-0.0.3/igbpyutils/file.py` & `igbpyutils-0.0.4/igbpyutils/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,23 +43,28 @@
 def _(item :str): return Path(item)
 @_topath.register
 def _(item :os.PathLike): return Path(item)
 # noinspection PyPep8Naming
 @singledispatch
 def to_Paths(paths :AnyPaths) -> Generator[Path, None, None]:
     """Convert various inputs to ``pathlib.Path`` objects."""
-    yield from map(_topath, iter(paths))
+    # mypy says this: Argument 1 to "iter" has incompatible type
+    # "Union[Union[str, PathLike[Any]], bytes, Iterable[Union[Union[str, PathLike[Any]], bytes]]]"; expected
+    # "SupportsIter[Iterator[Union[int, str, PathLike[Any], bytes]]]"
+    # => I'm not sure where the "int" is coming from, this seems like some kind of misdetection
+    yield from map(_topath, iter(paths))  # type: ignore
+# I'd like to use Union[bytes, str, os.PathLike] to combine the following three, but apparently singledispatch doesn't support that
 @to_Paths.register
-def _(paths :str) -> Generator[Path, None, None]:
+def _(paths :bytes) -> Generator[Path, None, None]:
     yield _topath(paths)
 @to_Paths.register
-def _(paths :os.PathLike) -> Generator[Path, None, None]:
+def _(paths :str) -> Generator[Path, None, None]:
     yield _topath(paths)
 @to_Paths.register
-def _(paths :bytes) -> Generator[Path, None, None]:
+def _(paths :os.PathLike) -> Generator[Path, None, None]:
     yield _topath(paths)
 
 def autoglob(files :Iterable[str], *, force :bool=False) -> Generator[str, None, None]:
     """In Windows, automatically apply ``glob`` and ``expanduser``, otherwise don't change the input."""
     from glob import glob
     from os.path import expanduser
     if sys.platform.startswith('win32') or force:
@@ -82,15 +87,15 @@
         os.chdir(self.newdir)
         return
     def __exit__(self, exc_type, exc_val, exc_tb):
         os.chdir(self.prevdir)
         return False  # raise exception if any
 if sys.hexversion>=0x030B00F0:  # cover-not-le3.10
     import contextlib
-    Pushd = contextlib.chdir
+    Pushd = contextlib.chdir  # type: ignore
 else: pass  # cover-not-ge3.11
 
 def filetypestr(st :os.stat_result) -> str:
     """Return a string naming the file type reported by ``stat``."""
     if stat.S_ISDIR(st.st_mode): return "directory"
     elif stat.S_ISCHR(st.st_mode): return "character special device file"  # pragma: no cover
     elif stat.S_ISBLK(st.st_mode): return "block special device file"  # pragma: no cover
@@ -187,15 +192,15 @@
         os.unlink(tf)
         raise
 
 # noinspection PyPep8Naming
 @contextmanager
 def NamedTempFileDeleteLater(*args, **kwargs) -> Generator:  # cover-not-ge3.12
     """A ``NamedTemporaryFile`` that is unlinked on context manager exit, not on close."""
-    tf = NamedTemporaryFile(*args, **kwargs, delete=False)
+    tf = NamedTemporaryFile(*args, **kwargs, delete=False)  # type: ignore
     try: yield tf
     finally: os.unlink(tf.name)
 #TODO Later: Once 3.12 is released, change the following to 0x030C00F0
 if sys.hexversion>=0x030C0000:  # cover-not-le3.11
     from functools import partial
-    NamedTempFileDeleteLater = partial(NamedTemporaryFile, delete=True, delete_on_close=False)
+    NamedTempFileDeleteLater = partial(NamedTemporaryFile, delete=True, delete_on_close=False)  # type: ignore
 else: pass  # cover-not-ge3.12
```

### Comparing `igbpyutils-0.0.3/igbpyutils/iter.py` & `igbpyutils-0.0.4/igbpyutils/iter.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """Like Python's ``zip``, but requires all iterables to return the same number of items."""
     for combo in zip_longest(*iterables, fillvalue=_marker):
         if any( v is _marker for v in combo ):
             raise ValueError("Iterables have different lengths")
         yield combo
 if sys.hexversion>=0x030A00F0:  # cover-not-le3.9
     from functools import partial
-    zip_strict = partial(zip, strict=True)
+    zip_strict = partial(zip, strict=True)  # type: ignore
 else: pass  # cover-not-ge3.10
 
 _T = TypeVar('_T', covariant=True)
 class SizedCallbackIterator(Generic[_T], Sized, Iterator[_T]):
     """Wrapper to add ``len`` support to an iterator.
 
     For example, this can be used to wrap a generator which has a known output length
@@ -82,40 +82,39 @@
         else:
             if self.callback:
                 self.callback(self._count, val)
             self._count += 1
             return val
 
 _V = TypeVar('_V', covariant=True)
-def is_unique_everseen(iterable :Iterable[_V], *, key :Callable[[_V], Any] = None) -> Generator[bool, None, None]:
+def is_unique_everseen(iterable :Iterable[_V], *, key :Optional[Callable[[_V], Any]] = None) -> Generator[bool, None, None]:
     """For each element in the input iterable, return either ``True`` if this
     element is unique, or ``False`` if it is not.
 
     The implementation is very similar :func:`more_itertools.unique_everseen`
     and is subject to the same performance considerations.
     """
     seen_set = set()
     seen_list = []
-    use_key = key is not None
     for element in iterable:
-        k = key(element) if use_key else element
+        k = element if key is None else key(element)
         try:
             if k not in seen_set:
                 seen_set.add(k)
                 yield True
             else:
                 yield False
         except TypeError:
             if k not in seen_list:
                 seen_list.append(k)
                 yield True
             else:
                 yield False
 
-def no_duplicates(iterable :Iterable[_V], *, key :Callable[[_V], Any] = None, name :str="item") -> Generator[_V, None, None]:
+def no_duplicates(iterable :Iterable[_V], *, key :Optional[Callable[[_V], Any]] = None, name :str="item") -> Generator[_V, None, None]:
     """Raise a ``ValueError`` if there are any duplicate elements in the
     input iterable.
 
     Remember that if you don't want to use this iterator's return values,
     but only use it for checking a list, you need to force it to execute
     by wrapping the call e.g. in a ``set()`` or ``list()``.
     Alternatively, use ``not all(is_unique_everseen(iterable))``.
```

### Comparing `igbpyutils-0.0.3/igbpyutils/test.py` & `igbpyutils-0.0.4/igbpyutils/test.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.3/igbpyutils.egg-info/PKG-INFO` & `igbpyutils-0.0.4/igbpyutils.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: igbpyutils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Various Python Utilities
 Author-email: Hauke D <haukex@zero-g.net>
 Project-URL: Homepage, https://github.com/haukex/igbpyutils
 Project-URL: Bug Tracker, https://github.com/haukex/igbpyutils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,14 +23,15 @@
 ====================
 
 This is a collection of various Python tools, libraries, and utilities
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
 (IGB) in the Forschungsverbund Berlin e.V. (<https://www.igb-berlin.de/en>).
 
 Please see the individual files in this project for documentation.
+(TODO: Check and generate documentation with Sphinx)
 
 This is a companion library to the `igbdatatools` library
 (<https://github.com/haukex/igbdatatools>) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
 cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
```

### Comparing `igbpyutils-0.0.3/pyproject.toml` & `igbpyutils-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "igbpyutils"
 description = "Various Python Utilities"
-version = "0.0.3"
+version = "0.0.4"
 authors = [ { name="Hauke D", email="haukex@zero-g.net" } ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
```

### Comparing `igbpyutils-0.0.3/tests/test_dt.py` & `igbpyutils-0.0.4/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.3/tests/test_error.py` & `igbpyutils-0.0.4/tests/test_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,29 +25,36 @@
 import sys
 import os
 import subprocess
 import inspect
 from contextlib import redirect_stderr
 from pathlib import Path
 from warnings import warn
-from igbpyutils.error import running_in_unittest, javaishstacktrace, CustomHandlers, init_handlers
+from igbpyutils.error import running_in_unittest, javaishstacktrace, CustomHandlers, init_handlers, extype_fullname, ex_repr
 # noinspection PyProtectedMember
 from igbpyutils.error import _basepath
 import tests.error_test_funcs
 import tests.error_test_unraisable
 
 class TestErrorUtils(unittest.TestCase):
 
     def setUp(self):
         self.mybasepath = Path(__file__).parent.parent.joinpath('tests').resolve(strict=True).relative_to(_basepath)
         self.maxDiff = None
         # for subprocess.run: env must include SYSTEMROOT, so just make a copy of the current env and add to it
         self.environ = dict(os.environ)
         self.environ['PYTHONPATH'] = str(Path(__file__).parent.parent)
 
+    def test_error_names(self):
+        from tests.error_test_funcs import TestError
+        self.assertEqual( extype_fullname(TestError), 'tests.error_test_funcs.TestError' )
+        self.assertEqual( extype_fullname(TimeoutError), 'TimeoutError' )
+        self.assertEqual( ex_repr( TestError('Hello', 'world') ), "tests.error_test_funcs.TestError('Hello', 'world')" )
+        self.assertEqual( ex_repr( ConnectionResetError('foo', 'bar') ), "ConnectionResetError('foo', 'bar')" )
+
     def test_running_in_unittest(self):
         self.assertTrue(running_in_unittest())
         sp1 = subprocess.run([sys.executable, '-c', 'import igbpyutils.error; print(repr(igbpyutils.error.running_in_unittest()))'],
             check=True, capture_output=True, cwd=Path(__file__).parent.parent, env=self.environ)
         self.assertEqual(b'False', sp1.stdout.strip())
         self.assertEqual(b'', sp1.stderr)
         sp2 = subprocess.run([sys.executable, '-c', 'import unittest; import igbpyutils.error; print(repr(igbpyutils.error.running_in_unittest()))'],
```

### Comparing `igbpyutils-0.0.3/tests/test_file.py` & `igbpyutils-0.0.4/tests/test_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see https://www.gnu.org/licenses/
 """
 import unittest
+from typing import Optional
 from unittest.mock import patch
 import sys
 import os
 import stat
 from pathlib import Path
 from tempfile import TemporaryDirectory, NamedTemporaryFile
 from igbpyutils.file import to_Paths, autoglob, Pushd, filetypestr, is_windows_filename_bad, replacer, replace_symlink, NamedTempFileDeleteLater
@@ -183,15 +184,15 @@
         if os.name == 'posix':
             with TemporaryDirectory() as td:
                 tp = Path(td)
                 fx = tp/'x.txt'
                 fy = tp/'y.txt'
                 with fx.open('w', encoding='ASCII') as fh: fh.write("Hello, World\n")
 
-                def assert_state(linktarg :str, xtra :list[Path]=None):
+                def assert_state(linktarg :str, xtra :Optional[list[Path]]=None):
                     if not xtra: xtra = []
                     self.assertEqual( sorted(tp.iterdir()), sorted([fx,fy]+xtra) )
                     self.assertTrue( fx.is_file() )
                     self.assertTrue( fy.is_symlink() )
                     self.assertEqual( os.readlink(fy), linktarg )
 
                 self.assertEqual( list(tp.iterdir()), [fx] )
```

### Comparing `igbpyutils-0.0.3/tests/test_iter.py` & `igbpyutils-0.0.4/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.3/tests/test_test.py` & `igbpyutils-0.0.4/tests/test_test.py`

 * *Files identical despite different names*

