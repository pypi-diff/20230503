# Comparing `tmp/airrship-0.1.3.tar.gz` & `tmp/airrship-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/s1404341/Documents/PhD/Simulations/airrship_cowan/dist/.tmp-mhxv07uo/airrship-0.1.3.tar", last modified: Fri Mar 31 15:37:08 2023, max compression
+gzip compressed data, was "/Users/s1404341/Documents/PhD/Simulations/airrship_cowan/dist/.tmp-qxjixoht/airrship-0.1.4.tar", last modified: Wed May  3 09:46:22 2023, max compression
```

## Comparing `airrship-0.1.3.tar` & `airrship-0.1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-03-31 15:37:08.000000 airrship-0.1.3/
--rw-r--r--   0 s1404341   (501) staff       (20)    34523 2022-12-16 13:44:11.000000 airrship-0.1.3/LICENSE
--rw-r--r--   0 s1404341   (501) staff       (20)    41786 2023-03-31 15:37:08.000000 airrship-0.1.3/PKG-INFO
--rw-r--r--   0 s1404341   (501) staff       (20)     1231 2023-03-31 09:31:55.000000 airrship-0.1.3/README.md
-drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-03-31 15:37:08.000000 airrship-0.1.3/airrship/
--rw-r--r--   0 s1404341   (501) staff       (20)       22 2023-03-30 18:41:35.000000 airrship-0.1.3/airrship/__init__.py
--rwx------   0 s1404341   (501) staff       (20)   109175 2023-03-31 10:55:59.000000 airrship-0.1.3/airrship/create_repertoire.py
-drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-03-31 15:37:08.000000 airrship-0.1.3/airrship/data/
--rw-r--r--   0 s1404341   (501) staff       (20)     3866 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/D_3_family_trimming_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     3481 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/D_5_family_trimming_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      356 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/IGHD_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      909 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/IGHD_usage_gene.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      168 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/IGHJ_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      167 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/IGHJ_usage_gene.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      421 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/IGHV_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     3239 2023-01-20 17:37:33.000000 airrship-0.1.3/airrship/data/IGHV_usage_gene.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     3473 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/J_family_trimming_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    10675 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/V_family_trimming_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)        0 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/__init__.py
--rw-r--r--   0 s1404341   (501) staff       (20)    31632 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/cdr1_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    39947 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/cdr2_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    46095 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/cdr3_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    69757 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/cdr_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    38976 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/fwr1_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    43833 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/fwr2_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    73585 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/fwr3_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     7942 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/fwr4_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    82819 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/fwr_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     4839 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/imgt_human_IGHD.fasta
--rw-r--r--   0 s1404341   (501) staff       (20)     1790 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/imgt_human_IGHJ.fasta
--rw-r--r--   0 s1404341   (501) staff       (20)   175791 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/imgt_human_IGHV.fasta
--rw-r--r--   0 s1404341   (501) staff       (20)  2240771 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/mut_freq_per_seq_per_family.csv
--rw-r--r--   0 s1404341   (501) staff       (20)       99 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/np1_first_base_probs.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      988 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/np1_lengths_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    12922 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/np1_transition_probs_per_position_igag.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    12933 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/np1_transition_probs_per_position_igdm.csv
--rw-r--r--   0 s1404341   (501) staff       (20)       99 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/np2_first_base_probs.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     1073 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/np2_lengths_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    12883 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/np2_transition_probs_per_position_igag.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    12925 2022-12-16 13:44:11.000000 airrship-0.1.3/airrship/data/np2_transition_probs_per_position_igdm.csv
-drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-03-31 15:37:08.000000 airrship-0.1.3/airrship.egg-info/
--rw-r--r--   0 s1404341   (501) staff       (20)    41786 2023-03-31 15:37:08.000000 airrship-0.1.3/airrship.egg-info/PKG-INFO
--rw-r--r--   0 s1404341   (501) staff       (20)     1569 2023-03-31 15:37:08.000000 airrship-0.1.3/airrship.egg-info/SOURCES.txt
--rw-r--r--   0 s1404341   (501) staff       (20)        1 2023-03-31 15:37:08.000000 airrship-0.1.3/airrship.egg-info/dependency_links.txt
--rw-r--r--   0 s1404341   (501) staff       (20)       61 2023-03-31 15:37:08.000000 airrship-0.1.3/airrship.egg-info/entry_points.txt
--rw-r--r--   0 s1404341   (501) staff       (20)        9 2023-03-31 15:37:08.000000 airrship-0.1.3/airrship.egg-info/top_level.txt
--rw-r--r--   0 s1404341   (501) staff       (20)      957 2023-01-25 11:07:34.000000 airrship-0.1.3/pyproject.toml
--rw-r--r--   0 s1404341   (501) staff       (20)      213 2023-03-31 15:37:08.000000 airrship-0.1.3/setup.cfg
--rw-r--r--   0 s1404341   (501) staff       (20)       37 2022-12-19 16:04:00.000000 airrship-0.1.3/setup.py
+drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 09:46:22.000000 airrship-0.1.4/
+-rw-r--r--   0 s1404341   (501) staff       (20)    34523 2022-12-16 13:44:11.000000 airrship-0.1.4/LICENSE
+-rw-r--r--   0 s1404341   (501) staff       (20)    41786 2023-05-03 09:46:22.000000 airrship-0.1.4/PKG-INFO
+-rw-r--r--   0 s1404341   (501) staff       (20)     1231 2023-03-31 09:31:55.000000 airrship-0.1.4/README.md
+drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship/
+-rw-r--r--   0 s1404341   (501) staff       (20)       22 2023-04-25 16:21:26.000000 airrship-0.1.4/airrship/__init__.py
+-rwx------   0 s1404341   (501) staff       (20)   109925 2023-04-28 13:58:47.000000 airrship-0.1.4/airrship/create_repertoire.py
+drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship/data/
+-rw-r--r--   0 s1404341   (501) staff       (20)     3866 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/D_3_family_trimming_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     3481 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/D_5_family_trimming_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      356 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHD_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      909 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHD_usage_gene.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      168 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHJ_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      167 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHJ_usage_gene.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      421 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHV_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     3239 2023-01-20 17:37:33.000000 airrship-0.1.4/airrship/data/IGHV_usage_gene.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     3473 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/J_family_trimming_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    10675 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/V_family_trimming_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)        0 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/__init__.py
+-rw-r--r--   0 s1404341   (501) staff       (20)    31632 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/cdr1_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    39947 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/cdr2_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    46095 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/cdr3_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    69757 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/cdr_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    38976 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr1_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    43833 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr2_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    73585 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr3_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     7942 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr4_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    82819 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     4839 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/imgt_human_IGHD.fasta
+-rw-r--r--   0 s1404341   (501) staff       (20)     1790 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/imgt_human_IGHJ.fasta
+-rw-r--r--   0 s1404341   (501) staff       (20)   175791 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/imgt_human_IGHV.fasta
+-rw-r--r--   0 s1404341   (501) staff       (20)  2240771 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/mut_freq_per_seq_per_family.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)       99 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np1_first_base_probs.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      988 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np1_lengths_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    12922 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np1_transition_probs_per_position_igag.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    12933 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np1_transition_probs_per_position_igdm.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)       99 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np2_first_base_probs.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     1073 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np2_lengths_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    12883 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np2_transition_probs_per_position_igag.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    12925 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np2_transition_probs_per_position_igdm.csv
+drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/
+-rw-r--r--   0 s1404341   (501) staff       (20)    41786 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/PKG-INFO
+-rw-r--r--   0 s1404341   (501) staff       (20)     1569 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/SOURCES.txt
+-rw-r--r--   0 s1404341   (501) staff       (20)        1 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/dependency_links.txt
+-rw-r--r--   0 s1404341   (501) staff       (20)       61 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/entry_points.txt
+-rw-r--r--   0 s1404341   (501) staff       (20)        9 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/top_level.txt
+-rw-r--r--   0 s1404341   (501) staff       (20)      957 2023-01-25 11:07:34.000000 airrship-0.1.4/pyproject.toml
+-rw-r--r--   0 s1404341   (501) staff       (20)      213 2023-05-03 09:46:22.000000 airrship-0.1.4/setup.cfg
+-rw-r--r--   0 s1404341   (501) staff       (20)       37 2022-12-19 16:04:00.000000 airrship-0.1.4/setup.py
```

### Comparing `airrship-0.1.3/LICENSE` & `airrship-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/PKG-INFO` & `airrship-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airrship
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simulation of B cell receptor repertoires
 Author-email: Catherine Sutherland <catherine.sutherland@ed.ac.uk>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `airrship-0.1.3/README.md` & `airrship-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/create_repertoire.py` & `airrship-0.1.4/airrship/create_repertoire.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 import re
 import argparse
 import sys
 import importlib.resources
 from importlib.metadata import version
 
 
+
 # Classes
 
 
 class Allele:
     """Class that represents a V, D or J allele.
 
     Attributes:
@@ -337,17 +338,25 @@
             current_base (str): Current base in NP region sequence.
             position (int): Current position in NP region sequence.
 
         Returns:
             base (str): Next base in the NP region sequence.
         """
 
-        base = weighted_choice(
-            list(zip(self.bases, [self.transition_probs[position][current_base][next_base]
-                                  for next_base in self.bases])))
+        if position in self.transition_probs:
+
+            if current_base in self.transition_probs[position]:
+                base = weighted_choice(
+                    list(zip(self.bases, [self.transition_probs[position][current_base][next_base]
+                                        for next_base in self.bases])))
+            else:
+                base = random.choice(["A","C","G","T"])
+        else:
+            base = random.choice(["A","C","G","T"])
+
         return base
 
     def generate_np_seq(self):
         """Creates an NP region sequence using a first order Markov chain.
 
         Returns:
             sequence (str): Final NP region sequence.
@@ -1214,15 +1223,15 @@
     """
     with open(out_name, 'w') as f:
         f.write("AIRRSHIP was run with the following arguments: \n")
         output = str(args).rstrip(")").lstrip("Namespace(")
         f.write(str(output))
 
 
-def get_genotype(data_folder=None, het_list=[1, 1, 1], haplotype=True, locus=None):
+def get_genotype(data_folder=None, het_list=[1, 1, 1], haplotype=True, locus=None,species="human"):
     """Wrapper that generates a locus for use in sequence generations
 
     Args:
         data_folder (path, optional): Path to data folder with required data. 
             When not specified will use package data. Defaults to None.
         het_list (list, optional): Proportion of genes [V, D, J] to be heterozygous.
             Defaults to [1, 1, 1].
@@ -1234,18 +1243,17 @@
     Returns:
         locus (list): List of two dictionaries. Each is a dictionary containing 
             the gene segment as keys and the chosen alleles as values. Format is
             {Segment : [Allele, Allele ...], ...}
     """
     if data_folder != None:
         path_to_data = data_folder
-
-        v_alleles = create_allele_dict(f"{path_to_data}/imgt_human_IGHV.fasta")
-        d_alleles = create_allele_dict(f"{path_to_data}/imgt_human_IGHD.fasta")
-        j_alleles = create_allele_dict(f"{path_to_data}/imgt_human_IGHJ.fasta")
+        v_alleles = create_allele_dict(f"{path_to_data}/imgt_{species}_IGHV.fasta")
+        d_alleles = create_allele_dict(f"{path_to_data}/imgt_{species}_IGHD.fasta")
+        j_alleles = create_allele_dict(f"{path_to_data}/imgt_{species}_IGHJ.fasta")
 
     else:
         try:
             path_to_data = importlib.resources.files(
                 'airrship').joinpath("data")
         except AttributeError:
             with importlib.resources.path('airrship', 'data') as p:
@@ -1479,15 +1487,18 @@
     sequence = sequence
     mut_seq = sequence[:2]
     ungapped_seq = sequence.replace(".", "")
     mutations = {}
     v_family = v_family
 
     if mut_rate == None and number_muts == None:
-        mut_dict = mut_per_seq[v_family]
+        if v_family in mut_per_seq:
+            mut_dict = mut_per_seq[v_family]
+        else:
+            mut_dict = random.choice(list(mut_per_seq.values()))
         mut_rate = weighted_choice(mut_dict.items())
         if mut_rate != 0:
             mut_rate = mut_rate * mut_multiplier
         number_muts = int(round(len(sequence) * mut_rate))
     elif number_muts == None:
         number_muts = int(round(len(sequence) * mut_rate))
     else:
@@ -2113,15 +2124,15 @@
     parser.add_argument("--het",
                         # if using haplotype, decide how many of the genes should have two differing alleles
                         action="store",
                         metavar="PROP",
                         help="Proportion of genes to be heterozygous, specify as  V D J, values must be between 0 and 1. Not compatible with --all_alleles.",
                         nargs=3,
                         type=float,
-                        default=[0.74, 0.16, 0.67])
+                        default=[0, 0, 0])
     parser.add_argument("--shm",
                         action="store_true",  # SHM is false unless "-shm" is specified
                         help="Apply somatic hypermutation.")
     parser.add_argument("--shm_multiplier",
                         action="store",
                         type=float_range(0,5.0),
                         help="Apply a multiplication factor to mutation rate distribution. Value between 0 and 5. Use with --shm or --shm_random, not compatible with --shm_flat.")
@@ -2184,29 +2195,34 @@
                         action = "store",
                         metavar="PROP",
                         type=float_range(0,1.0),
                         help="Specify a proportion of sequences to be non_productive. Used with --non_productive.")
     parser.add_argument("--seed",
                         type=int,
                         help="Set random seed.")
+    parser.add_argument("--species",
+                        type=str,
+                        action = "store",
+                        default = "human",
+                        help="Specify if simulating non-human sequences. Will be used to find the imgt_{species}_IGH[V|D|J].fasta files in the specified --datadir.")
 
 
     args = parser.parse_args(args)
 
     if args.shm_flat == False and (args.mut_num is not None or args.mut_rate is not None):
         parser.error("--mut_num and --mut_rate only apply when --shm_flat is used.")
 
     if args.shm_multiplier is not None and (args.shm_random == False and args.shm == False):
         parser.error("--shm_multiplier can only be specified with --shm or --shm_random.")
 
     if args.shm_multiplier is not None and args.shm_flat == True:
         parser.error("--shm_multiplier cannot be used with --shm_flat.")
     
     if args.prop_non_productive is not None and (args.non_productive == False):
-        parser.error("Can only specificy --prop_non_productive when --non_productive is used.")
+        parser.error("Can only specify --prop_non_productive when --non_productive is used.")
 
 
 
 
     # Print copyright notice
 
     print("AIRRSHIP Copyright (C) 2022  Catherine Sutherland \nThis program comes with ABSOLUTELY NO WARRANTY. \nThis is free software, and you are welcome to redistribute \nit under certain conditions. Refer to the GNU Affero General \nPublic License for further details.")
@@ -2237,14 +2253,15 @@
     out_locus = args.outdir + "/" + args.out_name + "_locus.csv"
     out_summary = args.outdir + "/" + args.out_name + "_summary.txt"
 
     if args.seed:
         random.seed(args.seed)
     else:
         random.seed(random.random())
+    
 
     # Set up mutation rates
 
     mutation_number = None
     mutation_rate = None
     if args.shm_flat == True:
         if args.mut_num != None:
@@ -2273,15 +2290,15 @@
 
     # Read in all the reference data
 
     data_dict = load_data(path_to_data, mutate)
 
     # Set up the genotype to be used
 
-    locus = get_genotype(path_to_data, args.het, haplotype, args.locus)
+    locus = get_genotype(path_to_data, args.het, haplotype, args.locus,args.species)
 
     # Write out locus file
 
     write_locus_file(out_locus, locus)
 
     # Write out summary file
```

