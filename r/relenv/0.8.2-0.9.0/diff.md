# Comparing `tmp/relenv-0.8.2-py3-none-any.whl.zip` & `tmp/relenv-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 42340 bytes, number of entries: 20
--rw-r--r--  2.0 unx      109 b- defN 23-Mar-17 20:18 relenv/__init__.py
--rw-r--r--  2.0 unx     1283 b- defN 23-Mar-17 20:18 relenv/__main__.py
--rw-r--r--  2.0 unx    10338 b- defN 23-Mar-17 20:18 relenv/common.py
--rw-r--r--  2.0 unx     3868 b- defN 23-Mar-17 20:18 relenv/create.py
--rw-r--r--  2.0 unx     1551 b- defN 23-Mar-17 20:18 relenv/fetch.py
--rw-r--r--  2.0 unx    11432 b- defN 23-Mar-17 20:18 relenv/relocate.py
--rw-r--r--  2.0 unx    13955 b- defN 23-Mar-17 20:18 relenv/runtime.py
--rw-r--r--  2.0 unx     5370 b- defN 23-Mar-17 20:18 relenv/toolchain.py
--rw-r--r--  2.0 unx     4365 b- defN 23-Mar-17 20:18 relenv/build/__init__.py
--rw-r--r--  2.0 unx    45605 b- defN 23-Mar-17 20:18 relenv/build/common.py
--rw-r--r--  2.0 unx     3551 b- defN 23-Mar-17 20:18 relenv/build/darwin.py
--rw-r--r--  2.0 unx    16888 b- defN 23-Mar-17 20:18 relenv/build/linux.py
--rw-r--r--  2.0 unx     5692 b- defN 23-Mar-17 20:18 relenv/build/windows.py
--rw-r--r--  2.0 unx     9919 b- defN 23-Mar-17 20:18 relenv-0.8.2.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1269 b- defN 23-Mar-17 20:18 relenv-0.8.2.dist-info/METADATA
--rw-r--r--  2.0 unx      548 b- defN 23-Mar-17 20:18 relenv-0.8.2.dist-info/NOTICE
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-17 20:18 relenv-0.8.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       48 b- defN 23-Mar-17 20:18 relenv-0.8.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-17 20:18 relenv-0.8.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1556 b- defN 23-Mar-17 20:18 relenv-0.8.2.dist-info/RECORD
-20 files, 137446 bytes uncompressed, 39850 bytes compressed:  71.0%
+Zip file size: 42931 bytes, number of entries: 20
+-rw-r--r--  2.0 unx      109 b- defN 23-Mar-20 07:52 relenv/__init__.py
+-rw-r--r--  2.0 unx     1283 b- defN 23-Mar-20 07:52 relenv/__main__.py
+-rw-r--r--  2.0 unx    10338 b- defN 23-Mar-20 07:52 relenv/common.py
+-rw-r--r--  2.0 unx     3868 b- defN 23-Mar-20 07:52 relenv/create.py
+-rw-r--r--  2.0 unx     1551 b- defN 23-Mar-20 07:52 relenv/fetch.py
+-rw-r--r--  2.0 unx    11432 b- defN 23-Mar-20 07:52 relenv/relocate.py
+-rw-r--r--  2.0 unx    15583 b- defN 23-Mar-20 07:52 relenv/runtime.py
+-rw-r--r--  2.0 unx     5370 b- defN 23-Mar-20 07:52 relenv/toolchain.py
+-rw-r--r--  2.0 unx     4365 b- defN 23-Mar-20 07:52 relenv/build/__init__.py
+-rw-r--r--  2.0 unx    45706 b- defN 23-Mar-20 07:52 relenv/build/common.py
+-rw-r--r--  2.0 unx     3551 b- defN 23-Mar-20 07:52 relenv/build/darwin.py
+-rw-r--r--  2.0 unx    16999 b- defN 23-Mar-20 07:52 relenv/build/linux.py
+-rw-r--r--  2.0 unx     5692 b- defN 23-Mar-20 07:52 relenv/build/windows.py
+-rw-r--r--  2.0 unx     9919 b- defN 23-Mar-20 07:52 relenv-0.9.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1269 b- defN 23-Mar-20 07:52 relenv-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      548 b- defN 23-Mar-20 07:52 relenv-0.9.0.dist-info/NOTICE
+-rw-r--r--  2.0 unx       92 b- defN 23-Mar-20 07:52 relenv-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 23-Mar-20 07:52 relenv-0.9.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Mar-20 07:52 relenv-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1556 b- defN 23-Mar-20 07:52 relenv-0.9.0.dist-info/RECORD
+20 files, 139286 bytes uncompressed, 40441 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -33,29 +33,29 @@
 
 Filename: relenv/build/linux.py
 Comment: 
 
 Filename: relenv/build/windows.py
 Comment: 
 
