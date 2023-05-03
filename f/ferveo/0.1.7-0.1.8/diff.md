# Comparing `tmp/ferveo-0.1.7.tar.gz` & `tmp/ferveo-0.1.8.tar.gz`

## Comparing `ferveo-0.1.7.tar` & `ferveo-0.1.8.tar`

### file list

```diff
@@ -1,58 +1,57 @@
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 ferveo-0.1.7/local_dependencies/ferveo/Cargo.toml
--rw-rw-r--   0     1000     1000    51910 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/Cargo.lock
--rw-rw-r--   0     1000     1000      111 2023-04-05 16:16:20.000000 ferveo-0.1.7/local_dependencies/ferveo/README.md
--rw-rw-r--   0     1000     1000      214 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/bench_main.rs
--rw-rw-r--   0     1000     1000     3863 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs
--rw-rw-r--   0     1000     1000       71 2023-04-05 16:15:54.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/mod.rs
--rw-rw-r--   0     1000     1000    11868 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/pairing.rs
--rw-rw-r--   0     1000     1000     3516 2023-04-12 12:02:25.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs
--rw-rw-r--   0     1000     1000     3207 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs
--rw-rw-r--   0     1000     1000     4131 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/examples/bench_primitives_size.rs
--rw-rw-r--   0     1000     1000     2326 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/examples/pvdkg.rs
--rw-rw-r--   0     1000     1000    12719 2023-04-14 14:00:32.000000 ferveo-0.1.7/local_dependencies/ferveo/src/api.rs
--rw-rw-r--   0     1000     1000      410 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/src/dkg/common.rs
--rw-rw-r--   0     1000     1000    23980 2023-04-14 08:59:50.000000 ferveo-0.1.7/local_dependencies/ferveo/src/dkg/pv.rs
--rw-rw-r--   0     1000     1000      547 2023-04-13 21:16:41.000000 ferveo-0.1.7/local_dependencies/ferveo/src/dkg.rs
--rw-rw-r--   0     1000     1000    16674 2023-04-14 16:12:38.000000 ferveo-0.1.7/local_dependencies/ferveo/src/lib.rs
--rw-rw-r--   0     1000     1000      560 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/src/primitives.rs
--rw-rw-r--   0     1000     1000    18984 2023-04-14 11:01:01.000000 ferveo-0.1.7/local_dependencies/ferveo/src/vss/pvss.rs
--rw-rw-r--   0     1000     1000      558 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/ferveo/src/vss.rs
--rw-r--r--   0        0        0      356 1970-01-01 00:00:00.000000 ferveo-0.1.7/local_dependencies/ferveo-common/Cargo.toml
--rw-rw-r--   0     1000     1000     2469 2023-04-14 08:59:50.000000 ferveo-0.1.7/local_dependencies/ferveo-common/src/keypair.rs
--rw-rw-r--   0     1000     1000      831 2023-04-06 21:18:33.000000 ferveo-0.1.7/local_dependencies/ferveo-common/src/lib.rs
--rw-rw-r--   0     1000     1000     4008 2023-04-06 21:18:33.000000 ferveo-0.1.7/local_dependencies/ferveo-common/src/serialization.rs
--rw-rw-r--   0     1000     1000       74 2023-04-06 21:18:33.000000 ferveo-0.1.7/local_dependencies/ferveo-common/src/utils.rs
--rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/Cargo.toml
--rw-rw-r--   0     1000     1000     5872 2023-01-19 15:29:04.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/BENCHMARK.md
--rw-rw-r--   0     1000     1000      470 2023-04-05 16:16:20.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/README.md
--rw-rw-r--   0     1000     1000     9295 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/benches/arkworks.rs
--rw-rw-r--   0     1000     1000    19197 2023-04-14 11:01:02.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/benches/tpke.rs
--rw-rw-r--   0     1000     1000     1255 2023-04-14 13:31:54.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/api.rs
--rw-rw-r--   0     1000     1000     7788 2023-04-14 09:08:00.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/ciphertext.rs
--rw-rw-r--   0     1000     1000     5498 2023-04-14 11:01:02.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/combine.rs
--rw-rw-r--   0     1000     1000     3453 2023-04-14 11:01:02.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/context.rs
--rw-rw-r--   0     1000     1000    11743 2023-04-14 10:33:06.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/decryption.rs
--rw-rw-r--   0     1000     1000     4254 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs
--rw-rw-r--   0     1000     1000     2179 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/key_share.rs
--rw-rw-r--   0     1000     1000    29218 2023-04-14 16:18:03.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/lib.rs
--rw-rw-r--   0     1000     1000     3487 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/refresh.rs
--rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 ferveo-0.1.7/local_dependencies/subproductdomain/Cargo.toml
--rw-rw-r--   0     1000     1000    16742 2023-04-06 21:18:34.000000 ferveo-0.1.7/local_dependencies/subproductdomain/src/lib.rs
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 ferveo-0.1.7/Cargo.toml
--rw-rw-r--   0     1000     1000       54 2023-04-06 21:18:33.000000 ferveo-0.1.7/.gitignore
--rwxrwxr-x   0     1000     1000    34916 2023-04-06 21:18:33.000000 ferveo-0.1.7/LICENSE
--rw-rw-r--   0     1000     1000       77 2023-04-06 21:18:33.000000 ferveo-0.1.7/MANIFEST.in
--rw-rw-r--   0     1000     1000      161 2023-04-06 21:18:33.000000 ferveo-0.1.7/README.md
--rw-rw-r--   0     1000     1000       71 2023-04-06 21:18:33.000000 ferveo-0.1.7/build.rs
--rw-rw-r--   0     1000     1000     3481 2023-04-14 14:02:04.000000 ferveo-0.1.7/examples/server_api_precomputed.py
--rw-rw-r--   0     1000     1000     3392 2023-04-14 14:02:04.000000 ferveo-0.1.7/examples/server_api_simple.py
--rw-rw-r--   0     1000     1000      410 2023-04-14 14:43:54.000000 ferveo-0.1.7/ferveo/__init__.py
--rw-rw-r--   0     1000     1000     3787 2023-04-14 13:53:26.000000 ferveo-0.1.7/ferveo/__init__.pyi
--rw-rw-r--   0     1000     1000        0 2023-04-06 21:18:33.000000 ferveo-0.1.7/ferveo/py.typed
--rw-rw-r--   0     1000     1000      316 2023-04-14 08:59:50.000000 ferveo-0.1.7/pyproject.toml
--rw-rw-r--   0     1000     1000     1444 2023-04-14 16:19:01.000000 ferveo-0.1.7/setup.py
--rw-rw-r--   0     1000     1000    11220 2023-04-14 13:37:22.000000 ferveo-0.1.7/src/lib.rs
--rw-rw-r--   0     1000     1000     3554 2023-04-14 15:26:28.000000 ferveo-0.1.7/test/test_ferveo.py
--rw-rw-r--   0     1000     1000     1514 2023-04-14 15:12:10.000000 ferveo-0.1.7/test/test_serialization.py
--rw-rw-r--   0     1000     1000    56115 2023-04-14 16:19:10.000000 ferveo-0.1.7/Cargo.lock
--rw-r--r--   0        0        0      610 1970-01-01 00:00:00.000000 ferveo-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      231 1970-01-01 00:00:00.000000 ferveo-0.1.8/local_dependencies/subproductdomain/Cargo.toml
+-rw-rw-r--   0     1000     1000    16742 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/subproductdomain/src/lib.rs
+-rw-r--r--   0        0        0     1073 1970-01-01 00:00:00.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/Cargo.toml
+-rw-rw-r--   0     1000     1000     5872 2023-01-19 15:29:04.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/BENCHMARK.md
+-rw-rw-r--   0     1000     1000      470 2023-04-05 16:16:20.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/README.md
+-rw-rw-r--   0     1000     1000     9295 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/benches/arkworks.rs
+-rw-rw-r--   0     1000     1000    19154 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/benches/tpke.rs
+-rw-rw-r--   0     1000     1000     1259 2023-04-25 07:31:20.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/api.rs
+-rw-rw-r--   0     1000     1000     7780 2023-04-28 12:33:25.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/ciphertext.rs
+-rw-rw-r--   0     1000     1000     5498 2023-04-26 08:55:27.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/combine.rs
+-rw-rw-r--   0     1000     1000     3429 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/context.rs
+-rw-rw-r--   0     1000     1000    11504 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/decryption.rs
+-rw-rw-r--   0     1000     1000     4254 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs
+-rw-rw-r--   0     1000     1000     2183 2023-04-25 07:31:20.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/key_share.rs
+-rw-rw-r--   0     1000     1000    28735 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/lib.rs
+-rw-rw-r--   0     1000     1000     3487 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/refresh.rs
+-rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 ferveo-0.1.8/local_dependencies/ferveo/Cargo.toml
+-rw-rw-r--   0     1000     1000    51910 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/Cargo.lock
+-rw-rw-r--   0     1000     1000      111 2023-04-05 16:16:20.000000 ferveo-0.1.8/local_dependencies/ferveo/README.md
+-rw-rw-r--   0     1000     1000      214 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/bench_main.rs
+-rw-rw-r--   0     1000     1000     3863 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs
+-rw-rw-r--   0     1000     1000       71 2023-04-05 16:15:54.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/mod.rs
+-rw-rw-r--   0     1000     1000    11868 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/pairing.rs
+-rw-rw-r--   0     1000     1000     3478 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs
+-rw-rw-r--   0     1000     1000     3257 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs
+-rw-rw-r--   0     1000     1000     2897 2023-04-25 07:31:20.000000 ferveo-0.1.8/local_dependencies/ferveo/examples/bench_ark_sizes.rs
+-rw-rw-r--   0     1000     1000     4336 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/examples/bench_primitives_size.rs
+-rw-rw-r--   0     1000     1000    18555 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/api.rs
+-rw-rw-r--   0     1000     1000    24426 2023-04-26 12:06:08.000000 ferveo-0.1.8/local_dependencies/ferveo/src/dkg/pv.rs
+-rw-rw-r--   0     1000     1000    24978 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/dkg.rs
+-rw-rw-r--   0     1000     1000    17470 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/lib.rs
+-rw-rw-r--   0     1000     1000      560 2023-04-06 21:18:34.000000 ferveo-0.1.8/local_dependencies/ferveo/src/primitives.rs
+-rw-rw-r--   0     1000     1000    21326 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/pvss.rs
+-rw-rw-r--   0     1000     1000     1976 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo/src/validator.rs
+-rw-r--r--   0        0        0      358 1970-01-01 00:00:00.000000 ferveo-0.1.8/local_dependencies/ferveo-common/Cargo.toml
+-rw-rw-r--   0     1000     1000     6907 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo-common/src/keypair.rs
+-rw-rw-r--   0     1000     1000      120 2023-05-03 13:21:11.000000 ferveo-0.1.8/local_dependencies/ferveo-common/src/lib.rs
+-rw-rw-r--   0     1000     1000     4000 2023-04-26 12:06:08.000000 ferveo-0.1.8/local_dependencies/ferveo-common/src/serialization.rs
+-rw-rw-r--   0     1000     1000      406 2023-04-25 07:31:20.000000 ferveo-0.1.8/local_dependencies/ferveo-common/src/utils.rs
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 ferveo-0.1.8/Cargo.toml
+-rw-rw-r--   0     1000     1000       54 2023-04-06 21:18:33.000000 ferveo-0.1.8/.gitignore
+-rwxrwxr-x   0     1000     1000    34916 2023-04-06 21:18:33.000000 ferveo-0.1.8/LICENSE
+-rw-rw-r--   0     1000     1000       77 2023-04-06 21:18:33.000000 ferveo-0.1.8/MANIFEST.in
+-rw-rw-r--   0     1000     1000      226 2023-05-03 13:35:12.000000 ferveo-0.1.8/README.md
+-rw-rw-r--   0     1000     1000       71 2023-04-06 21:18:33.000000 ferveo-0.1.8/build.rs
+-rw-rw-r--   0     1000     1000     3007 2023-05-03 13:21:11.000000 ferveo-0.1.8/examples/server_api_precomputed.py
+-rw-rw-r--   0     1000     1000     3128 2023-05-03 13:21:11.000000 ferveo-0.1.8/examples/server_api_simple.py
+-rw-rw-r--   0     1000     1000      383 2023-04-26 12:06:08.000000 ferveo-0.1.8/ferveo/__init__.py
+-rw-rw-r--   0     1000     1000     3691 2023-04-26 12:06:08.000000 ferveo-0.1.8/ferveo/__init__.pyi
+-rw-rw-r--   0     1000     1000        0 2023-04-06 21:18:33.000000 ferveo-0.1.8/ferveo/py.typed
+-rw-rw-r--   0     1000     1000      316 2023-04-14 08:59:50.000000 ferveo-0.1.8/pyproject.toml
+-rw-rw-r--   0     1000     1000     1444 2023-05-03 13:28:52.000000 ferveo-0.1.8/setup.py
+-rw-rw-r--   0     1000     1000    20357 2023-05-03 13:21:11.000000 ferveo-0.1.8/src/lib.rs
+-rw-rw-r--   0     1000     1000     3494 2023-05-03 13:21:11.000000 ferveo-0.1.8/test/test_ferveo.py
+-rw-rw-r--   0     1000     1000     1507 2023-05-03 13:21:11.000000 ferveo-0.1.8/test/test_serialization.py
+-rw-rw-r--   0     1000     1000    55603 2023-05-03 13:29:17.000000 ferveo-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 ferveo-0.1.8/PKG-INFO
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/Cargo.toml` & `ferveo-0.1.8/local_dependencies/ferveo/Cargo.toml`

 * *Files 26% similar despite different names*

```diff
@@ -7,46 +7,46 @@
 readme = "README.md"
 description = "An implementation of a DKG protocol for front-running protection on public blockchains."
 keywords = ["DKG"]
 categories = ["cryptography"]
 authors = ["Heliax AG <hello@heliax.dev>"]
 
 [dependencies]
-group-threshold-cryptography = { path = "../group-threshold-cryptography", features = ["api"] }
-ferveo-common = { path = "../ferveo-common" }
-subproductdomain = { path = "../subproductdomain" }
-ark-std = "0.4"
 ark-bls12-381 = "0.4"
 ark-ec = "0.4"
 ark-ff = "0.4"
 ark-poly = "0.4"
 ark-serialize = "0.4"
-rand = "0.8"
-rand_old = { package = "rand", version = "0.7" } # used by benchmarks/pairing.rs
-serde = { version = "1.0", features = ["derive"] }
+ark-std = "0.4"
 bincode = "1.3"
-itertools = "0.10.1"
+ferveo-common = { path = "../ferveo-common" }
+group-threshold-cryptography = { path = "../group-threshold-cryptography", features = ["api"] }
+hex = "0.4.3"
+itertools = "0.10.5"
 measure_time = "0.8"
+rand = "0.8"
 rand_core = "0.6.4"
-serde_with = "2.0.1"
+rand_old = { package = "rand", version = "0.7" } # used by benchmarks/pairing.rs
+serde = { version = "1.0", features = ["derive"] }
+serde_with = "2.2.0"
+subproductdomain = { path = "../subproductdomain" }
 thiserror = "1.0"
 
 [package.metadata.cargo-machete]
 ignored = ["ark-serialize"]
 
 [lib]
 bench = false
 
 [features]
 test-common = []
 
 [[example]]
-name = "pvdkg"
-path = "examples/pvdkg.rs"
-
+name = "bench_primitives_size"
+path = "examples/bench_primitives_size.rs"
 #[[bench]]
 #name = "pvdkg"
 #path = "benches/benchmarks/pvdkg.rs"
 #harness = false
 
 [[bench]]
 name = "benchmarks"
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/Cargo.lock` & `ferveo-0.1.8/local_dependencies/ferveo/Cargo.lock`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs` & `ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/block_proposer.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/pairing.rs` & `ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/pairing.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs` & `ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/pvdkg.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 pub use ark_bls12_381::Bls12_381 as EllipticCurve;
 use criterion::{criterion_group, criterion_main, Criterion};
