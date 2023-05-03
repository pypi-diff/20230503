# Comparing `tmp/facefinder-0.1.3.tar.gz` & `tmp/facefinder-0.1.4.tar.gz`

## Comparing `facefinder-0.1.3.tar` & `facefinder-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.3/Cargo.toml
--rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.3/.gitignore
--rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.3/src/python/facefinder/__init__.py
--rw-r--r--   0        0        0     6651 2023-04-20 14:34:18.000000 facefinder-0.1.3/src/python/facefinder/interact.py
--rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.3/src/python/facefinder/metadata.py
--rw-r--r--   0        0        0    19845 2023-04-30 10:25:34.000000 facefinder-0.1.3/src/python/facefinder/metrics.py
--rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.3/src/python/facefinder/prompting.py
--rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.3/src/rust/lib.rs
--rw-r--r--   0        0        0     7654 2023-04-30 10:54:28.000000 facefinder-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      270 1970-01-01 00:00:00.000000 facefinder-0.1.4/Cargo.toml
+-rw-r--r--   0        0        0     2795 2023-04-10 04:37:28.000000 facefinder-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      697 2023-04-20 14:44:25.000000 facefinder-0.1.4/.gitignore
+-rw-r--r--   0        0        0      541 2023-04-20 07:56:10.000000 facefinder-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-04-30 10:00:01.000000 facefinder-0.1.4/src/python/facefinder/__init__.py
+-rw-r--r--   0        0        0     6759 2023-05-02 06:23:15.000000 facefinder-0.1.4/src/python/facefinder/interact.py
+-rw-r--r--   0        0        0     3871 2023-04-20 09:22:54.000000 facefinder-0.1.4/src/python/facefinder/metadata.py
+-rw-r--r--   0        0        0    22216 2023-05-03 03:58:18.000000 facefinder-0.1.4/src/python/facefinder/metrics.py
+-rw-r--r--   0        0        0     4892 2023-03-14 01:32:39.000000 facefinder-0.1.4/src/python/facefinder/prompting.py
+-rw-r--r--   0        0        0      349 2023-04-20 07:54:19.000000 facefinder-0.1.4/src/rust/lib.rs
+-rw-r--r--   0        0        0     7654 2023-05-03 04:00:17.000000 facefinder-0.1.4/Cargo.lock
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 facefinder-0.1.4/PKG-INFO
```

### Comparing `facefinder-0.1.3/.github/workflows/CI.yml` & `facefinder-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.3/.gitignore` & `facefinder-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.3/pyproject.toml` & `facefinder-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.3/src/python/facefinder/interact.py` & `facefinder-0.1.4/src/python/facefinder/interact.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,31 +26,31 @@
     @staticmethod
     def show_image(image: np.ndarray, text: str = "image") -> None:
         cv2.imshow(text, image)
         cv2.waitKey(0)
         cv2.destroyAllWindows()
 
     def show_match(self, rank: int) -> None:
-        idx = self.metrics["indices"]["match"][rank]
-        j = self.metrics["paths"]["input"][idx[0]]
+        idx = self.metrics["indices"]["candidate_embedding_pair_idx"][rank]
+        j = self.metrics["paths"]["candidate"][idx[0]]
         k = self.metrics["paths"]["embedding"][idx[1]]
 
         im1 = cv2.imread(str(j))
         im2 = cv2.imread(str(k))
 
         h1, w1 = im1.shape[:2]
         h2, w2 = im2.shape[:2]
         h, w = max(h1, h2), max(w1, w2)
 
-        match_distance = self.metrics["distances"]["input_embedding"][idx]
-        target_distance = self.metrics["distances"]["input_target"][idx[0]].item()
+        match_distance = self.metrics["distances"]["pairs"][idx]
+        target_distance = self.metrics["distances"]["candidate_target"][idx[0]].item()
         embedding_distance = np.mean(
-            self.metrics["distances"]["input_embedding"][idx[0]]
+            self.metrics["distances"]["candidate_embedding"][idx[0]]
         )
