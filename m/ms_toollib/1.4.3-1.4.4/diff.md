# Comparing `tmp/ms_toollib-1.4.3.tar.gz` & `tmp/ms_toollib-1.4.4.tar.gz`

## Comparing `ms_toollib-1.4.3.tar` & `ms_toollib-1.4.4.tar`

### file list

```diff
@@ -1,7 +1,13 @@
--rw-r--r--   0        0        0        9 2022-01-24 09:59:18.000000 ms_toollib-1.4.3/.gitignore
--rw-r--r--   0        0        0     1533 2023-03-02 11:38:35.000000 ms_toollib-1.4.3/Cargo.toml
--rw-r--r--   0        0        0     1258 2023-03-02 11:30:30.000000 ms_toollib-1.4.3/pyproject.toml
--rw-r--r--   0        0        0       15 2022-01-24 09:59:18.000000 ms_toollib-1.4.3/readme.md
--rw-r--r--   0        0        0    60796 2023-03-02 10:29:23.000000 ms_toollib-1.4.3/src/board.rs
--rw-r--r--   0        0        0    10387 2023-03-02 11:30:49.000000 ms_toollib-1.4.3/src/lib.rs
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 ms_toollib-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0        9 2022-01-24 09:59:18.000000 ms_toollib-1.4.4/.gitignore
+-rw-r--r--   0        0        0     1629 2023-05-03 05:16:56.000000 ms_toollib-1.4.4/Cargo.toml
+-rw-r--r--   0        0        0     1258 2023-05-03 05:16:48.000000 ms_toollib-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0       15 2022-01-24 09:59:18.000000 ms_toollib-1.4.4/readme.md
+-rw-r--r--   0        0        0    10574 2023-04-24 11:27:39.000000 ms_toollib-1.4.4/src/avf_video.rs
+-rw-r--r--   0        0        0    13490 2023-05-02 06:24:42.000000 ms_toollib-1.4.4/src/base_video.rs
+-rw-r--r--   0        0        0     8340 2023-04-26 14:13:23.000000 ms_toollib-1.4.4/src/board.rs
+-rw-r--r--   0        0        0    10578 2023-04-24 11:26:27.000000 ms_toollib-1.4.4/src/evf_video.rs
+-rw-r--r--   0        0        0     2776 2023-04-27 13:10:22.000000 ms_toollib-1.4.4/src/gameboard.rs
+-rw-r--r--   0        0        0    10728 2023-04-27 04:53:18.000000 ms_toollib-1.4.4/src/lib.rs
+-rw-r--r--   0        0        0    10574 2023-04-24 11:27:32.000000 ms_toollib-1.4.4/src/mvf_video.rs
+-rw-r--r--   0        0        0    10570 2023-04-24 11:27:46.000000 ms_toollib-1.4.4/src/rmv_video.rs
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 ms_toollib-1.4.4/PKG-INFO
```

### Comparing `ms_toollib-1.4.3/Cargo.toml` & `ms_toollib-1.4.4/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ms_toollib"
-version = "1.4.3"
+version = "1.4.4"
 description = "Algorithms  for Minesweeper"
 documentation = "https://docs.rs/ms_toollib/"
 license = "MIT"
 readme = "readme.md"
 keywords = ["minesweeper", "possibility", "solver", "laymine", "3BV"]
 edition = "2021"
 authors = ["Wang Jianing <wangjianing@88.com>"]
@@ -40,11 +40,14 @@
 maintainer = "eee555"
 maintainer-email = "wangjn@88.com"
 requires-python = ">=3.7"
 project-url = { homepage = "https://github.com/eee555/" }
 
 
 