-use ferveo_common::ExternalValidator;
 use pprof::criterion::{Output, PProfProfiler};
 
 use ferveo::*;
 
 pub fn dkgs(c: &mut Criterion) {
     use rand::SeedableRng;
     let _rng = rand::rngs::StdRng::seed_from_u64(0);
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs` & `ferveo-0.1.8/local_dependencies/ferveo/benches/benchmarks/validity_checks.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 #![allow(clippy::redundant_closure)]
 #![allow(clippy::unit_arg)]
 
+use std::str::FromStr;
+
 use ark_bls12_381::Bls12_381;
 pub use ark_bls12_381::Bls12_381 as EllipticCurve;
 use criterion::{black_box, criterion_group, BenchmarkId, Criterion};
 use digest::crypto_common::rand_core::SeedableRng;
 use ferveo::*;
-use ferveo_common::ExternalValidator;
 use rand::prelude::StdRng;
 
 const NUM_SHARES_CASES: [usize; 5] = [4, 8, 16, 32, 64];
 
 // TODO: Can we expose ferveo test methods to reuse `setup_dkg` et al instead of reimplementing it here?
 
 fn gen_keypairs(num: u32) -> Vec<ferveo_common::Keypair<EllipticCurve>> {
     let rng = &mut ark_std::test_rng();
     (0..num)
         .map(|_| ferveo_common::Keypair::<EllipticCurve>::new(rng))
         .collect()
 }
 
+pub fn gen_address(i: usize) -> EthereumAddress {
+    EthereumAddress::from_str(&format!("0x{:040}", i)).unwrap()
+}
+
 fn gen_validators(
     keypairs: &[ferveo_common::Keypair<EllipticCurve>],
-) -> Vec<ExternalValidator<EllipticCurve>> {
+) -> Vec<Validator<EllipticCurve>> {
     (0..keypairs.len())
-        .map(|i| ExternalValidator {
-            address: format!("validator_{}", i),
+        .map(|i| Validator {
+            address: gen_address(i),
             public_key: keypairs[i].public(),
         })
         .collect()
 }
 
 fn setup_dkg(
     validator: usize,
     shares_num: u32,
 ) -> PubliclyVerifiableDkg<EllipticCurve> {
     let keypairs = gen_keypairs(shares_num);
     let validators = gen_validators(&keypairs);
     let me = validators[validator].clone();
     PubliclyVerifiableDkg::new(
         &validators,
-        Params {
+        &DkgParams {
             tau: 0,
             security_threshold: shares_num / 3,
             shares_num,
         },
         &me,
-        keypairs[validator],
     )
     .expect("Setup failed")
 }
 
 fn setup(
     shares_num: u32,
     rng: &mut StdRng,
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/examples/bench_primitives_size.rs` & `ferveo-0.1.8/local_dependencies/ferveo/examples/bench_primitives_size.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 use std::{
     collections::BTreeSet,
     fs::{create_dir_all, OpenOptions},
     io::prelude::*,
     path::PathBuf,
+    str::FromStr,
 };
 
 use ark_bls12_381::Bls12_381 as EllipticCurve;
 use ferveo::*;
-use ferveo_common::ExternalValidator;
 use itertools::iproduct;
 use rand::prelude::StdRng;
 use rand_core::SeedableRng;
 
 const OUTPUT_DIR_PATH: &str = "/tmp/benchmark_setup";
 const OUTPUT_FILE_NAME: &str = "results.md";
 
@@ -55,20 +55,24 @@
 fn gen_keypairs(num: u32) -> Vec<ferveo_common::Keypair<EllipticCurve>> {
     let rng = &mut ark_std::test_rng();
     (0..num)
         .map(|_| ferveo_common::Keypair::<EllipticCurve>::new(rng))
         .collect()
 }
 
+pub fn gen_address(i: usize) -> EthereumAddress {
+    EthereumAddress::from_str(&format!("0x{:040}", i)).unwrap()
+}
+
 fn gen_validators(
     keypairs: &[ferveo_common::Keypair<EllipticCurve>],
-) -> Vec<ExternalValidator<EllipticCurve>> {
+) -> Vec<Validator<EllipticCurve>> {
     (0..keypairs.len())
-        .map(|i| ExternalValidator {
-            address: format!("validator_{}", i),
+        .map(|i| Validator {
+            address: gen_address(i),
             public_key: keypairs[i].public(),
         })
         .collect()
 }
 
 fn setup_dkg(
     validator: usize,
@@ -76,39 +80,40 @@
     security_threshold: u32,
 ) -> PubliclyVerifiableDkg<EllipticCurve> {
     let keypairs = gen_keypairs(shares_num);
     let validators = gen_validators(&keypairs);
     let me = validators[validator].clone();
     PubliclyVerifiableDkg::new(
         &validators,
-        Params {
+        &DkgParams {
             tau: 0,
             security_threshold,
             shares_num,
         },
         &me,
-        keypairs[validator],
     )
     .expect("Setup failed")
 }
 
 fn setup(
     shares_num: u32,
     security_threshold: u32,
     rng: &mut StdRng,
 ) -> PubliclyVerifiableDkg<EllipticCurve> {
     let mut transcripts = vec![];
     for i in 0..shares_num {
         let mut dkg = setup_dkg(i as usize, shares_num, security_threshold);
-        transcripts.push(dkg.share(rng).expect("Test failed"));
+        let message = dkg.share(rng).expect("Test failed");
+        let sender = dkg.get_validator(&dkg.me.validator.public_key).unwrap();
+        transcripts.push((sender.clone(), message.clone()));
     }
 
     let mut dkg = setup_dkg(0, shares_num, security_threshold);
-    for (sender, pvss) in transcripts.into_iter().enumerate() {
-        dkg.apply_message(dkg.validators[sender].validator.clone(), pvss)
+    for (sender, pvss) in transcripts.into_iter() {
+        dkg.apply_message(&sender.validator, &pvss)
             .expect("Setup failed");
     }
     dkg
 }
 
 fn main() {
     let rng = &mut StdRng::seed_from_u64(0);
@@ -128,15 +133,16 @@
         .collect::<BTreeSet<_>>();
 
     println!("Running benchmarks for {:?}", configs);
 
     for (shares_num, threshold) in configs {
         println!("shares_num: {}, threshold: {}", shares_num, threshold);
         let dkg = setup(*shares_num as u32, threshold, rng);
-        let transcript_bytes = bincode::serialize(&dkg.vss[&0]).unwrap();
+        let transcript = &dkg.vss.values().next().unwrap();
+        let transcript_bytes = bincode::serialize(&transcript).unwrap();
 
         save_data(
             *shares_num as usize,
             threshold as usize,
             transcript_bytes.len(),
         );
     }
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/src/api.rs` & `ferveo-0.1.8/local_dependencies/ferveo/src/api.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,147 +1,206 @@
-use ark_poly::EvaluationDomain;
+use std::io;
+
+use ark_poly::{EvaluationDomain, Radix2EvaluationDomain};
 use ark_serialize::{CanonicalDeserialize, CanonicalSerialize};
+use bincode;
 use ferveo_common::serialization;
-pub use ferveo_common::{ExternalValidator, Keypair, PublicKey};
+pub use ferveo_common::{Keypair, PublicKey};
 use group_threshold_cryptography as tpke;
 use rand::RngCore;
 use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 pub use tpke::api::{
     decrypt_with_shared_secret, encrypt, prepare_combine_simple,
     share_combine_precomputed, share_combine_simple, Ciphertext,
     DecryptionSharePrecomputed, DecryptionShareSimple, DomainPoint, Fr,
     G1Affine, G1Prepared, SharedSecret, E,
 };
 
-pub use crate::{PubliclyVerifiableSS as Transcript, Result};
+use crate::{do_verify_aggregation, PVSSMap, Result};
+pub use crate::{
+    EthereumAddress, PubliclyVerifiableSS as Transcript, Validator,
+};
+
+// Normally, we would use a custom trait for this, but we can't because
+// the arkworks will not let us create a blanket implementation for G1Affine
+// and Fr types. So instead, we're using this shared utility function:
+pub fn to_bytes<T: CanonicalSerialize>(item: &T) -> Result<Vec<u8>> {
+    let mut writer = Vec::new();
+    item.serialize_compressed(&mut writer)?;
+    Ok(writer)
+}
+
+pub fn from_bytes<T: CanonicalDeserialize>(bytes: &[u8]) -> Result<T> {
+    let mut reader = io::Cursor::new(bytes);
+    let item = T::deserialize_compressed(&mut reader)?;
+    Ok(item)
+}
 
 #[serde_as]
 #[derive(Copy, Clone, Debug, PartialEq, Serialize, Deserialize)]
 pub struct DkgPublicKey(
     #[serde_as(as = "serialization::SerdeAs")] pub G1Affine,
 );
 
 impl DkgPublicKey {
     pub fn to_bytes(&self) -> Result<Vec<u8>> {
-        let mut writer = Vec::new();
-        self.0.serialize_uncompressed(&mut writer)?;
-        Ok(writer)
+        to_bytes(&self.0)
     }
 
     pub fn from_bytes(bytes: &[u8]) -> Result<DkgPublicKey> {
-        let mut reader = bytes;
-        let pk = G1Affine::deserialize_uncompressed(&mut reader)?;
-        Ok(Self(pk))
+        from_bytes(bytes).map(DkgPublicKey)
+    }
+
+    pub fn serialized_size() -> usize {
+        48
     }
 }
 
-pub type LagrangeCoefficient = FieldPoint;
 pub type UnblindingKey = FieldPoint;
 
 #[serde_as]
-#[derive(Copy, Clone, Debug, PartialEq, Serialize, Deserialize)]
+#[derive(Copy, Clone, Debug, PartialEq, Eq, Serialize, Deserialize)]
 pub struct FieldPoint(#[serde_as(as = "serialization::SerdeAs")] pub Fr);
 
 impl FieldPoint {
     pub fn to_bytes(&self) -> Result<Vec<u8>> {
-        let mut writer = Vec::new();
-        self.0.serialize_uncompressed(&mut writer)?;
-        Ok(writer)
+        to_bytes(&self.0)
     }
 
     pub fn from_bytes(bytes: &[u8]) -> Result<FieldPoint> {
-        let mut reader = bytes;
-        let coeff = Fr::deserialize_uncompressed(&mut reader)?;
-        Ok(Self(coeff))
+        from_bytes(bytes).map(FieldPoint)
     }
 }
 
+pub type ValidatorMessage = (Validator<E>, Transcript<E>);
+
 #[derive(Clone)]
 pub struct Dkg(crate::PubliclyVerifiableDkg<E>);
 
 impl Dkg {
     pub fn new(
-        tau: u64,
+        tau: u32,
         shares_num: u32,
         security_threshold: u32,
-        validators: &[ExternalValidator<E>],
-        me: &ExternalValidator<E>,
+        validators: &[Validator<E>],
+        me: &Validator<E>,
     ) -> Result<Self> {
-        let params = crate::Params {
+        let dkg_params = crate::DkgParams {
             tau,
             security_threshold,
             shares_num,
         };
-        let session_keypair = Keypair::<E> {
-            decryption_key: ark_ff::UniformRand::rand(&mut ark_std::test_rng()),
-        };
         let dkg = crate::PubliclyVerifiableDkg::<E>::new(
             validators,
-            params,
+            &dkg_params,
             me,
-            session_keypair,
         )?;
         Ok(Self(dkg))
     }
 
     pub fn final_key(&self) -> DkgPublicKey {
         DkgPublicKey(self.0.final_key())
     }
 
     pub fn generate_transcript<R: RngCore>(
         &self,
         rng: &mut R,
-    ) -> Result<crate::PubliclyVerifiableSS<E>> {
+    ) -> Result<Transcript<E>> {
         self.0.create_share(rng)
     }
 
     pub fn aggregate_transcripts(
         &mut self,
-        messages: &Vec<(ExternalValidator<E>, Transcript<E>)>,
+        messages: &[ValidatorMessage],
     ) -> Result<AggregatedTranscript> {
-        // Avoid mutating current state
-        // TODO: Rewrite `deal` to not require mutability after validating this API design
+        // We must use `deal` here instead of to produce AggregatedTranscript instead of simply
+        // creating an AggregatedTranscript from the messages, because `deal` also updates the
+        // internal state of the DKG.
+        // If we didn't do that, that would cause the DKG to produce incorrect decryption shares
+        // in the future.
+        // TODO: Remove this dependency on DKG state
+        // TODO: Avoid mutating current state here
         for (validator, transcript) in messages {
-            self.0.deal(validator.clone(), transcript.clone())?;
+            self.0.deal(validator, transcript)?;
         }
-        Ok(AggregatedTranscript(crate::pvss::aggregate(&self.0)))
+        Ok(AggregatedTranscript(crate::pvss::aggregate(&self.0.vss)))
     }
 
     pub fn public_params(&self) -> DkgPublicParameters {
         DkgPublicParameters {
             g1_inv: self.0.pvss_params.g_inv(),
             domain_points: self.0.domain.elements().collect(),
         }
     }
 }
 
-#[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
-pub struct AggregatedTranscript(
-    crate::PubliclyVerifiableSS<E, crate::Aggregated>,
-);
+fn make_pvss_map(messages: &[ValidatorMessage]) -> PVSSMap<E> {
+    let mut pvss_map: PVSSMap<E> = PVSSMap::new();
+    messages.iter().for_each(|(validator, transcript)| {
+        pvss_map.insert(validator.address.clone(), transcript.clone());
+    });
+    pvss_map
+}
+
+#[derive(Clone, Debug, PartialEq, Eq, Serialize, Deserialize)]
+pub struct AggregatedTranscript(Transcript<E, crate::Aggregated>);
 
 impl AggregatedTranscript {
-    pub fn validate(&self, dkg: &Dkg) -> bool {
-        self.0.verify_full(&dkg.0)
+    pub fn new(messages: &[ValidatorMessage]) -> Self {
+        let pvss_map = make_pvss_map(messages);
+        AggregatedTranscript(crate::pvss::aggregate(&pvss_map))
+    }
+
+    pub fn verify(
+        &self,
+        shares_num: u32,
+        messages: &[ValidatorMessage],
+    ) -> Result<bool> {
+        let pvss_params = crate::pvss::PubliclyVerifiableParams::<E>::default();
+        let domain = Radix2EvaluationDomain::<Fr>::new(shares_num as usize)
+            .expect("Unable to construct an evaluation domain");
+
+        let is_valid_optimistic = self.0.verify_optimistic();
+        if !is_valid_optimistic {
+            return Err(crate::Error::InvalidTranscriptAggregate);
+        }
+
+        let pvss_map = make_pvss_map(messages);
+        let validators: Vec<_> = messages
+            .iter()
+            .map(|(validator, _)| validator)
+            .cloned()
+            .collect();
+
+        // This check also includes `verify_full`. See impl. for details.
+        let is_valid = do_verify_aggregation(
+            &self.0.coeffs,
+            &self.0.shares,
+            &pvss_params,
+            &validators,
+            &domain,
+            &pvss_map,
+        )?;
+        Ok(is_valid)
     }
 
     pub fn create_decryption_share_precomputed(
         &self,
         dkg: &Dkg,
         ciphertext: &Ciphertext,
         aad: &[u8],
         validator_keypair: &Keypair<E>,
     ) -> Result<DecryptionSharePrecomputed> {
         let domain_points: Vec<_> = dkg.0.domain.elements().collect();
         self.0.make_decryption_share_simple_precomputed(
             ciphertext,
             aad,
             &validator_keypair.decryption_key,
-            dkg.0.me,
+            dkg.0.me.share_index,
             &domain_points,
             &dkg.0.pvss_params.g_inv(),
         )
     }
 
     pub fn create_decryption_share_simple(
         &self,
@@ -150,15 +209,15 @@
         aad: &[u8],
         validator_keypair: &Keypair<E>,
     ) -> Result<DecryptionShareSimple> {
         self.0.make_decryption_share_simple(
             ciphertext,
             aad,
             &validator_keypair.decryption_key,
-            dkg.0.me,
+            dkg.0.me.share_index,
             &dkg.0.pvss_params.g_inv(),
         )
     }
 }
 
 #[serde_as]
 #[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
@@ -166,47 +225,58 @@
     #[serde_as(as = "serialization::SerdeAs")]
     pub g1_inv: G1Prepared,
     #[serde_as(as = "serialization::SerdeAs")]
     pub domain_points: Vec<Fr>,
 }
 
 impl DkgPublicParameters {
-    pub fn from_bytes(bytes: &[u8]) -> Self {
-        bincode::deserialize(bytes).unwrap()
+    pub fn from_bytes(bytes: &[u8]) -> Result<Self> {
+        bincode::deserialize(bytes).map_err(|e| e.into())
     }
 
-    pub fn to_bytes(&self) -> Vec<u8> {
-        bincode::serialize(self).unwrap()
+    pub fn to_bytes(&self) -> Result<Vec<u8>> {
+        bincode::serialize(self).map_err(|e| e.into())
     }
 }
 
+pub fn combine_shares_simple(
+    dkg_public_params: &DkgPublicParameters,
+    shares: &[DecryptionShareSimple],
+) -> SharedSecret {
+    let domain_points = &dkg_public_params.domain_points;
+    let lagrange_coefficients = prepare_combine_simple::<E>(&domain_points[..]);
+    let shared_secret =
+        share_combine_simple(shares, &lagrange_coefficients[..]);
+    SharedSecret(shared_secret)
+}
+
 #[cfg(test)]
 mod test_ferveo_api {
     use itertools::izip;
     use rand::{prelude::StdRng, thread_rng, SeedableRng};
 
     use crate::{api::*, dkg::test_common::*};
 
-    #[test]
-    fn test_server_api_tdec_precomputed() {
-        let rng = &mut StdRng::seed_from_u64(0);
+    type E = ark_bls12_381::Bls12_381;
 
-        let tau = 1;
-        let shares_num = 4;
-        // In precomputed variant, the security threshold is equal to the number of shares
-        // TODO: Refactor DKG contractor to not require security threshold or this case
-        // TODO: Or figure out a different way to simplify the precomputed variant API
-        let security_threshold = shares_num;
+    type TestInputs =
+        (Vec<ValidatorMessage>, Vec<Validator<E>>, Vec<Keypair<E>>);
 
-        let validator_keypairs = gen_n_keypairs(shares_num);
+    fn make_test_inputs(
+        rng: &mut StdRng,
+        tau: u32,
+        security_threshold: u32,
+        shares_num: u32,
+    ) -> TestInputs {
+        let validator_keypairs = gen_keypairs(shares_num);
         let validators = validator_keypairs
             .iter()
             .enumerate()
-            .map(|(i, keypair)| ExternalValidator {
-                address: format!("validator-{}", i),
+            .map(|(i, keypair)| Validator {
+                address: gen_address(i),
                 public_key: keypair.public(),
             })
             .collect::<Vec<_>>();
 
         // Each validator holds their own DKG instance and generates a transcript every
         // every validator, including themselves
         let messages: Vec<_> = validators
@@ -219,49 +289,89 @@
                     &validators,
                     sender,
                 )
                 .unwrap();
                 (sender.clone(), dkg.generate_transcript(rng).unwrap())
             })
             .collect();
+        (messages, validators, validator_keypairs)
+    }
+
+    #[test]
+    fn test_dkg_public_key_serialization() {
+        let shares_num = 4;
+        let validator_keypairs = gen_keypairs(shares_num);
+        let validators = validator_keypairs
+            .iter()
+            .enumerate()
+            .map(|(i, keypair)| Validator {
+                address: gen_address(i),
+                public_key: keypair.public(),
+            })
+            .collect::<Vec<_>>();
+
+        let dkg =
+            Dkg::new(1, shares_num, 2, &validators, &validators[0]).unwrap();
+
+        let serialized = dkg.final_key().to_bytes().unwrap();
+        assert_eq!(serialized.len(), DkgPublicKey::serialized_size());
+
+        let deserialized = DkgPublicKey::from_bytes(&serialized).unwrap();
+        assert_eq!(dkg.final_key(), deserialized);
+    }
+
+    #[test]
+    fn test_server_api_tdec_precomputed() {
+        let rng = &mut StdRng::seed_from_u64(0);
+
+        let tau = 1;
+        let shares_num = 4;
+        // In precomputed variant, the security threshold is equal to the number of shares
+        // TODO: Refactor DKG constructor to not require security threshold or this case.
+        //  Or figure out a different way to simplify the precomputed variant API.
+        let security_threshold = shares_num;
+
+        let (messages, validators, validator_keypairs) =
+            make_test_inputs(rng, tau, security_threshold, shares_num);
 
         // Now that every validator holds a dkg instance and a transcript for every other validator,
         // every validator can aggregate the transcripts
         let me = validators[0].clone();
         let mut dkg =
             Dkg::new(tau, shares_num, security_threshold, &validators, &me)
                 .unwrap();
 
         // Lets say that we've only receives `security_threshold` transcripts
         let messages = messages[..security_threshold as usize].to_vec();
         let pvss_aggregated = dkg.aggregate_transcripts(&messages).unwrap();
+        assert!(pvss_aggregated.verify(shares_num, &messages).unwrap());
 
         // At this point, any given validator should be able to provide a DKG public key
-        let public_key = dkg.final_key();
+        let dkg_public_key = dkg.final_key();
 
         // In the meantime, the client creates a ciphertext and decryption request
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
         let rng = &mut thread_rng();
-        let ciphertext = encrypt(msg, aad, &public_key.0, rng).unwrap();
+        let ciphertext = encrypt(msg, aad, &dkg_public_key.0, rng).unwrap();
 
         // Having aggregated the transcripts, the validators can now create decryption shares
         let decryption_shares: Vec<_> = izip!(&validators, &validator_keypairs)
             .map(|(validator, validator_keypair)| {
                 // Each validator holds their own instance of DKG and creates their own aggregate
                 let mut dkg = Dkg::new(
                     tau,
                     shares_num,
                     security_threshold,
                     &validators,
                     validator,
                 )
                 .unwrap();
                 let aggregate = dkg.aggregate_transcripts(&messages).unwrap();
-                assert!(pvss_aggregated.validate(&dkg));
+                assert!(pvss_aggregated.verify(shares_num, &messages).unwrap());
                 aggregate
                     .create_decryption_share_precomputed(
                         &dkg,
                         &ciphertext,
                         aad,
                         validator_keypair,
                     )
@@ -288,57 +398,34 @@
     fn test_server_api_tdec_simple() {
         let rng = &mut StdRng::seed_from_u64(0);
 
         let tau = 1;
         let shares_num = 4;
         let security_threshold = 3;
 
-        let validator_keypairs = gen_n_keypairs(shares_num);
-        let validators = validator_keypairs
-            .iter()
-            .enumerate()
-            .map(|(i, keypair)| ExternalValidator {
-                address: format!("validator-{}", i),
-                public_key: keypair.public(),
-            })
-            .collect::<Vec<_>>();
-
-        // Each validator holds their own DKG instance and generates a transcript every
-        // every validator, including themselves
-        let messages: Vec<_> = validators
-            .iter()
-            .map(|sender| {
-                let dkg = Dkg::new(
-                    tau,
-                    shares_num,
-                    security_threshold,
-                    &validators,
-                    sender,
-                )
-                .unwrap();
-                (sender.clone(), dkg.generate_transcript(rng).unwrap())
-            })
-            .collect();
+        let (messages, validators, validator_keypairs) =
+            make_test_inputs(rng, tau, security_threshold, shares_num);
 
         // Now that every validator holds a dkg instance and a transcript for every other validator,
         // every validator can aggregate the transcripts
         let me = validators[0].clone();
         let mut dkg =
             Dkg::new(tau, shares_num, security_threshold, &validators, &me)
                 .unwrap();
 
         // Lets say that we've only receives `security_threshold` transcripts
         let messages = messages[..security_threshold as usize].to_vec();
         let pvss_aggregated = dkg.aggregate_transcripts(&messages).unwrap();
+        assert!(pvss_aggregated.verify(shares_num, &messages).unwrap());
 
         // At this point, any given validator should be able to provide a DKG public key
         let public_key = dkg.final_key();
 
         // In the meantime, the client creates a ciphertext and decryption request
-        let msg: &[u8] = "abc".as_bytes();
+        let msg: &[u8] = "my-msg".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
         let rng = &mut thread_rng();
         let ciphertext = encrypt(msg, aad, &public_key.0, rng).unwrap();
 
         // Having aggregated the transcripts, the validators can now create decryption shares
         let decryption_shares: Vec<_> = izip!(&validators, &validator_keypairs)
             .map(|(validator, validator_keypair)| {
@@ -348,34 +435,106 @@
                     shares_num,
                     security_threshold,
                     &validators,
                     validator,
                 )
                 .unwrap();
                 let aggregate = dkg.aggregate_transcripts(&messages).unwrap();
-                assert!(pvss_aggregated.validate(&dkg));
+                assert!(aggregate.verify(shares_num, &messages).unwrap());
                 aggregate
-                    .create_decryption_share_precomputed(
+                    .create_decryption_share_simple(
                         &dkg,
                         &ciphertext,
                         aad,
                         validator_keypair,
                     )
                     .unwrap()
             })
             .collect();
 
         // Now, the decryption share can be used to decrypt the ciphertext
         // This part is part of the client API
 
-        let shared_secret = share_combine_precomputed(&decryption_shares);
+        let lagrange_coeffs =
+            prepare_combine_simple::<E>(&dkg.public_params().domain_points);
+        let shared_secret =
+            share_combine_simple(&decryption_shares, &lagrange_coeffs);
 
         let plaintext = decrypt_with_shared_secret(
             &ciphertext,
             aad,
             &shared_secret,
-            &dkg.0.pvss_params.g_inv(),
+            &dkg.public_params().g1_inv,
         )
         .unwrap();
         assert_eq!(plaintext, msg);
     }
+
+    #[test]
+    fn server_side_local_verification() {
+        let rng = &mut StdRng::seed_from_u64(0);
+
+        let tau = 1;
+        let security_threshold = 3;
+        let shares_num = 4;
+
+        let (messages, validators, _) =
+            make_test_inputs(rng, tau, security_threshold, shares_num);
+
+        // Now that every validator holds a dkg instance and a transcript for every other validator,
+        // every validator can aggregate the transcripts
+        let me = validators[0].clone();
+        let mut dkg =
+            Dkg::new(tau, shares_num, security_threshold, &validators, &me)
+                .unwrap();
+
+        let local_aggregate = dkg.aggregate_transcripts(&messages).unwrap();
+        assert!(local_aggregate
+            .verify(dkg.0.dkg_params.shares_num, &messages)
+            .is_ok());
+    }
+
+    #[test]
+    fn client_side_local_verification() {
+        let rng = &mut StdRng::seed_from_u64(0);
+
+        let tau = 1;
+        let security_threshold = 3;
+        let shares_num = 4;
+
+        let (messages, _, _) =
+            make_test_inputs(rng, tau, security_threshold, shares_num);
+
+        // We only need `security_threshold` transcripts to aggregate
+        let messages = &messages[..security_threshold as usize];
+
+        // Create an aggregated transcript on the client side
+        let aggregated_transcript = AggregatedTranscript::new(messages);
+
+        // We are separating the verification from the aggregation since the client may fetch
+        // the aggregate from a side-channel or decide to persist it and verify it later
+
+        // Now, the client can verify the aggregated transcript
+        let result = aggregated_transcript.verify(shares_num, messages);
+        assert!(result.is_ok());
+        assert!(result.unwrap());
+
+        // Test negative cases
+
+        // Not enough transcripts
+        let not_enough_messages = &messages[..2];
+        assert!(not_enough_messages.len() < security_threshold as usize);
+        let insufficient_aggregate =
+            AggregatedTranscript::new(not_enough_messages);
+        let result = insufficient_aggregate.verify(shares_num, messages);
+        assert!(result.is_err());
+
+        // Unexpected transcripts in the aggregate or transcripts from a different ritual
+        // Using same DKG parameters, but different DKG instances and validators
+        let (bad_messages, _, _) =
+            make_test_inputs(rng, tau, security_threshold, shares_num);
+        let mixed_messages = [&messages[..2], &bad_messages[..1]].concat();
+        let bad_aggregate = AggregatedTranscript::new(&mixed_messages);
+        let result = bad_aggregate.verify(shares_num, messages);
+        assert!(result.is_err());
+    }
 }
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/src/dkg/pv.rs` & `ferveo-0.1.8/local_dependencies/ferveo/src/dkg/pv.rs`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 use serde_with::serde_as;
 
 use crate::{
     aggregate, make_validators, AggregatedPvss, DkgState, Error, Params,
     PubliclyVerifiableParams, PubliclyVerifiableSS, Pvss, Result,
 };
 
+pub type PVSSMap<E> = BTreeMap<u32, PubliclyVerifiableSS<E>>;
+
 /// The DKG context that holds all of the local state for participating in the DKG
 // TODO: Consider removing Clone to avoid accidentally NOT-mutating state.
 //  Currently, we're assuming that the DKG is only mutated by the owner of the instance.
 //  Consider removing Clone after finalizing ferveo::api
 #[derive(Clone, Debug)]
 pub struct PubliclyVerifiableDkg<E: Pairing> {
     pub params: Params,
     pub pvss_params: PubliclyVerifiableParams<E>,
     // TODO: What is session_keypair?
     pub session_keypair: ferveo_common::Keypair<E>,
     pub validators: Vec<ferveo_common::Validator<E>>,
-    pub vss: BTreeMap<u32, PubliclyVerifiableSS<E>>,
+    pub vss: PVSSMap<E>,
     pub domain: ark_poly::Radix2EvaluationDomain<E::ScalarField>,
     pub state: DkgState<E>,
     pub me: usize,
 }
 
 impl<E: Pairing> PubliclyVerifiableDkg<E> {
     /// Create a new DKG context to participate in the DKG
@@ -47,15 +49,15 @@
         if !is_power_of_2(params.shares_num) {
             return Err(Error::InvalidShareNumberParameter(params.shares_num));
         }
 
         let domain = ark_poly::Radix2EvaluationDomain::<E::ScalarField>::new(
             params.shares_num as usize,
         )
-        .expect("unable to construct domain");
+        .expect("Unable to construct an evaluation domain");
 
         // keep track of the owner of this instance in the validator set
         let me = validators
             .iter()
             .position(|probe| me == probe)
             .ok_or_else(|| Error::ValidatorNotInSet(me.clone().address))?;
 
@@ -103,15 +105,15 @@
 
     /// Aggregate all received PVSS messages into a single message, prepared to post on-chain
     pub fn aggregate(&self) -> Result<Message<E>> {
         match self.state {
             DkgState::Dealt => {
                 let final_key = self.final_key();
                 Ok(Message::Aggregate(Aggregation {
-                    vss: aggregate(self),
+                    vss: aggregate(&self.vss),
                     final_key,
                 }))
             }
             _ => Err(Error::InvalidDkgStateToAggregate),
         }
     }
 
@@ -159,26 +161,33 @@
                 }
             }
             Message::Aggregate(Aggregation { vss, final_key })
                 if matches!(self.state, DkgState::Dealt) =>
             {
                 let minimum_shares =
                     self.params.shares_num - self.params.security_threshold;
-                let verified_shares = vss.verify_aggregation(self)?;
+                let actual_shares = vss.shares.len() as u32;
                 // we reject aggregations that fail to meet the security threshold
-                if verified_shares < minimum_shares {
-                    Err(Error::InsufficientTranscriptsForAggregate(
+                if actual_shares < minimum_shares {
+                    return Err(Error::InsufficientTranscriptsForAggregate(
                         minimum_shares,
-                        verified_shares,
-                    ))
-                } else if &self.final_key() == final_key {
-                    Ok(())
-                } else {
-                    Err(Error::InvalidFinalKey)
+                        actual_shares,
+                    ));
+                }
+
+                let is_aggregate_valid = vss.verify_aggregation(self)?;
+                if !is_aggregate_valid {
+                    return Err(Error::InvalidTranscriptAggregate);
                 }
+
+                if &self.final_key() == final_key {
+                    return Ok(());
+                }
+
+                Err(Error::InvalidFinalKey)
             }
             _ => Err(Error::InvalidDkgStateToVerify),
         }
     }
 
     /// After consensus has agreed to include a verified
     /// message on the blockchain, we apply the chains
@@ -224,26 +233,28 @@
                 };
                 Ok(())
             }
             _ => Err(Error::InvalidDkgStateToIngest),
         }
     }
 
+    // TODO: Instead of using this mutable functions, remove all state-fullness from the DKG
+    // implementation and make it a pure function that takes a DkgState and returns a new one
     pub fn deal(
         &mut self,
-        sender: ExternalValidator<E>,
-        pvss: Pvss<E>,
+        sender: &ExternalValidator<E>,
+        pvss: &Pvss<E>,
     ) -> Result<()> {
         // Add the ephemeral public key and pvss transcript
         let sender = self
             .validators
             .iter()
             .position(|probe| sender.address == probe.validator.address)
-            .ok_or_else(|| Error::UnknownDealer(sender.address))?;
-        self.vss.insert(sender as u32, pvss);
+            .ok_or_else(|| Error::UnknownDealer(sender.clone().address))?;
+        self.vss.insert(sender as u32, pvss.clone());
         Ok(())
     }
 }
 
 #[serde_as]
 #[derive(Serialize, Deserialize, Clone, Debug)]
 #[serde(bound(
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/src/lib.rs` & `ferveo-0.1.8/local_dependencies/ferveo/src/lib.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+use ark_ec::pairing::Pairing;
+use group_threshold_cryptography as tpke;
+use itertools::zip_eq;
+
 pub mod api;
 pub mod dkg;
 pub mod primitives;
-mod vss;
+pub mod pvss;
+pub mod validator;
 
 pub use dkg::*;
-use group_threshold_cryptography as tpke;
 pub use primitives::*;
-pub use vss::*;
+pub use pvss::*;
+pub use validator::*;
 
 #[derive(Debug, thiserror::Error)]
 pub enum Error {
     /// Threshold encryption error
     #[error("Threshold encryption error")]
     ThresholdEncryptionError(#[from] tpke::Error),
 
@@ -32,23 +37,23 @@
 
     /// DKG is not in a valid state to ingest PVSS transcripts
     #[error("Invalid DKG state to ingest PVSS transcripts")]
     InvalidDkgStateToIngest,
 
     /// DKG validator set must contain the validator with the given address
     #[error("Expected validator to be a part of the DKG validator set: {0}")]
-    ValidatorNotInSet(String),
+    DealerNotInValidatorSet(EthereumAddress),
 
     /// DKG received an unknown dealer. Dealer must be the part of the DKG validator set.
     #[error("DKG received an unknown dealer: {0}")]
-    UnknownDealer(String),
+    UnknownDealer(EthereumAddress),
 
     /// DKG received a PVSS transcript from a dealer that has already been dealt.
     #[error("DKG received a PVSS transcript from a dealer that has already been dealt: {0}")]
-    DuplicateDealer(String),
+    DuplicateDealer(EthereumAddress),
 
     /// DKG received an invalid transcript for which optimistic verification failed
     #[error("DKG received an invalid transcript")]
     InvalidPvssTranscript,
 
     /// Aggregation failed because the DKG did not receive enough PVSS transcripts
     #[error(
@@ -64,73 +69,90 @@
     #[error("Not enough validators (expected {0}, got {1})")]
     InsufficientValidators(u32, u32),
 
     /// Transcript aggregate doesn't match the received PVSS instances
     #[error("Transcript aggregate doesn't match the received PVSS instances")]
     InvalidTranscriptAggregate,
 
-    /// Serialization error
-    #[error("Serialization error")]
-    SerializationError(#[from] ark_serialize::SerializationError),
+    /// Serialization failed
+    #[error("Serialization failed")]
+    BincodeSerializationError(#[from] bincode::Error),
+
+    /// Serialization failed
+    #[error("Serialization failed")]
+    ArkworksSerializationError(#[from] ark_serialize::SerializationError),
+
+    /// DKG validators must be sorted by their Ethereum address
+    #[error("DKG validators not sorted")]
+    ValidatorsNotSorted,
+
+    /// The validator public key doesn't match the one in the DKG
+    #[error("Validator public key mismatch")]
+    ValidatorPublicKeyMismatch,
 }
 
 pub type Result<T> = std::result::Result<T, Error>;
 
+pub fn make_pvss_map<E: Pairing>(
+    transcripts: &[PubliclyVerifiableSS<E>],
+    validators: &[Validator<E>],
+) -> PVSSMap<E> {
+    let mut pvss_map: PVSSMap<E> = PVSSMap::new();
+    zip_eq(transcripts, validators).for_each(|(transcript, validator)| {
+        pvss_map.insert(validator.address.clone(), transcript.clone());
+    });
+    pvss_map
+}
+
 #[cfg(test)]
 mod test_dkg_full {
     use std::collections::HashMap;
 
     use ark_bls12_381::{Bls12_381 as E, Fr, G1Affine};
     use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup};
     use ark_ff::{UniformRand, Zero};
     use ark_poly::EvaluationDomain;
     use ark_std::test_rng;
     use ferveo_common::Keypair;
     use group_threshold_cryptography as tpke;
     use group_threshold_cryptography::{
         Ciphertext, DecryptionSharePrecomputed, DecryptionShareSimple,
     };
-    use itertools::{izip, Itertools};
+    use itertools::izip;
 
     use super::*;
-    use crate::dkg::pv::test_common::*;
+    use crate::dkg::test_common::*;
 
     type TargetField = <E as Pairing>::TargetField;
 
     fn make_shared_secret_simple_tdec(
         dkg: &PubliclyVerifiableDkg<E>,
         aad: &[u8],
         ciphertext: &Ciphertext<E>,
         validator_keypairs: &[Keypair<E>],
     ) -> (
         PubliclyVerifiableSS<E, Aggregated>,
         Vec<DecryptionShareSimple<E>>,
         TargetField,
     ) {
-        // Make sure validators are in the same order dkg is by comparing their public keys
-        dkg.validators
-            .iter()
-            .zip_eq(validator_keypairs.iter())
-            .for_each(|(v, k)| {
-                assert_eq!(v.validator.public_key, k.public());
-            });
-
-        let pvss_aggregated = aggregate(dkg);
+        let pvss_aggregated = aggregate(&dkg.vss);
+        assert!(pvss_aggregated.verify_aggregation(dkg).is_ok());
 
         let decryption_shares: Vec<DecryptionShareSimple<E>> =
             validator_keypairs
                 .iter()
-                .enumerate()
-                .map(|(validator_index, validator_keypair)| {
+                .map(|validator_keypair| {
+                    let validator =
+                        dkg.get_validator(&validator_keypair.public()).unwrap();
                     pvss_aggregated
                         .make_decryption_share_simple(
                             ciphertext,
                             aad,
                             &validator_keypair.decryption_key,
-                            validator_index,
+                            validator.share_index,
                             &dkg.pvss_params.g_inv(),
                         )
                         .unwrap()
                 })
                 .collect();
 
         let domain = &dkg
@@ -152,21 +174,20 @@
         (pvss_aggregated, decryption_shares, shared_secret)
     }
 
     #[test]
     fn test_dkg_simple_tdec() {
         let rng = &mut test_rng();
 
-        let dkg = setup_dealt_dkg_with_n_validators(3, 4);
+        let (dkg, validator_keypairs) = setup_dealt_dkg_with_n_validators(3, 4);
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
         let public_key = dkg.final_key();
         let ciphertext =
             tpke::encrypt::<E>(msg, aad, &public_key, rng).unwrap();
-        let validator_keypairs = gen_n_keypairs(4);
 
         let (_, _, shared_secret) = make_shared_secret_simple_tdec(
             &dkg,
             aad,
             &ciphertext,
             &validator_keypairs,
         );
@@ -181,40 +202,40 @@
         assert_eq!(plaintext, msg);
     }
 
     #[test]
     fn test_dkg_simple_tdec_precomputed() {
         let rng = &mut test_rng();
 
-        let dkg = setup_dealt_dkg_with_n_validators(3, 4);
+        let (dkg, validator_keypairs) = setup_dealt_dkg_with_n_validators(3, 4);
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
         let public_key = dkg.final_key();
         let ciphertext =
             tpke::encrypt::<E>(msg, aad, &public_key, rng).unwrap();
-        let validator_keypairs = gen_n_keypairs(4);
 
-        let pvss_aggregated = aggregate(&dkg);
+        let pvss_aggregated = aggregate(&dkg.vss);
+        pvss_aggregated.verify_aggregation(&dkg).unwrap();
         let domain_points = dkg
             .domain
             .elements()
             .take(validator_keypairs.len())
             .collect::<Vec<_>>();
 
         let decryption_shares: Vec<DecryptionSharePrecomputed<E>> =
             validator_keypairs
                 .iter()
                 .enumerate()
-                .map(|(validator_index, validator_keypair)| {
+                .map(|(validator_address, validator_keypair)| {
                     pvss_aggregated
                         .make_decryption_share_simple_precomputed(
                             &ciphertext,
                             aad,
                             &validator_keypair.decryption_key,
-                            validator_index,
+                            validator_address,
                             &domain_points,
                             &dkg.pvss_params.g_inv(),
                         )
                         .unwrap()
                 })
                 .collect();
 
@@ -232,21 +253,20 @@
         assert_eq!(plaintext, msg);
     }
 
     #[test]
     fn test_dkg_simple_tdec_share_verification() {
         let rng = &mut test_rng();
 
-        let dkg = setup_dealt_dkg_with_n_validators(3, 4);
+        let (dkg, validator_keypairs) = setup_dealt_dkg_with_n_validators(3, 4);
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
         let public_key = dkg.final_key();
         let ciphertext =
             tpke::encrypt::<E>(msg, aad, &public_key, rng).unwrap();
-        let validator_keypairs = gen_n_keypairs(4);
 
         let (pvss_aggregated, decryption_shares, _) =
             make_shared_secret_simple_tdec(
                 &dkg,
                 aad,
                 &ciphertext,
                 &validator_keypairs,
@@ -292,20 +312,19 @@
         ));
     }
 
     #[test]
     fn test_dkg_simple_tdec_share_recovery() {
         let rng = &mut test_rng();
 
-        let mut dkg = setup_dealt_dkg_with_n_validators(3, 4);
+        let (dkg, validator_keypairs) = setup_dealt_dkg_with_n_validators(3, 4);
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
         let public_key = &dkg.final_key();
         let ciphertext = tpke::encrypt::<E>(msg, aad, public_key, rng).unwrap();
-        let mut validator_keypairs = gen_n_keypairs(4);
 
         // Create an initial shared secret
         let (_, _, old_shared_secret) = make_shared_secret_simple_tdec(
             &dkg,
             aad,
             &ciphertext,
             &validator_keypairs,
@@ -313,55 +332,60 @@
 
         // Now, we're going to recover a new share at a random point and check that the shared secret is still the same
 
         // Our random point
         let x_r = Fr::rand(rng);
 
         // Remove one participant from the contexts and all nested structure
-        let removed_validator = dkg.validators.pop().unwrap();
-        validator_keypairs.pop();
+        let removed_validator_addr =
+            dkg.validators.keys().last().unwrap().clone();
+        let mut remaining_validators = dkg.validators.clone();
+        remaining_validators.remove(&removed_validator_addr);
+
         // Remember to remove one domain point too
         let mut domain_points = dkg.domain.elements().collect::<Vec<_>>();
         domain_points.pop().unwrap();
 
         // Each participant prepares an update for each other participant
-        let share_updates = &dkg
-            .validators
-            .iter()
-            .map(|p| {
+        let share_updates = remaining_validators
+            .keys()
+            .map(|v_addr| {
                 let deltas_i = tpke::prepare_share_updates_for_recovery::<E>(
                     &domain_points,
                     &dkg.pvss_params.h.into_affine(),
                     &x_r,
-                    dkg.params.security_threshold as usize,
+                    dkg.dkg_params.security_threshold as usize,
                     rng,
                 );
-                (p.share_index, deltas_i)
+                (v_addr.clone(), deltas_i)
             })
             .collect::<HashMap<_, _>>();
 
         // Participants share updates and update their shares
-        let pvss_aggregated = aggregate(&dkg);
+        let pvss_aggregated = aggregate(&dkg.vss);
 
         // Now, every participant separately:
-        let updated_shares: Vec<_> = validator_keypairs
+        let updated_shares: Vec<_> = remaining_validators
             .iter()
-            .enumerate()
-            .map(|(validator_index, validator_keypair)| {
+            .map(|(validator_address, validator)| {
                 // Receives updates from other participants
-                let updates_for_participant: Vec<_> = share_updates
-                    .values()
-                    .map(|updates| *updates.get(validator_index).unwrap())
-                    .collect();
+                let updates_for_participant =
+                    share_updates.get(validator_address).unwrap();
+
+                // Each validator uses their decryption key to update their share
+                let decryption_key = validator_keypairs
+                    .get(validator.share_index)
+                    .unwrap()
+                    .decryption_key;
 
                 // Creates updated private key shares
                 pvss_aggregated.update_private_key_share_for_recovery(
-                    &validator_keypair.decryption_key,
-                    validator_index,
-                    &updates_for_participant,
+                    &decryption_key,
+                    validator.share_index,
+                    updates_for_participant,
                 )
             })
             .collect();
 
         // Now, we have to combine new share fragments into a new share
         let new_private_key_share =
             tpke::recover_share_from_updated_private_shares(
@@ -371,33 +395,31 @@
             );
 
         // Get decryption shares from remaining participants
         let mut decryption_shares: Vec<DecryptionShareSimple<E>> =
             validator_keypairs
                 .iter()
                 .enumerate()
-                .map(|(validator_index, validator_keypair)| {
+                .map(|(share_index, validator_keypair)| {
                     pvss_aggregated
                         .make_decryption_share_simple(
                             &ciphertext,
                             aad,
                             &validator_keypair.decryption_key,
-                            validator_index,
+                            share_index,
                             &dkg.pvss_params.g_inv(),
                         )
                         .unwrap()
                 })
                 .collect();
 
         // Create a decryption share from a recovered private key share
         let new_validator_decryption_key = Fr::rand(rng);
-        let validator_index = removed_validator.share_index;
         decryption_shares.push(
             DecryptionShareSimple::create(
-                validator_index,
                 &new_validator_decryption_key,
                 &new_private_key_share,
                 &ciphertext,
                 aad,
                 &dkg.pvss_params.g_inv(),
             )
             .unwrap(),
@@ -409,56 +431,55 @@
 
         assert_eq!(old_shared_secret, new_shared_secret);
     }
 
     #[test]
     fn simple_tdec_share_refreshing() {
         let rng = &mut test_rng();
-        let dkg = setup_dealt_dkg_with_n_validators(3, 4);
+        let (dkg, validator_keypairs) = setup_dealt_dkg_with_n_validators(3, 4);
 
         let msg: &[u8] = "abc".as_bytes();
         let aad: &[u8] = "my-aad".as_bytes();
         let public_key = dkg.final_key();
         let ciphertext =
             tpke::encrypt::<E>(msg, aad, &public_key, rng).unwrap();
 
-        let validator_keypairs = gen_n_keypairs(4);
-        let pvss_aggregated = aggregate(&dkg);
+        let pvss_aggregated = aggregate(&dkg.vss);
 
         // Create an initial shared secret
         let (_, _, old_shared_secret) = make_shared_secret_simple_tdec(
             &dkg,
             aad,
             &ciphertext,
             &validator_keypairs,
         );
 
         // Now, we're going to refresh the shares and check that the shared secret is the same
 
         // Dealer computes a new random polynomial with constant term x_r = 0
         let polynomial = tpke::make_random_polynomial_at::<E>(
-            dkg.params.security_threshold as usize,
+            dkg.dkg_params.security_threshold as usize,
             &Fr::zero(),
             rng,
         );
 
         // Dealer shares the polynomial with participants
 
         // Participants computes new decryption shares
         let new_decryption_shares: Vec<DecryptionShareSimple<E>> =
             validator_keypairs
                 .iter()
                 .enumerate()
-                .map(|(validator_index, validator_keypair)| {
+                .map(|(validator_address, validator_keypair)| {
                     pvss_aggregated
                         .refresh_decryption_share(
                             &ciphertext,
                             aad,
                             &validator_keypair.decryption_key,
-                            validator_index,
+                            validator_address,
                             &polynomial,
                             &dkg,
                         )
                         .unwrap()
                 })
                 .collect();
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/src/primitives.rs` & `ferveo-0.1.8/local_dependencies/ferveo/src/primitives.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/ferveo/src/vss/pvss.rs` & `ferveo-0.1.8/local_dependencies/ferveo/src/pvss.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 use std::{marker::PhantomData, ops::Mul};
 
-use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup};
+use ark_ec::{pairing::Pairing, AffineRepr, CurveGroup, Group};
 use ark_ff::{Field, Zero};
 use ark_poly::{
     polynomial::univariate::DensePolynomial, DenseUVPolynomial,
     EvaluationDomain,
 };
+use ferveo_common::is_sorted;
 use group_threshold_cryptography as tpke;
 use itertools::Itertools;
-use measure_time::print_time;
 use rand::RngCore;
 use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 use subproductdomain::fast_multiexp;
 use tpke::{
     prepare_combine_simple, refresh_private_key_share,
     update_share_for_recovery, Ciphertext, DecryptionSharePrecomputed,
     DecryptionShareSimple, PrivateKeyShare,
 };
 
 use crate::{
-    batch_to_projective_g1, batch_to_projective_g2, Error,
-    PubliclyVerifiableDkg, Result,
+    batch_to_projective_g1, batch_to_projective_g2, Error, PVSSMap,
+    PubliclyVerifiableDkg, Result, Validator,
 };
 
 /// These are the blinded evaluations of shares of a single random polynomial
 pub type ShareEncryptions<E> = <E as Pairing>::G2Affine;
 
 /// Marker struct for unaggregated PVSS transcripts
-#[derive(Serialize, Deserialize, Clone, Debug, PartialEq)]
+#[derive(Serialize, Deserialize, Clone, Debug, PartialEq, Eq)]
 pub struct Unaggregated;
 
 /// Marker struct for aggregated PVSS transcripts
-#[derive(Serialize, Deserialize, Clone, Debug, PartialEq)]
+#[derive(Serialize, Deserialize, Clone, Debug, PartialEq, Eq)]
 pub struct Aggregated;
 
 /// Trait gate used to add extra methods to aggregated PVSS transcripts
 pub trait Aggregate {}
 
 /// Apply trait gate to Aggregated marker struct
 impl Aggregate for Aggregated {}
@@ -56,19 +56,28 @@
 
 impl<E: Pairing> PubliclyVerifiableParams<E> {
     pub fn g_inv(&self) -> E::G1Prepared {
         E::G1Prepared::from(-self.g)
     }
 }
 
+impl<E: Pairing> Default for PubliclyVerifiableParams<E> {
+    fn default() -> Self {
+        Self {
+            g: E::G1::generator(),
+            h: E::G2::generator(),
+        }
+    }
+}
+
 /// Each validator posts a transcript to the chain. Once enough
 /// validators have done this (their total voting power exceeds
 /// 2/3 the total), this will be aggregated into a final key
 #[serde_as]
-#[derive(Serialize, Deserialize, Clone, Debug, PartialEq)]
+#[derive(Serialize, Deserialize, Clone, Debug, PartialEq, Eq)]
 pub struct PubliclyVerifiableSS<E: Pairing, T = Unaggregated> {
     /// Used in Feldman commitment to the VSS polynomial, F = g^{\phi}
     #[serde_as(as = "ferveo_common::serialization::SerdeAs")]
     pub coeffs: Vec<E::G1Affine>,
 
     /// The shares to be dealt to each validator
     #[serde_as(as = "ferveo_common::serialization::SerdeAs")]
@@ -92,32 +101,32 @@
     pub fn new<R: RngCore>(
         s: &E::ScalarField,
         dkg: &PubliclyVerifiableDkg<E>,
         rng: &mut R,
     ) -> Result<Self> {
         // Our random polynomial, \phi(x) = s + \sum_{i=1}^{t-1} a_i x^i
         let mut phi = DensePolynomial::<E::ScalarField>::rand(
-            (dkg.params.security_threshold - 1) as usize,
+            (dkg.dkg_params.security_threshold - 1) as usize,
             rng,
         );
         phi.coeffs[0] = *s; // setting the first coefficient to secret value
 
         // Evaluations of the polynomial over the domain
         let evals = phi.evaluate_over_domain_by_ref(dkg.domain);
         // commitment to coeffs, F_i
         let coeffs = fast_multiexp(&phi.coeffs, dkg.pvss_params.g);
         let shares = dkg
             .validators
-            .iter()
-            .map(|val| {
+            .values()
+            .map(|validator| {
                 // ek_{i}^{eval_i}, i = validator index
                 fast_multiexp(
                     // &evals.evals[i..i] = &evals.evals[i]
-                    &[evals.evals[val.share_index]], // one share per validator
-                    val.validator.public_key.encryption_key.into_group(),
+                    &[evals.evals[validator.share_index]], // one share per validator
+                    validator.validator.public_key.encryption_key.into_group(),
                 )[0]
             })
             .collect::<Vec<ShareEncryptions<E>>>();
         if shares.len() != dkg.validators.len() {
             return Err(Error::InsufficientValidators(
                 shares.len() as u32,
                 dkg.validators.len() as u32,
@@ -136,95 +145,149 @@
         Ok(vss)
     }
 
     /// Verify the pvss transcript from a validator. This is not the full check,
     /// i.e. we optimistically do not check the commitment. This is deferred
     /// until the aggregation step
     pub fn verify_optimistic(&self) -> bool {
+        let pvss_params = PubliclyVerifiableParams::<E>::default();
         // We're only checking the proof of knowledge here, sigma ?= h^s
         // "Does the first coefficient of the secret polynomial match the proof of knowledge?"
         E::pairing(
             self.coeffs[0].into_group(), // F_0 = g^s
-            E::G2Affine::generator(),    // h
+            pvss_params.h,
         ) == E::pairing(
-            E::G1Affine::generator(), // g
-            self.sigma,               // h^s
+            pvss_params.g,
+            self.sigma, // h^s
         )
     }
 
     /// Part of checking the validity of an aggregated PVSS transcript
     ///
     /// Implements check #4 in 4.2.3 section of https://eprint.iacr.org/2022/898.pdf
     ///
     /// If aggregation fails, a validator needs to know that their pvss
     /// transcript was at fault so that the can issue a new one. This
     /// function may also be used for that purpose.
     pub fn verify_full(&self, dkg: &PubliclyVerifiableDkg<E>) -> bool {
-        // compute the commitment
-        let mut commitment = batch_to_projective_g1::<E>(&self.coeffs);
-        print_time!("commitment fft");
-        dkg.domain.fft_in_place(&mut commitment);
-
-        // Each validator checks that their share is correct
-        dkg.validators
-            .iter()
-            .zip(self.shares.iter())
-            .all(|(validator, y_i)| {
-                // TODO: Check #3 is missing
-                // See #3 in 4.2.3 section of https://eprint.iacr.org/2022/898.pdf
-
-                // Validator checks checks aggregated shares against commitment
-                let ek_i =
-                    validator.validator.public_key.encryption_key.into_group();
-                let a_i = &commitment[validator.share_index];
-                // We verify that e(G, Y_i) = e(A_i, ek_i) for validator i
-                // See #4 in 4.2.3 section of https://eprint.iacr.org/2022/898.pdf
-                // e(G,Y) = e(A, ek)
-                E::pairing(dkg.pvss_params.g, *y_i) == E::pairing(a_i, ek_i)
-            })
+        let validators = dkg
+            .validators
+            .values()
+            .map(|v| v.validator.clone())
+            .collect::<Vec<_>>();
+        let validators = validators.as_slice();
+        do_verify_full(
+            &self.coeffs,
+            &self.shares,
+            &dkg.pvss_params,
+            validators,
+            &dkg.domain,
+        )
+    }
+}
+
+// TODO: Return validator that failed the check
+pub fn do_verify_full<E: Pairing>(
+    pvss_coefficients: &[E::G1Affine],
+    pvss_encrypted_shares: &[E::G2Affine],
+    pvss_params: &PubliclyVerifiableParams<E>,
+    validators: &[Validator<E>],
+    domain: &ark_poly::Radix2EvaluationDomain<E::ScalarField>,
+) -> bool {
+    let mut commitment = batch_to_projective_g1::<E>(pvss_coefficients);
+    domain.fft_in_place(&mut commitment);
+
+    // At this point, validators must be sorted
+    assert!(is_sorted(validators));
+
+    // Each validator checks that their share is correct
+    validators
+        .iter()
+        .zip(pvss_encrypted_shares.iter())
+        .enumerate()
+        .all(|(share_index, (validator, y_i))| {
+            // TODO: Check #3 is missing
+            // See #3 in 4.2.3 section of https://eprint.iacr.org/2022/898.pdf
+
+            // Validator checks aggregated shares against commitment
+            let ek_i = validator.public_key.encryption_key.into_group();
+            let a_i = &commitment[share_index];
+            // We verify that e(G, Y_i) = e(A_i, ek_i) for validator i
+            // See #4 in 4.2.3 section of https://eprint.iacr.org/2022/898.pdf
+            // e(G,Y) = e(A, ek)
+            E::pairing(pvss_params.g, *y_i) == E::pairing(a_i, ek_i)
+        })
+}
+
+pub fn do_verify_aggregation<E: Pairing>(
+    pvss_agg_coefficients: &[E::G1Affine],
+    pvss_agg_encrypted_shares: &[E::G2Affine],
+    pvss_params: &PubliclyVerifiableParams<E>,
+    validators: &[Validator<E>],
+    domain: &ark_poly::Radix2EvaluationDomain<E::ScalarField>,
+    vss: &PVSSMap<E>,
+) -> Result<bool> {
+    let is_valid = do_verify_full(
+        pvss_agg_coefficients,
+        pvss_agg_encrypted_shares,
+        pvss_params,
+        validators,
+        domain,
+    );
+    if !is_valid {
+        return Err(Error::InvalidTranscriptAggregate);
+    }
+
+    // Now, we verify that the aggregated PVSS transcript is a valid aggregation
+    let mut y = E::G1::zero();
+    for (_, pvss) in vss.iter() {
+        y += pvss.coeffs[0].into_group();
+    }
+    if y.into_affine() == pvss_agg_coefficients[0] {
+        Ok(true)
+    } else {
+        Err(Error::InvalidTranscriptAggregate)
     }
 }
 
 /// Extra methods available to aggregated PVSS transcripts
 impl<E: Pairing, T: Aggregate> PubliclyVerifiableSS<E, T> {
     /// Verify that this PVSS instance is a valid aggregation of
     /// the PVSS instances, produced by [`aggregate`],
     /// and received by the DKG context `dkg`
-    /// Returns the total valid weight of the aggregated PVSS
+    /// Returns the total nr of shares in the aggregated PVSS
     pub fn verify_aggregation(
         &self,
         dkg: &PubliclyVerifiableDkg<E>,
-    ) -> Result<u32> {
-        print_time!("PVSS verify_aggregation");
-        self.verify_full(dkg);
-        // Now, we verify that the aggregated PVSS transcript is a valid aggregation
-        // If it is, we return the total weights of the PVSS transcripts
-        let mut y = E::G1::zero();
-        // TODO: If we don't deal with share weights anymore, do we even need to call `verify_aggregation`?
-        let mut shares_total = 0u32;
-        for (_, pvss) in dkg.vss.iter() {
-            y += pvss.coeffs[0].into_group();
-            shares_total += 1
-        }
-        if y.into_affine() == self.coeffs[0] {
-            Ok(shares_total)
-        } else {
-            Err(Error::InvalidTranscriptAggregate)
-        }
+    ) -> Result<bool> {
+        let validators = dkg
+            .validators
+            .values()
+            .map(|v| v.validator.clone())
+            .collect::<Vec<_>>();
+        let validators = validators.as_slice();
+        do_verify_aggregation(
+            &self.coeffs,
+            &self.shares,
+            &dkg.pvss_params,
+            validators,
+            &dkg.domain,
+            &dkg.vss,
+        )
     }
 
     pub fn decrypt_private_key_share(
         &self,
         validator_decryption_key: &E::ScalarField,
-        validator_index: usize,
+        share_index: usize,
     ) -> PrivateKeyShare<E> {
         // Decrypt private key shares https://nikkolasg.github.io/ferveo/pvss.html#validator-decryption-of-private-key-shares
         let private_key_share = self
             .shares
-            .get(validator_index)
+            .get(share_index)
             .unwrap()
             .mul(
                 validator_decryption_key
                     .inverse()
                     .expect("Validator decryption key must have an inverse"),
             )
             .into_affine();
@@ -232,116 +295,105 @@
     }
 
     pub fn make_decryption_share_simple(
         &self,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
         validator_decryption_key: &E::ScalarField,
-        validator_index: usize,
+        share_index: usize,
         g_inv: &E::G1Prepared,
     ) -> Result<DecryptionShareSimple<E>> {
-        let private_key_share = self.decrypt_private_key_share(
-            validator_decryption_key,
-            validator_index,
-        );
+        let private_key_share = self
+            .decrypt_private_key_share(validator_decryption_key, share_index);
         DecryptionShareSimple::create(
-            validator_index,
             validator_decryption_key,
             &private_key_share,
             ciphertext,
             aad,
             g_inv,
         )
         .map_err(|e| e.into())
     }
     pub fn make_decryption_share_simple_precomputed(
         &self,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
         validator_decryption_key: &E::ScalarField,
-        validator_index: usize,
+        share_index: usize,
         domain_points: &[E::ScalarField],
         g_inv: &E::G1Prepared,
     ) -> Result<DecryptionSharePrecomputed<E>> {
-        let private_key_share = self.decrypt_private_key_share(
-            validator_decryption_key,
-            validator_index,
-        );
+        let private_key_share = self
+            .decrypt_private_key_share(validator_decryption_key, share_index);
 
         let lagrange_coeffs = prepare_combine_simple::<E>(domain_points);
 
         DecryptionSharePrecomputed::new(
-            validator_index,
+            share_index,
             validator_decryption_key,
             &private_key_share,
             ciphertext,
             aad,
-            &lagrange_coeffs[validator_index],
+            &lagrange_coeffs[share_index],
             g_inv,
         )
         .map_err(|e| e.into())
     }
 
     pub fn refresh_decryption_share(
         &self,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
         validator_decryption_key: &E::ScalarField,
-        validator_index: usize,
+        share_index: usize,
         polynomial: &DensePolynomial<E::ScalarField>,
         dkg: &PubliclyVerifiableDkg<E>,
     ) -> Result<DecryptionShareSimple<E>> {
-        let validator_private_key_share = self.decrypt_private_key_share(
-            validator_decryption_key,
-            validator_index,
-        );
+        let validator_private_key_share = self
+            .decrypt_private_key_share(validator_decryption_key, share_index);
         let h = dkg.pvss_params.h;
-        let domain_point = dkg.domain.element(validator_index);
+        let domain_point = dkg.domain.element(share_index);
         let refreshed_private_key_share = refresh_private_key_share(
             &h,
             &domain_point,
             polynomial,
             &validator_private_key_share,
         );
         DecryptionShareSimple::create(
-            validator_index,
             validator_decryption_key,
             &refreshed_private_key_share,
             ciphertext,
             aad,
             &dkg.pvss_params.g_inv(),
         )
         .map_err(|e| e.into())
     }
 
     pub fn update_private_key_share_for_recovery(
         &self,
         validator_decryption_key: &E::ScalarField,
-        validator_index: usize,
+        share_index: usize,
         share_updates: &[E::G2],
     ) -> PrivateKeyShare<E> {
         // Retrieves their private key share
-        let private_key_share = self.decrypt_private_key_share(
-            validator_decryption_key,
-            validator_index,
-        );
+        let private_key_share = self
+            .decrypt_private_key_share(validator_decryption_key, share_index);
 
         // And updates their share
         update_share_for_recovery::<E>(&private_key_share, share_updates)
     }
 }
 
 /// Aggregate the PVSS instances in `pvss` from DKG session `dkg`
 /// into a new PVSS instance
 /// See: https://nikkolasg.github.io/ferveo/pvss.html?highlight=aggregate#aggregation
 pub fn aggregate<E: Pairing>(
-    dkg: &PubliclyVerifiableDkg<E>,
+    pvss_map: &PVSSMap<E>,
 ) -> PubliclyVerifiableSS<E, Aggregated> {
-    let pvss = &dkg.vss;
-    let mut pvss_iter = pvss.iter();
+    let mut pvss_iter = pvss_map.iter();
     let (_, first_pvss) = pvss_iter
         .next()
         .expect("May not aggregate empty PVSS instances");
     let mut coeffs = batch_to_projective_g1::<E>(&first_pvss.coeffs);
     let mut sigma = first_pvss.sigma;
 
     let mut shares = batch_to_projective_g2::<E>(&first_pvss.shares);
@@ -397,53 +449,58 @@
 }
 
 #[cfg(test)]
 mod test_pvss {
     use ark_bls12_381::Bls12_381 as EllipticCurve;
     use ark_ec::AffineRepr;
     use ark_ff::UniformRand;
+    use ferveo_common::is_sorted;
+    use rand::seq::SliceRandom;
 
     use super::*;
-    use crate::dkg::pv::test_common::*;
+    use crate::dkg::test_common::*;
 
     type ScalarField = <EllipticCurve as Pairing>::ScalarField;
     type G1 = <EllipticCurve as Pairing>::G1Affine;
     type G2 = <EllipticCurve as Pairing>::G2Affine;
 
     /// Test the happy flow that a pvss with the correct form is created
     /// and that appropriate validations pass
     #[test]
     fn test_new_pvss() {
         let rng = &mut ark_std::test_rng();
-        let dkg = setup_dkg(0);
+        let (dkg, _) = setup_dkg(0);
         let s = ScalarField::rand(rng);
         let pvss =
             Pvss::<EllipticCurve>::new(&s, &dkg, rng).expect("Test failed");
-        // check that the chosen secret coefficient is correct
+        // Check that the chosen secret coefficient is correct
         assert_eq!(pvss.coeffs[0], G1::generator().mul(s));
-        //check that a polynomial of the correct degree was created
-        assert_eq!(pvss.coeffs.len(), dkg.params.security_threshold as usize);
-        // check that the correct number of shares were created
+        // Check that a polynomial of the correct degree was created
+        assert_eq!(
+            pvss.coeffs.len(),
+            dkg.dkg_params.security_threshold as usize
+        );
+        // Check that the correct number of shares were created
         assert_eq!(pvss.shares.len(), dkg.validators.len());
-        // check that the prove of knowledge is correct
+        // Check that the prove of knowledge is correct
         assert_eq!(pvss.sigma, G2::generator().mul(s));
-        // check that the optimistic verify returns true
+        // Check that the optimistic verify returns true
         assert!(pvss.verify_optimistic());
-        // check that the full verify returns true
+        // Check that the full verify returns true
         assert!(pvss.verify_full(&dkg));
     }
 
     /// Check that if the proof of knowledge is wrong,
     /// the optimistic verification of PVSS fails
     #[test]
     fn test_verify_pvss_wrong_proof_of_knowledge() {
         let rng = &mut ark_std::test_rng();
-        let dkg = setup_dkg(0);
+        let (dkg, _) = setup_dkg(0);
         let mut s = ScalarField::rand(rng);
-        // ensure that the proof of knowledge is not zero
+        // Ensure that the proof of knowledge is not zero
         while s == ScalarField::zero() {
             s = ScalarField::rand(rng);
         }
         let mut pvss =
             PubliclyVerifiableSS::<EllipticCurve>::new(&s, &dkg, rng)
                 .expect("Test failed");
 
@@ -451,15 +508,15 @@
         assert!(!pvss.verify_optimistic());
     }
 
     /// Check that if PVSS shares are tampered with, the full verification fails
     #[test]
     fn test_verify_pvss_bad_shares() {
         let rng = &mut ark_std::test_rng();
-        let dkg = setup_dkg(0);
+        let (dkg, _) = setup_dkg(0);
         let s = ScalarField::rand(rng);
         let pvss = Pvss::<EllipticCurve>::new(&s, &dkg, rng).unwrap();
 
         // So far, everything works
         assert!(pvss.verify_optimistic());
         assert!(pvss.verify_full(&dkg));
 
@@ -469,47 +526,77 @@
 
         // Optimistic verification should not catch this issue
         assert!(bad_pvss.verify_optimistic());
         // Full verification should catch this issue
         assert!(!bad_pvss.verify_full(&dkg));
     }
 
+    /// Check that the explicit ordering of validators is expected and enforced
+    /// by the DKG methods.
+    #[test]
+    fn test_ordering_of_validators_is_enforced() {
+        let rng = &mut ark_std::test_rng();
+
+        let shares_num = 4;
+        let security_threshold = shares_num - 1;
+        let keypairs = gen_keypairs(shares_num);
+        let mut validators = gen_validators(&keypairs);
+        let me = validators[0].clone();
+
+        // Validators are not sorted
+        validators.shuffle(rng);
+        assert!(!is_sorted(&validators));
+
+        // And because of that the DKG should fail
+        let result = PubliclyVerifiableDkg::new(
+            &validators,
+            &DkgParams {
+                tau: 0,
+                security_threshold,
+                shares_num,
+            },
+            &me,
+        );
+        assert!(result.is_err());
+        assert_eq!(
+            result.unwrap_err().to_string(),
+            Error::ValidatorsNotSorted.to_string()
+        );
+    }
+
     /// Check that happy flow of aggregating PVSS transcripts
     /// Should have the correct form and validations pass
     #[test]
     fn test_aggregate_pvss() {
-        let dkg = setup_dealt_dkg();
-        let aggregate = aggregate(&dkg);
-        //check that a polynomial of the correct degree was created
+        let (dkg, _) = setup_dealt_dkg();
+        let aggregate = aggregate(&dkg.vss);
+        // Check that a polynomial of the correct degree was created
         assert_eq!(
             aggregate.coeffs.len(),
-            dkg.params.security_threshold as usize
+            dkg.dkg_params.security_threshold as usize
         );
-        // check that the correct number of shares were created
+        // Check that the correct number of shares were created
         assert_eq!(aggregate.shares.len(), dkg.validators.len());
-        // check that the optimistic verify returns true
+        // Check that the optimistic verify returns true
         assert!(aggregate.verify_optimistic());
-        // check that the full verify returns true
+        // Check that the full verify returns true
         assert!(aggregate.verify_full(&dkg));
-        // check that the verification of aggregation passes
-        assert_eq!(
-            aggregate.verify_aggregation(&dkg).expect("Test failed"),
-            dkg.validators.len() as u32
-        );
+        // Check that the verification of aggregation passes
+        assert!(aggregate.verify_aggregation(&dkg).expect("Test failed"),);
     }
 
     /// Check that if the aggregated pvss transcript has an
     /// incorrect constant term, the verification fails
     #[test]
     fn test_verify_aggregation_fails_if_constant_term_wrong() {
-        let dkg = setup_dealt_dkg();
-        let mut aggregated = aggregate(&dkg);
+        let (dkg, _) = setup_dealt_dkg();
+        let mut aggregated = aggregate(&dkg.vss);
         while aggregated.coeffs[0] == G1::zero() {
-            let dkg = setup_dkg(0);
-            aggregated = aggregate(&dkg);
+            let (dkg, _) = setup_dkg(0);
+            aggregated = aggregate(&dkg.vss);
         }
         aggregated.coeffs[0] = G1::zero();
         assert_eq!(
             aggregated
                 .verify_aggregation(&dkg)
                 .expect_err("Test failed")
                 .to_string(),
```

### Comparing `ferveo-0.1.7/local_dependencies/ferveo-common/src/serialization.rs` & `ferveo-0.1.8/local_dependencies/ferveo-common/src/serialization.rs`

 * *Files 3% similar despite different names*

```diff
@@ -25,29 +25,29 @@
         val: impl CanonicalSerialize,
         serializer: S,
     ) -> Result<S::Ok, S::Error>
     where
         S: serde::Serializer,
     {
         let mut bytes = vec![];
-        val.serialize_uncompressed(&mut bytes)
+        val.serialize_compressed(&mut bytes)
             .map_err(serde::ser::Error::custom)?;
 
         Bytes::serialize_as(&bytes, serializer)
     }
 
     /// You can use this to deserialize an arkworks type with serde and the "deserialize_with" attribute.
     /// See <https://serde.rs/field-attrs.html>
     pub fn deserialize<'de, T, D>(deserializer: D) -> Result<T, D::Error>
     where
         T: CanonicalDeserialize,
         D: serde::Deserializer<'de>,
     {
         let bytes: Vec<u8> = Bytes::deserialize_as(deserializer)?;
-        T::deserialize_uncompressed(&mut &bytes[..])
+        T::deserialize_compressed(&mut &bytes[..])
             .map_err(serde::de::Error::custom)
     }
 }
 
 //
 // Serialization with [serde_with]
 //
@@ -63,15 +63,15 @@
     T: CanonicalSerialize,
 {
     fn serialize_as<S>(val: &T, serializer: S) -> Result<S::Ok, S::Error>
     where
         S: serde::Serializer,
     {
         let mut bytes = vec![];
-        val.serialize_uncompressed(&mut bytes)
+        val.serialize_compressed(&mut bytes)
             .map_err(serde::ser::Error::custom)?;
 
         Bytes::serialize_as(&bytes, serializer)
     }
 }
 
 impl<'de, T> serde_with::DeserializeAs<'de, T> for SerdeAs
@@ -79,15 +79,15 @@
     T: CanonicalDeserialize,
 {
     fn deserialize_as<D>(deserializer: D) -> Result<T, D::Error>
     where
         D: serde::Deserializer<'de>,
     {
         let bytes: Vec<u8> = Bytes::deserialize_as(deserializer)?;
-        T::deserialize_uncompressed(&mut &bytes[..])
+        T::deserialize_compressed(&mut &bytes[..])
             .map_err(serde::de::Error::custom)
     }
 }
 
 // TODO: Trait aliases are experimental
 // trait ByteSerializable = ToBytes + FromBytes;
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/Cargo.toml` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/Cargo.toml`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -12,33 +12,33 @@
 bench = false
 
 [features]
 test-common = []
 api = []
 
 [dependencies]
-subproductdomain = { path = "../subproductdomain" }
-ferveo-common = { path = "../ferveo-common" }
-rand_core = "0.6"
-rand = "0.8"
-thiserror = "1.0"
-miracl_core = "=2.3.0"
-ark-ff = "0.4"
+ark-bls12-381 = "0.4"
 ark-ec = "0.4"
+ark-ff = "0.4"
 ark-poly = "0.4"
 ark-serialize = "0.4"
 ark-std = "0.4"
-ark-bls12-381 = "0.4"
-itertools = "0.10"
+bincode = "1.3.3"
 chacha20poly1305 = "0.10.1"
+ferveo-common = { path = "../ferveo-common" }
+itertools = "0.10"
+miracl_core = "=2.3.0"
+rand = "0.8"
+rand_core = "0.6"
 serde = { version = "1.0", features = ["derive"] }
+serde_bytes = "0.11.9"
 serde_with = "2.0.1"
-bincode = "1.3.3"
 sha2 = "0.10.6"
-serde_bytes = "0.11.9"
+subproductdomain = { path = "../subproductdomain" }
+thiserror = "1.0"
 
 [package.metadata.cargo-machete]
 ignored = ["serde_bytes"]
 
 [[bench]]
 name = "tpke"
 path = "benches/tpke.rs"
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/BENCHMARK.md` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/BENCHMARK.md`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/benches/arkworks.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/benches/arkworks.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/benches/tpke.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/benches/tpke.rs`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,14 @@
                     // This way we could test the performance of this method for a single participant.
                     setup
                         .contexts
                         .iter()
                         .map(|ctx| {
                             // Using create_unchecked here to avoid the cost of verifying the ciphertext
                             DecryptionShareSimple::create_unchecked(
-                                ctx.index,
                                 &ctx.validator_private_key,
                                 &ctx.private_key_share,
                                 &setup.shared.ciphertext,
                             )
                         })
                         .collect::<Vec<_>>()
                 })
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/api.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/api.rs`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 pub use crate::{
     decrypt_symmetric, decrypt_with_shared_secret, encrypt,
     prepare_combine_simple, share_combine_precomputed, share_combine_simple,
 };
 
 #[serde_as]
-#[derive(Copy, Clone, Debug, PartialEq, Serialize, Deserialize)]
+#[derive(Copy, Clone, Debug, PartialEq, Eq, Serialize, Deserialize)]
 pub struct DomainPoint(#[serde_as(as = "serialization::SerdeAs")] pub Fr);
 
 #[serde_as]
 #[derive(Copy, Clone, Debug, PartialEq, Serialize, Deserialize)]
 pub struct SharedSecret(
     #[serde_as(as = "serialization::SerdeAs")] pub TargetField,
 );
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/ciphertext.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/ciphertext.rs`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 use serde::{Deserialize, Serialize};
 use serde_with::serde_as;
 use sha2::{digest::Digest, Sha256};
 
 use crate::{htp_bls12381_g2, Error, Result};
 
 #[serde_as]
-#[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
+#[derive(Clone, Debug, PartialEq, Eq, Serialize, Deserialize)]
 pub struct Ciphertext<E: Pairing> {
     // U
     #[serde_as(as = "serialization::SerdeAs")]
     pub commitment: E::G1Affine,
 
     // W
     #[serde_as(as = "serialization::SerdeAs")]
@@ -39,15 +39,15 @@
             [hash_g2, self.auth_tag.into()],
         )
         .0 == E::TargetField::one())
     }
 
     fn construct_tag_hash(&self) -> Result<E::G2Affine> {
         let mut hash_input = Vec::<u8>::new();
-        self.commitment.serialize_uncompressed(&mut hash_input)?;
+        self.commitment.serialize_compressed(&mut hash_input)?;
         hash_input.extend_from_slice(&self.ciphertext);
 
         hash_to_g2(&hash_input)
     }
 
     pub fn serialized_length(&self) -> usize {
         self.commitment.serialized_size(Compress::No)
@@ -169,44 +169,44 @@
     result.to_vec()
 }
 
 pub fn shared_secret_to_chacha<E: Pairing>(
     s: &E::TargetField,
 ) -> Result<ChaCha20Poly1305> {
     let mut prf_key = Vec::new();
-    s.serialize_uncompressed(&mut prf_key)?;
+    s.serialize_compressed(&mut prf_key)?;
     let prf_key_32 = sha256(&prf_key);
 
     Ok(ChaCha20Poly1305::new(GenericArray::from_slice(&prf_key_32)))
 }
 
 fn nonce_from_commitment<E: Pairing>(commitment: E::G1Affine) -> Result<Nonce> {
     let mut commitment_bytes = Vec::new();
-    commitment.serialize_uncompressed(&mut commitment_bytes)?;
+    commitment.serialize_compressed(&mut commitment_bytes)?;
     let commitment_hash = sha256(&commitment_bytes);
     Ok(*Nonce::from_slice(&commitment_hash[..12]))
 }
 
 fn hash_to_g2<T: ark_serialize::CanonicalDeserialize>(
     message: &[u8],
 ) -> Result<T> {
     let point = htp_bls12381_g2(message);
     let mut point_ser: Vec<u8> = Vec::new();
-    point.serialize_uncompressed(&mut point_ser)?;
-    T::deserialize_uncompressed(&point_ser[..])
+    point.serialize_compressed(&mut point_ser)?;
+    T::deserialize_compressed(&point_ser[..])
         .map_err(Error::ArkworksSerializationError)
 }
 
 fn construct_tag_hash<E: Pairing>(
     commitment: E::G1Affine,
     stream_ciphertext: &[u8],
     aad: &[u8],
 ) -> Result<E::G2Affine> {
     let mut hash_input = Vec::<u8>::new();
-    commitment.serialize_uncompressed(&mut hash_input)?;
+    commitment.serialize_compressed(&mut hash_input)?;
     hash_input.extend_from_slice(stream_ciphertext);
     hash_input.extend_from_slice(aad);
     hash_to_g2(&hash_input)
 }
 
 #[cfg(test)]
 mod tests {
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/combine.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/combine.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/context.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,14 @@
 impl<E: Pairing> PrivateDecryptionContextSimple<E> {
     pub fn create_share(
         &self,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
     ) -> Result<DecryptionShareSimple<E>> {
         DecryptionShareSimple::create(
-            self.index,
             &self.validator_private_key,
             &self.private_key_share,
             ciphertext,
             aad,
             &self.setup_params.g_inv,
         )
     }
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/decryption.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/decryption.rs`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 pub struct DecryptionShareFast<E: Pairing> {
     pub decrypter_index: usize,
     #[serde_as(as = "serialization::SerdeAs")]
     pub decryption_share: E::G1Affine,
 }
 
 #[serde_as]
-#[derive(Serialize, Deserialize, Debug, Clone, PartialEq)]
+#[derive(Serialize, Deserialize, Debug, Clone, PartialEq, Eq)]
 pub struct ValidatorShareChecksum<E: Pairing> {
     #[serde_as(as = "serialization::SerdeAs")]
     pub checksum: E::G1Affine,
 }
 
 impl<E: Pairing> ValidatorShareChecksum<E> {
     pub fn new(
@@ -69,51 +69,46 @@
         }
 
         true
     }
 }
 
 #[serde_as]
-#[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
+#[derive(Clone, Debug, PartialEq, Eq, Serialize, Deserialize)]
 #[serde(bound(
     serialize = "ValidatorShareChecksum<E>: Serialize",
     deserialize = "ValidatorShareChecksum<E>: DeserializeOwned"
 ))]
 pub struct DecryptionShareSimple<E: Pairing> {
-    // TODO: Add decryptor public key? Replace decryptor_index with public key?
-    pub decrypter_index: usize,
     #[serde_as(as = "serialization::SerdeAs")]
     pub decryption_share: E::TargetField,
     pub validator_checksum: ValidatorShareChecksum<E>,
 }
 
 impl<E: Pairing> DecryptionShareSimple<E> {
     /// Create a decryption share from the given parameters.
     /// This function checks that the ciphertext is valid.
     pub fn create(
-        validator_index: usize,
         validator_decryption_key: &E::ScalarField,
         private_key_share: &PrivateKeyShare<E>,
         ciphertext: &Ciphertext<E>,
         aad: &[u8],
         g_inv: &E::G1Prepared,
     ) -> Result<Self> {
         check_ciphertext_validity::<E>(ciphertext, aad, g_inv)?;
         Self::create_unchecked(
-            validator_index,
             validator_decryption_key,
             private_key_share,
             ciphertext,
         )
     }
 
     /// Create a decryption share from the given parameters.
     /// This function does not check that the ciphertext is valid.
     pub fn create_unchecked(
-        validator_index: usize,
         validator_decryption_key: &E::ScalarField,
         private_key_share: &PrivateKeyShare<E>,
         ciphertext: &Ciphertext<E>,
     ) -> Result<Self> {
         // D_i = e(U, Z_i)
         let decryption_share = E::pairing(
             ciphertext.commitment,
@@ -121,15 +116,14 @@
         )
         .0;
 
         let validator_checksum =
             ValidatorShareChecksum::new(validator_decryption_key, ciphertext)?;
 
         Ok(Self {
-            decrypter_index: validator_index,
             decryption_share,
             validator_checksum,
         })
     }
     /// Verify that the decryption share is valid.
     pub fn verify(
         &self,
@@ -145,15 +139,15 @@
             h,
             ciphertext,
         )
     }
 }
 
 #[serde_as]
-#[derive(Clone, Debug, PartialEq, Serialize, Deserialize)]
+#[derive(Clone, Debug, PartialEq, Eq, Serialize, Deserialize)]
 #[serde(bound(
     serialize = "ValidatorShareChecksum<E>: Serialize",
     deserialize = "ValidatorShareChecksum<E>: DeserializeOwned"
 ))]
 pub struct DecryptionSharePrecomputed<E: Pairing> {
     pub decrypter_index: usize,
     #[serde_as(as = "serialization::SerdeAs")]
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/hash_to_curve.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/key_share.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/key_share.rs`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     pub fn multiply_by_omega_inv(&mut self, omega_inv: &E::ScalarField) {
         self.blinded_key_share =
             self.blinded_key_share.mul(-*omega_inv).into_affine();
     }
 }
 
-#[derive(Debug, Clone, PartialEq)]
+#[derive(Debug, Clone, PartialEq, Eq)]
 pub struct PrivateKeyShare<E: Pairing> {
     pub private_key_share: E::G2Affine,
 }
 
 impl<E: Pairing> PrivateKeyShare<E> {
     pub fn blind(&self, b: E::ScalarField) -> BlindedKeyShare<E> {
         let blinding_key = E::G2Affine::generator().mul(b).into_affine();
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/lib.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -29,31 +29,19 @@
 #[derive(Debug, thiserror::Error)]
 pub enum Error {
     /// Ciphertext verification failed
     /// Refers to the check 4.4.2 in the paper: https://eprint.iacr.org/2022/898.pdf
     #[error("Ciphertext verification failed")]
     CiphertextVerificationFailed,
 
-    /// Symmetric ciphertext decryption failed
-    #[error("Ciphertext decryption failed")]
-    CiphertextDecryptionFailed,
-
     /// Decryption share verification failed
     /// Refers to the check 4.4.4 in the paper: https://eprint.iacr.org/2022/898.pdf
     #[error("Decryption share verification failed")]
     DecryptionShareVerificationFailed,
 
-    /// Hashing to curve failed
-    #[error("Could not hash to curve")]
-    HashToCurveError,
-
-    /// Plaintext verification failed
-    #[error("Plaintext verification failed")]
-    PlaintextVerificationFailed,
-
     /// Serialization failed
     #[error("Bytes serialization failed")]
     BytesSerializationError(#[from] bincode::Error),
 
     /// Symmetric encryption failed"
     #[error("Symmetric encryption failed")]
     SymmetricEncryptionError(chacha20poly1305::aead::Error),
@@ -725,15 +713,15 @@
         // Now, we're going to recover a new share at a random point and check that the shared secret is still the same
 
         // Our random point
         let x_r = ScalarField::rand(rng);
 
         // Remove one participant from the contexts and all nested structures
         let mut remaining_participants = contexts.clone();
-        let removed_participant = remaining_participants.pop().unwrap();
+        remaining_participants.pop().unwrap();
         for p in &mut remaining_participants {
             p.public_decryption_contexts.pop().unwrap();
         }
 
         let new_share_fragments = make_new_share_fragments(
             rng,
             threshold,
@@ -757,18 +745,16 @@
         let mut decryption_shares: Vec<_> = remaining_participants
             .iter()
             .map(|c| c.create_share(&ciphertext, aad).unwrap())
             .collect();
 
         // Create a decryption share from a recovered private key share
         let new_validator_decryption_key = ScalarField::rand(rng);
-        let validator_index = removed_participant.index;
         decryption_shares.push(
             DecryptionShareSimple::create(
-                validator_index,
                 &new_validator_decryption_key,
                 &new_private_key_share,
                 &ciphertext,
                 aad,
                 g_inv,
             )
             .unwrap(),
@@ -824,15 +810,14 @@
                 let private_key_share = refresh_private_key_share::<E>(
                     &p.setup_params.h.into_group(),
                     &p.public_decryption_contexts[i].domain,
                     &polynomial,
                     &p.private_key_share,
                 );
                 DecryptionShareSimple::create(
-                    p.index,
                     &p.validator_private_key,
                     &private_key_share,
                     &ciphertext,
                     aad,
                     g_inv,
                 )
                 .unwrap()
```

### Comparing `ferveo-0.1.7/local_dependencies/group-threshold-cryptography/src/refresh.rs` & `ferveo-0.1.8/local_dependencies/group-threshold-cryptography/src/refresh.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/local_dependencies/subproductdomain/src/lib.rs` & `ferveo-0.1.8/local_dependencies/subproductdomain/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/LICENSE` & `ferveo-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ferveo-0.1.7/examples/server_api_precomputed.py` & `ferveo-0.1.8/examples/server_api_simple.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-import os
-
 from ferveo_py import (
     encrypt,
-    combine_decryption_shares_precomputed,
+    combine_decryption_shares_simple,
     decrypt_with_shared_secret,
     Keypair,
-    PublicKey,
-    ExternalValidator,
-    Transcript,
+    Validator,
     Dkg,
-    Ciphertext,
-    UnblindingKey,
-    DecryptionSharePrecomputed,
     AggregatedTranscript,
-    DkgPublicKey,
-    DkgPublicParameters,
-    SharedSecret,
 )
 
+
+def gen_eth_addr(i: int) -> str:
+    return f"0x{i:040x}"
+
+
 tau = 1
+security_threshold = 3
 shares_num = 4
-# In precomputed variant, security threshold must be equal to shares_num
-security_threshold = shares_num
 validator_keypairs = [Keypair.random() for _ in range(0, shares_num)]
 validators = [
-    ExternalValidator(f"validator-{i}", keypair.public_key)
+    Validator(gen_eth_addr(i), keypair.public_key())
     for i, keypair in enumerate(validator_keypairs)
 ]
 
+# Validators must be sorted by their public key
+validators.sort(key=lambda v: v.address)
+
 # Each validator holds their own DKG instance and generates a transcript every
 # validator, including themselves
 messages = []
 for sender in validators:
     dkg = Dkg(
         tau=tau,
         shares_num=shares_num,
@@ -47,23 +44,25 @@
 dkg = Dkg(
     tau=tau,
     shares_num=shares_num,
     security_threshold=security_threshold,
     validators=validators,
     me=me,
 )
+
 # Let's say that we've only received `security_threshold` transcripts
 messages = messages[:security_threshold]
-pvss_aggregated = dkg.aggregate_transcripts(messages)
-assert pvss_aggregated.validate(dkg)
 
-# Server can persist transcripts and the aggregated transcript
-transcripts_ser = [bytes(transcript) for _, transcript in messages]
-_transcripts_deser = [Transcript.from_bytes(t) for t in transcripts_ser]
-agg_transcript_ser = bytes(pvss_aggregated)
+# Server can aggregate the transcripts
+server_aggregate = dkg.aggregate_transcripts(messages)
+assert server_aggregate.verify(shares_num, messages)
+
+# And the client can also aggregate and verify the transcripts
+client_aggregate = AggregatedTranscript(messages)
+assert client_aggregate.verify(shares_num, messages)
 
 # In the meantime, the client creates a ciphertext and decryption request
 msg = "abc".encode()
 aad = "my-aad".encode()
 ciphertext = encrypt(msg, aad, dkg.final_key)
 
 # The client can serialize/deserialize ciphertext for transport
@@ -75,32 +74,31 @@
     dkg = Dkg(
         tau=tau,
         shares_num=shares_num,
         security_threshold=security_threshold,
         validators=validators,
         me=validator,
     )
-    # Assume the aggregated transcript is obtained through deserialization from a side-channel
-    agg_transcript_deser = AggregatedTranscript.from_bytes(agg_transcript_ser)
-    agg_transcript_deser.validate(dkg)
+
+    # We can also obtain the aggregated transcript from the side-channel (deserialize)
+    aggregate = AggregatedTranscript(messages)
+    assert aggregate.verify(shares_num, messages)
 
     # The ciphertext is obtained from the client
-    ciphertext_deser = Ciphertext.from_bytes(ciphertext_ser)
 
     # Create a decryption share for the ciphertext
-    decryption_share = agg_transcript_deser.create_decryption_share_precomputed(
+    decryption_share = aggregate.create_decryption_share_simple(
         dkg, ciphertext, aad, validator_keypair
     )
     decryption_shares.append(decryption_share)
 
 # Now, the decryption share can be used to decrypt the ciphertext
 # This part is in the client API
 
-# The client should have access to the public parameters of the DKG
-dkg_public_params_ser = bytes(dkg.public_params)
-dkg_public_params_deser = DkgPublicParameters.from_bytes(dkg_public_params_ser)
+shared_secret = combine_decryption_shares_simple(decryption_shares, dkg.public_params)
 
-shared_secret = combine_decryption_shares_precomputed(decryption_shares)
+# The client should have access to the public parameters of the DKG
 
-plaintext = decrypt_with_shared_secret(ciphertext, aad, shared_secret, dkg_public_params_deser)
+plaintext = decrypt_with_shared_secret(ciphertext, aad, shared_secret, dkg.public_params)
 assert bytes(plaintext) == msg
 
+print("Success!")
```

### Comparing `ferveo-0.1.7/ferveo/__init__.pyi` & `ferveo-0.1.8/ferveo/__init__.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -7,33 +7,38 @@
         ...
 
     @staticmethod
     def from_secure_randomness(data: bytes) -> Keypair:
         ...
 
     @staticmethod
+    def secure_randomness_size(data: bytes) -> int:
+        ...
+
+    @staticmethod
     def from_bytes(data: bytes) -> Keypair:
         ...
 
     def __bytes__(self) -> bytes:
         ...
 
-    public_key: PublicKey
+    def public_key(self) -> PublicKey:
+        ...
 
 
 class PublicKey:
     @staticmethod
     def from_bytes(data: bytes) -> PublicKey:
         ...
 
     def __bytes__(self) -> bytes:
         ...
 
 
-class ExternalValidator:
+class Validator:
 
     def __init__(self, address: str, public_key: PublicKey):
         ...
 
     address: str
 
     public_key: PublicKey
@@ -60,49 +65,39 @@
 class Dkg:
 
     def __init__(
             self,
             tau: int,
             shares_num: int,
             security_threshold: int,
-            validators: Sequence[ExternalValidator],
-            me: ExternalValidator,
+            validators: Sequence[Validator],
+            me: Validator,
     ):
         ...
 
     final_key: DkgPublicKey
 
     public_params: DkgPublicParameters
 
     def generate_transcript(self) -> Transcript:
         ...
 
-    def aggregate_transcripts(self, transcripts: Sequence[(ExternalValidator, Transcript)]) -> Transcript:
+    def aggregate_transcripts(self, messages: Sequence[(Validator, Transcript)]) -> AggregatedTranscript:
         ...
 
 
 class Ciphertext:
     @staticmethod
     def from_bytes(data: bytes) -> Ciphertext:
         ...
 
     def __bytes__(self) -> bytes:
         ...
 
 
-class UnblindingKey:
-
-    @staticmethod
-    def from_bytes(data: bytes) -> Keypair:
-        ...
-
-    def __bytes__(self) -> bytes:
-        ...
-
-
 class DecryptionShareSimple:
     @staticmethod
     def from_bytes(data: bytes) -> DecryptionShareSimple:
         ...
 
     def __bytes__(self) -> bytes:
         ...
@@ -124,14 +119,20 @@
 
     def __bytes__(self) -> bytes:
         ...
 
 
 class AggregatedTranscript:
 
+    def __init__(self, messages: Sequence[(Validator, Transcript)]):
+        ...
+
+    def verify(self, shares_num: int, messages: Sequence[(Validator, Transcript)]) -> bool:
+        ...
+
     def create_decryption_share_simple(
             self,
             dkg: Dkg,
             ciphertext: Ciphertext,
             aad: bytes,
             validator_keypair: Keypair
     ) -> DecryptionShareSimple:
@@ -142,35 +143,23 @@
             dkg: Dkg,
             ciphertext: Ciphertext,
             aad: bytes,
             validator_keypair: Keypair
     ) -> DecryptionSharePrecomputed:
         ...
 
-    def validate(self, dkg: Dkg) -> bool:
-        ...
 
     @staticmethod
     def from_bytes(data: bytes) -> AggregatedTranscript:
         ...
 
     def __bytes__(self) -> bytes:
         ...
 
 
-class LagrangeCoefficient:
-
-    @staticmethod
-    def from_bytes(data: bytes) -> LagrangeCoefficient:
-        ...
-
-    def __bytes__(self) -> bytes:
-        ...
-
-
 class SharedSecret:
 
     @staticmethod
     def from_bytes(data: bytes) -> SharedSecret:
         ...
 
     def __bytes__(self) -> bytes:
@@ -179,15 +168,15 @@
 
 def encrypt(message: bytes, add: bytes, dkg_public_key: DkgPublicKey) -> Ciphertext:
     ...
 
 
 def combine_decryption_shares_simple(
         decryption_shares: Sequence[DecryptionShareSimple],
-        lagrange_coefficients: LagrangeCoefficient,
+        dkg_public_params: DkgPublicParameters,
 ) -> bytes:
     ...
 
 
 def combine_decryption_shares_precomputed(
         decryption_shares: Sequence[DecryptionSharePrecomputed],
 ) -> SharedSecret:
```

### Comparing `ferveo-0.1.7/setup.py` & `ferveo-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ferveo",
     description="Ferveo DKG scheme",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.1.7",
+    version="0.1.8",
     author="Piotr Roslaniec",
     author_email="p.roslaniec@gmail.com",
     url="https://github.com/nucypher/ferveo/tree/master/ferveo-python",
     rust_extensions=[RustExtension(
         "ferveo._ferveo", binding=Binding.PyO3, debug=False)],
     packages=["ferveo"],
     package_data={
```

### Comparing `ferveo-0.1.7/test/test_ferveo.py` & `ferveo-0.1.8/test/test_ferveo.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,24 @@
 
 from ferveo_py import (
     encrypt,
     combine_decryption_shares_simple,
     combine_decryption_shares_precomputed,
     decrypt_with_shared_secret,
     Keypair,
-    PublicKey,
-    ExternalValidator,
-    Transcript,
+    Validator,
     Dkg,
-    Ciphertext,
-    UnblindingKey,
-    DecryptionShareSimple,
-    DecryptionSharePrecomputed,
     AggregatedTranscript,
-    DkgPublicKey,
-    DkgPublicParameters,
-    SharedSecret,
 )
 
 
+def gen_eth_addr(i: int) -> str:
+    return f"0x{i:040x}"
+
+
 def decryption_share_for_variant(variant, agg_transcript):
     if variant == "simple":
         return agg_transcript.create_decryption_share_simple
     elif variant == "precomputed":
         return agg_transcript.create_decryption_share_precomputed
     else:
         raise ValueError("Unknown variant")
@@ -42,57 +37,64 @@
 def scenario_for_variant(variant, shares_num=4, security_threshold=3):
     if variant not in ["simple", "precomputed"]:
         raise ValueError("Unknown variant: " + variant)
 
     tau = 1
     validator_keypairs = [Keypair.random() for _ in range(0, shares_num)]
     validators = [
-        ExternalValidator(f"validator-{i}", keypair.public_key)
+        Validator(gen_eth_addr(i), keypair.public_key())
         for i, keypair in enumerate(validator_keypairs)
     ]
+    validators.sort(key=lambda v: v.address)
+
     messages = []
     for sender in validators:
         dkg = Dkg(
             tau=tau,
             shares_num=shares_num,
             security_threshold=security_threshold,
             validators=validators,
             me=sender,
         )
         messages.append((sender, dkg.generate_transcript()))
+
     me = validators[0]
     dkg = Dkg(
         tau=tau,
         shares_num=shares_num,
         security_threshold=security_threshold,
         validators=validators,
         me=me,
     )
     pvss_aggregated = dkg.aggregate_transcripts(messages)
-    assert pvss_aggregated.validate(dkg)
+    assert pvss_aggregated.verify(shares_num, messages)
+
     msg = "abc".encode()
     aad = "my-aad".encode()
     ciphertext = encrypt(msg, aad, dkg.final_key)
+
     decryption_shares = []
     for validator, validator_keypair in zip(validators, validator_keypairs):
         dkg = Dkg(
             tau=tau,
             shares_num=shares_num,
             security_threshold=security_threshold,
             validators=validators,
             me=validator,
         )
         agg_transcript_deser = AggregatedTranscript.from_bytes(bytes(pvss_aggregated))
-        agg_transcript_deser.validate(dkg)
+        agg_transcript_deser.verify(shares_num, messages)
 
         decryption_share = decryption_share_for_variant('simple', agg_transcript_deser)(
             dkg, ciphertext, aad, validator_keypair
         )
         decryption_shares.append(decryption_share)
+
     shared_secret = combine_shares_for_variant('simple')(decryption_shares, dkg.public_params)
+
     plaintext = decrypt_with_shared_secret(ciphertext, aad, shared_secret, dkg.public_params)
     assert bytes(plaintext) == msg
 
 
 def test_tdec_workflow_for_simple_variant():
     # nr of shares must be a multiple of 2
     for shares_num in [2, 4, 8]:
```

### Comparing `ferveo-0.1.7/test/test_serialization.py` & `ferveo-0.1.8/test/test_serialization.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from ferveo_py import (
     Keypair,
-    PublicKey,
-    ExternalValidator,
-    Transcript,
+    Validator,
     Dkg,
-    AggregatedTranscript,
-    DkgPublicKey,
     DkgPublicParameters,
-    SharedSecret,
 )
 
+
+def gen_eth_addr(i: int) -> str:
+    return f"0x{i:040x}"
+
+
 tau = 1
 security_threshold = 3
 shares_num = 4
 validator_keypairs = [Keypair.random() for _ in range(shares_num)]
 validators = [
-    ExternalValidator(f"validator-{i}", keypair.public_key)
+    Validator(gen_eth_addr(i), keypair.public_key())
     for i, keypair in enumerate(validator_keypairs)
 ]
-
+validators.sort(key=lambda v: v.address)
 
 def make_dkg_public_params():
     me = validators[0]
     dkg = Dkg(
         tau=tau,
         shares_num=shares_num,
         security_threshold=security_threshold,
```

### Comparing `ferveo-0.1.7/Cargo.lock` & `ferveo-0.1.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 [[package]]
 name = "ahash"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2c99f64d1e06488f620f932677e24bc6e2897582980441ae90a671415bd7ec2f"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "android_system_properties"
 version = "0.1.5"
@@ -122,28 +122,28 @@
 [[package]]
 name = "ark-ff-asm"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fc8f7ec7fdcc20f3f110783c043d80479b42f500003cf92b71ca90f34a2ba0e"
 dependencies = [
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "ark-ff-macros"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "15aa320e38052d644e569740bad208e5f9f5fafedcc9e6b1557f723be1b7ff8d"
 dependencies = [
  "num-bigint",
  "num-traits",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "ark-poly"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "88d2e8741caf33ab3063f1fc65617716ffb18cba8e872998aa2eef0d4e4b56d1"
@@ -171,15 +171,15 @@
 name = "ark-serialize-derive"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "101333772a4020c883890811500d5ecc704c545a90140629af5c3b9f00d78953"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "ark-std"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94893f1e0c6eeab764ade8dc4c0db24caf4fe7cbbaafc0eba0a9030f447b5185"
@@ -215,15 +215,15 @@
 name = "backtrace"
 version = "0.3.67"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "233d376d6d185f2a3093e58f283f60f880315b6c60075b01f36b3b85154564ca"
 dependencies = [
  "addr2line",
  "cc",
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
@@ -290,31 +290,25 @@
 name = "cc"
 version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cfg-if"
-version = "0.1.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4785bdd1c96b2a846b2bd7cc02e86b6b3dbf14e7e53446c4f54c92a361040822"
-
-[[package]]
-name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chacha20"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7fc89c7c5b9e7a02dfe45cd2367bae382f9ed31c61ca8debe5f827c420a2f08"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "cipher",
  "cpufeatures",
 ]
 
 [[package]]
 name = "chacha20poly1305"
 version = "0.10.1"
@@ -423,15 +417,15 @@
 
 [[package]]
 name = "console_error_panic_hook"
 version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -439,15 +433,15 @@
 
 [[package]]
 name = "cpp_demangle"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eeaa953eaad386a53111e47172c2fedba671e5684c8dd601a5f474f4f118710f"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
 ]
 
 [[package]]
 name = "cpufeatures"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
@@ -529,49 +523,49 @@
 
 [[package]]
 name = "crossbeam-channel"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c2dd04ddaf88237dc3b8d8f9a3c1004b506b54b3313403944054d23c0870c521"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "715e8152b692bba2d374b53d4875445368fdf21a94751410af607a5ac677d1fc"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "crossbeam-epoch",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-epoch"
 version = "0.9.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "01a9af1f4c2ef74bb8aa1f7e19706bc72d03598c8a570bb5de72243c7a9d9d5a"
 dependencies = [
  "autocfg",
- "cfg-if 1.0.0",
+ "cfg-if",
  "crossbeam-utils",
  "memoffset 0.7.1",
  "scopeguard",
 ]
 
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb766fa798726286dbbb842f174001dab8abc7b627a1dd86e0b7222a95d929f"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
@@ -623,15 +617,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "457ce6757c5c70dc6ecdbda6925b958aae7f959bda7d8fb9bde889e34a09dc03"
@@ -640,15 +634,15 @@
 name = "cxxbridge-macro"
 version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ebf883b7aacd7b2aeb2a7b338648ee19f57c140d4ee8e52c68979c6b2f7f2263"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "darling"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0808e1bd8671fb44a113a14e13497557533369847788fa2ae912b6ebfce9fa8"
@@ -664,26 +658,26 @@
 checksum = "001d80444f28e193f30c2f293455da62dcf9a6b29918a4253152ae2b1de592cb"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
  "strsim",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b36230598a2d5de7ec1c6f51f72d8a99a9208daff41de2084d06e3fd3ea56685"
 dependencies = [
  "darling_core",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "debugid"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d6ee87af31d84ef885378aebca32be3d682b0e0dc119d5b4860a2c5bb5046730"
@@ -695,26 +689,26 @@
 name = "derivative"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fcc3dd5e9e9c0b295d6e1e4d811fb6f157d5ffd784b8d202fc62eac8035a770b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "derive_more"
 version = "0.99.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4fb810d30a7c1953f91334de7244731fc3f3c10d7fe163338a35b9f640960321"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "digest"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
@@ -749,14 +743,15 @@
  "ark-serialize",
  "ark-std",
  "bincode",
  "criterion 0.3.6",
  "digest",
  "ferveo-common",
  "group-threshold-cryptography",
+ "hex",
  "itertools",
  "measure_time",
  "pprof",
  "rand 0.7.3",
  "rand 0.8.5",
  "rand_core 0.6.4",
  "serde",
@@ -778,25 +773,46 @@
  "rand_core 0.6.4",
  "serde",
  "serde_with",
 ]
 
 [[package]]
 name = "ferveo-python"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "derive_more",
  "ferveo",
  "ferveo-common",
+ "itertools",
  "pyo3",
- "pyo3-build-config 0.17.3",
+ "pyo3-build-config",
  "rand 0.8.5",
 ]
 
 [[package]]
+name = "ferveo-wasm"
+version = "0.1.0"
+dependencies = [
+ "console_error_panic_hook",
+ "derive_more",
+ "ferveo",
+ "ferveo-common",
+ "getrandom 0.2.8",
+ "group-threshold-cryptography",
+ "itertools",
+ "js-sys",
+ "rand 0.8.5",
+ "rand_core 0.6.4",
+ "serde",
+ "wasm-bindgen",
+ "wasm-bindgen-derive",
+ "wasm-bindgen-test",
+]
+
+[[package]]
 name = "findshlibs"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "40b9e59cd0f7e0806cca4be089683ecb6434e602038df21fe6bf6711b2f07f64"
 dependencies = [
  "cc",
  "lazy_static",
@@ -822,26 +838,26 @@
 
 [[package]]
 name = "getrandom"
 version = "0.1.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8fc3cb4d91f53b50155bdcfd23f6a4c39ae1969c2ae85982b135750cccaf5fce"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
 
 [[package]]
@@ -998,15 +1014,15 @@
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "itertools"
@@ -1071,15 +1087,15 @@
 
 [[package]]
 name = "log"
 version = "0.4.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
 ]
 
 [[package]]
 name = "measure_time"
 version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56220900f1a0923789ecd6bf25fbae8af3b2f1ff3e9e297fc9b6b8674dd4d852"
@@ -1127,20 +1143,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
-name = "memory_units"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8452105ba047068f40ff7093dd1d9da90898e63dd61736462e9cdda6a90ad3c3"
-
-[[package]]
 name = "miniz_oxide"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
 dependencies = [
  "adler",
 ]
@@ -1155,15 +1165,15 @@
 name = "nix"
 version = "0.23.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f3790c00a0150112de0f4cd161e3d7fc4b2d8a5542ffc35f099a2562aecb35c"
 dependencies = [
  "bitflags",
  "cc",
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
  "memoffset 0.6.5",
 ]
 
 [[package]]
 name = "num-bigint"
 version = "0.4.3"
@@ -1270,29 +1280,29 @@
 
 [[package]]
 name = "parking_lot_core"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "instant",
  "libc",
  "redox_syscall",
  "smallvec",
  "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
@@ -1343,15 +1353,15 @@
 [[package]]
 name = "pprof"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55f35f865aa964be21fcde114cbd1cfbd9bf8a471460ed965b0f84f96c711401"
 dependencies = [
  "backtrace",
- "cfg-if 1.0.0",
+ "cfg-if",
  "criterion 0.3.6",
  "findshlibs",
  "inferno",
  "lazy_static",
  "libc",
  "log",
  "nix",
@@ -1366,50 +1376,40 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.51"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d727cae5b39d21da60fa540906919ad737832fe0b1c165da3a34d6548c849d6"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "indoc",
  "libc",
  "memoffset 0.8.0",
  "parking_lot 0.12.1",
- "pyo3-build-config 0.18.2",
+ "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
-dependencies = [
- "once_cell",
- "target-lexicon",
-]
-
-[[package]]
-name = "pyo3-build-config"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
@@ -1417,54 +1417,54 @@
 [[package]]
 name = "pyo3-ffi"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
 dependencies = [
  "libc",
- "pyo3-build-config 0.18.2",
+ "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
 version = "0.18.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "quick-xml"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8533f14c8382aaad0d592c812ac3b826162128b65662331e1127b45c3d18536b"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.7.3"
@@ -1692,15 +1692,15 @@
 name = "serde_derive"
 version = "1.0.152"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af487d118eecd09402d70a5d72551860e788df87b464af30e5ea6a38c75c541e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.93"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cad406b69c91885b5107daf2c29572f6c8cdb3c66826821e286c533490c0bc76"
@@ -1731,24 +1731,24 @@
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1966009f3c05f095697c537312f5415d1e3ed31ce0a56942bac4c771c5c335e"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
 ]
 
 [[package]]
 name = "sha2"
 version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "smallvec"
 version = "1.10.0"
@@ -1822,22 +1822,33 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.15"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "synstructure"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "unicode-xid",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1845,15 +1856,15 @@
 
 [[package]]
 name = "tempfile"
 version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5cdb1ef4eaeeaddc8fbd371e5017057064af0911902ef36b39801f67cc6d79e4"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "fastrand",
  "libc",
  "redox_syscall",
  "remove_dir_all",
  "winapi",
 ]
 
@@ -1879,30 +1890,30 @@
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
-version = "1.0.30"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "854babe52e4df1653706b98fcfc05843010039b406875930a70e4d9644e5c417"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.30"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aa32fd3f627f367fe16f893e2597ae3c05020f8bba2666a4e6ea73d377e5714b"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "time"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a561bf4617eebd33bca6434b988f39ed798e527f51a1e797d0ee4f61c0a38376"
@@ -1935,44 +1946,14 @@
 checksum = "be4d6b5f19ff7664e8c98d03e2139cb510db9b0a60b55f8e8709b689d939b6bc"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
-name = "tpke-python"
-version = "0.1.0"
-dependencies = [
- "ferveo-common",
- "group-threshold-cryptography",
- "pyo3",
- "pyo3-build-config 0.17.3",
-]
-
-[[package]]
-name = "tpke-wasm"
-version = "0.1.0-alpha.1"
-dependencies = [
- "ark-serialize",
- "console_error_panic_hook",
- "ferveo",
- "ferveo-common",
- "getrandom 0.2.8",
- "group-threshold-cryptography",
- "js-sys",
- "rand 0.8.5",
- "rand_core 0.6.4",
- "serde",
- "serde_with",
- "wasm-bindgen",
- "wasm-bindgen-test",
- "wee_alloc",
-]
-
-[[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
 [[package]]
 name = "unicode-ident"
@@ -2045,15 +2026,15 @@
 
 [[package]]
 name = "wasm-bindgen"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "serde",
  "serde_json",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
@@ -2062,25 +2043,38 @@
 checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
+name = "wasm-bindgen-derive"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c7301886930edaa72b7d102655ea395774aa9f0614c1a491393648a5fec34435"
+dependencies = [
+ "js-sys",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.107",
+ "wasm-bindgen",
+]
+
+[[package]]
 name = "wasm-bindgen-futures"
 version = "0.4.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
 dependencies = [
- "cfg-if 1.0.0",
+ "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
@@ -2096,15 +2090,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.84"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.84"
@@ -2142,26 +2136,14 @@
 checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
-name = "wee_alloc"
-version = "0.4.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb3b5a6b2bb17cb6ad44a2e68a43e8d2722c997da10e928665c72ec6c0a0b8e"
-dependencies = [
- "cfg-if 0.1.10",
- "libc",
- "memory_units",
- "winapi",
-]
-
-[[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
  "winapi-i686-pc-windows-gnu",
  "winapi-x86_64-pc-windows-gnu",
@@ -2267,10 +2249,10 @@
 name = "zeroize_derive"
 version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44bf07cb3e50ea2003396695d58bf46bc9887a1f362260446fad6bc4e79bd36c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.107",
  "synstructure",
 ]
```

### Comparing `ferveo-0.1.7/PKG-INFO` & `ferveo-0.1.8/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ferveo
-Version: 0.1.7
+Version: 0.1.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author: Piotr Roslaniec <p.roslaniec@gmail.com>
 Author-email: Piotr Roslaniec <p.roslaniec@gmail.com>
 Requires-Python: >=3.7
@@ -12,7 +12,14 @@
 
 # Python bindings for `ferveo`
 
 ## Build
 
 You will need to have `setuptools-rust` installed. Then, for development, you can just do `pip install -e .` as usual.
 
+## Publish
+
+```bash
+maturin build --release
+maturin publish
+```
+
```