-Filename: relenv-0.8.2.dist-info/LICENSE.md
+Filename: relenv-0.9.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: relenv-0.8.2.dist-info/METADATA
+Filename: relenv-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: relenv-0.8.2.dist-info/NOTICE
+Filename: relenv-0.9.0.dist-info/NOTICE
 Comment: 
 
-Filename: relenv-0.8.2.dist-info/WHEEL
+Filename: relenv-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: relenv-0.8.2.dist-info/entry_points.txt
+Filename: relenv-0.9.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: relenv-0.8.2.dist-info/top_level.txt
+Filename: relenv-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: relenv-0.8.2.dist-info/RECORD
+Filename: relenv-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## relenv/common.py

```diff
@@ -12,15 +12,15 @@
 import tarfile
 import textwrap
 import time
 import urllib.error
 import urllib.request
 
 # relenv package version
-__version__ = "0.8.2"
+__version__ = "0.9.0"
 
 MODULE_DIR = pathlib.Path(__file__).resolve().parent
 
 LINUX = "linux"
 WIN32 = "win32"
 DARWIN = "darwin"
```

## relenv/runtime.py

```diff
@@ -14,16 +14,17 @@
 import functools
 import importlib
 import os
 import pathlib
 import shutil
 import subprocess
 import sys
+import textwrap
 
-from .common import MODULE_DIR, format_shebang
+from .common import MODULE_DIR, format_shebang, get_triplet, work_dirs
 
 
 def get_major_version():
     """
     Current python major version.
     """
     return "{}.{}".format(*sys.version_info)
@@ -273,133 +274,218 @@
                     if relocate.is_elf(file):
                         debug(f"Relenv - Found elf {file}")
                         relocate.handle_elf(plat / file, rootdir / "lib", True, rootdir)
 
     return wrapper
 
 
+class Wrapper:
+    """
+    Wrap methods of an imported module.
+    """
+
+    def __init__(self, module, wrapper, matcher="equals", _loading=False):
+        self.module = module
+        self.wrapper = wrapper
+        self.matcher = matcher
+        self.loading = _loading
+
+    def matches(self, module):
+        """
+        Check if wrapper metches module being imported.
+        """
+        if self.matcher == "startswith":
+            return module.startswith(self.module)
+        return self.module == module
+
+    def __call__(self, module_name):
+        """
+        Preform the wrapper operation.
+        """
+        return self.wrapper(module_name)
+
+
 class RelenvImporter:
     """
-    An importer to be added to ``sys.meta_path`` to handle importing into a relenv environment.
+    Handle runtime wrapping of module methods.
     """
 
-    loading_pip_scripts = False
-    loading_sysconfig_data = False
-    loading_sysconfig = False
-    loading_distutils = False
-    loading_op_wheel = False
-    loading_op_legacy = False
+    def __init__(self, wrappers=None, _loads=None):
+        if wrappers is None:
+            wrappers = []
+        self.wrappers = wrappers
+        if _loads is None:
+            _loads = {}
+        self._loads = _loads
 
     def find_module(self, module_name, package_path=None):
         """
-        Find a module for importing into the relenv environment.
-
-        :param module_name: The name of the module
-        :type module_name: str
-        :param package_path: The path to the package, defaults to None
-        :type package_path: str, optional
-        :return: The instance that called this method if it found the module, or None if it didn't
-        :rtype: RelenvImporter or None
-        """
-        if module_name.startswith("sysconfig"):  # and sys.platform == "win32":
-            if self.loading_sysconfig:
-                return None
-            debug(f"RelenvImporter - match {module_name}")
-            self.loading_sysconfig = True
-            return self
-        elif module_name == "pip._vendor.distlib.scripts":
-            if self.loading_pip_scripts:
-                return None
-            debug(f"RelenvImporter - match {module_name}")
-            self.loading_pip_scripts = True
-            return self
-        elif module_name == "distutils.command.build_ext":
-            if self.loading_distutils:
-                return None
-            debug(f"RelenvImporter - match {module_name}")
-            self.loading_distutils = True
-            return self
-        elif module_name == "pip._internal.operations.install.wheel":
-            if self.loading_op_wheel:
-                return None
-            debug(f"RelenvImporter - match {module_name}")
-            self.loading_op_wheel = True
-            return self
-        elif module_name == "pip._internal.operations.install.legacy":
-            if self.loading_op_legacy:
-                return None
-            debug(f"RelenvImporter - match {module_name}")
-            self.loading_op_legacy = True
-            return self
-        return None
+        Find modules being imported.
+        """
+        for wrapper in self.wrappers:
+            if wrapper.matches(module_name) and not wrapper.loading:
+                debug(f"RelenvImporter - match {module_name}")
+                wrapper.loading = True
+                return self
 
     def load_module(self, name):
         """
-        Load the given module.
-
-        :param name: The module name to load
-        :type name: str
-        :return: The loaded module or the calling instance if importing sysconfigdata
-        :rtype: types.ModuleType or RelenvImporter
-        """
-        if name.startswith("sysconfig"):
-            debug(f"RelenvImporter - load_module {name}")
-            mod = importlib.import_module("sysconfig")
-            mod.get_config_var = get_config_var_wrapper(mod.get_config_var)
-            mod._PIP_USE_SYSCONFIG = True
-            try:
-                # Python >= 3.10
-                scheme = mod.get_default_scheme()
-            except AttributeError:
-                # Python < 3.10
-                scheme = mod._get_default_scheme()
-            mod.get_paths = get_paths_wrapper(mod.get_paths, scheme)
-            self.loading_sysconfig = False
-        elif name == "pip._vendor.distlib.scripts":
-            debug(f"RelenvImporter - load_module {name}")
-            mod = importlib.import_module(name)
-            mod.ScriptMaker._build_shebang = _build_shebang
-            self.loading_pip_scripts = False
-        elif name == "distutils.command.build_ext":
-            debug(f"RelenvImporter - load_module {name}")
-            mod = importlib.import_module(name)
-            mod.build_ext.finalize_options = finalize_options_wrapper(
-                mod.build_ext.finalize_options
-            )
-        elif name == "pip._internal.operations.install.wheel":
-            debug(f"RelenvImporter - load_module {name}")
-            mod = importlib.import_module(name)
-            mod.install_wheel = install_wheel_wrapper(mod.install_wheel)
-            self.loading_op_wheel = False
-        elif name == "pip._internal.operations.install.legacy":
-            debug(f"RelenvImporter - load_module {name}")
-            mod = importlib.import_module(name)
-            mod.install = install_legacy_wrapper(mod.install)
-            self.loading_op_legacy = False
+        Load an imported module.
+        """
+        for wrapper in self.wrappers:
+            if wrapper.matches(name):
+                debug(f"RelenvImporter - load_module {name}")
+                mod = wrapper(name)
+                wrapper.loading = False
+                break
         sys.modules[name] = mod
         return mod
 
+    def create_module(self, spec):
+        """
+        Create the module via a spec.
+        """
+        return self.load_module(spec.name)
 
-def bootstrap():
+    def exec_module(self, module):
+        """
+        Exec module noop.
+        """
+        return None
+
+
+def wrap_sysconfig(name):
     """
-    Bootstrap the relenv environment.
+    Sysconfig wrapper.
     """
-    cross = os.environ.get("RELENV_CROSS", "")
-    if cross:
-        crossroot = pathlib.Path(cross).resolve()
-        sys.prefix = str(crossroot)
-        sys.exec_prefix = str(crossroot)
-        # XXX What about dist-packages
-        pyver = f"python{sys.version_info.major}.{sys.version_info.minor}"
-        sys.path = [
-            str(crossroot / "lib" / pyver),
-            str(crossroot / "lib" / pyver / "lib-dynload"),
-            str(crossroot / "lib" / pyver / "site-packages"),
-        ] + [_ for _ in sys.path if "site-packages" not in _]
+    mod = importlib.import_module("sysconfig")
+    mod.get_config_var = get_config_var_wrapper(mod.get_config_var)
+    mod._PIP_USE_SYSCONFIG = True
+    try:
+        # Python >= 3.10
+        scheme = mod.get_default_scheme()
+    except AttributeError:
+        # Python < 3.10
+        scheme = mod._get_default_scheme()
+    mod.get_paths = get_paths_wrapper(mod.get_paths, scheme)
+    return mod
+
+
+def wrap_pip_distlib_scripts(name):
+    """
+    pip.distlib.scripts wrapper.
+    """
+    mod = importlib.import_module(name)
+    mod.ScriptMaker._build_shebang = _build_shebang
+    return mod
 
+
+def wrap_distutils_command(name):
+    """
+    distutils.command wrapper.
+    """
+    mod = importlib.import_module(name)
+    mod.build_ext.finalize_options = finalize_options_wrapper(
+        mod.build_ext.finalize_options
+    )
+    return mod
+
+
+def wrap_pip_install_wheel(name):
+    """
+    pip._internal.operations.install.wheel wrapper.
+    """
+    mod = importlib.import_module(name)
+    mod.install_wheel = install_wheel_wrapper(mod.install_wheel)
+    return mod
+
+
+def wrap_pip_install_legacy(name):
+    """
+    pip._internal.operations.install.legacy wrapper.
+    """
+    mod = importlib.import_module(name)
+    mod.install = install_legacy_wrapper(mod.install)
+    return mod
+
+
+def wrap_pip_build_wheel(name):
+    """
+    pip._internal.operations.build wrapper.
+    """
+    mod = importlib.import_module(name)
+
+    def wrap(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            dirs = work_dirs()
+            toolchain = dirs.toolchain / get_triplet()
+            cargo_home = str(toolchain / "cargo")
+            if "CARGO_HOME" in os.environ and os.environ["CARGO_HOME"] != cargo_home:
+                print(
+                    f"Warning: CARGO_HOME environment not set to relenv's toolchain!\n"
+                    f"expected: {cargo_home}\ncurrent: {os.environ['CARGO_HOME']}"
+                )
+            else:
+                print("SET CARGO HOME")
+                os.environ["CARGO_HOME"] = cargo_home
+            return func(*args, **kwargs)
+
+        return wrapper
+
+    mod.build_wheel_pep517 = wrap(mod.build_wheel_pep517)
+    return mod
+
+
+importer = RelenvImporter(
+    wrappers=[
+        Wrapper("sysconfig", wrap_sysconfig, "startswith"),
+        Wrapper("pip._vendor.distlib.scripts", wrap_pip_distlib_scripts),
+        Wrapper("distutils.command.build_ext", wrap_distutils_command),
+        Wrapper("pip._internal.operations.install.wheel", wrap_pip_install_wheel),
+        Wrapper("pip._internal.operations.install.legacy", wrap_pip_install_legacy),
+        Wrapper("pip._internal.operations.build.wheel", wrap_pip_build_wheel),
+    ],
+)
+
+
+def install_cargo_config():
+    """
+    Setup cargo config.
+    """
+    if sys.platform != "linux":
+        return
+    triplet = get_triplet()
+    dirs = work_dirs()
+    toolchain = dirs.toolchain / triplet
+    cargo_home = toolchain / "cargo"
+    if not cargo_home.exists():
+        cargo_home.mkdir()
+    cargo_config = cargo_home / "config.toml"
+    if not cargo_config.exists():
+        if triplet == "x86_64-linux-gnu":
+            cargo_triplet = "x86_64-unknown-linux-gnu"
+        else:
+            cargo_triplet = "aarch64-unknown-linux-gnu"
+        gcc = toolchain / "bin" / f"{triplet}-gcc"
+        with open(cargo_config, "w") as fp:
+            fp.write(
+                textwrap.dedent(
+                    """\
+            [target.{}]
+            linker = "{}"
+            """
+                ).format(cargo_triplet, gcc)
+            )
+
+
+def setup_openssl():
+    """
+    Configure openssl certificate locations.
+    """
     # Use system openssl dirs
     # XXX Should we also setup SSL_CERT_FILE, OPENSSL_CONF &
     # OPENSSL_CONF_INCLUDE?
     if "SSL_CERT_DIR" not in os.environ and sys.platform != "win32":
         openssl_bin = shutil.which("openssl")
         if not openssl_bin:
             debug("Could not find the 'openssl' binary in the path")
@@ -422,9 +508,35 @@
                 path = pathlib.Path(directory.strip().strip('"'))
                 if not os.environ.get("SSL_CERT_DIR"):
                     os.environ["SSL_CERT_DIR"] = str(path / "certs")
                 cert_file = path / "cert.pem"
                 if cert_file.exists() and not os.environ.get("SSL_CERT_FILE"):
                     os.environ["SSL_CERT_FILE"] = str(cert_file)
 
-    importer = RelenvImporter()
+
+def setup_crossroot():
+    """
+    Setup cross root if needed.
+    """
+    cross = os.environ.get("RELENV_CROSS", "")
+    if cross:
+        crossroot = pathlib.Path(cross).resolve()
+        sys.prefix = str(crossroot)
+        sys.exec_prefix = str(crossroot)
+        # XXX What about dist-packages
+        pyver = f"python{sys.version_info.major}.{sys.version_info.minor}"
+        sys.path = [
+            str(crossroot / "lib" / pyver),
+            str(crossroot / "lib" / pyver / "lib-dynload"),
+            str(crossroot / "lib" / pyver / "site-packages"),
+        ] + [_ for _ in sys.path if "site-packages" not in _]
+
+
+def bootstrap():
+    """
+    Bootstrap the relenv environment.
+    """
+    setup_crossroot()
+    setup_openssl()
+    install_cargo_config()
     sys.meta_path = [importer] + sys.meta_path
+    sys.RELENV = relenv_root()
```

