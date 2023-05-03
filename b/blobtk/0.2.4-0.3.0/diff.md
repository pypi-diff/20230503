# Comparing `tmp/blobtk-0.2.4.tar.gz` & `tmp/blobtk-0.3.0.tar.gz`

## Comparing `blobtk-0.2.4.tar` & `blobtk-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,29 @@
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 blobtk-0.2.4/Cargo.toml
--rw-r--r--   0      501       20    27350 2023-02-23 14:04:20.000000 blobtk-0.2.4/Cargo.lock
--rw-r--r--   0      501       20      313 2023-02-23 14:04:20.000000 blobtk-0.2.4/pyproject.toml
--rw-r--r--   0      501       20     9018 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/bam.rs
--rw-r--r--   0      501       20     4849 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/cli.rs
--rw-r--r--   0      501       20      553 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/depth.rs
--rw-r--r--   0      501       20     1855 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/fasta.rs
--rw-r--r--   0      501       20     6177 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/fastq.rs
--rw-r--r--   0      501       20     1440 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/filter.rs
--rw-r--r--   0      501       20     2795 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/io.rs
--rw-r--r--   0      501       20      642 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/lib.rs
--rw-r--r--   0      501       20      479 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/main.rs
--rw-r--r--   0      501       20     3172 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/python/depth.rs
--rw-r--r--   0      501       20     3518 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/python/filter.rs
--rw-r--r--   0      501       20     1879 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/python/utils.rs
--rw-r--r--   0      501       20      491 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/python.rs
--rw-r--r--   0      501       20      585 2023-02-23 14:04:20.000000 blobtk-0.2.4/src/utils.rs
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 blobtk-0.3.0/Cargo.toml
+-rw-r--r--   0      501       20    59715 2023-05-03 14:59:16.000000 blobtk-0.3.0/Cargo.lock
+-rw-r--r--   0      501       20      313 2023-05-03 14:59:16.000000 blobtk-0.3.0/pyproject.toml
+-rw-r--r--   0      501       20     9018 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/bam.rs
+-rw-r--r--   0      501       20    16853 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/blobdir.rs
+-rw-r--r--   0      501       20     7517 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/cli.rs
+-rw-r--r--   0      501       20      553 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/depth.rs
+-rw-r--r--   0      501       20     1855 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/fasta.rs
+-rw-r--r--   0      501       20     6177 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/fastq.rs
+-rw-r--r--   0      501       20     1440 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/filter.rs
+-rw-r--r--   0      501       20     2738 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/io.rs
+-rw-r--r--   0      501       20      788 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/lib.rs
+-rw-r--r--   0      501       20      659 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/main.rs
+-rw-r--r--   0      501       20     4015 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/axis.rs
+-rw-r--r--   0      501       20    17018 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/blob.rs
+-rw-r--r--   0      501       20     2918 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/category.rs
+-rw-r--r--   0      501       20     4029 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/chart.rs
+-rw-r--r--   0      501       20    34935 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/component.rs
+-rw-r--r--   0      501       20     2927 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/data.rs
+-rw-r--r--   0      501       20    29455 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/snail.rs
+-rw-r--r--   0      501       20     1020 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot/style.rs
+-rw-r--r--   0      501       20     9156 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/plot.rs
+-rw-r--r--   0      501       20     3172 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/python/depth.rs
+-rw-r--r--   0      501       20     3518 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/python/filter.rs
+-rw-r--r--   0      501       20     1879 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/python/utils.rs
+-rw-r--r--   0      501       20      491 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/python.rs
+-rw-r--r--   0      501       20     6721 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/taxonomy.rs
+-rw-r--r--   0      501       20     7612 2023-05-03 14:59:16.000000 blobtk-0.3.0/src/utils.rs
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 blobtk-0.3.0/PKG-INFO
```

### Comparing `blobtk-0.2.4/Cargo.toml` & `blobtk-0.3.0/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "blobtk"
-version = "0.2.4"
+version = "0.3.0"
 edition = "2021"
 authors = [
     "Rich Challis <rc28@sanger.ac.uk>",
 ]
 license = "MIT"
 description = "Core utilities for BlobToolKit."
 homepage = "https://github.com/blobtoolkit/blobtk"
@@ -28,14 +28,32 @@
 lto = true
 codegen-units = 1
 panic = "abort"
 
 [dependencies]
 atty = "0.2.14"
 clap = { version = "4.0.29", features = [ "derive" ]}
+colorous = "1.0.10"
+coord_transforms = "1.4.0"
 flate2 = "1.0.25"
