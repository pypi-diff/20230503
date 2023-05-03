# Comparing `tmp/hpo3-0.1.0.tar.gz` & `tmp/hpo3-0.2.0.tar.gz`

## Comparing `hpo3-0.1.0.tar` & `hpo3-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 hpo3-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     1553 2022-12-19 18:39:06.000000 hpo3-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      713 2023-01-19 21:37:55.000000 hpo3-0.1.0/.gitignore
--rw-r--r--   0      501       20      637 2023-01-19 18:00:40.000000 hpo3-0.1.0/Makefile
--rw-r--r--   0      501       20     4177 2023-05-01 06:31:38.000000 hpo3-0.1.0/README.md
--rw-r--r--   0      501       20      138 2023-01-19 19:00:38.000000 hpo3-0.1.0/docs/annotations.rst
--rw-r--r--   0      501       20     1068 2023-01-19 19:30:23.000000 hpo3-0.1.0/docs/conf.py
--rw-r--r--   0      501       20      111 2023-02-04 16:22:19.000000 hpo3-0.1.0/docs/enrichment.rst
--rw-r--r--   0      501       20       78 2023-02-04 16:22:49.000000 hpo3-0.1.0/docs/hposet.rst
--rw-r--r--   0      501       20       81 2023-01-19 18:57:06.000000 hpo3-0.1.0/docs/hpoterm.rst
--rw-r--r--   0      501       20     5709 2023-02-04 17:58:46.000000 hpo3-0.1.0/docs/index.rst
--rw-r--r--   0      501       20     1568 2023-01-19 20:46:20.000000 hpo3-0.1.0/docs/ontology.rst
--rw-r--r--   0      501       20        0 2023-01-01 16:59:41.000000 hpo3-0.1.0/hpo3.pyi
--rw-r--r--   0      501       20      803 2023-01-19 21:38:33.000000 hpo3-0.1.0/make.bat
--rw-r--r--   0      501       20  5055109 2023-01-19 20:20:40.000000 hpo3-0.1.0/ontology.hpo
--rw-r--r--   0      501       20      951 2023-01-18 05:50:28.000000 hpo3-0.1.0/pyproject.toml
--rw-r--r--   0      501       20     5450 2023-02-04 16:52:47.000000 hpo3-0.1.0/src/annotations.rs
--rw-r--r--   0      501       20     4211 2023-03-30 16:29:45.000000 hpo3-0.1.0/src/enrichment.rs
--rw-r--r--   0      501       20     1927 2023-01-21 18:42:18.000000 hpo3-0.1.0/src/information_content.rs
--rw-r--r--   0      501       20     7336 2023-05-01 06:27:18.000000 hpo3-0.1.0/src/lib.rs
--rw-r--r--   0      501       20     7599 2023-03-30 16:28:34.000000 hpo3-0.1.0/src/ontology.rs
--rw-r--r--   0      501       20     9925 2023-05-01 06:26:59.000000 hpo3-0.1.0/src/set.rs
--rw-r--r--   0      501       20    12871 2023-03-06 21:32:20.000000 hpo3-0.1.0/src/term.rs
--rw-r--r--   0      501       20    18663 2023-05-01 06:26:08.000000 hpo3-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     5104 1970-01-01 00:00:00.000000 hpo3-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      329 1970-01-01 00:00:00.000000 hpo3-0.2.0/Cargo.toml
+-rw-r--r--   0      501       20     1553 2022-12-19 18:39:06.000000 hpo3-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      713 2023-01-19 21:37:55.000000 hpo3-0.2.0/.gitignore
+-rw-r--r--   0      501       20      637 2023-01-19 18:00:40.000000 hpo3-0.2.0/Makefile
+-rw-r--r--   0      501       20     8902 2023-05-01 15:34:11.000000 hpo3-0.2.0/README.md
+-rw-r--r--   0      501       20      150 2023-05-01 17:11:20.000000 hpo3-0.2.0/docs/annotations.rst
+-rw-r--r--   0      501       20     1068 2023-05-01 17:13:39.000000 hpo3-0.2.0/docs/conf.py
+-rw-r--r--   0      501       20      112 2023-05-01 17:02:22.000000 hpo3-0.2.0/docs/enrichment.rst
+-rw-r--r--   0      501       20       79 2023-05-01 17:02:26.000000 hpo3-0.2.0/docs/hposet.rst
+-rw-r--r--   0      501       20       82 2023-05-01 17:02:32.000000 hpo3-0.2.0/docs/hpoterm.rst
+-rw-r--r--   0      501       20     5715 2023-05-01 17:03:23.000000 hpo3-0.2.0/docs/index.rst
+-rw-r--r--   0      501       20     1580 2023-05-01 17:15:59.000000 hpo3-0.2.0/docs/ontology.rst
+-rw-r--r--   0      501       20      803 2023-01-19 21:38:33.000000 hpo3-0.2.0/make.bat
+-rw-r--r--   0      501       20  5055109 2023-01-19 20:20:40.000000 hpo3-0.2.0/ontology.hpo
+-rw-r--r--   0      501       20        0 2023-05-01 17:46:15.000000 hpo3-0.2.0/pyhpo.pyi
+-rw-r--r--   0      501       20     1131 2023-05-03 05:48:03.000000 hpo3-0.2.0/pyproject.toml
+-rw-r--r--   0      501       20     5453 2023-05-01 15:00:50.000000 hpo3-0.2.0/src/annotations.rs
+-rw-r--r--   0      501       20     4216 2023-05-01 16:59:59.000000 hpo3-0.2.0/src/enrichment.rs
+-rw-r--r--   0      501       20     1927 2023-01-21 18:42:18.000000 hpo3-0.2.0/src/information_content.rs
+-rw-r--r--   0      501       20     9817 2023-05-01 17:31:07.000000 hpo3-0.2.0/src/lib.rs
+-rw-r--r--   0      501       20     8470 2023-05-02 04:38:42.000000 hpo3-0.2.0/src/ontology.rs
+-rw-r--r--   0      501       20    11420 2023-05-01 17:31:07.000000 hpo3-0.2.0/src/set.rs
+-rw-r--r--   0      501       20    13070 2023-05-01 17:31:07.000000 hpo3-0.2.0/src/term.rs
+-rw-r--r--   0      501       20    18663 2023-05-01 06:26:08.000000 hpo3-0.2.0/Cargo.lock
+-rw-r--r--   0        0        0    10021 1970-01-01 00:00:00.000000 hpo3-0.2.0/PKG-INFO
```

### Comparing `hpo3-0.1.0/.github/workflows/CI.yml` & `hpo3-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `hpo3-0.1.0/.gitignore` & `hpo3-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `hpo3-0.1.0/Makefile` & `hpo3-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `hpo3-0.1.0/docs/conf.py` & `hpo3-0.2.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # For the full list of built-in configuration values, see the documentation:
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'hpo3'
-copyright = '2022, Jonas Marcello'
+copyright = '2023, Jonas Marcello'
 author = 'Jonas Marcello'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = [
     'sphinx.ext.autodoc',
```