-        score = self.metrics["metrics"]["scores"][idx[0]]
+        score = self.metrics["metrics"]["candidate_scores"][idx[0]]
 
         text_area = np.zeros((h, 500, 3), dtype="uint8")
         text_area.fill(255)
         text1 = f"score: {score}"
         text2 = f"match distance: {match_distance}"
         text3 = f"target distance: {target_distance}"
         text4 = f"embedding distance: {embedding_distance}"
@@ -77,24 +77,26 @@
         image = np.concatenate((im1, im2), axis=1)
         image = np.concatenate((image, text_area), axis=1)
 
         self.show_image(image)
 
     def show_cumulative(self, rank: int, target: bool = False) -> None:
         idx = (
-            self.metrics["indices"]["target"][rank]
+            self.metrics["indices"]["candidate_target_idx"][rank]
             if target
-            else self.metrics["indices"]["cumulative"][rank]
+            else self.metrics["indices"]["candidate_score_idx"][rank]
         )
-        image = cv2.imread(str(self.metrics["paths"]["input"][idx]))
+        image = cv2.imread(str(self.metrics["paths"]["candidate"][idx]))
 
         h, w = image.shape[:2]
-        target_distance = self.metrics["distances"]["input_target"][idx].item()
-        embedding_distance = np.mean(self.metrics["distances"]["input_embedding"][idx])
-        score = self.metrics["metrics"]["scores"][idx]
+        target_distance = self.metrics["distances"]["candidate_target"][idx].item()
+        embedding_distance = np.mean(
+            self.metrics["distances"]["candidate_embedding"][idx]
+        )
+        score = self.metrics["metrics"]["candidate_scores"][idx]
 
         text_area = np.zeros((h, 500, 3)).astype("uint8")
         text_area.fill(255)
         text1 = f"score: {score}"
         text2 = f"target distance: {target_distance}"
         text3 = f"embedding distance: {embedding_distance}"
 
@@ -130,15 +132,15 @@
 
         parts = user_input.split(" ")
         if len(parts) < 2:
             raise ValueError(
                 f"Missing arguments: Please provide a function (m, e, t) and a stopping point/range (as an integer)"
             )
         f, _range, *other_args = parts
-        n_images = len(self.metrics["paths"]["input"])
+        n_images = len(self.metrics["paths"]["candidate"])
 
         if f.startswith("m"):
             f = self.show_match
         elif f.startswith("e"):
             f = self.show_cumulative
         elif f.startswith("t"):
             f = partial(self.show_cumulative, target=True)
```

### Comparing `facefinder-0.1.3/src/python/facefinder/metadata.py` & `facefinder-0.1.4/src/python/facefinder/metadata.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.3/src/python/facefinder/metrics.py` & `facefinder-0.1.4/src/python/facefinder/metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -169,25 +169,48 @@
     candidate_paths = np.array(candidate_paths)[non_duplicate_idx]
     candidate_reprs = np.array(candidate_reprs)[non_duplicate_idx]
     target_distances = np.array(target_distances)[non_duplicate_idx]
 
     return candidate_paths, candidate_reprs, target_distances
 
 