+glob = "0.3.1"
 indexmap = "1.9.2"
 indicatif = "0.17.2"
 needletail = "0.5.0"
+num-integer = "0.1.45"
 pyo3 = { version = "0.18.1", features = ["extension-module"] }
 regex = "1.7.0"
+resvg = "0.31.0"
 rust-htslib = "0.40.2"
+rust_decimal = "1.29.1"
+serde = { version = "1.0.152", features= ["derive"] }
+serde-aux = "4.2.0"
+serde_json = "1.0.93"
+serde_with = "2.3.2"
+svg = "0.13.1"
+tiny-skia = "0.8.3"
+titlecase = "2.2.1"
+url = { version = "2.3.1", features = ["serde"] }
+usvg = "0.31.0"
+
+[build-dependencies]
+pyo3-build-config = "0.18.3"
```

### Comparing `blobtk-0.2.4/src/bam.rs` & `blobtk-0.3.0/src/bam.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.2.4/src/cli.rs` & `blobtk-0.3.0/src/cli.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use std::collections::HashSet;
 use std::path::PathBuf;
 
-use clap::{ArgGroup, Parser, Subcommand};
+use clap::{ArgGroup, Parser, Subcommand, ValueEnum};
 use pyo3::pyclass;
 
 // fn float_range(s: &str, min: f64, max: f64) -> Result<f64, String> {
 //     debug_assert!(min <= max, "minimum of {} exceeds maximum of {}", min, max);
 //     let val = match s.parse::<f64>() {
 //         Ok(v) => v,
 //         Err(e) => panic!("{:?}", e),
@@ -51,14 +51,20 @@
 pub enum SubCommand {
     /// Calculate sequencing coverage depth.
     /// Called as `blobtk depth`
     Depth(DepthOptions),
     /// Filter files based on list of sequence names.
     /// Called as `blobtk filter`
     Filter(FilterOptions),
+    /// Process a BlobDir and produce static plots.
+    /// Called as `blobtk plot`
+    Plot(PlotOptions),
+    /// Process a taxonomy and lookup lineages.
+    /// Called as `blobtk taxonomy`
+    Taxonomy(TaxonomyOptions),
 }
 
 /// Options to pass to `blobtk depth`
 #[derive(Parser, Debug)]
 #[command(group(
     ArgGroup::new("alignment")
         .required(false)
@@ -148,11 +154,93 @@
     )]
     pub fastq_out: bool,
     /// Path to output list of read IDs
     #[arg(long = "read-list", short = 'O', value_name = "TXT")]
     pub read_list: Option<PathBuf>,
 }
 
+#[derive(ValueEnum, Clone, Debug)]
+pub enum View {
+    Blob,
+    Cumulative,
+    Snail,
+}
+
+#[derive(ValueEnum, Clone, Debug)]
+pub enum Palette {
+    Default,
+    Inverse,
+    Viridis,
+}
+
+/// Options to pass to `blobtk plot`
+#[derive(Parser, Debug)]
+#[pyclass]
+pub struct PlotOptions {
+    /// Path to BlobDir directory
+    #[arg(long, short = 'd')]
+    pub blobdir: PathBuf,
+    /// View to plot
+    #[arg(long, short = 'v')]
+    #[clap(value_enum)]
+    pub view: Option<View>,
+    /// Output filename
+    #[arg(long, short = 'o', default_value_t = String::from("output.svg"))]
+    pub output: String,
+    #[arg(long, short = 'f')]
+    pub filter: Vec<String>,
+    /// Segment count for snail plot
+    #[arg(long, short = 's', default_value_t = 1000)]
+    pub segments: usize,
+    /// Max span for snail plot
+    #[arg(long = "max-span")]
+    pub max_span: Option<usize>,
+    /// max scaffold length for snail plot
+    #[arg(long = "max-scaffold")]
+    pub max_scaffold: Option<usize>,
+    /// X-axis field for blob plot
+    #[arg(long = "x-field", short = 'x')]
+    pub x_field: Option<String>,
+    /// Y-axis field for blob plot
+    #[arg(long = "y-field", short = 'y')]
+    pub y_field: Option<String>,
+    /// Z-axis field for blob plot
+    #[arg(long = "z-field", short = 'z')]
+    pub z_field: Option<String>,
+    /// Category field for blob plot
+    #[arg(long = "category", short = 'c')]
+    /// Category field for blob plot
+    #[arg(long = "category", short = 'c')]
+    pub cat_field: Option<String>,
+    /// Resolution for blob plot
+    #[arg(long, default_value_t = 30)]
+    pub resolution: usize,
+    /// Maximum number of categories for blob/cumulative plot
+    #[arg(long = "cat-count", default_value_t = 10)]
+    pub cat_count: usize,
+    /// Category order for blob/cumulative plot (<cat1>,<cat2>,...)
+    #[arg(long = "cat-order")]
+    pub cat_order: Option<String>,
+    /// Colour palette for categories
+    #[arg(long, value_enum)]
+    pub palette: Option<Palette>,
+    /// Individual colours to modify palette (<index>=<hexcode>)
+    #[arg(long)]
+    pub color: Option<Vec<String>>,
+}
+
+/// Options to pass to `blobtk taxonomy`
+#[derive(Parser, Debug)]
+#[pyclass]
+pub struct TaxonomyOptions {
+    /// Path to NCBI taxdump directory
+    #[arg(long, short = 't')]
+    pub taxdump: Option<PathBuf>,
+    /// Root taxon to build taxonomy for
+    #[arg(long = "root-id", short = 'r')]
+    pub root_id: Option<String>,
+}
+
 /// Command line argument parser
 pub fn parse() -> Arguments {
     Arguments::parse()
 }
