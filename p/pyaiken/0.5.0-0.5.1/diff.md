# Comparing `tmp/pyaiken-0.5.0.tar.gz` & `tmp/pyaiken-0.5.1.tar.gz`

## Comparing `pyaiken-0.5.0.tar` & `pyaiken-0.5.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0      402 1970-01-01 00:00:00.000000 pyaiken-0.5.0/Cargo.toml
--rw-r--r--   0     1001      123      329 2023-04-26 07:33:32.000000 pyaiken-0.5.0/.ci/deploy_to_pypi.sh
--rw-r--r--   0     1001      123     1506 2023-04-26 07:33:32.000000 pyaiken-0.5.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      123     6782 2023-04-26 07:33:32.000000 pyaiken-0.5.0/.gitignore
--rw-r--r--   0     1001      123      527 2023-04-26 07:33:32.000000 pyaiken-0.5.0/.travis.yml
--rw-r--r--   0     1001      123     1053 2023-04-26 07:33:32.000000 pyaiken-0.5.0/LICENSE.txt
--rw-r--r--   0     1001      123     2049 2023-04-26 07:33:32.000000 pyaiken-0.5.0/README.md
--rw-r--r--   0     1001      123      894 2023-04-26 07:33:32.000000 pyaiken-0.5.0/pyproject.toml
--rwxr-xr-x   0     1001      123      833 2023-04-26 07:34:01.000000 pyaiken-0.5.0/run-maturin-action.sh
--rw-r--r--   0     1001      123     3689 2023-04-26 07:33:32.000000 pyaiken-0.5.0/src/lib.rs
--rw-r--r--   0        0        0    30683 2023-04-26 07:35:09.000000 pyaiken-0.5.0/Cargo.lock
--rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 pyaiken-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 pyaiken-0.5.1/Cargo.toml
+-rw-r--r--   0     1001      123      329 2023-05-03 07:12:30.000000 pyaiken-0.5.1/.ci/deploy_to_pypi.sh
+-rw-r--r--   0     1001      123      330 2023-05-03 07:12:30.000000 pyaiken-0.5.1/.github/release.yml
+-rw-r--r--   0     1001      123     1788 2023-05-03 07:12:30.000000 pyaiken-0.5.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      493 2023-05-03 07:12:30.000000 pyaiken-0.5.1/.github/workflows/python.yml
+-rw-r--r--   0     1001      123     6782 2023-05-03 07:12:30.000000 pyaiken-0.5.1/.gitignore
+-rw-r--r--   0     1001      123      516 2023-05-03 07:12:30.000000 pyaiken-0.5.1/.travis.yml
+-rw-r--r--   0     1001      123     1053 2023-05-03 07:12:30.000000 pyaiken-0.5.1/LICENSE.txt
+-rw-r--r--   0     1001      123     2049 2023-05-03 07:12:30.000000 pyaiken-0.5.1/README.md
+-rw-r--r--   0     1001      123      894 2023-05-03 07:12:30.000000 pyaiken-0.5.1/pyproject.toml
+-rwxr-xr-x   0     1001      123      833 2023-05-03 07:13:06.000000 pyaiken-0.5.1/run-maturin-action.sh
+-rw-r--r--   0     1001      123     3689 2023-05-03 07:12:30.000000 pyaiken-0.5.1/src/lib.rs
+-rw-r--r--   0        0        0    30683 2023-05-03 07:14:34.000000 pyaiken-0.5.1/Cargo.lock
+-rw-r--r--   0        0        0     2827 1970-01-01 00:00:00.000000 pyaiken-0.5.1/PKG-INFO
```

### Comparing `pyaiken-0.5.0/.github/workflows/CI.yml` & `pyaiken-0.5.1/.github/workflows/CI.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 name: CI
 
 on:
   push:
     branches:
       - main
       - master
+    tags:
+      - "*.*.*"
   pull_request:
   workflow_dispatch:
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     steps:
@@ -47,23 +49,29 @@
         command: build
         args: --release -o dist --universal2 --find-interpreter
     - name: Upload wheels
       uses: actions/upload-artifact@v3
       with:
         name: wheels
         path: dist
-
   release:
     name: Release
     runs-on: ubuntu-latest
     needs: [ macos, windows, linux ]
+    if: github.ref_type == 'tag'
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
           command: upload
-          args: --skip-existing *
+          args: --skip-existing *
+      # If there isn't a release for this version, create a new one.
+      - uses: ncipollo/release-action@v1
+        with:
+          generateReleaseNotes: true
+          makeLatest: true
+          skipIfReleaseExists: true
```

### Comparing `pyaiken-0.5.0/.gitignore` & `pyaiken-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyaiken-0.5.0/.travis.yml` & `pyaiken-0.5.1/.travis.yml`

 * *Files 22% similar despite different names*

```diff
@@ -25,9 +25,9 @@
 script:
  - maturin build
 
 deploy:
   provider: script
   script: bash .ci/deploy_to_pypi.sh
   on:
-    branch: master
-    repo: ImperatorLang/pyaiken
+    tags: true
+    repo: OpShin/pyaiken
```

### Comparing `pyaiken-0.5.0/LICENSE.txt` & `pyaiken-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyaiken-0.5.0/README.md` & `pyaiken-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pyaiken-0.5.0/pyproject.toml` & `pyaiken-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyaiken-0.5.0/run-maturin-action.sh` & `pyaiken-0.5.1/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `pyaiken-0.5.0/src/lib.rs` & `pyaiken-0.5.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyaiken-0.5.0/Cargo.lock` & `pyaiken-0.5.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arrayvec"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23b62fc65de8e4e7f52534fb52b0f3ed04746ae267519eef2a83941e8085068b"
 
@@ -282,17 +282,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.3.4"
+version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
+checksum = "b64f40e5e03e0d54f03845c8197d0291253cdbedfb1cb46b13c2c117554a9f4c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -596,15 +596,15 @@
 checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyaiken"
-version = "0.5.0"
+version = "0.5.1"
 dependencies = [
  "hex",
  "miette",
  "pyo3",
  "uplc",
 ]
 
@@ -713,17 +713,17 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustix"
-version = "0.37.15"
+version = "0.37.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0661814f891c57c930a610266415528da53c4933e6dea5fb350cbfe048a9ece"
+checksum = "8bbfc1d1c7c40c01715f47d71444744a81669ca84e8b63e25a55e169b1f86433"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys 0.48.0",
```

### Comparing `pyaiken-0.5.0/PKG-INFO` & `pyaiken-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaiken
-Version: 0.5.0
+Version: 0.5.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

