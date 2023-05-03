# Comparing `tmp/pyscemu-0.1.8.tar.gz` & `tmp/pyscemu-0.1.9.tar.gz`

## Comparing `pyscemu-0.1.8.tar` & `pyscemu-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.8/Cargo.toml
--rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.8/.github/workflows/CI.yml
--rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.8/.gitignore
--rw-r--r--   0     1000     1000    11671 2023-05-01 10:48:40.000000 pyscemu-0.1.8/DOCUMENTATION.md
--rw-r--r--   0     1000     1000    10073 2023-05-01 10:57:14.000000 pyscemu-0.1.8/README.md
--rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.1.8/examples/danabot_rsa.ipynb
--rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.1.8/examples/raccoon_strings.ipynb
--rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.1.8/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
--rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.1.8/examples/scripts/raccoon_strings.py
--rw-r--r--   0     1000     1000      755 2023-04-30 17:09:34.000000 pyscemu-0.1.8/examples/scripts/test.py
--rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.8/examples/scripts/xloader_dexor.py
--rw-r--r--   0     1000     1000      427 2023-05-01 14:50:10.000000 pyscemu-0.1.8/examples/scripts/xloader_keygen.py
--rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.1.8/examples/xloader_keygen.ipynb
--rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.1.8/pyproject.toml
--rw-r--r--   0     1000     1000    26607 2023-05-01 10:48:57.000000 pyscemu-0.1.8/src/lib.rs
--rw-r--r--   0     1000     1000    32749 2023-05-02 14:50:06.000000 pyscemu-0.1.8/Cargo.lock
--rw-r--r--   0        0        0    10399 1970-01-01 00:00:00.000000 pyscemu-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 pyscemu-0.1.9/Cargo.toml
+-rw-r--r--   0     1000     1000     2809 2023-04-28 16:18:25.000000 pyscemu-0.1.9/.github/workflows/CI.yml
+-rw-r--r--   0     1000     1000      692 2023-04-29 18:18:29.000000 pyscemu-0.1.9/.gitignore
+-rw-r--r--   0     1000     1000    11671 2023-05-01 10:48:40.000000 pyscemu-0.1.9/DOCUMENTATION.md
+-rw-r--r--   0     1000     1000    10073 2023-05-01 10:57:14.000000 pyscemu-0.1.9/README.md
+-rw-r--r--   0     1000     1000     2017 2023-04-30 22:51:14.000000 pyscemu-0.1.9/examples/danabot_rsa.ipynb
+-rw-r--r--   0     1000     1000     6831 2023-04-30 22:52:26.000000 pyscemu-0.1.9/examples/raccoon_strings.ipynb
+-rw-r--r--   0     1000     1000        0 2023-04-30 16:12:18.000000 pyscemu-0.1.9/examples/scripts/.ipynb_checkpoints/test-checkpoint.py
+-rw-r--r--   0     1000     1000      727 2023-04-30 13:08:15.000000 pyscemu-0.1.9/examples/scripts/raccoon_strings.py
+-rw-r--r--   0     1000     1000      755 2023-04-30 17:09:34.000000 pyscemu-0.1.9/examples/scripts/test.py
+-rw-r--r--   0     1000     1000      561 2023-04-29 17:52:46.000000 pyscemu-0.1.9/examples/scripts/xloader_dexor.py
+-rw-r--r--   0     1000     1000      427 2023-05-01 14:50:10.000000 pyscemu-0.1.9/examples/scripts/xloader_keygen.py
+-rw-r--r--   0     1000     1000     1757 2023-04-30 15:03:12.000000 pyscemu-0.1.9/examples/xloader_keygen.ipynb
+-rw-r--r--   0     1000     1000      433 2023-05-01 11:01:29.000000 pyscemu-0.1.9/pyproject.toml
+-rw-r--r--   0     1000     1000    26607 2023-05-01 10:48:57.000000 pyscemu-0.1.9/src/lib.rs
+-rw-r--r--   0     1000     1000    32749 2023-05-02 20:40:19.000000 pyscemu-0.1.9/Cargo.lock
+-rw-r--r--   0        0        0    10399 1970-01-01 00:00:00.000000 pyscemu-0.1.9/PKG-INFO
```

### Comparing `pyscemu-0.1.8/.github/workflows/CI.yml` & `pyscemu-0.1.9/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/.gitignore` & `pyscemu-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/DOCUMENTATION.md` & `pyscemu-0.1.9/DOCUMENTATION.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/README.md` & `pyscemu-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/examples/danabot_rsa.ipynb` & `pyscemu-0.1.9/examples/danabot_rsa.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/examples/raccoon_strings.ipynb` & `pyscemu-0.1.9/examples/raccoon_strings.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/examples/scripts/raccoon_strings.py` & `pyscemu-0.1.9/examples/scripts/raccoon_strings.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/examples/scripts/test.py` & `pyscemu-0.1.9/examples/scripts/test.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/examples/scripts/xloader_dexor.py` & `pyscemu-0.1.9/examples/scripts/xloader_dexor.py`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/examples/xloader_keygen.ipynb` & `pyscemu-0.1.9/examples/xloader_keygen.ipynb`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/src/lib.rs` & `pyscemu-0.1.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyscemu-0.1.8/Cargo.lock` & `pyscemu-0.1.9/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -394,17 +394,17 @@
 name = "libc"
 version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libscemu"
-version = "0.11.8"
+version = "0.11.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69b6a7b3425adce0f6b153904721009046d805ff447783c2dd2e00b03ac6afc9"
+checksum = "0430b60f3b7ee3bb62a523ee3546bb6c582d05b2dd69f67571099bdb7925699f"
 dependencies = [
  "attohttpc",
  "atty",
  "chrono",
  "ctrlc",
  "iced-x86",
  "lazy_static",
@@ -684,15 +684,15 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyscemu"
-version = "0.1.8"
+version = "0.1.9"
 dependencies = [
  "libscemu",
  "pyo3",
 ]
 
 [[package]]
 name = "quote"
```

### Comparing `pyscemu-0.1.8/PKG-INFO` & `pyscemu-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscemu
-Version: 0.1.8
+Version: 0.1.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PYSCEMU
```