```

### Comparing `blobtk-0.2.4/src/depth.rs` & `blobtk-0.3.0/src/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.2.4/src/fasta.rs` & `blobtk-0.3.0/src/fasta.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.2.4/src/fastq.rs` & `blobtk-0.3.0/src/fastq.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.2.4/src/filter.rs` & `blobtk-0.3.0/src/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.2.4/src/io.rs` & `blobtk-0.3.0/src/io.rs`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
             Ok(l) => l.as_bytes().to_vec(),
         };
         list.push(line_as_vec)
     }
     list
 }
 
-fn read_lines<P>(filename: P) -> io::Result<io::Lines<io::BufReader<File>>>
+pub fn read_lines<P>(filename: P) -> io::Result<io::Lines<io::BufReader<File>>>
 where
     P: AsRef<Path>,
 {
     let file = File::open(filename).expect("no such file");
     Ok(io::BufReader::new(file).lines())
 }
 
@@ -60,15 +60,14 @@
 pub fn get_file_writer(file_path: &PathBuf) -> Box<dyn Write> {
     let file = match File::create(file_path) {
         Err(why) => panic!("couldn't open {}: {}", file_path.display(), why),
         Ok(file) => file,
     };
 
     let writer: Box<dyn Write> = if file_path.extension() == Some(OsStr::new("gz")) {
-        // Error is here: Created file isn't gzip-compressed
         Box::new(BufWriter::with_capacity(
             128 * 1024,
             write::GzEncoder::new(file, Compression::default()),
         ))
     } else {
         Box::new(BufWriter::with_capacity(128 * 1024, file))
     };
```

### Comparing `blobtk-0.2.4/src/lib.rs` & `blobtk-0.3.0/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 //! `blobtk` is a set of core command line utilities and python bindings for
 //! processing common file formats used by [BlobToolKit](https://blobtoolkit.genomehubs.org).
 
 /// Functions for processing BAM files.
 pub mod bam;
 
+/// Functions for processing a BlobDir.
+pub mod blobdir;
+
 /// The BlobTk Command Line Interface.
 pub mod cli;
 
 /// Summarise windowed coverage depth.
 pub mod depth;
 
 /// Functions for processing FASTA files.
@@ -18,12 +21,18 @@
 
 /// Filter files based on a list of sequence IDs.
 pub mod filter;
 
 /// Functions for file/terminal IO.
 pub mod io;
 
+/// Generate a plot.
+pub mod plot;
+
 /// Python bindings.
 pub mod python;
 
+/// Parse and subset a taxonomy.
+pub mod taxonomy;
+
 /// Utility functions.
 pub mod utils;
```

### Comparing `blobtk-0.2.4/src/python/depth.rs` & `blobtk-0.3.0/src/python/depth.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.2.4/src/python/filter.rs` & `blobtk-0.3.0/src/python/filter.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.2.4/src/python/utils.rs` & `blobtk-0.3.0/src/python/utils.rs`

 * *Files identical despite different names*

### Comparing `blobtk-0.2.4/PKG-INFO` & `blobtk-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blobtk
-Version: 0.2.4
+Version: 0.3.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Core utilities for BlobToolKit.
 Keywords: bioinformatics,blobtoolkit,genome,genomics
 Home-Page: https://github.com/blobtoolkit/blobtk
 Author: Rich Challis <rc28@sanger.ac.uk>
```

