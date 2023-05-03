# Comparing `tmp/igbpyutils-0.0.4.tar.gz` & `tmp/igbpyutils-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "igbpyutils-0.0.4.tar", last modified: Wed May  3 16:59:53 2023, max compression
+gzip compressed data, was "igbpyutils-0.0.5.tar", last modified: Wed May  3 20:34:45 2023, max compression
```

## Comparing `igbpyutils-0.0.4.tar` & `igbpyutils-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/
--rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.4/LICENSE.txt
--rw-------   0 haukex    (1000) haukex    (1000)     2427 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)     1549 2023-05-03 16:06:37.000000 igbpyutils-0.0.4/README.md
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/igbpyutils/
--rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.4/igbpyutils/__init__.py
--rw-------   0 haukex    (1000) haukex    (1000)     1528 2023-04-16 11:28:55.000000 igbpyutils-0.0.4/igbpyutils/dt.py
--rw-------   0 haukex    (1000) haukex    (1000)     5730 2023-05-03 16:39:35.000000 igbpyutils-0.0.4/igbpyutils/error.py
--rw-------   0 haukex    (1000) haukex    (1000)     9717 2023-05-03 16:48:00.000000 igbpyutils-0.0.4/igbpyutils/file.py
--rw-------   0 haukex    (1000) haukex    (1000)     5442 2023-05-03 16:48:35.000000 igbpyutils-0.0.4/igbpyutils/iter.py
--rw-------   0 haukex    (1000) haukex    (1000)     1429 2023-04-14 19:21:32.000000 igbpyutils-0.0.4/igbpyutils/test.py
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/igbpyutils.egg-info/
--rw-------   0 haukex    (1000) haukex    (1000)     2427 2023-05-03 16:59:53.000000 igbpyutils-0.0.4/igbpyutils.egg-info/PKG-INFO
--rw-------   0 haukex    (1000) haukex    (1000)      383 2023-05-03 16:59:53.000000 igbpyutils-0.0.4/igbpyutils.egg-info/SOURCES.txt
--rw-------   0 haukex    (1000) haukex    (1000)        1 2023-05-03 16:59:53.000000 igbpyutils-0.0.4/igbpyutils.egg-info/dependency_links.txt
--rw-------   0 haukex    (1000) haukex    (1000)       11 2023-05-03 16:59:53.000000 igbpyutils-0.0.4/igbpyutils.egg-info/top_level.txt
--rw-------   0 haukex    (1000) haukex    (1000)      904 2023-05-03 16:51:32.000000 igbpyutils-0.0.4/pyproject.toml
--rw-------   0 haukex    (1000) haukex    (1000)       38 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/setup.cfg
-drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 16:59:53.585088 igbpyutils-0.0.4/tests/
--rwxr-xr-x   0 haukex    (1000) haukex    (1000)     2023 2023-04-16 11:23:30.000000 igbpyutils-0.0.4/tests/test_dt.py
--rwx------   0 haukex    (1000) haukex    (1000)     6923 2023-05-03 16:39:39.000000 igbpyutils-0.0.4/tests/test_error.py
--rwx------   0 haukex    (1000) haukex    (1000)    11434 2023-05-03 16:24:28.000000 igbpyutils-0.0.4/tests/test_file.py
--rwx------   0 haukex    (1000) haukex    (1000)     9018 2023-04-16 11:21:31.000000 igbpyutils-0.0.4/tests/test_iter.py
--rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.4/tests/test_test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 20:34:45.853783 igbpyutils-0.0.5/
+-rw-------   0 haukex    (1000) haukex    (1000)    35149 2023-04-14 17:49:50.000000 igbpyutils-0.0.5/LICENSE.txt
+-rw-------   0 haukex    (1000) haukex    (1000)      950 2023-05-03 20:34:45.853783 igbpyutils-0.0.5/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)     1491 2023-05-03 20:27:15.000000 igbpyutils-0.0.5/README.rst
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 20:34:45.853783 igbpyutils-0.0.5/igbpyutils/
+-rw-------   0 haukex    (1000) haukex    (1000)        0 2023-04-14 19:16:14.000000 igbpyutils-0.0.5/igbpyutils/__init__.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1537 2023-05-03 20:27:15.000000 igbpyutils-0.0.5/igbpyutils/dt.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5737 2023-05-03 20:27:15.000000 igbpyutils-0.0.5/igbpyutils/error.py
+-rw-------   0 haukex    (1000) haukex    (1000)     9756 2023-05-03 20:27:15.000000 igbpyutils-0.0.5/igbpyutils/file.py
+-rw-------   0 haukex    (1000) haukex    (1000)     5494 2023-05-03 20:27:15.000000 igbpyutils-0.0.5/igbpyutils/iter.py
+-rw-------   0 haukex    (1000) haukex    (1000)     1457 2023-05-03 20:27:15.000000 igbpyutils-0.0.5/igbpyutils/test.py
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 20:34:45.853783 igbpyutils-0.0.5/igbpyutils.egg-info/
+-rw-------   0 haukex    (1000) haukex    (1000)      950 2023-05-03 20:34:45.000000 igbpyutils-0.0.5/igbpyutils.egg-info/PKG-INFO
+-rw-------   0 haukex    (1000) haukex    (1000)      384 2023-05-03 20:34:45.000000 igbpyutils-0.0.5/igbpyutils.egg-info/SOURCES.txt
+-rw-------   0 haukex    (1000) haukex    (1000)        1 2023-05-03 20:34:45.000000 igbpyutils-0.0.5/igbpyutils.egg-info/dependency_links.txt
+-rw-------   0 haukex    (1000) haukex    (1000)       11 2023-05-03 20:34:45.000000 igbpyutils-0.0.5/igbpyutils.egg-info/top_level.txt
+-rw-------   0 haukex    (1000) haukex    (1000)      969 2023-05-03 20:30:23.000000 igbpyutils-0.0.5/pyproject.toml
+-rw-------   0 haukex    (1000) haukex    (1000)       38 2023-05-03 20:34:45.853783 igbpyutils-0.0.5/setup.cfg
+drwx------   0 haukex    (1000) haukex    (1000)        0 2023-05-03 20:34:45.853783 igbpyutils-0.0.5/tests/
+-rwxr-xr-x   0 haukex    (1000) haukex    (1000)     2023 2023-04-16 11:23:30.000000 igbpyutils-0.0.5/tests/test_dt.py
+-rwx------   0 haukex    (1000) haukex    (1000)     6923 2023-05-03 16:39:39.000000 igbpyutils-0.0.5/tests/test_error.py
+-rwx------   0 haukex    (1000) haukex    (1000)    11434 2023-05-03 16:24:28.000000 igbpyutils-0.0.5/tests/test_file.py
+-rwx------   0 haukex    (1000) haukex    (1000)     9018 2023-04-16 11:21:31.000000 igbpyutils-0.0.5/tests/test_iter.py
+-rwx------   0 haukex    (1000) haukex    (1000)     1606 2023-04-14 19:26:01.000000 igbpyutils-0.0.5/tests/test_test.py
```

### Comparing `igbpyutils-0.0.4/LICENSE.txt` & `igbpyutils-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.4/README.md` & `igbpyutils-0.0.5/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 IGB Python Utilities
 ====================
 
 This is a collection of various Python tools, libraries, and utilities
 developed at the Leibniz Institute of Freshwater Ecology and Inland Fisheries