## relenv/build/common.py

```diff
@@ -360,15 +360,15 @@
 
 def sqlite_version(href):
     if "releaselog" in href:
         link = href.split("/")[1][:-5]
         return "{:d}{:02d}{:02d}00".format(*[int(_) for _ in link.split("_")])
 
 
-def ffi_version(href):
+def github_version(href):
     if "tag/" in href:
         return href.split("/v")[-1]
 
 
 def krb_version(href):
     if re.match(r"\d\.\d\d/", href):
         return href[:-1]
@@ -933,22 +933,23 @@
 
         if sys.platform == "win32":
             env = os.environ.copy()
         else:
             env = {
                 "PATH": os.environ["PATH"],
             }
-
         env["RELENV_DEBUG"] = "1"
         env["RELENV_HOST"] = self.triplet
         env["RELENV_HOST_ARCH"] = self.arch
         env["RELENV_BUILD"] = self.build_triplet
         env["RELENV_BUILD_ARCH"] = self.build_arch
         env["RELENV_PY_VERSION"] = self.recipies["python"]["download"].version
         env["RELENV_PY_MAJOR_VERSION"] = env["RELENV_PY_VERSION"].rsplit(".", 1)[0]
+        if "RELENV_DATA" in os.environ:
+            env["RELENV_DATA"] = os.environ["RELENV_DATA"]
         if self.build_arch != self.arch:
             native_root = DATA_DIR / "native"
             env["RELENV_NATIVE_PY"] = str(native_root / "bin" / "python3")
 
         self.populate_env(env, dirs)
 
         logfp.write("*" * 80 + "\n")
```