### Comparing `hpo3-0.1.0/docs/index.rst` & `hpo3-0.2.0/docs/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
    sphinx-quickstart on Sat Dec 31 16:56:03 2022.
    You can adapt this file completely to your liking, but it should at least
    contain the root `toctree` directive.
 
 Welcome to hpo3's documentation!
 ================================
 
-.. currentmodule:: hpo3
+.. currentmodule:: pyhpo
 
 .. toctree::
    :maxdepth: 1
    :caption: API documentation:
 
    ontology
    hpoterm
@@ -33,15 +33,15 @@
 
 
 Examples
 ~~~~~~~~
 
 .. code-block:: python
 
-   from hpo3 import stats, Ontology, HPOSet, Gene
+   from pyhpo import stats, Ontology, HPOSet, Gene
 
    # initilize the Ontology
    _ = Ontology()
 
    # Declare the clinical information of the patients
    patient_1 = HPOSet.from_queries([
       'HP:0002943',
@@ -117,15 +117,15 @@
 
 
 **Calculate the pairwise similarity of the HPOSets from all genes**
 
 .. code-block:: python
 
    import itertools
-   from hpo3 import Ontology, HPOSet, helper
+   from pyhpo import Ontology, HPOSet, helper
 
    Ontology()
 
    gene_sets = [g.hpo_set() for g in Ontology.genes]
    gene_set_combinations = [
       (a[0], a[1]) for a in itertools.combinations(gene_sets, 2)
    ]
@@ -139,15 +139,15 @@
 
 
 **Calculate the similarity of of a patient's HPO term to all diseases**
 
 .. code-block:: python
 
    import itertools
-   from hpo3 import Ontology, HPOSet, helper
+   from pyhpo import Ontology, HPOSet, helper
 
    Ontology()
 
    patient_1 = HPOSet.from_queries([
       'HP:0002943',
       'HP:0008458',
       'HP:0100884',
@@ -173,15 +173,15 @@
 
 
 **Calculate the disease enrichment for every gene's HPOSet**
 
 .. code-block:: python
 
    import itertools
-   from hpo3 import Ontology, HPOSet, helper
+   from pyhpo import Ontology, HPOSet, helper
 
    Ontology()
 
    # casting the gene set to a list to main order for later lookups
    genes = list(Ontology.genes)
    gene_sets = [g.hpo_set() for g in genes]
 
@@ -190,15 +190,15 @@
 
 
 **Or vice versa (genes enriched for every disease)**
 
 .. code-block:: python
 
    import itertools
-   from hpo3 import Ontology, HPOSet, helper
+   from pyhpo import Ontology, HPOSet, helper
 
    Ontology()
 
    # casting the gene set to a list to main order for later lookups
    diseases = list(Ontology.omim_diseases)
    disease_sets = [d.hpo_set() for d in diseases]
```

### Comparing `hpo3-0.1.0/docs/ontology.rst` & `hpo3-0.2.0/docs/ontology.rst`

 * *Files 24% similar despite different names*

```diff
@@ -14,60 +14,60 @@
     Whether the input format is binary (default true)
 
 Examples
 ~~~~~~~~
 
 .. code-block:: python
 
-    from hpo3 import Ontology
+    from pyhpo import Ontology
     
     ont = Ontology("path/to/ontology.hpo")
     
     term = ont.hpo(11968)
     term.name()  # ==> 'Feeding difficulties'
     term.id()    # ==> 'HP:0011968'
     int(tern)    # ==> 11968
 
 
-The following code with multiple modules works, because the Ontology mus only be loaded once:
+The following code with multiple modules works, because the Ontology must only be loaded once:
 
 **File main.py**
 
 .. code-block:: python
 
-    from hpo3 import Ontology
+    from pyhpo import Ontology
 
     import submodule
     from submodule import foo
     
     ont = Ontology("path/to/ontology.hpo")
     
     foo()
     submodule.bar()
 
 
 **File submodule.py**
 
 .. code-block:: python
 
-    from hpo3 import Ontology
+    from pyhpo import Ontology
 
     def foo():
         print(len(Ontology))
 
     def bar():
         print(len(Ontology))
 
 
 Attributes
 ----------
-.. autoattribute:: hpo3.Ontology.__class__.genes
-.. autoattribute:: hpo3.Ontology.__class__.omim_diseases
+.. autoattribute:: pyhpo.Ontology.__class__.genes
+.. autoattribute:: pyhpo.Ontology.__class__.omim_diseases
 
 Methods
 -------
-.. autofunction:: hpo3.Ontology.__class__.__call__
-.. autofunction:: hpo3.Ontology.__class__.get_hpo_object
-.. autofunction:: hpo3.Ontology.__class__.match
-.. autofunction:: hpo3.Ontology.__class__.path
-.. autofunction:: hpo3.Ontology.__class__.search
-.. autofunction:: hpo3.Ontology.__class__.hpo
+.. autofunction:: pyhpo.Ontology.__class__.__call__
+.. autofunction:: pyhpo.Ontology.__class__.get_hpo_object
+.. autofunction:: pyhpo.Ontology.__class__.match
+.. autofunction:: pyhpo.Ontology.__class__.path
+.. autofunction:: pyhpo.Ontology.__class__.search
+.. autofunction:: pyhpo.Ontology.__class__.hpo
```

### Comparing `hpo3-0.1.0/make.bat` & `hpo3-0.2.0/make.bat`

 * *Files identical despite different names*

### Comparing `hpo3-0.1.0/ontology.hpo` & `hpo3-0.2.0/ontology.hpo`

 * *Files identical despite different names*

### Comparing `hpo3-0.1.0/pyproject.toml` & `hpo3-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "hpo3"
-version = "0.1.0"
+version = "0.2.0"
 description = "A drop-in replacement for PyHPO using a Rust backend for faster performance"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
@@ -19,7 +19,12 @@
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
     "Topic :: Scientific/Engineering :: Medical Science Apps.",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 license = {text = "MIT"}
 authors = [{name = "Jonas Marcello", email = "jonas.marcello@esbme.com"}]
+
+[project.urls]
+homepage = "https://github.com/anergictcell/hpo3"
+repository = "https://github.com/anergictcell/hpo3"
+"Bug Tracker" = "https://github.com/anergictcell/hpo3/issues"
```

### Comparing `hpo3-0.1.0/src/annotations.rs` & `hpo3-0.2.0/src/annotations.rs`

 * *Files 8% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     /// Returns the Gene Id
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     gene = ont.genes()[0]
     ///     gene.id()    # ==> 11212
     ///
     #[getter(id)]
     pub fn id(&self) -> u32 {
         self.id.as_u32()
@@ -45,15 +45,15 @@
     /// Returns the name of the HPO Term
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     gene = ont.genes()[0]
     ///     gene.name()
     ///     # >> 'BRCA2'
     ///
     #[getter(name)]
     pub fn name(&self) -> &str {
@@ -61,15 +61,15 @@
     }
 
     #[getter(hpo)]
     pub fn hpo(&self) -> PyResult<HashSet<u32>> {
         let ont = get_ontology()?;
         Ok(ont
             .gene(&self.id)
-            .expect("ontology must. be present and gene must be included")
+            .expect("ontology must be present and gene must be included")
             .hpo_terms()
             .iter()
             .fold(HashSet::new(), |mut set, tid| {
                 set.insert(tid.as_u32());
                 set
             }))
     }
@@ -149,15 +149,15 @@
     /// Returns the OmimDisease Id
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     gene = ont.omim_diseases()[0]
     ///     gene.id    # ==> 41232
     ///
     #[getter(id)]
     pub fn id(&self) -> u32 {
         self.id.as_u32()
@@ -166,15 +166,15 @@
     /// Returns the name of the HPO Term
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     gene = ont.omim_diseases()[0]
     ///     gene.name  # ==> 'Gaucher'
     ///
     #[getter(name)]
     pub fn name(&self) -> &str {
         &self.name
```

### Comparing `hpo3-0.1.0/src/enrichment.rs` & `hpo3-0.2.0/src/enrichment.rs`

 * *Files 3% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 ///     Specify `gene` or `omim` to determine which enrichments to calculate
 ///
 /// Examples
 /// --------
 ///
 /// .. code-block:: python
 ///
-///     from hpo3 import Ontology, Gene, Omim
-///     from hpo3 import stats
+///     from pyhpo import Ontology, Gene, Omim
+///     from pyhpo import stats
 ///
 ///     ont = Ontology()
 ///     model = stats.EnrichmentModel("omim")
 ///
 ///     # use the `model.enrichment` method to calculate
 ///     # the enrichment of Omim Diseases within an HPOSet
 ///
@@ -55,25 +55,25 @@
 
     /// Calculate the enrichment for all genes or diseeases in the `HPOSet`
     ///
     /// Parameters
     /// ----------
     /// method: str
     ///     Currently, only `hypergeom` is implemented
-    /// hposet: :class:`hpo3.HPOSet`
+    /// hposet: :class:`pyhpo.HPOSet`
     ///     The set of HPOTerms to use as sampleset for calculation of
     ///     enrichment. The full ontology is used as background set.
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology, Gene, Omim
-    ///     from hpo3 import stats
+    ///     from pyhpo import Ontology, Gene, Omim
+    ///     from pyhpo import stats
     ///
     ///     ont = Ontology()
     ///     model = stats.EnrichmentModel("omim")
     ///
     ///     # you can crate a custom HPOset or use a Gene or Disease
     ///     term_set = Gene.get("GBA1").hpo_set()
     ///
```

### Comparing `hpo3-0.1.0/src/information_content.rs` & `hpo3-0.2.0/src/information_content.rs`

 * *Files identical despite different names*

### Comparing `hpo3-0.1.0/src/lib.rs` & `hpo3-0.2.0/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 use rayon::prelude::*;
 
 use pyo3::exceptions::{PyKeyError, PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::PyDict;
 
 use hpo::annotations::{AnnotationId, GeneId, OmimDiseaseId};
-use hpo::similarity::{GroupSimilarity, StandardCombiner};
+use hpo::similarity::{GroupSimilarity, Similarity, StandardCombiner};
 use hpo::stats::hypergeom::{disease_enrichment, gene_enrichment};
 use hpo::term::HpoTermId;
 use hpo::{HpoTerm, Ontology as ActualOntology};
 
 mod annotations;
 mod enrichment;
 mod information_content;
@@ -100,53 +100,92 @@
 }
 
 /// Python bindings for the Rust hpo crate
 ///
 /// This library aims to be a drop-in replacement for
 /// `pyhpo <https://pypi.org/project/pyhpo/>`_
 #[pymodule]
-fn hpo3(py: Python, m: &PyModule) -> PyResult<()> {
+fn pyhpo(py: Python, m: &PyModule) -> PyResult<()> {
     let ont = PyOntology::blank();
     m.add_class::<PyGene>()?;
     m.add_class::<PyOmimDisease>()?;
     m.add_class::<PyHpoSet>()?;
     m.add_class::<PyHpoTerm>()?;
     m.add("Ontology", ont)?;
+    m.add("BasicHPOSet", set::BasicPyHpoSet::default())?;
     register_helper_module(py, m)?;
     register_stats_module(py, m)?;
+    register_set_module(py, m)?;
+    register_annotations_module(py, m)?;
+    Ok(())
+}
+
+fn register_annotations_module(py: Python<'_>, parent_module: &PyModule) -> PyResult<()> {
+    let child_module = PyModule::new(py, "annotations")?;
+    child_module.add_class::<PyGene>()?;
+    child_module.add_class::<PyOmimDisease>()?;
+    parent_module.add_submodule(child_module)?;
+
+    py.import("sys")?
+        .getattr("modules")?
+        .set_item("pyhpo.annotations", child_module)?;
+
+    Ok(())
+}
+
+fn register_set_module(py: Python<'_>, parent_module: &PyModule) -> PyResult<()> {
+    let child_module = PyModule::new(py, "set")?;
+    child_module.add_class::<set::BasicPyHpoSet>()?;
+    child_module.add_class::<set::PyHpoSet>()?;
+    parent_module.add_submodule(child_module)?;
+
+    py.import("sys")?
+        .getattr("modules")?
+        .set_item("pyhpo.set", child_module)?;
+
     Ok(())
 }
 
 fn register_helper_module(py: Python<'_>, parent_module: &PyModule) -> PyResult<()> {
     let child_module = PyModule::new(py, "helper")?;
+    child_module.add_function(wrap_pyfunction!(batch_similarity, child_module)?)?;
     child_module.add_function(wrap_pyfunction!(set_batch_similarity, child_module)?)?;
     child_module.add_function(wrap_pyfunction!(batch_gene_enrichment, child_module)?)?;
     child_module.add_function(wrap_pyfunction!(batch_disease_enrichment, child_module)?)?;
     parent_module.add_submodule(child_module)?;
+
+    py.import("sys")?
+        .getattr("modules")?
+        .set_item("pyhpo.helper", child_module)?;
     Ok(())
 }
 
 fn register_stats_module(py: Python<'_>, parent_module: &PyModule) -> PyResult<()> {
     let child_module = PyModule::new(py, "stats")?;
     child_module.add_class::<PyEnrichmentModel>()?;
     parent_module.add_submodule(child_module)?;
+
+    py.import("sys")?
+        .getattr("modules")?
+        .set_item("pyhpo.stats", child_module)?;
+
     Ok(())
 }
 
-/// Calculate `similarity between `HPOSet`s in batches
+/// Calculate similarity between `HPOSet`s in batches
 ///
 /// This method runs parallelized on all avaible CPU
 ///
 /// Examples
 /// --------
 ///
 /// .. code-block:: python
 ///
 ///     import itertools
-///     from hpo3 import Ontology, HPOSet, helper
+///     from pyhpo import Ontology, HPOSet, helper
 ///
 ///     Ontology()
 ///
 ///     gene_sets = [g.hpo_set() for g in Ontology.genes]
 ///     gene_set_combinations = [(a[0], a[1]) for a in itertools.combinations(gene_sets,2)]
 ///     similarities = helper.set_batch_similarity(gene_set_combinations[0:100], kind="omim", method="graphic", combine = "funSimAvg")
 ///
@@ -175,14 +214,54 @@
             let set_a = comp.0.set(ont);
             let set_b = comp.1.set(ont);
             g_sim.calculate(&set_a, &set_b)
         })
         .collect())
 }
 
+/// Calculate similarity between `HPOTerm`s in batches
+///
+/// This method runs parallelized on all avaible CPU
+///
+/// Examples
+/// --------
+///
+/// .. code-block:: python
+///
+///     import itertools
+///     from pyhpo import Ontology, HPOSet, helper
+///
+///     Ontology()
+///
+///     terms = [t for t in Ontology]
+///     term_combinations = [(a[0], a[1]) for a in itertools.combinations(terms,2)]
+///     similarities = helper.batch_similarity(term_combinations[0:10000], kind="omim", method="graphic")
+///
+#[pyfunction]
+#[pyo3(signature = (comparisons, kind = "omim", method = "graphic"))]
+#[pyo3(text_signature = "(comparisons, kind, method)")]
+fn batch_similarity(
+    comparisons: Vec<(PyHpoTerm, PyHpoTerm)>,
+    kind: &str,
+    method: &str,
+) -> PyResult<Vec<f32>> {
+    let kind = PyInformationContentKind::try_from(kind)?;
+    let similarity = hpo::similarity::Builtins::new(method, kind.into())
+        .map_err(|_| PyRuntimeError::new_err("Unknown method to calculate similarity"))?;
+
+    Ok(comparisons
+        .par_iter()
+        .map(|comp| {
+            let t1: hpo::HpoTerm = (&comp.0).into();
+            let t2: hpo::HpoTerm = (&comp.1).into();
+            similarity.calculate(&t1, &t2)
+        })
+        .collect())
+}
+
 #[pyfunction]
 fn batch_gene_enrichment(py: Python, hposets: Vec<PyHpoSet>) -> PyResult<Vec<Vec<&PyDict>>> {
     let ont = get_ontology()?;
     let enrichments = hposets
         .par_iter()
         .map(|pyset| {
             let mut enrichment = gene_enrichment(ont, &pyset.set(ont));
```

### Comparing `hpo3-0.1.0/src/ontology.rs` & `hpo3-0.2.0/src/ontology.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 use std::collections::VecDeque;
 
-use pyo3::exceptions::{PyIndexError, PyRuntimeError};
+use pyo3::exceptions::PyRuntimeError;
 use pyo3::prelude::*;
 use pyo3::PyResult;
 
 use hpo::annotations::AnnotationId;
 
 use crate::annotations::PyOmimDisease;
 use crate::{from_binary, from_obo, get_ontology, pyterm_from_id, term_from_query, PyQuery};
 
 use crate::PyGene;
 use crate::PyHpoTerm;
 
-#[pyclass(module = "hpo3", name = "Ontology")]
+#[pyclass(name = "Ontology")]
 pub struct PyOntology {}
 
 impl PyOntology {
     pub fn blank() -> Self {
         Self {}
     }
 }
 
 #[pymethods]
 impl PyOntology {
     /// A list of all genes included in the ontology
     ///
     /// Returns
     /// -------
-    /// list[:class:`hpo3.Gene`]
-    ///     All genes that are associated to the :class:`hpo.HPOTerm` in the ontology
+    /// list[:class:`pyhpo.Gene`]
+    ///     All genes that are associated to the :class:`pyhpo.HPOTerm` in the ontology
     ///
     #[getter(genes)]
     fn genes(&self) -> PyResult<Vec<PyGene>> {
         let ont = get_ontology()?;
 
         let mut res = Vec::new();
         for gene in ont.genes() {
@@ -41,16 +41,16 @@
         Ok(res)
     }
 
     /// A list of all Omim Diseases included in the ontology
     ///
     /// Returns
     /// -------
-    /// list[:class:`hpo3.Omim`]
-    ///     All Omim diseases that are associated to the :class:`hpo.HPOTerm` in the ontology
+    /// list[:class:`pyhpo.Omim`]
+    ///     All Omim diseases that are associated to the :class:`pyhpo.HPOTerm` in the ontology
     ///
     #[getter(omim_diseases)]
     fn omim_diseases(&self) -> PyResult<Vec<PyOmimDisease>> {
         let ont = get_ontology()?;
 
         let mut res = Vec::new();
         for disease in ont.omim_diseases() {
@@ -59,34 +59,34 @@
         Ok(res)
     }
 
     /// Returns a single `HPOTerm` based on its name, synonym or id
     ///
     /// Parameters
     /// ----------
-    /// query: str or int
+    /// query: `str` or `int`
     ///
     ///     * **str** HPO term ``Scoliosis``
     ///     * **str** synonym ``Curved spine``
     ///     * **str** HPO-ID ``HP:0002650``
     ///     * **int** HPO term id ``2650``
     ///
     /// Returns
     /// -------
-    /// :class:`hpo.HPOTerm`
+    /// :class:`pyhpo.HPOTerm`
     ///     A single matching HPO term instance
     ///
     /// Raises
     /// ------
-    /// RuntimeError
+    /// `RuntimeError`
     ///     No HPO term is found for the provided query
-    /// TypeError
+    /// `TypeError`
     ///     The provided query is an unsupported type and can't be properly
     ///     converted
-    /// ValueError
+    /// `ValueError`
     ///     The provided HPO ID cannot be converted to the correct
     ///     integer representation
     ///
     /// Example
     /// -------
     ///     ::
     ///
@@ -107,45 +107,77 @@
     ///         HP:0000003 | Multicystic kidney dysplasia
     ///
     #[pyo3(text_signature = "($self, query)")]
     fn get_hpo_object(&self, query: PyQuery) -> PyResult<PyHpoTerm> {
         Ok(PyHpoTerm::from(term_from_query(query)?))
     }
 
+    /// Returns a single `HPOTerm` based on its name
+    ///
+    /// Parameters
+    /// ----------
+    /// query: `str`
+    ///     Name of the HPO term, e.g. ``Scoliosis``
+    ///
+    /// Returns
+    /// -------
+    /// :class:`pyhpo.HPOTerm`
+    ///     A single matching HPO term instance
+    ///
+    /// Raises
+    /// ------
+    /// `RuntimeError`
+    ///     No HPO term is found for the provided query
     #[pyo3(text_signature = "($self, query)")]
     fn r#match(&self, query: &str) -> PyResult<PyHpoTerm> {
         let ont = get_ontology()?;
         for term in ont {
             if term.name() == query {
                 return Ok(PyHpoTerm::from(term));
             }
         }
 
         Err(PyRuntimeError::new_err("No HPO entry found"))
     }
 
-    /// Calculates the shortest path from one to another HPO Term
+    /// Returns the shortest path from one to another HPO Term
+    ///
+    /// Parameters
+    /// ----------
+    /// query1: `str` or `int`
+    ///     HPO term 1, synonym or HPO-ID (HP:00001) to match
+    ///     HPO term id (Integer based)
+    ///     e.g: ``Abnormality of the nervous system``
+    /// query2: `str` or `int`
+    ///     HPO term 2, synonym or HPO-ID (HP:00001) to match
+    ///     HPO term id (Integer based)
+    ///     e.g: ``Abnormality of the nervous system``
+    ///
+    /// Returns
+    /// -------
+    /// int
+    ///     Length of path
+    /// tuple
+    ///     Tuple of HPOTerms in the path
+    /// int
+    ///     Number of steps from term-1 to the common parent
+    ///     **(Not yet implemented. Returns ``0``)**
+    /// int
+    ///     Number of steps from term-2 to the common parent
+    ///     **(Not yet implemented. Returns ``0``)**
     ///
-    /// IMPORTANT NOTE
-    /// --------------
-    /// This method is not correctly implemented and will only return
-    /// the distance, but not the actual path. It will instead return
-    /// an empty list
     #[pyo3(text_signature = "($self, query1, query2)")]
     fn path(
         &self,
         query1: PyQuery,
         query2: PyQuery,
     ) -> PyResult<(usize, Vec<PyHpoTerm>, usize, usize)> {
-        let t1 = term_from_query(query1)?;
-        let t2 = term_from_query(query2)?;
-        let dist = t1
-            .distance_to_term(&t2)
-            .ok_or_else(|| PyIndexError::new_err("no path between the two terms"))?;
-        Ok((dist, vec![], 0, 0))
+        let t1: PyHpoTerm = term_from_query(query1)?.into();
+        let t2: PyHpoTerm = term_from_query(query2)?.into();
+        t1.path_to_other(&t2)
     }
 
     /// TODO: Return an actual iterator instead
     #[pyo3(text_signature = "($self, query)")]
     fn search(&self, query: &str) -> PyResult<Vec<PyHpoTerm>> {
         let mut res = Vec::new();
         let ont = get_ontology()?;
@@ -163,23 +195,23 @@
     /// Arguments
     /// ---------
     /// a: `int`
     ///     ID of the term as `int` (`HP:0000123` --> `123`)
     ///
     /// Returns
     /// -------
-    /// :class:`hpo3.HpoTerm`
+    /// :class:`pyhpo.HPOTerm`
     ///     The HPO-Term
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     
     ///     ont = Ontology()
     ///     
     ///     term = ont.hpo(11968)
     ///     term.name()  # ==> 'Feeding difficulties'
     ///     term.id()    # ==> 'HP:0011968'
     ///     int(tern)    # ==> 11968
@@ -216,39 +248,39 @@
     ///     The number of HPO-Terms in the Ontology
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     len(ont)  # ==> 17059
     ///
     fn __len__(&self) -> PyResult<usize> {
         Ok(get_ontology()?.len())
     }
 
     fn __repr__(&self) -> String {
         match get_ontology() {
-            Ok(ont) => format!("<hpo3.Ontology with {} terms>", ont.len()),
-            _ => String::from("<hpo3.Ontology (no data loaded, yet)>"),
+            Ok(ont) => format!("<pyhpo.Ontology with {} terms>", ont.len()),
+            _ => String::from("<pyhpo.Ontology (no data loaded, yet)>"),
         }
     }
 
     fn __getitem__(&self, id: u32) -> PyResult<PyHpoTerm> {
         self.hpo(id)
     }
 
     fn __iter__(&self) -> OntologyIterator {
         OntologyIterator::new()
     }
 }
 
-#[pyclass(module = "hpo3", name = "OntologyIterator")]
+#[pyclass(name = "OntologyIterator")]
 struct OntologyIterator {
     ids: VecDeque<u32>,
 }
 
 impl OntologyIterator {
     fn new() -> Self {
         let ids: VecDeque<u32> = get_ontology()
```

### Comparing `hpo3-0.1.0/src/set.rs` & `hpo3-0.2.0/src/set.rs`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 /// A set of HPO terms
 ///
 /// Examples
 /// --------
 ///
 /// .. code-block: python
 ///
-///     from hpo3 import Ontology, HPOSet
+///     from pyhpo import Ontology, HPOSet
 ///     ont = Ontology()
 ///     s = HPOSet([1, 118])
 ///     len(s)  
 ///     # >> 2
 ///
 #[pymethods]
 impl PyHpoSet {
@@ -154,15 +154,15 @@
     ///
     /// This method runs parallelized on all avaible CPU
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     gene_sets = [g.hpo_set() for g in Ontology.genes]
     ///     gene_sets[0].similarity(gene_sets[1])
     ///     # >> 0.29546087980270386
     ///
     #[pyo3(signature = (other, kind = "omim", method = "graphic", combine = "funSimAvg"))]
     #[pyo3(text_signature = "($self, other, kind, method, combine)")]
@@ -194,15 +194,15 @@
     /// This method runs parallelized on all avaible CPU
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     gene_sets = [g.hpo_set() for g in Ontology.genes]
     ///     similarities = gene_sets[0].batch_similarity(gene_sets)
     ///     similarities[0:4]
     ///     # >> [1.0, 0.5000048279762268, 0.29546087980270386, 0.5000059008598328]
     ///
     #[pyo3(signature =(other, kind = "omim", method = "graphic", combine = "funSimAvg"))]
@@ -333,7 +333,55 @@
         Ok(ont
             .omim_disease(&disease.id().into())
             .expect("ontology must. be present and gene must be included")
             .to_hpo_set(ont)
             .into())
     }
 }
+
+#[pyclass(name = "BasicHPOSet")]
+#[derive(Clone, Default, Debug)]
+pub(crate) struct BasicPyHpoSet;
+
+impl BasicPyHpoSet {
+    fn build<I: IntoIterator<Item = HpoTermId>>(ids: I) -> PyHpoSet {
+        let ont = get_ontology().expect("Ontology must be initialized");
+        let mut group = HpoGroup::new();
+        for id in ids {
+            group.insert(id);
+        }
+        let mut set = HpoSet::new(ont, group);
+        let mut set = set.child_nodes();
+        set.replace_obsolete();
+        set.remove_obsolete();
+        set.remove_modifier();
+        PyHpoSet::new(set.iter().map(|term| term.id().as_u32()).collect())
+    }
+}
+
+#[pymethods]
+impl BasicPyHpoSet {
+    fn __call__(&self, terms: Vec<u32>) -> PyHpoSet {
+        BasicPyHpoSet::build(terms.iter().map(|id| HpoTermId::from_u32(*id)))
+    }
+
+    #[classmethod]
+    fn from_queries(_cls: &PyType, queries: Vec<PyQuery>) -> PyResult<PyHpoSet> {
+        let mut ids: Vec<HpoTermId> = Vec::with_capacity(queries.len());
+        for q in queries {
+            ids.push(term_from_query(q)?.id());
+        }
+        Ok(BasicPyHpoSet::build(ids))
+    }
+
+    #[classmethod]
+    fn from_serialized(_cls: &PyType, pickle: &str) -> PyResult<PyHpoSet> {
+        Ok(BasicPyHpoSet::build(
+            pickle
+                .split('+')
+                .map(|id| id.parse::<u32>())
+                .collect::<Result<Vec<u32>, ParseIntError>>()?
+                .iter()
+                .map(|id| HpoTermId::from_u32(*id)),
+        ))
+    }
+}
```

### Comparing `hpo3-0.1.0/src/term.rs` & `hpo3-0.2.0/src/term.rs`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 use crate::PyGene;
 use crate::PyInformationContent;
 use crate::PyInformationContentKind;
 use crate::PyOmimDisease;
 
 #[pyclass(name = "HPOTerm")]
+#[derive(Clone)]
 pub struct PyHpoTerm {
     id: HpoTermId,
     name: String,
 }
 
 impl PyHpoTerm {
     pub fn new(id: HpoTermId, name: String) -> Self {
@@ -68,15 +69,15 @@
     /// Returns the HPO Term ID
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     term = ont.hpo(11968)
     ///     term.id()    # ==> 'HP:0011968'
     ///
     #[getter(id)]
     fn id(&self) -> String {
         self.id.to_string()
@@ -85,15 +86,15 @@
     /// Returns the name of the HPO Term
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     term = ont.hpo(11968)
     ///     term.name()  # ==> 'Feeding difficulties'
     ///
     #[getter(name)]
     fn name(&self) -> &str {
         &self.name
@@ -102,15 +103,15 @@
     /// Returns the Information Content of the HPO Term
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     term = ont.hpo(11968)
     ///     term.information_content.omim  # ==> 2.5363943576812744
     ///     term.information_content.gene  # ==> 1.457185983657837
     ///
     #[getter(information_content)]
     fn information_content(&self) -> PyInformationContent {
@@ -120,15 +121,15 @@
     /// A list of direct parents
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     term = ont.hpo(108)
     ///     term.parents  # ==> {<HpoTerm (HP:0011035)>, <HpoTerm (HP:0000107)>, <HpoTerm (HP:0100957)>}
     ///
     #[getter(parents)]
     fn parents(&self) -> HashSet<PyHpoTerm> {
         self.hpo().parents().fold(HashSet::new(), |mut set, term| {
@@ -143,15 +144,15 @@
     /// A list of all parents
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     term = ont.hpo(108)
     ///     term.all_parents  # ==> {large set}
     ///
     #[getter(all_parents)]
     fn all_parents(&self) -> HashSet<PyHpoTerm> {
         self.hpo()
@@ -168,15 +169,15 @@
     /// A list of direct children
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     term = ont.hpo(1)
     ///     term.children  # ==> {<HpoTerm (HP:0000005)>, <HpoTerm (HP:0000118)>, <HpoTerm (HP:0012823)>, <HpoTerm (HP:0032443)>, <HpoTerm (HP:0040279)>, <HpoTerm (HP:0032223)>}
     ///
     #[getter(children)]
     fn children(&self) -> HashSet<PyHpoTerm> {
         self.hpo().children().fold(HashSet::new(), |mut set, term| {
@@ -194,15 +195,15 @@
     /// linked to the term, but to one of its children
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     term = ont.hpo(188)
     ///     for gene in term.genes:
     ///         print(gene.name)
     ///
     #[getter(genes)]
     fn genes(&self) -> HashSet<PyGene> {
@@ -218,15 +219,15 @@
     /// linked to the term, but to one of its children
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///     ont = Ontology()
     ///     term = ont.hpo(188)
     ///     for disease in term.diseases:
     ///         print(disease.name)
     ///
     #[getter(omim_diseases)]
     fn diseases(&self) -> HashSet<PyOmimDisease> {
@@ -252,15 +253,16 @@
     fn parent_ids(&self) -> Vec<u32> {
         self.hpo().parent_ids().iter().map(|t| t.as_u32()).collect()
     }
 
     #[pyo3(text_signature = "($self, other)")]
     fn common_ancestors(&self, other: &PyHpoTerm) -> HashSet<PyHpoTerm> {
         self.hpo()
-            .common_ancestors(&other.hpo()).iter()
+            .common_ancestors(&other.hpo())
+            .iter()
             .fold(HashSet::new(), |mut set, term| {
                 set.insert(PyHpoTerm::from(term));
                 set
             })
     }
 
     #[pyo3(text_signature = "($self)")]
@@ -300,23 +302,33 @@
         )
     }
 
     /// Calculates the shortest path to another HPO Term
     ///
     /// IMPORTANT NOTE
     /// --------------
-    /// This method is not correctly implemented and will only return
-    /// the distance, but not the actual path. It will instead return
-    /// an empty list
-    ///
-    /// TODO: Double check if error handling might be required for e.g. obsolete terms
+    /// This method is not correctly implemented and will not return
+    /// the sub-paths distances
     #[pyo3(text_signature = "($self, other)")]
-    fn path_to_other(&self, other: &PyHpoTerm) -> (usize, Vec<PyHpoTerm>, usize, usize) {
-        let dist = self.hpo().distance_to_term(&other.into()).unwrap();
-        (dist, vec![], 0, 0)
+    pub fn path_to_other(
+        &self,
+        other: &PyHpoTerm,
+    ) -> PyResult<(usize, Vec<PyHpoTerm>, usize, usize)> {
+        let path = self
+            .hpo()
+            .path_to_term(&other.into())
+            .ok_or_else(|| PyRuntimeError::new_err("No path found"))?;
+        Ok((
+            path.len(),
+            path.iter()
+                .map(|id| pyterm_from_id(id.as_u32()).expect("term must be part of Ontology"))
+                .collect(),
+            0,
+            0,
+        ))
     }
 
     /// Calculates the similarity score of two HPO Terms
     ///
     /// Arguments
     /// ---------
     /// other: `int`
@@ -353,15 +365,15 @@
     ///     The similarity score
     ///
     /// Examples
     /// --------
     ///
     /// .. code-block:: python
     ///
-    ///     from hpo3 import Ontology
+    ///     from pyhpo import Ontology
     ///
     ///     ont = Ontology()
     ///     term = ont.hpo(11968)
     ///
     ///     term.similarity(1743)  
     ///
     ///     # compare HP:0011968 and HP:0001743 using Gene
```

### Comparing `hpo3-0.1.0/Cargo.lock` & `hpo3-0.2.0/Cargo.lock`

 * *Files identical despite different names*