-def calculate_image_scores(
+def calculate_weighted_distances_old(
     embedding_target_distances: list[float],
     candidate_embedding_distances: list[list[float]],
-    weight_relevance: int = 1,
+    target_distance_bias: int = 1,
 ) -> list[float]:
-    weights = np.power(embedding_target_distances.T, weight_relevance)
+    weights = np.power(embedding_target_distances.T, target_distance_bias)
     weighted_distances = np.power(
-        candidate_embedding_distances * weights, 1 / (weight_relevance + 1)
+        candidate_embedding_distances * weights,
+        1 / (target_distance_bias + 1),
     )
-    candidate_scores = np.mean(weighted_distances, axis=1)
-    return candidate_scores
+    return np.mean(weighted_distances, axis=1)
+
+
+def calculate_weighted_distances(
+    embedding_target_distances: list[float],
+    candidate_embedding_distances: list[list[float]],
+    target_distance_bias: int = 1,
+) -> list[float]:
+    weights = np.power(embedding_target_distances.T, 1 / (target_distance_bias + 1))
+    weighted_distances = candidate_embedding_distances * weights
+    return weighted_distances.mean(axis=1)
+
+
+def calculate_scores(
+    target_distances: np.ndarray,
+    weighted_distances: np.ndarray,
+    embedding_accuracy: float,
+) -> np.ndarray:
+    wd_weight = 0.8 * (0.5 ** (5 * embedding_accuracy))
+    td_weight = 1 - wd_weight
+    scores = (target_distances.flatten() * td_weight) + (
+        weighted_distances.flatten() * wd_weight
+    )
+    return scores
 
 
 def get_embedding_metrics(
     model: str,
     target_path: Optional[Path] = None,
     embedding_dir: Optional[Path] = None,
 ) -> dict[str, Any]:
@@ -225,123 +248,143 @@
 
 def get_candidate_metrics(
     model: str,
     target_repr: list[float],
     embedding_reprs: list[list[float]],
     embedding_target_distances: list[float],
     candidate_dir: Optional[Path] = None,
-    weight_relevance: int = 1,
+    target_distance_bias: int = 1,
 ) -> dict[str, Any]:
     candidate_dir = candidate_dir or metadata.PATHS.UNPROCESSED_IMAGES
 
     # Initial (non-filtered) candidate representations
     paths, representations = get_representations(candidate_dir, model)
     x = 0
 
     # Filtering processed images by distance to target
     paths, representations, candidate_target_distances = get_filtered(
         target_repr, representations, paths
     )
 
     # Distances between candidates and embeddings
-    candidate_embedding_distances = cosine_dist(embedding_reprs, representations)
+    candidate_embedding_pair_distances = cosine_dist(embedding_reprs, representations)
+    candidate_embedding_distances = candidate_embedding_pair_distances.mean(axis=1)
 
     # Weighting the candidate distances by the embedding image scores (relative to the target)
-    scores = calculate_image_scores(
-        embedding_target_distances, candidate_target_distances, weight_relevance
+    candidate_weighted_distances = calculate_weighted_distances(
+        embedding_target_distances,
+        candidate_embedding_pair_distances,
+        target_distance_bias,
     )
 
     # Doing the same for embedding images
-    embedding_scores = calculate_image_scores(
-        embedding_target_distances, embedding_target_distances, weight_relevance
+    embedding_weighted_distances = calculate_weighted_distances(
+        embedding_target_distances,
+        cosine_dist(embedding_reprs, embedding_reprs),
+        target_distance_bias,
     )
 
-    # Gathering sorted indices for interactive functions (candidate images only)
-    candidate_embedding_idx = list(
-        zip(
-            *np.unravel_index(
-                np.argsort(candidate_embedding_distances, axis=None),
-                candidate_embedding_distances.shape,
-            )
-        )
-    )
-    candidate_score_idx = np.argsort(scores, axis=None).tolist()
-    candidate_target_idx = np.argsort(candidate_target_distances, axis=None).tolist()
-
-    # Gathering sorted indices for interactive functions (embedding images only)
-    embedding_score_idx = np.argsort(embedding_scores, axis=None).tolist()
-    embedding_target_idx = np.argsort(embedding_target_distances, axis=None).tolist()
-
     return {
         "paths": paths,
         "representations": representations,
         "candidate_target_distances": candidate_target_distances,
+        "candidate_embedding_pair_distances": candidate_embedding_pair_distances,
         "candidate_embedding_distances": candidate_embedding_distances,
-        "candidate_scores": scores,
-        "embedding_scores": embedding_scores,
+        "candidate_weighted_distances": candidate_weighted_distances,
+        "embedding_weighted_distances": embedding_weighted_distances,
     }
 
 
 def get_indices(metrics: dict) -> dict:
     # Gathering sorted indices for interactive functions (candidate images only)
+    candidate_embedding_pair_distances = metrics["distances"]["pairs"]
     candidate_embedding_distances = metrics["distances"]["candidate_embedding"]
-    candidate_scores = metrics["metrics"]["candidate_scores"]
+    candidate_weighted_distances = metrics["metrics"]["candidate_weighted_distances"]
     candidate_target_distances = metrics["distances"]["candidate_target"]
+    candidate_scores = metrics["metrics"]["candidate_scores"]
 
-    candidate_embedding_idx = list(
+    candidate_embedding_pair_idx = list(
         zip(
             *np.unravel_index(
-                np.argsort(candidate_embedding_distances, axis=None),
-                candidate_embedding_distances.shape,
+                np.argsort(candidate_embedding_pair_distances, axis=None),
+                candidate_embedding_pair_distances.shape,
             )
         )
     )
+    candidate_embedding_idx = np.argsort(
+        candidate_embedding_distances, axis=None
+    ).tolist()
+    candidate_weighted_idx = np.argsort(
+        candidate_weighted_distances, axis=None
+    ).tolist()
     candidate_score_idx = np.argsort(candidate_scores, axis=None).tolist()
     candidate_target_idx = np.argsort(candidate_target_distances, axis=None).tolist()
 
     # Gathering sorted indices for interactive functions (embedding images only)
     embedding_embedding_distances = metrics["distances"]["embedding_embedding"]
-    embedding_scores = metrics["metrics"]["embedding_scores"]
+    embedding_weighted_distances = metrics["metrics"]["embedding_weighted_distances"]
     embedding_target_distances = metrics["distances"]["embedding_target"]
+    embedding_scores = metrics["metrics"]["embedding_scores"]
 
     embedding_embedding_idx = np.argsort(
         embedding_embedding_distances, axis=None
     ).tolist()
+    embedding_weighted_idx = np.argsort(
+        embedding_weighted_distances, axis=None
+    ).tolist()
     embedding_score_idx = np.argsort(embedding_scores, axis=None).tolist()
     embedding_target_idx = np.argsort(embedding_target_distances, axis=None).tolist()
 
     return {
         "candidate_embedding_idx": candidate_embedding_idx,
         "candidate_score_idx": candidate_score_idx,
         "candidate_target_idx": candidate_target_idx,
+        "candidate_weighted_idx": candidate_weighted_idx,
         "embedding_embedding_idx": embedding_embedding_idx,
         "embedding_score_idx": embedding_score_idx,
         "embedding_target_idx": embedding_target_idx,
+        "embedding_weighted_idx": embedding_weighted_idx,
+        "candidate_embedding_pair_idx": candidate_embedding_pair_idx,
     }
 
 
+def add_scores(metrics: dict) -> dict:
+    candidate_scores = calculate_scores(
+        metrics["distances"]["candidate_target"],
+        metrics["metrics"]["candidate_weighted_distances"],
+        metrics["metrics"]["embedding_accuracy"],
+    )
+    embedding_scores = calculate_scores(
+        metrics["distances"]["embedding_target"],
+        metrics["metrics"]["embedding_weighted_distances"],
+        metrics["metrics"]["embedding_accuracy"],
+    )
+    metrics["metrics"]["candidate_scores"] = candidate_scores
+    metrics["metrics"]["embedding_scores"] = embedding_scores
+
+
 def get_metrics(
     model: str,
     target_path: Optional[str | Path] = None,
     embedding_dir: Optional[str | Path] = None,
     candidate_dir: Optional[str | Path] = None,
-    weight_relevance: int = 1,
+    target_distance_bias: int = 1,
 ) -> dict[str, Any]:
     target_path = target_path or metadata.PATHS.TARGET_IMAGE
     embedding_dir = embedding_dir or metadata.PATHS.EMBEDDING_IMAGES
     candidate_dir = candidate_dir or metadata.PATHS.UNPROCESSED_IMAGES
 
     embedding_metrics = get_embedding_metrics(model, target_path, embedding_dir)
     candidate_metrics = get_candidate_metrics(
         model,
         embedding_metrics["target_representation"],
         embedding_metrics["representations"],
         embedding_metrics["embedding_target_distances"],
         candidate_dir,
-        weight_relevance,
+        target_distance_bias,
     )
     metrics = {
         "paths": {
             "target": embedding_metrics["target_path"],
             "embedding": embedding_metrics["paths"],
             "candidate": candidate_metrics["paths"],
         },
@@ -351,35 +394,47 @@
             "candidate": candidate_metrics["representations"],
         },
         "distances": {
             "embedding_target": embedding_metrics["embedding_target_distances"],
             "embedding_embedding": embedding_metrics["embedding_embedding_distances"],
             "candidate_target": candidate_metrics["candidate_target_distances"],
             "candidate_embedding": candidate_metrics["candidate_embedding_distances"],
+            "pairs": candidate_metrics["candidate_embedding_pair_distances"],
         },
         "metrics": {
             "embedding_accuracy": embedding_metrics["mean_target_distance"],
             "embedding_coherence": embedding_metrics["mean_embedding_distance"],
-            "candidate_scores": candidate_metrics["candidate_scores"],
-            "embedding_scores": candidate_metrics["embedding_scores"],
+            "candidate_weighted_distances": candidate_metrics[
+                "candidate_weighted_distances"
+            ],
+            "embedding_weighted_distances": candidate_metrics[
+                "embedding_weighted_distances"
+            ],
         },
-        "metadata": {"model": model, "weight_relevance": weight_relevance},
+        "metadata": {"model": model, "target_distance_bias": target_distance_bias},
     }
+
+    add_scores(metrics)
     metrics["indices"] = get_indices(metrics)
     return metrics
 
 
 def get_quantiles(metrics: dict) -> dict:
     preprocess = {
         "embedding_target_distances": metrics["distances"]["embedding_target"],
         "embedding_embedding_distances": metrics["distances"]["embedding_embedding"],
-        "embedding_scores": metrics["metrics"]["embedding_scores"],
+        "embedding_weighted_distances": metrics["metrics"][
+            "embedding_weighted_distances"
+        ],
         "candidate_target_distances": metrics["distances"]["candidate_target"],
         "candidate_embedding_distances": metrics["distances"]["candidate_embedding"],
-        "candidate_scores": metrics["metrics"]["candidate_scores"],
+        "candidate_weighted_distances": metrics["metrics"][
+            "candidate_weighted_distances"
+        ],
+        "pair_distances": metrics["distances"]["pairs"],
     }
 
     quantile_values = np.arange(0, 1, 0.01)
     return {k: np.quantile(v, quantile_values) for k, v in preprocess.items()}
 
 
 def create_scaler(n: float) -> Callable:
@@ -406,81 +461,87 @@
 
 
 def merge_metrics(metrics: list[dict[str, Any]]) -> dict[str, Any]:
     paths = metrics[0]["paths"]
     representations = {m["metadata"]["model"]: m["representations"] for m in metrics}
     metadata = {
         "model": [m["metadata"]["model"] for m in metrics],
-        "weight_relevance": [m["metadata"]["weight_relevance"] for m in metrics],
+        "target_distance_bias": [
+            m["metadata"]["target_distance_bias"] for m in metrics
+        ],
     }
     means = [distance_mean(m["distances"]) for m in metrics]
     grand_mean = np.mean(np.array(means))
     distances = {
         "embedding_target": [],
         "embedding_embedding": [],
         "candidate_target": [],
         "candidate_embedding": [],
+        "pairs": [],
     }
     for m, mean in zip(metrics, means):
         scaler = create_scaler(mean)
         for k, v in m["distances"].items():
             if len(v.shape) == 1:
                 v = v[:, None]
             distances[k].append(scaler(v)[:, :, None])
     distances = {
-        k: np.mean(np.concatenate(v, axis=2), axis=2) * grand_mean
+        k: np.mean(np.concatenate(v, axis=2), axis=2) * 2 * grand_mean
         for k, v in distances.items()
     }
 
-    candidate_scores = calculate_image_scores(
+    candidate_weighted_distances = calculate_weighted_distances(
         distances["embedding_target"],
         distances["candidate_embedding"],
-        np.mean(metadata["weight_relevance"]),
+        np.mean(metadata["target_distance_bias"]),
     )
-    embedding_scores = calculate_image_scores(
+    embedding_weighted_distances = calculate_weighted_distances(
         distances["embedding_target"],
         distances["embedding_embedding"],
-        np.mean(metadata["weight_relevance"]),
+        np.mean(metadata["target_distance_bias"]),
     )
     embedding_accuracy = np.mean(distances["embedding_target"])
     embedding_coherence = np.mean(distances["embedding_embedding"])
     sub_metrics = {
         "embedding_accuracy": embedding_accuracy,
         "embedding_coherence": embedding_coherence,
-        "candidate_scores": candidate_scores,
-        "embedding_scores": embedding_scores,
+        "candidate_weighted_distances": candidate_weighted_distances,
+        "embedding_weighted_distances": embedding_weighted_distances,
     }
 
     metrics = {
         "paths": paths,
         "representations": representations,
         "distances": distances,
         "metrics": sub_metrics,
         "metadata": metadata,
     }
 
+    add_scores(metrics)
     metrics["indices"] = get_indices(metrics)
     metrics["quantiles"] = get_quantiles(metrics)
 
     return metrics
 
 
 def get_multimodel_metrics(
     models: list[str],
     target_path: Optional[str | Path] = None,
     embedding_dir: Optional[str | Path] = None,
     candidate_dir: Optional[str | Path] = None,
-    weight_relevance: int = 1,
+    target_distance_bias: int = 1,
 ) -> dict[str, Any]:
     target_path = target_path or metadata.PATHS.TARGET_IMAGE
     embedding_dir = embedding_dir or metadata.PATHS.EMBEDDING_IMAGES
     candidate_dir = candidate_dir or metadata.PATHS.UNPROCESSED_IMAGES
 
     all_metrics = [
-        get_metrics(model, target_path, embedding_dir, candidate_dir, weight_relevance)
+        get_metrics(
+            model, target_path, embedding_dir, candidate_dir, target_distance_bias
+        )
         for model in models
     ]
     return merge_metrics(all_metrics)
 
 
 def save_processed_embedding_images(
     metrics: dict[str, Any], output_dir: Optional[Path] = None
@@ -514,15 +575,15 @@
     if not os.path.exists(output_dir):
         os.makedirs(output_dir)
 
     n_images = len(metrics["paths"]["candidate"])
     for path, score, accuracy, coherence in tqdm(
         zip(
             metrics["paths"]["candidate"],
-            metrics["metrics"]["scores"],
+            metrics["metrics"]["candidate_weighted_distances"],
             metrics["distances"]["candidate_target"],
             np.mean(metrics["distances"]["candidate_embedding"], axis=1),
         ),
         desc=f"Saving {n_images}, Processed Images",
         total=n_images,
     ):
         image_id = path.name.split("-")[0]
@@ -532,15 +593,15 @@
         image_path = str(output_dir.joinpath(image_name))
         cv2.imwrite(image_path, cv2.imread(str(path)))
 
 
 def main(interactive: bool = False) -> None:
     # Processing Images
     metrics = get_multimodel_metrics(
-        ["Facenet512"], weight_relevance=1
+        ["Facenet512"], target_distance_bias=1
     )  # "SFace", "ArcFace"])
 
     # Saving scored images
     save_processed_embedding_images(metrics)
     save_processed_candidate_images(metrics)
 
     if interactive:
```

### Comparing `facefinder-0.1.3/src/python/facefinder/prompting.py` & `facefinder-0.1.4/src/python/facefinder/prompting.py`

 * *Files identical despite different names*

### Comparing `facefinder-0.1.3/Cargo.lock` & `facefinder-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "facefinder"
-version = "0.1.3"
+version = "0.1.4"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "indoc"
 version = "1.0.9"
```