## relenv/build/linux.py

```diff
@@ -400,14 +400,16 @@
 
 build.add(
     "libxcrypt",
     download={
         "url": "https://github.com/besser82/libxcrypt/releases/download/v{version}/libxcrypt-{version}.tar.xz",
         "version": "4.4.33",
         "md5sum": "d83b7bb334c4daf4e64a253b78f320da",
+        "checkfunc": github_version,
+        "checkurl": "https://github.com/besser82/libxcrypt/releases/",
     },
 )
 
 build.add(
     "XZ",
     download={
         "url": "http://tukaani.org/xz/xz-{version}.tar.gz",
@@ -472,15 +474,15 @@
     "libffi",
     build_libffi,
     download={
         "url": "https://github.com/libffi/libffi/releases/download/v{version}/libffi-{version}.tar.gz",
         "fallback_url": "https://woz.io/relenv/dependencies/libffi-{version}.tar.gz",
         "version": "3.4.4",
         "md5sum": "0da1a5ed7786ac12dcbaf0d499d8a049",
-        "checkfunc": ffi_version,
+        "checkfunc": github_version,
         "checkurl": "https://github.com/libffi/libffi/releases/",
     },
 )
 
 build.add(
     "zlib",
     build_zlib,
```

## Comparing `relenv-0.8.2.dist-info/LICENSE.md` & `relenv-0.9.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `relenv-0.8.2.dist-info/METADATA` & `relenv-0.9.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relenv
-Version: 0.8.2
+Version: 0.9.0
 Project-URL: Source Code, https://github.com/saltstack/relative-environment-for-python
 Project-URL: Documentation, https://relenv.readthedocs.io/en/latest/
 Project-URL: Changelog, https://relenv.readthedocs.io/en/latest/changelog.html
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: NOTICE
```

## Comparing `relenv-0.8.2.dist-info/NOTICE` & `relenv-0.9.0.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `relenv-0.8.2.dist-info/RECORD` & `relenv-0.9.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 relenv/__init__.py,sha256=128_eo7EYWjVSZqh_Artw-e8fMtzzrR3KG-DJjaz6bI,109
 relenv/__main__.py,sha256=sx2mA72sAE-_CfdHxWjBFxCELOP3QBZnK0zzPT118pE,1283
-relenv/common.py,sha256=5DIL7A-HAoe9EkUJTguznwZY9sdwXTEuhFGunnKbP8s,10338
+relenv/common.py,sha256=JH356VTmNuB4XK_piK4stw5m7T6YR8cJFQexFkNl2nA,10338
 relenv/create.py,sha256=xTqEiTKHHtzGFJ8YXgPQ3vpbddpD77VFY9fogKuh08w,3868
 relenv/fetch.py,sha256=Yznr2N-Wk-3kftGZ9s9jZNic2iquzb7-rt5RFPSBTLU,1551
 relenv/relocate.py,sha256=FAb60ypdYPlHbVZDh_hSTKJ0dXfXmV05nPfxrpZAJ9U,11432
-relenv/runtime.py,sha256=b2tXwm9k-7dgzOVmssSWvsepSDU36L5jdIHBMHywaVM,13955
+relenv/runtime.py,sha256=s8mOpE-ar9Ezd-6eSLpUxl26ArNK_KfIgpT1Qx_0L5c,15583
 relenv/toolchain.py,sha256=VHUBrUs2Adtmz3r_un-4LL0Vna_j06bCim7d-G8wXvI,5370
 relenv/build/__init__.py,sha256=cHPeCuaWfWeFPelyr4J6tPabLyAzLH38-EQX4PSE4eo,4365
-relenv/build/common.py,sha256=okfl-Yfz9wsPier9aGKhBeRLwCVfV1CFfMK2CP6DiSw,45605
+relenv/build/common.py,sha256=3lggcHa73ewxHX0q3eA-QVFRZaSRJ_VK4DjD-96Sks4,45706
 relenv/build/darwin.py,sha256=-zBk_LsE-M2mUoc3DwJ_JpUz_PRf1h6jFDlJfMiRQz4,3551
-relenv/build/linux.py,sha256=06JOrCavPL47yQyLHvikDrOcI8kAIv4niANUvr7246o,16888
+relenv/build/linux.py,sha256=39WIMnDwTTcqNm46iil1Vk60rASzN5PeUlIMed60jiA,16999
 relenv/build/windows.py,sha256=RNPvwVLwfM14ExtbCo8-SL8_clw23eR_iNVQ0YI9Dhk,5692
-relenv-0.8.2.dist-info/LICENSE.md,sha256=T0SRk3vJM1YcAJjDz9vsX9gsCRatAVSBS7LeU0tklRM,9919
-relenv-0.8.2.dist-info/METADATA,sha256=tnTktc_DpDxFwY668PEmhUv_wyJawiqz81XYKPNIXgU,1269
-relenv-0.8.2.dist-info/NOTICE,sha256=Ns0AybPHBsgJKJJfjE6YnGgWEQQ9F7lQ6QNlYLlQT3E,548
-relenv-0.8.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-relenv-0.8.2.dist-info/entry_points.txt,sha256=dO66nWPPWl8ALWWnZFlHKAo6mfPFuQid7purYWL2ddc,48
-relenv-0.8.2.dist-info/top_level.txt,sha256=J-FRR_cVeGTWXKiXQB-Hgyg4cUQfoYJw17jIb9G-ocQ,7
-relenv-0.8.2.dist-info/RECORD,,
+relenv-0.9.0.dist-info/LICENSE.md,sha256=T0SRk3vJM1YcAJjDz9vsX9gsCRatAVSBS7LeU0tklRM,9919
+relenv-0.9.0.dist-info/METADATA,sha256=wlRV89tn2sqmqCMoiNmVpNvguvbLP5WAYvdwtFNc7NQ,1269
+relenv-0.9.0.dist-info/NOTICE,sha256=Ns0AybPHBsgJKJJfjE6YnGgWEQQ9F7lQ6QNlYLlQT3E,548
+relenv-0.9.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+relenv-0.9.0.dist-info/entry_points.txt,sha256=dO66nWPPWl8ALWWnZFlHKAo6mfPFuQid7purYWL2ddc,48
+relenv-0.9.0.dist-info/top_level.txt,sha256=J-FRR_cVeGTWXKiXQB-Hgyg4cUQfoYJw17jIb9G-ocQ,7
+relenv-0.9.0.dist-info/RECORD,,
```