### Comparing `airrship-0.1.3/airrship/data/D_3_family_trimming_proportions.csv` & `airrship-0.1.4/airrship/data/D_3_family_trimming_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/D_5_family_trimming_proportions.csv` & `airrship-0.1.4/airrship/data/D_5_family_trimming_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/IGHD_usage_gene.csv` & `airrship-0.1.4/airrship/data/IGHD_usage_gene.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/IGHV_usage_gene.csv` & `airrship-0.1.4/airrship/data/IGHV_usage_gene.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/J_family_trimming_proportions.csv` & `airrship-0.1.4/airrship/data/J_family_trimming_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/V_family_trimming_proportions.csv` & `airrship-0.1.4/airrship/data/V_family_trimming_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/cdr1_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/cdr1_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/cdr2_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/cdr2_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/cdr3_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/cdr3_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/cdr_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/cdr_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/fwr1_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/fwr1_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/fwr2_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/fwr2_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/fwr3_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/fwr3_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/fwr4_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/fwr4_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/fwr_kmer_base_usage.csv` & `airrship-0.1.4/airrship/data/fwr_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/imgt_human_IGHD.fasta` & `airrship-0.1.4/airrship/data/imgt_human_IGHD.fasta`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/imgt_human_IGHJ.fasta` & `airrship-0.1.4/airrship/data/imgt_human_IGHJ.fasta`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/imgt_human_IGHV.fasta` & `airrship-0.1.4/airrship/data/imgt_human_IGHV.fasta`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/mut_freq_per_seq_per_family.csv` & `airrship-0.1.4/airrship/data/mut_freq_per_seq_per_family.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/np1_lengths_proportions.csv` & `airrship-0.1.4/airrship/data/np1_lengths_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/np1_transition_probs_per_position_igag.csv` & `airrship-0.1.4/airrship/data/np1_transition_probs_per_position_igag.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/np1_transition_probs_per_position_igdm.csv` & `airrship-0.1.4/airrship/data/np1_transition_probs_per_position_igdm.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/np2_lengths_proportions.csv` & `airrship-0.1.4/airrship/data/np2_lengths_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/np2_transition_probs_per_position_igag.csv` & `airrship-0.1.4/airrship/data/np2_transition_probs_per_position_igag.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship/data/np2_transition_probs_per_position_igdm.csv` & `airrship-0.1.4/airrship/data/np2_transition_probs_per_position_igdm.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/airrship.egg-info/PKG-INFO` & `airrship-0.1.4/airrship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airrship
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simulation of B cell receptor repertoires
 Author-email: Catherine Sutherland <catherine.sutherland@ed.ac.uk>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `airrship-0.1.3/airrship.egg-info/SOURCES.txt` & `airrship-0.1.4/airrship.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airrship-0.1.3/pyproject.toml` & `airrship-0.1.4/pyproject.toml`

 * *Files identical despite different names*

