# Comparing `tmp/fepops-1.2.0.tar.gz` & `tmp/fepops-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fepops-1.2.0.tar", last modified: Sat Apr 15 21:05:36 2023, max compression
+gzip compressed data, was "fepops-1.3.0.tar", last modified: Wed May  3 13:57:10 2023, max compression
```

## Comparing `fepops-1.2.0.tar` & `fepops-1.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-15 21:05:36.973395 fepops-1.2.0/
--rw-rw-r--   0 justin    (1002) justin    (1002)     1068 2022-12-16 13:40:46.000000 fepops-1.2.0/LICENSE.md
--rw-rw-r--   0 justin    (1002) justin    (1002)     4499 2023-04-15 21:05:36.973395 fepops-1.2.0/PKG-INFO
--rw-rw-r--   0 justin    (1002) justin    (1002)     4078 2023-04-04 21:29:22.000000 fepops-1.2.0/README.md
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-15 21:05:36.973395 fepops-1.2.0/fepops/
--rw-rw-r--   0 justin    (1002) justin    (1002)       26 2023-03-28 16:17:49.000000 fepops-1.2.0/fepops/__init__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)     3717 2023-04-08 17:08:41.000000 fepops-1.2.0/fepops/__main__.py
--rw-rw-r--   0 justin    (1002) justin    (1002)    20613 2023-04-14 16:19:38.000000 fepops-1.2.0/fepops/fepops.py
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-15 21:05:36.973395 fepops-1.2.0/fepops.egg-info/
--rw-rw-r--   0 justin    (1002) justin    (1002)     4499 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/PKG-INFO
--rw-rw-r--   0 justin    (1002) justin    (1002)      269 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/SOURCES.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)        1 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/dependency_links.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)      119 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/requires.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)        7 2023-04-15 21:05:36.000000 fepops-1.2.0/fepops.egg-info/top_level.txt
--rw-rw-r--   0 justin    (1002) justin    (1002)      118 2023-04-01 11:25:23.000000 fepops-1.2.0/pyproject.toml
--rw-rw-r--   0 justin    (1002) justin    (1002)      680 2023-04-15 21:05:36.973395 fepops-1.2.0/setup.cfg
-drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-04-15 21:05:36.973395 fepops-1.2.0/test/
--rw-rw-r--   0 justin    (1002) justin    (1002)      956 2023-04-01 11:25:23.000000 fepops-1.2.0/test/tests.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-05-03 13:57:10.208404 fepops-1.3.0/
+-rw-rw-r--   0 justin    (1002) justin    (1002)     1068 2022-12-16 13:40:46.000000 fepops-1.3.0/LICENSE.md
+-rw-rw-r--   0 justin    (1002) justin    (1002)     4500 2023-05-03 13:57:10.208404 fepops-1.3.0/PKG-INFO
+-rw-rw-r--   0 justin    (1002) justin    (1002)     4079 2023-05-03 13:53:36.000000 fepops-1.3.0/README.md
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-05-03 13:57:10.192404 fepops-1.3.0/fepops/
+-rw-rw-r--   0 justin    (1002) justin    (1002)       26 2023-03-28 16:17:49.000000 fepops-1.3.0/fepops/__init__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)     3717 2023-04-08 17:08:41.000000 fepops-1.3.0/fepops/__main__.py
+-rw-rw-r--   0 justin    (1002) justin    (1002)    23245 2023-05-02 17:37:04.000000 fepops-1.3.0/fepops/fepops.py
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-05-03 13:57:10.192404 fepops-1.3.0/fepops.egg-info/
+-rw-rw-r--   0 justin    (1002) justin    (1002)     4500 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/PKG-INFO
+-rw-rw-r--   0 justin    (1002) justin    (1002)      269 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/SOURCES.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)        1 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/dependency_links.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)      136 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/requires.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)        7 2023-05-03 13:57:10.000000 fepops-1.3.0/fepops.egg-info/top_level.txt
+-rw-rw-r--   0 justin    (1002) justin    (1002)      118 2023-04-01 11:25:23.000000 fepops-1.3.0/pyproject.toml
+-rw-rw-r--   0 justin    (1002) justin    (1002)      696 2023-05-03 13:57:10.208404 fepops-1.3.0/setup.cfg
+drwxrwxr-x   0 justin    (1002) justin    (1002)        0 2023-05-03 13:57:10.192404 fepops-1.3.0/test/
+-rw-rw-r--   0 justin    (1002) justin    (1002)      956 2023-04-01 11:25:23.000000 fepops-1.3.0/test/tests.py
```

### Comparing `fepops-1.2.0/LICENSE.md` & `fepops-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `fepops-1.2.0/PKG-INFO` & `fepops-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fepops
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python implementation of the FEPOPS molecular descriptors
 Home-page: https://github.com/JustinYKC/FEPOPS
 Author: Yan-Kai Chen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -38,15 +38,15 @@
 A quickstart example to generate the FEPOPS descriptors for a molecule directly from its SMILES as follows: In terminal:
 ```
 python fepops.py get_fepops -ismi "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" 
 ```
 
 A quickstart example to calculate the FEPOPS similarity between two molecules using their SMILES as follows: In terminal:
 ```