-(IGB) in the Forschungsverbund Berlin e.V. (<https://www.igb-berlin.de/en>).
+(IGB) in the Forschungsverbund Berlin e.V. (https://www.igb-berlin.de/en).
 
-Please see the individual files in this project for documentation.
-(TODO: Check and generate documentation with Sphinx)
-
-This is a companion library to the `igbdatatools` library
-(<https://github.com/haukex/igbdatatools>) which normally targets the latest
+This is a companion library to the ``igbdatatools`` library
+(https://github.com/haukex/igbdatatools) which normally targets the latest
 Python version.
 This library is intended to contain more general-purpose tools and
 cover a slightly broader range of Python versions, currently Python 3.9 to 3.11.
 
+The documentation is available at https://igbpyutils.readthedocs.io/
+
 
 Author, Copyright, and License
 ------------------------------
 
-Copyright (c) 2022-2023 Hauke Daempfling <haukex@zero-g.net>
+Copyright (c) 2022-2023 Hauke Daempfling (haukex@zero-g.net)
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
-Berlin, Germany, <https://www.igb-berlin.de/>
+Berlin, Germany, https://www.igb-berlin.de/
 
 This program is free software: you can redistribute it and/or modify
 it under the terms of the GNU General Public License as published by
 the Free Software Foundation, either version 3 of the License, or
 (at your option) any later version.
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
-along with this program. If not, see <https://www.gnu.org/licenses/>.
+along with this program. If not, see https://www.gnu.org/licenses/
```

### Comparing `igbpyutils-0.0.4/igbpyutils/dt.py` & `igbpyutils-0.0.5/igbpyutils/dt.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!python3
-"""Library with datetime utility functions
+"""Datetime Utility Functions
 
 Author, Copyright, and License
 ------------------------------
 Copyright (c) 2022-2023 Hauke Daempfling (haukex@zero-g.net)
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
 Berlin, Germany, https://www.igb-berlin.de/
 
@@ -19,22 +19,23 @@
 
 You should have received a copy of the GNU General Public License
 along with this program. If not, see https://www.gnu.org/licenses/
 """
 from datetime import timedelta
 
 def timedelta_str(td :timedelta) -> str:
-    """Simple replacement for timedelta's default string formatting with nicer output of negative deltas.
+    """Simple replacement for the :class:`~datetime.timedelta` default string formatting with nicer output of negative deltas.
 
         >>> str(timedelta(hours=-1))
         '-1 day, 23:00:00'
         >>> timedelta_str(timedelta(hours=-1))
         '-1:00:00'
 
     Possible alternatives:
-    - https://dateutil.readthedocs.io/en/stable/relativedelta.html
-    - https://pypi.org/project/readabledelta/
+
+    * https://dateutil.readthedocs.io/en/stable/relativedelta.html
+    * https://pypi.org/project/readabledelta/
     """
     return '-' + str(-td) if td < timedelta(0) else str(td)
 
 #TODO Later: datetime truncate
 #TODO Later: datetime fromisoformat (backport support for Z suffix)
```

### Comparing `igbpyutils-0.0.4/igbpyutils/error.py` & `igbpyutils-0.0.5/igbpyutils/error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!python3
-"""Library with error handling and formatting utilities.
+"""Error Handling and Formatting Utilities
 
 Author, Copyright, and License
 ------------------------------
 Copyright (c) 2022-2023 Hauke Daempfling (haukex@zero-g.net)
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
 Berlin, Germany, https://www.igb-berlin.de/
 
@@ -26,15 +26,15 @@
 from collections.abc import Generator
 from pathlib import Path
 # noinspection PyPackageRequirements
 import __main__  # just to get __main__.__file__ below
 from traceback import extract_tb
 
 def running_in_unittest() -> bool:
-    """Attempt to detect if we're running under ``unittest``.
+    """Attempt to detect if we're running under :mod:`unittest`.
 
     This is slightly hackish and used in this module only for slightly nicer output during testing."""
     # note the following is actually tested, but the "false" case isn't seen by the "coverage" tool
     return 'unittest' in sys.modules and any(  # pragma: no cover
         Path(stack_frame.frame.f_code.co_filename).parts[-2:] == ('unittest','main.py')
         for stack_frame in inspect.stack() )
 
@@ -75,37 +75,37 @@
     err_msg = unraisable.err_msg if unraisable.err_msg else "Exception ignored in"
     print(f'{err_msg}: {unraisable.object!r}')
     for s in javaishstacktrace(unraisable.exc_value): print(s)
 
 class CustomHandlers:
     """A context manager that installs and removes this module's custom error and warning handlers.
 
-    This modifies ``warnings.showwarning``, ``sys.excepthook``, and ``sys.unraisablehook``."""
+    This modifies :func:`warnings.showwarning`, :func:`sys.excepthook`, and :func:`sys.unraisablehook`."""
     def __enter__(self):
         self.showwarning_orig = warnings.showwarning
         warnings.showwarning = _showwarning
         sys.excepthook = _excepthook
         sys.unraisablehook = _unraisablehook
         return self
     def __exit__(self, exc_type, exc_val, exc_tb):
         warnings.showwarning = self.showwarning_orig
         sys.excepthook = sys.__excepthook__
         sys.unraisablehook = sys.__unraisablehook__
         return False  # raise exception if any
 
 def init_handlers() -> None:
-    """Set up the ``CustomHandlers`` once and don't change them back."""
+    """Set up the :class:`CustomHandlers` once and don't change them back."""
     CustomHandlers().__enter__()
 
 def javaishstacktrace(ex :BaseException) -> Generator[str, None, None]:
     """Generate a stack trace in the style of Java.
 
     Compared to Java, the order of exceptions is reversed, so it reads more like a stack.
 
-    ``AssertionError``s are treated specially in that the line of source code that caused them is printed.
+    :exc:`AssertionError` is treated specially in that the line of source code that caused them is printed.
     """
     causes = [ex]
     while ex.__cause__:
         ex = ex.__cause__
         causes.append(ex)
     first = True
     for e in reversed(causes):
```

### Comparing `igbpyutils-0.0.4/igbpyutils/file.py` & `igbpyutils-0.0.5/igbpyutils/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!python3
-"""Library with some file-related utility functions.
+"""File-Related Utility Functions
 
 Author, Copyright, and License
 ------------------------------
 Copyright (c) 2022-2023 Hauke Daempfling (haukex@zero-g.net)
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
 Berlin, Germany, https://www.igb-berlin.de/
 
@@ -42,15 +42,15 @@
 @_topath.register
 def _(item :str): return Path(item)
 @_topath.register
 def _(item :os.PathLike): return Path(item)
 # noinspection PyPep8Naming
 @singledispatch
 def to_Paths(paths :AnyPaths) -> Generator[Path, None, None]:
-    """Convert various inputs to ``pathlib.Path`` objects."""
+    """Convert various inputs to :class:`~pathlib.Path` objects."""
     # mypy says this: Argument 1 to "iter" has incompatible type
     # "Union[Union[str, PathLike[Any]], bytes, Iterable[Union[Union[str, PathLike[Any]], bytes]]]"; expected
     # "SupportsIter[Iterator[Union[int, str, PathLike[Any], bytes]]]"
     # => I'm not sure where the "int" is coming from, this seems like some kind of misdetection
     yield from map(_topath, iter(paths))  # type: ignore
 # I'd like to use Union[bytes, str, os.PathLike] to combine the following three, but apparently singledispatch doesn't support that
 @to_Paths.register
@@ -60,15 +60,15 @@
 def _(paths :str) -> Generator[Path, None, None]:
     yield _topath(paths)
 @to_Paths.register
 def _(paths :os.PathLike) -> Generator[Path, None, None]:
     yield _topath(paths)
 
 def autoglob(files :Iterable[str], *, force :bool=False) -> Generator[str, None, None]:
-    """In Windows, automatically apply ``glob`` and ``expanduser``, otherwise don't change the input."""
+    """In Windows, automatically apply :func:`~glob.glob` and :func:`~os.path.expanduser`, otherwise don't change the input."""
     from glob import glob
     from os.path import expanduser
     if sys.platform.startswith('win32') or force:
         for f in files:
             f = expanduser(f)
             g = glob(f)  # note glob always returns a list
             # If a *NIX glob doesn't match anything, it isn't expanded,
@@ -91,15 +91,15 @@
         return False  # raise exception if any
 if sys.hexversion>=0x030B00F0:  # cover-not-le3.10
     import contextlib
     Pushd = contextlib.chdir  # type: ignore
 else: pass  # cover-not-ge3.11
 
 def filetypestr(st :os.stat_result) -> str:
-    """Return a string naming the file type reported by ``stat``."""
+    """Return a string naming the file type reported by :func:`os.stat`."""
     if stat.S_ISDIR(st.st_mode): return "directory"
     elif stat.S_ISCHR(st.st_mode): return "character special device file"  # pragma: no cover
     elif stat.S_ISBLK(st.st_mode): return "block special device file"  # pragma: no cover
     elif stat.S_ISREG(st.st_mode): return "regular file"
     elif stat.S_ISFIFO(st.st_mode): return "FIFO (named pipe)"
     elif stat.S_ISLNK(st.st_mode): return "symbolic link"
     elif stat.S_ISSOCK(st.st_mode): return "socket"  # pragma: no cover
@@ -136,15 +136,15 @@
 
     With this context manager, a temporary file is created in the same directory as the original file.
     The context manager gives you two file handles: the input file, and the output file, the latter
     being the temporary file. You can then read from the input file and write to the output file.
     When the context manager is exited, it will replace the input file over the temporary file.
     If an error occurs in the context manager, the temporary file is unlinked and the original file left unchanged.
 
-    Depending on the OS and file system, the ``os.replace`` used here *may* be an atomic operation.
+    Depending on the OS and file system, the :func:`os.replace` used here *may* be an atomic operation.
     However, this function doesn't provide protection against multiple writers and is therefore
     intended for files with a single writer and multiple readers.
     Multiple writers will need to be coordinated with external locking mechanisms.
     """
     fname = Path(file).resolve(strict=True)
     if not fname.is_file(): raise ValueError(f"not a regular file: {fname}")
     with fname.open(mode = 'rb' if binary else 'r', encoding=encoding, errors=errors, newline=newline) as infh:
@@ -161,15 +161,15 @@
     try: os.chmod(tf.name, origmode)
     except NotImplementedError: pass  # pragma: no cover
     os.replace(tf.name, fname)
 
 def replace_symlink(src :Filename, dst :Filename, missing_ok :bool=False):
     """Attempt to atomically replace (or create) a symbolic link pointing to ``src`` named ``dst``.
 
-    Depending on the OS and file system, the ``os.replace`` used here *may* be an atomic operation.
+    Depending on the OS and file system, the :func:`os.replace` used here *may* be an atomic operation.
     However, the surrounding operations (e.g. checking if ``dst`` exists etc.) present a small
     chance for race conditions, so this function is primarily suited for situations with a single
     writer and multiple readers.
     Multiple writers will need to be coordinated with external locking mechanisms.
     """
     if os.name != 'posix':  # pragma: no cover
         raise NotImplementedError("only available on POSIX systems")
@@ -191,15 +191,15 @@
     except BaseException:
         os.unlink(tf)
         raise
 
 # noinspection PyPep8Naming
 @contextmanager
 def NamedTempFileDeleteLater(*args, **kwargs) -> Generator:  # cover-not-ge3.12
-    """A ``NamedTemporaryFile`` that is unlinked on context manager exit, not on close."""
+    """A :func:`~tempfile.NamedTemporaryFile` that is unlinked on context manager exit, not on close."""
     tf = NamedTemporaryFile(*args, **kwargs, delete=False)  # type: ignore
     try: yield tf
     finally: os.unlink(tf.name)
 #TODO Later: Once 3.12 is released, change the following to 0x030C00F0
 if sys.hexversion>=0x030C0000:  # cover-not-le3.11
     from functools import partial
     NamedTempFileDeleteLater = partial(NamedTemporaryFile, delete=True, delete_on_close=False)  # type: ignore
```

### Comparing `igbpyutils-0.0.4/igbpyutils/iter.py` & `igbpyutils-0.0.5/igbpyutils/iter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python3
-"""A few useful iterators.
+"""A Few Useful Iterators
 
-Note the iterator ``gray_product`` that used to be in this module
-has been merged into ``more_itertools`` as of version 9.1.0.
+Note the iterator "``gray_product``" that used to be in this module
+has been merged into :mod:`more_itertools` as of its version 9.1.0.
 
 Author, Copyright, and License
 ------------------------------
 Copyright (c) 2022-2023 Hauke Daempfling (haukex@zero-g.net)
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
 Berlin, Germany, https://www.igb-berlin.de/
 
@@ -54,19 +54,19 @@
 if sys.hexversion>=0x030A00F0:  # cover-not-le3.9
     from functools import partial
     zip_strict = partial(zip, strict=True)  # type: ignore
 else: pass  # cover-not-ge3.10
 
 _T = TypeVar('_T', covariant=True)
 class SizedCallbackIterator(Generic[_T], Sized, Iterator[_T]):
-    """Wrapper to add ``len`` support to an iterator.
+    """Wrapper to add :func:`len` support to an iterator.
 
     For example, this can be used to wrap a generator which has a known output length
     (e.g. if it returns exactly one item per input item), so that it can then
-    be used in libraries like ``tqdm``."""
+    be used in libraries like `tqdm <https://tqdm.github.io/>`_."""
     def __init__(self, it :Iterable[_T], length :int, *, strict :bool=False, callback :Optional[Callable[[int, _T], None]]=None):
         if length<0: raise ValueError("length must be >= 0")
         self.it = iter(it)
         self.length = length
         self._count = 0
         self.strict = strict
         self.callback = callback
@@ -83,16 +83,16 @@
             if self.callback:
                 self.callback(self._count, val)
             self._count += 1
             return val
 
 _V = TypeVar('_V', covariant=True)
 def is_unique_everseen(iterable :Iterable[_V], *, key :Optional[Callable[[_V], Any]] = None) -> Generator[bool, None, None]:
-    """For each element in the input iterable, return either ``True`` if this
-    element is unique, or ``False`` if it is not.
+    """For each element in the input iterable, return either :obj:`True` if this
+    element is unique, or :obj:`False` if it is not.
 
     The implementation is very similar :func:`more_itertools.unique_everseen`
     and is subject to the same performance considerations.
     """
     seen_set = set()
     seen_list = []
     for element in iterable:
@@ -107,20 +107,20 @@
             if k not in seen_list:
                 seen_list.append(k)
                 yield True
             else:
                 yield False
 
 def no_duplicates(iterable :Iterable[_V], *, key :Optional[Callable[[_V], Any]] = None, name :str="item") -> Generator[_V, None, None]:
-    """Raise a ``ValueError`` if there are any duplicate elements in the
+    """Raise a :exc:`ValueError` if there are any duplicate elements in the
     input iterable.
 
     Remember that if you don't want to use this iterator's return values,
     but only use it for checking a list, you need to force it to execute
-    by wrapping the call e.g. in a ``set()`` or ``list()``.
+    by wrapping the call e.g. in a :class:`set` or :class:`list`.
     Alternatively, use ``not all(is_unique_everseen(iterable))``.
 
     The ``name`` argument is only to customize the error messages.
 
     :func:`more_itertools.duplicates_everseen` could also be used for this purpose,
     but this function returns the values of the input iterable.
```

### Comparing `igbpyutils-0.0.4/igbpyutils/test.py` & `igbpyutils-0.0.5/igbpyutils/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!python3
-"""Some utilities for testing.
+"""Utilities for Testing
 
-Note the ``MyNamedTempFile`` utility has been moved to ``igbpyutils.file.NamedTempFileDeleteLater``.
+Note the utility previously named "``MyNamedTempFile``"
+has been moved to :class:`igbpyutils.file.NamedTempFileDeleteLater`.
 
 Author, Copyright, and License
 ------------------------------
 Copyright (c) 2023 Hauke Daempfling (haukex@zero-g.net)
 at the Leibniz Institute of Freshwater Ecology and Inland Fisheries (IGB),
 Berlin, Germany, https://www.igb-berlin.de/
 
@@ -23,15 +24,15 @@
 along with this program. If not, see https://www.gnu.org/licenses/
 """
 from copy import deepcopy
 from typing import TypeVar, Generic
 
 _T = TypeVar('_T')
 class tempcopy(Generic[_T]):
-    """A simple context manager that provides a temporary ``deepcopy`` of the variable given to it."""
+    """A simple context manager that provides a temporary :func:`~copy.deepcopy` of the variable given to it."""
     def __init__(self, obj :_T):
         self.obj = deepcopy(obj)
     def __enter__(self) -> _T:
         return self.obj
     def __exit__(self, *exc):
         del self.obj
         return False  # don't suppress exception
```

### Comparing `igbpyutils-0.0.4/pyproject.toml` & `igbpyutils-0.0.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "igbpyutils"
 description = "Various Python Utilities"
-version = "0.0.4"
+version = "0.0.5"
 authors = [ { name="Hauke D", email="haukex@zero-g.net" } ]
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -21,7 +21,8 @@
     "Development Status :: 5 - Production/Stable",
     "Topic :: Software Development :: Libraries",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/haukex/igbpyutils"
 "Bug Tracker" = "https://github.com/haukex/igbpyutils/issues"
+"Documentation" = "https://igbpyutils.readthedocs.io/en/stable/"
```

### Comparing `igbpyutils-0.0.4/tests/test_dt.py` & `igbpyutils-0.0.5/tests/test_dt.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.4/tests/test_error.py` & `igbpyutils-0.0.5/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.4/tests/test_file.py` & `igbpyutils-0.0.5/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.4/tests/test_iter.py` & `igbpyutils-0.0.5/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `igbpyutils-0.0.4/tests/test_test.py` & `igbpyutils-0.0.5/tests/test_test.py`

 * *Files identical despite different names*