-
-
-
+# [profile.release]
+# opt-level = 'z'
+# lto = true
+# codegen-units = 1
+# panic = 'abort'
+# 4018
```

### Comparing `ms_toollib-1.4.3/pyproject.toml` & `ms_toollib-1.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ms_toollib"
-version = "1.4.3"
+version = "1.4.4"
 description = "Algorithms for minesweeper."
 readme = "readme.md"
 requires-python = ">=3.7"
 keywords = ["minesweeper", "possibility", "solver", "laymine", "3BV"]
 authors = [
   {email = "wangjianing@88.com"},
   {name = "Wang Jianing"}
```

### Comparing `ms_toollib-1.4.3/src/lib.rs` & `ms_toollib-1.4.4/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,33 @@
 use pyo3::wrap_pyfunction;
 // use pyo3::PyTraverseError;
 // use pyo3::class::basic::PyObjectProtocol;
 // use std::cmp::{max, min};
 
 use ms_toollib::*;
 mod board;
-pub use board::{
-    PyAvfVideo, PyBaseVideo, PyBoard, PyEvfVideo, PyGameBoard, PyMinesweeperBoard, PyMvfVideo,
-    PyRmvVideo,
-};
+pub use board::{PyMinesweeperBoard, PySafeMinesweeperBoard};
+
+mod gameboard;
+pub use gameboard::{PyBoard, PyGameBoard};
+
+mod base_video;
+pub use base_video::{PyBaseVideo, PySafeBoard};
+
+mod avf_video;
+pub use avf_video::PyAvfVideo;
+
+mod evf_video;
+pub use evf_video::PyEvfVideo;
+
+mod mvf_video;
+pub use mvf_video::PyMvfVideo;
+
+mod rmv_video;
+pub use rmv_video::PyRmvVideo;
 
 // pip install maturin
 // maturin publish --manylinux 2014
 
 #[pyfunction]
 #[pyo3(name = "refresh_matrix")]
 fn py_refresh_matrix(
@@ -36,15 +51,15 @@
 )> {
     Ok(refresh_matrixs(&board_of_game))
 }
 
 #[pyfunction]
 #[pyo3(name = "cal_op")]
 fn py_cal_op(board: Vec<Vec<i32>>) -> PyResult<usize> {
-    Ok(cal_op(board))
+    Ok(cal_op(&board))
 }
 
 #[pyfunction]
 #[pyo3(name = "laymine", text_signature = "(row, column, mine_num, x0, y0)")]
 fn py_laymine(
     row: usize,
     column: usize,
@@ -325,16 +340,18 @@
     m.add_function(wrap_pyfunction!(py_OBR_board, m)?)?;
     m.add_function(wrap_pyfunction!(py_cal_possibility_onboard, m)?)?;
     m.add_function(wrap_pyfunction!(py_mark_board, m)?)?;
     m.add_function(wrap_pyfunction!(py_is_guess_while_needless, m)?)?;
     m.add_function(wrap_pyfunction!(py_is_able_to_solve, m)?)?;
     m.add_function(wrap_pyfunction!(py_enuOneStep, m)?)?;
     m.add_class::<PyMinesweeperBoard>()?;
+    m.add_class::<PySafeMinesweeperBoard>()?;
     m.add_class::<PyAvfVideo>()?;
     m.add_class::<PyRmvVideo>()?;
     m.add_class::<PyMvfVideo>()?;
     m.add_class::<PyEvfVideo>()?;
     m.add_class::<PyBaseVideo>()?;
     m.add_class::<PyGameBoard>()?;
     m.add_class::<PyBoard>()?;
+    m.add_class::<PySafeBoard>()?;
     Ok(())
 }
```

### Comparing `ms_toollib-1.4.3/PKG-INFO` & `ms_toollib-1.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_toollib
-Version: 1.4.3
+Version: 1.4.4
 Classifiers: Development Status :: 4 - Beta
 Classifiers: License :: OSI Approved :: MIT License
 Classifiers: Programming Language :: Rust
 Classifiers: Programming Language :: Python
 Classifiers: Programming Language :: Python :: 3 :: Only
 Classifiers: Programming Language :: Python :: 3
 Classifiers: Programming Language :: Python :: 3.7
```