-python fepops.py cal_sim -ismi1 "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" -ismi2 "OC=1C=C(O)C=C(C1)C=2OC=3C=CC=CC3C2"
+python fepops.py calc_sim -ismi1 "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" -ismi2 "OC=1C=C(O)C=C(C1)C=2OC=3C=CC=CC3C2"
 ```
 
 An example of filtering molecules in the dataset of natural products: `COCONUT.DB.smi` [COCONUT.DB.smi](https://coconut.naturalproducts.net/download), for further use of the FEPOPS generation:
 ```
 python mol_filter.py
 ```
```

### Comparing `fepops-1.2.0/README.md` & `fepops-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 A quickstart example to generate the FEPOPS descriptors for a molecule directly from its SMILES as follows: In terminal:
 ```
 python fepops.py get_fepops -ismi "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" 
 ```
 
 A quickstart example to calculate the FEPOPS similarity between two molecules using their SMILES as follows: In terminal:
 ```
-python fepops.py cal_sim -ismi1 "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" -ismi2 "OC=1C=C(O)C=C(C1)C=2OC=3C=CC=CC3C2"
+python fepops.py calc_sim -ismi1 "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" -ismi2 "OC=1C=C(O)C=C(C1)C=2OC=3C=CC=CC3C2"
 ```
 
 An example of filtering molecules in the dataset of natural products: `COCONUT.DB.smi` [COCONUT.DB.smi](https://coconut.naturalproducts.net/download), for further use of the FEPOPS generation:
 ```
 python mol_filter.py
 ```
```

### Comparing `fepops-1.2.0/fepops/__main__.py` & `fepops-1.3.0/fepops/__main__.py`

 * *Files identical despite different names*

### Comparing `fepops-1.2.0/fepops/fepops.py` & `fepops-1.3.0/fepops/fepops.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,80 @@
 from rdkit import Chem
 from rdkit.Chem import AllChem
 from rdkit.Chem import MolStandardize
-from rdkit.Chem import Crippen
+from rdkit.Chem import Crippen, Lipinski
 from rdkit.Chem import rdMolTransforms
 from sklearn.cluster import KMeans as _SKLearnKMeans
 from fast_pytorch_kmeans import KMeans as _FastPTKMeans
 from sklearn.preprocessing import StandardScaler
 from scipy.spatial.distance import cdist, squareform, pdist
+from scipy.special import softmax
 import numpy as np
 import itertools
 import torch
-from typing import Union
+from typing import Union, Optional
 
 
 class Fepops:
 	"""Fepops molecular similarity object
 
 	Fepops allows the comparison of molecules using feature points, see
-	the original publication for more information. https://pubs.acs.org/doi/10.1021/jm049654z
+	the original publication for more information https://pubs.acs.org/doi/10.1021/jm049654z
+	In short, featurepoints reduce the number of points used to represent a molecule and can
+	be used to compare molecules in the hope of discovering biosimilars based on queries.
 
 	Parameters
 	----------
 	kmeans_method : str, optional
 		Method which should be used for kmeans calculation, can be
 		one of "sklearn", "pytorch-gpu", or "pytorch-cpu". By
 		default "pytorch-cpu".
 
 	Raises
 	------
 	ValueError
 		Invalid kmeans method
 	"""
-	implemented_kmeans_methods = ["sklearn", "pytorch-cpu", "pytorch-gpu"]
-	sort_by_features_col_index_dict = {
-		"charge": 0,
-		"logP": 1,
-		"hba": 2,
-		"hbd": 3,
-	}
-	donor_mol_from_smarts = Chem.MolFromSmarts("[!H0;#7,#8,#9]")
-	acceptor_mol_from_smarts = Chem.MolFromSmarts(
+
+	def __init__(
+			self,
+			kmeans_method: str = "pytorch-cpu",
+			max_tautomers:Optional[int]=None,
+			*,
+			num_fepops_per_mol:int=7,
+			num_centroids_per_fepop:int=4,
+			):
+
+		self.num_fepops_per_mol=num_fepops_per_mol
+		self.num_centroids_per_fepop=num_centroids_per_fepop
+		self.implemented_kmeans_methods = ["sklearn", "pytorch-cpu", "pytorch-gpu"]
+		self.sort_by_features_col_index_dict = {
+			"charge": 0,
+			"logP": 1,
+			"hba": 2,
+			"hbd": 3,
+		}
+		self.donor_mol_from_smarts = Chem.MolFromSmarts("[!H0;#7,#8,#9]")
+		self.acceptor_mol_from_smarts = Chem.MolFromSmarts(
 			"[!$([#6,F,Cl,Br,I,o,s,nX3,#7v5,#15v5,#16v4,#16v6,*+1,*+2,*+3])]"
 		)
-	rotatable_bond_from_smarts = Chem.MolFromSmarts(
+		self.rotatable_bond_from_smarts = Chem.MolFromSmarts(
 			"[!$(*#*)&!D1]-&!@[!$(*#*)&!D1]"
 		)
-
-	def __init__(self, kmeans_method: str = "pytorch-cpu"):
 		if kmeans_method not in self.implemented_kmeans_methods:
 			raise ValueError(
 				f"Supplied argument kmeans_method '{kmeans_method}' not found, please supply a string denoting an implemented kmeans method from {self.implemented_kmeans_methods}"
 			)
 		self.kmeans_method_str = kmeans_method
-		self.tautomer_enumerator = MolStandardize.tautomer.TautomerEnumerator()
+		self.tautomer_enumerator = MolStandardize.tautomer.TautomerEnumerator(**{'max_tautomers':max_tautomers} if max_tautomers is not None else {})
 		self.scaler = StandardScaler()
 
-	@staticmethod
-	def _get_k_medoids(input_x: np.ndarray, k: int = 7, seed:int=42) -> np.ndarray:
+	def _get_k_medoids(
+		self, input_x: np.ndarray, k: int = 7, seed: int = 42
+	) -> np.ndarray:
 		"""Select k Fopops conformers to generate the final Fepops descriptors
 
 		A private method used to perform k-medoids in order to derive the final Fepops descriptors
 		by selecting k representative Fepops conformers.
 
 		Parameters
 		----------
@@ -78,15 +92,15 @@
 
 		if input_x.shape[0] <= k:
 			return input_x
 
 		point_to_centroid_map = np.ones(input_x.shape[0])
 		point_to_centroid_map_prev = np.zeros_like(point_to_centroid_map)
 
-		np_rng=np.random.default_rng(seed=seed)
+		np_rng = np.random.default_rng(seed=seed)
 		medoids = input_x[
 			np_rng.choice(np.arange(input_x.shape[0]), size=k, replace=False), :
 		]
 
 		while (point_to_centroid_map != point_to_centroid_map_prev).any():
 			point_to_centroid_map_prev = point_to_centroid_map
 			point_to_centroid_map = np.argmin(
@@ -97,41 +111,23 @@
 				if len(medoid_members) == 0:
 					chosen_x_point = np_rng.choice(np.arange(input_x.shape[0]))
 					medoids[i] = input_x[chosen_x_point, :]
 					point_to_centroid_map[chosen_x_point] = i
 				medoids[i] = np.median(
 					input_x[point_to_centroid_map == i], axis=0
 				)  # Using median to ensure the minimum distance to its medoid_members to be returned
-		return medoids
+		# Return medoids sorted by the first column (charge), second to last, then 3rd first etc.
+		return medoids[np.lexsort(medoids.T[::-1])]
 
-	@staticmethod
-	def annotate_atom_idx(mol: Chem.rdchem.Mol):
+	def annotate_atom_idx(self, mol: Chem.rdchem.Mol):
 		for i, atom in enumerate(mol.GetAtoms()):
 			# For each atom, set the property "molAtomMapNumber" to a custom number, let's say, the index of the atom in the molecule
 			atom.SetProp("molAtomMapNumber", str(atom.GetIdx()))
 
-	def _get_tautomers(self, mol: Chem.rdchem.Mol) -> list:
-		"""Enumerate all tautomers for an input molecule
-
-		A private function used for generating all tautomers for a molecule.
-
-		Parameters
-		----------
-		mol : Chem.rdchem.Mol
-			The Rdkit mol object of the input molecule.
-
-		Returns
-		-------
-		List
-			List containing enumerated tautomers.
-		"""
-		return self.tautomer_enumerator.enumerate(mol)
-
-	@staticmethod
-	def _calculate_atomic_logPs(mol: Chem.rdchem.Mol) -> dict:
+	def _calculate_atomic_logPs(self, mol: Chem.rdchem.Mol) -> dict:
 		"""Calculate logP contribution for each of atom in a molecule
 
 		Parameters
 		----------
 		mol : Chem.rdchem.Mol
 			The Rdkit mol object of the input molecule.
 
@@ -143,16 +139,15 @@
 		return {
 			atom.GetIdx(): float(contribution[0])
 			for atom, contribution in zip(
 				mol.GetAtoms(), Crippen.rdMolDescriptors._CalcCrippenContribs(mol)
 			)
 		}
 
-	@staticmethod
-	def _calculate_partial_charges(mol: Chem.rdchem.Mol) -> dict:
+	def _calculate_partial_charges(self, mol: Chem.rdchem.Mol) -> dict:
 		"""Calculate the charge of each atom in a molecule
 
 		Parameters
 		----------
 		mol : Chem.rdchem.Mol
 			The Rdkit mol object of the input molecule.
 
@@ -163,17 +158,16 @@
 		"""
 		Chem.rdPartialCharges.ComputeGasteigerCharges(mol)
 		return {
 			atom.GetIdx(): float(atom.GetProp("_GasteigerCharge"))
 			for atom in mol.GetAtoms()
 		}
 
-	@staticmethod
 	def _sum_of_atomic_features_by_centroids(
-		feature_dict: dict, centroid_atom_idx: np.ndarray
+		self, feature_dict: dict, centroid_atom_idx: np.ndarray
 	) -> int:
 		"""Sum all atomic features according to their centroid group
 
 		A method that that is used to sum all the atomic features based on their centroid group.
 
 		Parameters
 		----------
@@ -185,16 +179,15 @@
 		Returns
 		-------
 		int
 			Sum of the features across the centroid group of atoms.
 		"""
 		return sum([v for k, v in feature_dict.items() if k in centroid_atom_idx])
 
-	@staticmethod
-	def _get_dihedrals(mol: Chem.rdchem.Mol) -> tuple:
+	def _get_dihedrals(self, mol: Chem.rdchem.Mol) -> tuple:
 		"""Identify dihedrals in order to obtain rotatable bonds in a molecule
 
 		Identify dihedrals using flanking atoms of rotatable bonds
 
 		Parameters
 		----------
 		mol : Chem.rdchem.Mol
@@ -202,26 +195,26 @@
 
 		Returns
 		-------
 		tuple
 			A tuple containing all identified dihedrals with the index of their four defined atoms.
 		"""
 		dihedrals = []
-		for atom_j, atom_k in mol.GetSubstructMatches(Fepops.rotatable_bond_from_smarts):
-			atom_i, atom_l = Fepops._get_flanking_atoms(mol.GetBonds(), atom_j, atom_k)
+		for atom_j, atom_k in mol.GetSubstructMatches(self.rotatable_bond_from_smarts):
+			atom_i, atom_l = self._get_flanking_atoms(mol.GetBonds(), atom_j, atom_k)
 			if atom_i is not None and atom_l is not None:
 				dihedrals.append((atom_i, atom_j, atom_k, atom_l))
 		return dihedrals
 
-	@staticmethod
 	def _perform_kmeans(
+		self,
 		atom_coords: np.ndarray,
 		num_centroids: int = 4,
 		kmeans_method: str = "pytorch-cpu",
-		seed:int=42,
+		seed: int = 42,
 	) -> tuple:
 		"""Perform kmeans calculation
 
 		Carry out kmeans calcaultion based on a given kmeans method and number of centroids.
 
 		Parameters
 		----------
@@ -237,54 +230,74 @@
 
 		Returns
 		-------
 		tuple
 			A tuple containing the centroid coordinates and the cluster labels of molecular atoms.
 		"""
 		if kmeans_method == "sklearn":
-			kmeans = _SKLearnKMeans(n_clusters=num_centroids, random_state=seed, n_init='auto').fit(atom_coords)
+			kmeans = _SKLearnKMeans(
+				n_clusters=num_centroids, random_state=seed, n_init="auto"
+			).fit(atom_coords)
 			centroid_coors = kmeans.cluster_centers_
 			instance_cluster_labels = kmeans.labels_
 		elif kmeans_method.startswith("pytorch"):
-			mol_coors_torch = torch.from_numpy(atom_coords).to('cuda' if kmeans_method.endswith("gpu") else "cpu")
+			torch.manual_seed(seed)
+			mol_coors_torch = torch.from_numpy(atom_coords).to(
+				"cuda" if kmeans_method.endswith("gpu") else "cpu"
+			)
 			kmeans = _FastPTKMeans(n_clusters=num_centroids, max_iter=300)
 			instance_cluster_labels = kmeans.fit_predict(
-				mol_coors_torch, centroids=torch.tensor(atom_coords[:num_centroids], device=mol_coors_torch.device)
+				mol_coors_torch,
+				centroids=torch.tensor(
+					atom_coords[:num_centroids], device=mol_coors_torch.device
+				),
 			).numpy()
 			centroid_coors = kmeans.centroids.numpy()
 		else:
 			raise ValueError(
-				f"The method selected for the k-means calculation is invalid, please use one of {Fepops.implemented_kmeans_methods}"
+				f"The method selected for the k-means calculation is invalid, please use one of {self.implemented_kmeans_methods}"
 			)
 		return centroid_coors, instance_cluster_labels
 
-	@staticmethod
 	def _sort_kmeans_centroid(
-		pharmacophore_features_arr: np.ndarray, sort_by_features: str = "charge"
+		self, pharmacophore_features_arr: np.ndarray, sort_by_features: str = "charge"
 	) -> np.ndarray:
-		sort_index = Fepops.sort_by_features_col_index_dict[sort_by_features]
+		sort_index = self.sort_by_features_col_index_dict[sort_by_features]
 		return pharmacophore_features_arr[:, sort_index].argsort()
 
-	@staticmethod
-	def _get_centroid_dist(centroid_dist_arr: np.ndarray) -> list:
-		centroid_dist = []
-		arr_row, arr_col = centroid_dist_arr.shape[0], centroid_dist_arr.shape[1]
-		for row in range(arr_row):
-			i, j = row, 0
-			while i < arr_row and j < arr_col and centroid_dist_arr[i][j] != 0:
-				if i == arr_row - 1 and j == 0:
-					centroid_dist.insert(0, centroid_dist_arr[i][j])
-				else:
-					centroid_dist.append(centroid_dist_arr[i][j])
-				i += 1
-				j += 1
-		return centroid_dist
+	def _get_centroid_distances(self, centroid_coords_or_distmat: np.ndarray, is_distance_matrix:bool) -> np.ndarray:
+		"""Get centroid distances array
 
-	@staticmethod
-	def _mol_from_smiles(smiles_string: str) -> Chem.rdchem.Mol:
+		In the fepops paper using 4 centroids, there is a specific order in
+		which to return the 4 distances:
+		d1-4, d1-2, d2-3, d3-4, d1-3, d2-4.
+		This order is the same as the way matrix determinants are calculated,
+		and as such this function generalises to other cardinalities of points.
+
+
+		Parameters
+		----------
+		centroid_coords : np.ndarray
+			MxN array of centroid coords, where M is the number of centroids,
+			and N is the number of coordinates (should be 3).
+
+		Returns
+		-------
+		np.ndarray
+			Ordered centroid distances
+		"""
+
+		if is_distance_matrix:
+			distance_matrix=centroid_coords_or_distmat
+		else:
+			distance_matrix=squareform(pdist(centroid_coords_or_distmat))
+		distances = np.array([distance_matrix[0,distance_matrix.shape[0]-1]]+[ele for arr in [distance_matrix.diagonal(i) for i in range(1,distance_matrix.shape[0]-1)] for ele in arr])
+		return distances
+
+	def _mol_from_smiles(self, smiles_string: str) -> Chem.rdchem.Mol:
 		"""Parse smiles to mol, catching errors
 
 		Parameters
 		----------
 		smiles_string : str
 			Smiles string
 
@@ -299,25 +312,24 @@
 			Unable to parse smiles into a molecule
 		"""
 		try:
 			mol = Chem.MolFromSmiles(smiles_string)
 		except:
 			try:
 				mol = Chem.MolFromSmiles(smiles_string, sanitize=False)
-			finally:
-				mol = None
+			except:
+				pass
 		if mol is None:
 			raise ValueError(
 				f"Could not parse smiles to a valid molecule, smiles was:{smiles_string}"
 			)
 		return mol
 
-	@staticmethod
 	def _get_flanking_atoms(
-		bonds: Chem.rdchem._ROBondSeq, atom_1_idx: int, atom_2_idx: int
+		self, bonds: Chem.rdchem._ROBondSeq, atom_1_idx: int, atom_2_idx: int
 	) -> tuple:
 		"""Search for two atoms connecting to either atom in a rotatable bond
 
 		A private method to identify two atoms flanking atoms in a rotatable bond
 
 		Parameters
 		----------
@@ -358,16 +370,15 @@
 					bound_to_atom_2 = bond_indexes[0]
 					continue
 
 				if bound_to_atom_1 is not None and bound_to_atom_2 is not None:
 					return bound_to_atom_1, bound_to_atom_2
 		return bound_to_atom_1, bound_to_atom_2
 
-	@staticmethod
-	def _sample_bond_states(n_rot: int, seed:int) -> list:
+	def _sample_bond_states(self, n_rot: int, seed: int) -> list:
 		"""Sample a set of conformers with different rotation angles
 
 		A private method used to generate a set of bond angle multipliers (0 to 3) using
 		all rotatable bonds within a molecule. Up to 1024 conformers are sampled for a molecule if
 		n_rot is greater than five, otherwise all n_rot^4 are returned.
 
 		Parameters
@@ -380,66 +391,68 @@
 		-------
 		List
 			A list containing the sampled bond states (rotation angles) for all of the rotatable bonds of a molecule.
 		"""
 		if n_rot <= 5:
 			return list(itertools.product(range(4), repeat=n_rot))
 
-		np_rng=np.random.default_rng(seed=seed)
+		np_rng = np.random.default_rng(seed=seed)
 
 		rotation_list = set(
-			tuple(np_rng.choice(range(4), size=n_rot))
-			for counter in range(1024)
+			tuple(np_rng.choice(range(4), size=n_rot)) for counter in range(1024)
 		)
 
 		while len(rotation_list) < 1024:
-			rotation_list.add(tuple(np_rng.choice(range(4),n_rot)))
+			rotation_list.add(tuple(np_rng.choice(range(4), n_rot)))
 		return list(rotation_list)
 
-	@staticmethod
-	def generate_conformers(mol: Chem.rdchem.Mol, random_seed: int = 42) -> list:
+	def generate_conformers(self, mol: Chem.rdchem.Mol, random_seed: int = 42) -> list:
 		"""Generate conformers with rotatable bonds
 
 		Generate conformers for a molecule, enumerating rotatable bonds over 90 degree angles.
 
 		Parameters
 		----------
 		mol : Chem.rdchem.Mol
 			The Rdkit mol object of the input molecule.
 		random_seed : reproducibility
 
 		Returns
 		-------
 		List
-				A list containing mol objects of different conformers with different angles of rotetable bonds.
+			A list containing mol objects of different conformers with different angles of rotetable bonds.
 		"""
 		try:
 			mol = Chem.AddHs(mol)
-			original_conformer = mol.GetConformer(AllChem.EmbedMolecule(mol, randomSeed=random_seed))
+			original_conformer = mol.GetConformer(
+				AllChem.EmbedMolecule(mol, randomSeed=random_seed)
+			)
 		except ValueError:
-			print ("Conformer embedding failed")
+			print("Conformer embedding failed")
 			return []
-		dihedrals = Fepops._get_dihedrals(mol)
+		dihedrals = self._get_dihedrals(mol)
 		starting_angles = [
 			rdMolTransforms.GetDihedralDeg(original_conformer, *dihedral_atoms)
 			for dihedral_atoms in dihedrals
 		]
-		bond_states = Fepops._sample_bond_states(len(dihedrals),abs(hash(str(mol.GetConformer(0).GetPositions()))))
+		bond_states = self._sample_bond_states(
+			len(dihedrals), abs(hash(str(mol.GetConformer(0).GetPositions())))
+		)
 
 		new_conf_mol_list = []
 		for bond_state in bond_states:
-			Fepops._generate_conf(
+			self._generate_conf(
 				original_conformer, dihedrals, starting_angles, bond_state
 			)
 			new_conf_mol_list.append(Chem.Mol(mol))
 
 		return new_conf_mol_list
 
-	@staticmethod
 	def _generate_conf(
+		self,
 		conformer: Chem.rdchem.Conformer,
 		dihedrals: tuple,
 		starting_angles: tuple,
 		bond_state: tuple,
 	) -> None:
 		"""Rotate the assigned rotatable bonds
 
@@ -462,86 +475,85 @@
 			dihedrals, bond_state, starting_angles
 		):
 			rdMolTransforms.SetDihedralDeg(
 				conformer,
 				*dihedral_atoms,
 				orig_torsion_angle + torsion_angle_multiplier * 90.0,
 			)
-	@staticmethod
+
 	def get_centroid_pharmacophoric_features(
+		self,
 		mol: Chem.rdchem.Mol,
-		kmeans_method_str:str,
-		num_centroids: int = 4,
-
+		kmeans_method_str: str,
 	) -> np.ndarray:
 		"""Obtain the four centroids and their corresponding pharmacophoric features
 
 		Obtain the four centroids and then calucate and assign their corresponding pharmacophoric
 		features (logP, charges, HBA, HBD, six distances between four centroids).
 
 		Parameters
 		----------
 		mol : Chem.rdchem.Mol
 			The Rdkit mol object of the input molecule.
 		num_centroids : int
-			The number of centoids used for clustering. By default 4.
+			sThe number of centoids used for clustering. By default 4.
 
 		Returns
 		-------
 		np.ndarray
 			A Numpy array containing 22 pharmacophoric features for all conformers.
 		"""
-		centroid_coors, instance_cluster_labels = Fepops._perform_kmeans(
-			mol.GetConformer(0).GetPositions(), num_centroids, kmeans_method=kmeans_method_str
-		)
-		centroid_dist_arr = cdist(centroid_coors, centroid_coors)
-		centroid_dist = list(
-			centroid_dist_arr[np.triu_indices_from(centroid_dist_arr, k=1)]
+		centroid_coords, instance_cluster_labels = self._perform_kmeans(
+			mol.GetConformer(0).GetPositions(),
+			num_centroids=self.num_centroids_per_fepop,
+			kmeans_method=kmeans_method_str,
 		)
 
-		atomic_logP_dict = Fepops._calculate_atomic_logPs(mol)
-		atomic_charge_dict = Fepops._calculate_partial_charges(mol)
+		atomic_logP_dict = self._calculate_atomic_logPs(mol)
+		atomic_charge_dict = self._calculate_partial_charges(mol)
 		hb_acceptors = set(
-			i[0] for i in mol.GetSubstructMatches(Fepops.acceptor_mol_from_smarts)
+			i[0] for i in mol.GetSubstructMatches(self.acceptor_mol_from_smarts)
 		)
 		hb_donors = set(
-			i[0] for i in mol.GetSubstructMatches(Fepops.donor_mol_from_smarts)
+			i[0] for i in mol.GetSubstructMatches(self.donor_mol_from_smarts)
 		)
-
-		pharmacophore_features_arr = np.empty(shape=[0, 4])
-		for centroid in range(num_centroids):
-			hba, hbd = 0.0, 0.0
+		pharmacophore_features_arr = np.empty(shape=[self.num_centroids_per_fepop, 4])
+		for centroid in range(self.num_centroids_per_fepop):
 			centroid_atomic_id = np.where(instance_cluster_labels == centroid)[0]
-			sum_of_logP = Fepops._sum_of_atomic_features_by_centroids(
+
+			sum_of_logP = self._sum_of_atomic_features_by_centroids(
 				atomic_logP_dict, centroid_atomic_id
 			)
-			sum_of_charge = Fepops._sum_of_atomic_features_by_centroids(
+			sum_of_charge = self._sum_of_atomic_features_by_centroids(
 				atomic_charge_dict, centroid_atomic_id
 			)
-			if len(hb_acceptors.intersection(set(centroid_atomic_id))) > 0:
-				hba = 1
-			if len(hb_donors.intersection(set(centroid_atomic_id))) > 0:
-				hbd = 1
-			pharmacophore_features_arr = np.vstack(
-				(pharmacophore_features_arr, [sum_of_charge, sum_of_logP, hbd, hba])
-			)
-		sorted_index_rank_arr = Fepops._sort_kmeans_centroid(
+
+			if any(atom_id in hb_acceptors for atom_id in centroid_atomic_id ):
+				hba=1
+			else:
+				hba=0
+			if any(atom_id in hb_donors for atom_id in centroid_atomic_id ):
+				hbd=1
+			else:
+				hbd=0
+
+			pharmacophore_features_arr[centroid,:] = sum_of_charge, sum_of_logP, hbd, hba
+
+		sorted_index_rank_arr = self._sort_kmeans_centroid(
 			pharmacophore_features_arr, "charge"
 		)
-		centroid_coors = centroid_coors[sorted_index_rank_arr]
+		centroid_coords = centroid_coords[sorted_index_rank_arr]
 		pharmacophore_features_arr = pharmacophore_features_arr[sorted_index_rank_arr]
-		centroid_dist_arr = cdist(centroid_coors, centroid_coors)
-		centroid_dist = Fepops._get_centroid_dist(centroid_dist_arr)
+		centroid_dist = self._get_centroid_distances(centroid_coords, is_distance_matrix=False)
 		pharmacophore_features_arr = np.append(
 			pharmacophore_features_arr, centroid_dist
 		)
-		# print (pharmacophore_features_arr, pharmacophore_features_arr.shape)
 		return pharmacophore_features_arr
 
-	def get_fepops(self, mol: Union[str,Chem.rdchem.Mol]) -> Union[np.ndarray, None]:
+	def get_fepops(self, mol: Union[str, Chem.rdchem.Mol]) -> Union[np.ndarray, None]:
 		"""Get Fepops descriptors
 
 		This method returns Fepops descriptors from a smiles string.
 
 
 		Parameters
 		----------
@@ -550,86 +562,132 @@
 
 		Returns
 		-------
 		np.ndarray
 			A Numpy array containing the calculated Fepops descriptors of an input molecule.
 		"""
 		if isinstance(mol, str):
-			mol = Fepops._mol_from_smiles(mol)
-		mol = Chem.AddHs(mol)
+			mol = self._mol_from_smiles(mol)
+		if mol is None:
+			return None
 
-		tautomers_list = self._get_tautomers(mol)
+		mol = Chem.AddHs(mol)
+		if Lipinski.HeavyAtomCount(mol) < self.num_centroids_per_fepop:
+			print (ValueError(f"Number of heavy atoms (:{Lipinski.HeavyAtomCount(mol)}) below requested feature points (:{self.num_centroids_per_fepop})"))
+			return None
+		
+		tautomers_list = self.tautomer_enumerator.enumerate(mol)
 		each_mol_with_all_confs_list = []
 		for index, t_mol in enumerate(tautomers_list):
-			conf_list = Fepops.generate_conformers(t_mol)
+			conf_list = self.generate_conformers(t_mol)
 			each_mol_with_all_confs_list.extend(conf_list)
 
-		if not len(each_mol_with_all_confs_list): return None
+		if each_mol_with_all_confs_list==[]:
+			return None
 
-		for index, each_mol in enumerate(each_mol_with_all_confs_list):
-			pharmacophore_feature = self.get_centroid_pharmacophoric_features(each_mol, kmeans_method_str=self.kmeans_method_str, num_centroids=4)
-			if index == 0:
-				pharmacophore_feature_all_confs = pharmacophore_feature
-				continue
-			pharmacophore_feature_all_confs = np.vstack(
-				(pharmacophore_feature_all_confs, pharmacophore_feature)
+		pharmacophore_feature_all_confs=np.array(
+			[self.get_centroid_pharmacophoric_features(each_mol,
+					      kmeans_method_str=self.kmeans_method_str,
 			)
-		return self._get_k_medoids(pharmacophore_feature_all_confs, 7)
+			for each_mol in each_mol_with_all_confs_list]
+		)
 
-	def _score(self, x1: np.ndarray, x2: np.ndarray) -> float:
-		"""Score function for the similarity calculation
+		return self._get_k_medoids(pharmacophore_feature_all_confs, self.num_fepops_per_mol)
 
-		The score function for the similarity calculation on the FEPOPS descriptors.
+
+	def _score_combialign(self, x1:np.ndarray, x2:np.ndarray):
+		"""Score fepops using CombiAlign
+
+		Instead of sorting feature points by charge, this algorithm matches 2
+		sets of medoids by holding one set constant and enumerating all
+		permutations of the other, and performing pearson correlation calculations
+		in a row-pairwise manner.  The highest summed correlation score permutation
+		is then used for the second set, and scoring proceeds using softmax of the
+		full fepops descriptors and the pearson correlation coefficient between
+		them.
+
+		The CombiAlign algorithm as defined in Nettles, James H., et al. "Flexible
+		3D pharmacophores as descriptors of dynamic biological space." Journal of
+		Molecular Graphics and Modelling 26.3 (2007): 622-633.
 
 		Parameters
 		----------
 		x1 : np.ndarray
-			A Numpy array containing the FEPOPS descriptors 1.
+			Query fepop
 		x2 : np.ndarray
-			A Numpy array containing the FEPOPS descriptors 2.
+			Candidate fepop
 
 		Returns
 		-------
 		float
-			The FEPOPS similarity score (Pearson correlation).
-		"""
-		x1 = self.scaler.fit_transform(x1.reshape(-1, 1))
-		x2 = self.scaler.fit_transform(x2.reshape(-1, 1))
-		return np.corrcoef(x1.flatten(), x2.flatten())[0, 1]
+			Fepops score, higher is better. 1 is the maximum.
+		"""		
+		n_distances=((self.num_centroids_per_fepop**2)-self.num_centroids_per_fepop)//2
+		x1_desc = x1[:-n_distances].reshape(self.num_centroids_per_fepop,-1)
+		x2_desc, x2_dists = x2[:-n_distances].reshape(self.num_centroids_per_fepop,-1), x2[-n_distances:]
+
+
+		permutation_tuples=list(itertools.permutations(range(self.num_centroids_per_fepop)))
+		# Find permutation which gives highest sum of correlations to x1 descriptor
+		best_permutaion=permutation_tuples[np.argmax([cdist(x1_desc, x2_desc[perm_tuple, :], metric=lambda x,y: np.corrcoef(x,y)[0,1]).diagonal().sum() for perm_tuple in permutation_tuples])]
+
+		# Rebuild x2 distances to squareform matrix, then reorder as per the best permutation and extract in required FEPOPS order.
+		dmat=np.zeros((self.num_centroids_per_fepop, self.num_centroids_per_fepop))
+		dmat[0,-1]=x2_dists[0]
+		dmat[-1,0]=x2_dists[0]
+		rows, cols = np.diag_indices_from(dmat)
+		for (r, c), v in zip([(x,y) for d in [np.stack((rows[:-i], cols[i:]), axis=1) for i in range(1, dmat.shape[0]-1)] for x,y in d], x2_dists):
+			dmat[r,c]=v
+			dmat[c,r]=v
+
+		# Reorder the distance matrix using best permutation
+		new_dmat=np.zeros_like(dmat)
+		for i, p in enumerate(best_permutaion):
+			for j in range(dmat.shape[0]):
+				if i==j:continue
+				new_dmat[i,j]=dmat[p,best_permutaion[j]]
+		
+		distances=self._get_centroid_distances(new_dmat, is_distance_matrix=True)
+		
+		# Reform x2 with reordered medoids and medoid distances
+		x2=np.hstack([x2_desc[[best_permutaion]].flatten(),distances])
+		
+		# Apply softmax and return pearson correlation between the two
+		return np.corrcoef(softmax(x1), softmax(x2))[0,1]
 
 	def calc_similarity(
 		self,
 		query: Union[np.ndarray, str],
 		candidate: Union[np.ndarray, str],
 	) -> float:
 		"""Calculate FEPOPS similarity
 
-		A static method for calculating molecular similarity based on their FEPOPS descriptors.
+		Method for calculating molecular similarity based on their FEPOPS descriptors.
 
 		Parameters
 		----------
-		fepops_features_1 : Union[np.ndarray, str]
+		query : Union[np.ndarray, str]
 			A Numpy array containing the FEPOPS descriptors of the query molecule
 			or a smiles string from which to generate FEPOPS descriptors for the
 			query molecule.
-		fepops_features_2 : Union[np.ndarray, str]
+		candidate : Union[np.ndarray, str]
 			A Numpy array containing the FEPOPS descriptors of the candidate
 			molecule or a smiles string from which to generate FEPOPS descriptors
 			for the query molecule.
 
 		Returns
 		-------
 		float
 			Fepops similarity between two molecules
 		"""
 		if isinstance(query, str):
 			query = self.get_fepops(query)
 		if isinstance(candidate, str):
 			candidate = self.get_fepops(candidate)
-		return np.max(cdist(query, candidate, metric=self._score))
+		return np.max(cdist(query, candidate, metric=self._score_combialign))
 
 	def __call__(
 		self,
 		query: Union[np.ndarray, str],
 		candidate: Union[np.ndarray, str],
 	) -> float:
 		return self.calc_similarity(query, candidate)
```

### Comparing `fepops-1.2.0/fepops.egg-info/PKG-INFO` & `fepops-1.3.0/fepops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fepops
-Version: 1.2.0
+Version: 1.3.0
 Summary: Python implementation of the FEPOPS molecular descriptors
 Home-page: https://github.com/JustinYKC/FEPOPS
 Author: Yan-Kai Chen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
@@ -38,15 +38,15 @@
 A quickstart example to generate the FEPOPS descriptors for a molecule directly from its SMILES as follows: In terminal:
 ```
 python fepops.py get_fepops -ismi "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" 
 ```
 
 A quickstart example to calculate the FEPOPS similarity between two molecules using their SMILES as follows: In terminal:
 ```
-python fepops.py cal_sim -ismi1 "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" -ismi2 "OC=1C=C(O)C=C(C1)C=2OC=3C=CC=CC3C2"
+python fepops.py calc_sim -ismi1 "O=C1OC2=CC3(C)C(CC4OC(=O)C(OC(=O)C)C5C6(OCC45C3C(O)C6O)C(=O)OC)C(C2=C1)C" -ismi2 "OC=1C=C(O)C=C(C1)C=2OC=3C=CC=CC3C2"
 ```
 
 An example of filtering molecules in the dataset of natural products: `COCONUT.DB.smi` [COCONUT.DB.smi](https://coconut.naturalproducts.net/download), for further use of the FEPOPS generation:
 ```
 python mol_filter.py
 ```
```

### Comparing `fepops-1.2.0/setup.cfg` & `fepops-1.3.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = fepops
-version = 1.2.0
+version = 1.3.0
 author = Yan-Kai Chen
 description = Python implementation of the FEPOPS molecular descriptors
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JustinYKC/FEPOPS
 classifiers = 
 	Programming Language :: Python :: 3
@@ -19,17 +19,17 @@
 python_requires = >=3.9
 install_requires = 
 	numpy>=1.19.0
 	pandas>=1.5.0
 	rdkit>=2019.09.0.0
 	scikit-learn>=0.20.4
 	scipy>=1.7.0
-	torch>= 1.0.0
-	fast_pytorch_kmeans
-	tqdm
+	Pytorch>=1.0.0
+	fast_pytorch_kmeans>=0.1.9
+	tqdm>=4.48.0
 
 [tool:pytest]
 testpaths = test
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `fepops-1.2.0/test/tests.py` & `fepops-1.3.0/test/tests.py`

 * *Files identical despite different names*

