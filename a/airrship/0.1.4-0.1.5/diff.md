# Comparing `tmp/airrship-0.1.4.tar.gz` & `tmp/airrship-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/s1404341/Documents/PhD/Simulations/airrship_cowan/dist/.tmp-qxjixoht/airrship-0.1.4.tar", last modified: Wed May  3 09:46:22 2023, max compression
+gzip compressed data, was "/Users/s1404341/Documents/PhD/Simulations/airrship_cowan/dist/.tmp-0c9b3scz/airrship-0.1.5.tar", last modified: Wed May  3 10:37:26 2023, max compression
```

## Comparing `airrship-0.1.4.tar` & `airrship-0.1.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 09:46:22.000000 airrship-0.1.4/
--rw-r--r--   0 s1404341   (501) staff       (20)    34523 2022-12-16 13:44:11.000000 airrship-0.1.4/LICENSE
--rw-r--r--   0 s1404341   (501) staff       (20)    41786 2023-05-03 09:46:22.000000 airrship-0.1.4/PKG-INFO
--rw-r--r--   0 s1404341   (501) staff       (20)     1231 2023-03-31 09:31:55.000000 airrship-0.1.4/README.md
-drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship/
--rw-r--r--   0 s1404341   (501) staff       (20)       22 2023-04-25 16:21:26.000000 airrship-0.1.4/airrship/__init__.py
--rwx------   0 s1404341   (501) staff       (20)   109925 2023-04-28 13:58:47.000000 airrship-0.1.4/airrship/create_repertoire.py
-drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship/data/
--rw-r--r--   0 s1404341   (501) staff       (20)     3866 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/D_3_family_trimming_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     3481 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/D_5_family_trimming_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      356 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHD_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      909 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHD_usage_gene.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      168 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHJ_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      167 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHJ_usage_gene.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      421 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/IGHV_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     3239 2023-01-20 17:37:33.000000 airrship-0.1.4/airrship/data/IGHV_usage_gene.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     3473 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/J_family_trimming_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    10675 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/V_family_trimming_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)        0 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/__init__.py
--rw-r--r--   0 s1404341   (501) staff       (20)    31632 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/cdr1_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    39947 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/cdr2_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    46095 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/cdr3_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    69757 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/cdr_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    38976 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr1_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    43833 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr2_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    73585 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr3_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     7942 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr4_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    82819 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/fwr_kmer_base_usage.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     4839 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/imgt_human_IGHD.fasta
--rw-r--r--   0 s1404341   (501) staff       (20)     1790 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/imgt_human_IGHJ.fasta
--rw-r--r--   0 s1404341   (501) staff       (20)   175791 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/imgt_human_IGHV.fasta
--rw-r--r--   0 s1404341   (501) staff       (20)  2240771 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/mut_freq_per_seq_per_family.csv
--rw-r--r--   0 s1404341   (501) staff       (20)       99 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np1_first_base_probs.csv
--rw-r--r--   0 s1404341   (501) staff       (20)      988 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np1_lengths_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    12922 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np1_transition_probs_per_position_igag.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    12933 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np1_transition_probs_per_position_igdm.csv
--rw-r--r--   0 s1404341   (501) staff       (20)       99 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np2_first_base_probs.csv
--rw-r--r--   0 s1404341   (501) staff       (20)     1073 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np2_lengths_proportions.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    12883 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np2_transition_probs_per_position_igag.csv
--rw-r--r--   0 s1404341   (501) staff       (20)    12925 2022-12-16 13:44:11.000000 airrship-0.1.4/airrship/data/np2_transition_probs_per_position_igdm.csv
-drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/
--rw-r--r--   0 s1404341   (501) staff       (20)    41786 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/PKG-INFO
--rw-r--r--   0 s1404341   (501) staff       (20)     1569 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/SOURCES.txt
--rw-r--r--   0 s1404341   (501) staff       (20)        1 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/dependency_links.txt
--rw-r--r--   0 s1404341   (501) staff       (20)       61 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/entry_points.txt
--rw-r--r--   0 s1404341   (501) staff       (20)        9 2023-05-03 09:46:22.000000 airrship-0.1.4/airrship.egg-info/top_level.txt
--rw-r--r--   0 s1404341   (501) staff       (20)      957 2023-01-25 11:07:34.000000 airrship-0.1.4/pyproject.toml
--rw-r--r--   0 s1404341   (501) staff       (20)      213 2023-05-03 09:46:22.000000 airrship-0.1.4/setup.cfg
--rw-r--r--   0 s1404341   (501) staff       (20)       37 2022-12-19 16:04:00.000000 airrship-0.1.4/setup.py
+drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 10:37:26.000000 airrship-0.1.5/
+-rw-r--r--   0 s1404341   (501) staff       (20)    34523 2022-12-16 13:44:11.000000 airrship-0.1.5/LICENSE
+-rw-r--r--   0 s1404341   (501) staff       (20)    41786 2023-05-03 10:37:26.000000 airrship-0.1.5/PKG-INFO
+-rw-r--r--   0 s1404341   (501) staff       (20)     1231 2023-03-31 09:31:55.000000 airrship-0.1.5/README.md
+drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 10:37:26.000000 airrship-0.1.5/airrship/
+-rw-r--r--   0 s1404341   (501) staff       (20)       22 2023-05-03 10:36:39.000000 airrship-0.1.5/airrship/__init__.py
+-rwx------   0 s1404341   (501) staff       (20)   109913 2023-05-03 10:34:08.000000 airrship-0.1.5/airrship/create_repertoire.py
+drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 10:37:26.000000 airrship-0.1.5/airrship/data/
+-rw-r--r--   0 s1404341   (501) staff       (20)     3866 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/D_3_family_trimming_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     3481 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/D_5_family_trimming_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      356 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/IGHD_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      909 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/IGHD_usage_gene.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      168 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/IGHJ_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      167 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/IGHJ_usage_gene.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      421 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/IGHV_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     3239 2023-01-20 17:37:33.000000 airrship-0.1.5/airrship/data/IGHV_usage_gene.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     3473 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/J_family_trimming_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    10675 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/V_family_trimming_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)        0 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/__init__.py
+-rw-r--r--   0 s1404341   (501) staff       (20)    31632 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/cdr1_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    39947 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/cdr2_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    46095 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/cdr3_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    69757 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/cdr_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    38976 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/fwr1_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    43833 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/fwr2_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    73585 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/fwr3_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     7942 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/fwr4_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    82819 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/fwr_kmer_base_usage.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     4839 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/imgt_human_IGHD.fasta
+-rw-r--r--   0 s1404341   (501) staff       (20)     1790 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/imgt_human_IGHJ.fasta
+-rw-r--r--   0 s1404341   (501) staff       (20)   175791 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/imgt_human_IGHV.fasta
+-rw-r--r--   0 s1404341   (501) staff       (20)  2240771 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/mut_freq_per_seq_per_family.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)       99 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/np1_first_base_probs.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)      988 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/np1_lengths_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    12922 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/np1_transition_probs_per_position_igag.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    12933 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/np1_transition_probs_per_position_igdm.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)       99 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/np2_first_base_probs.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)     1073 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/np2_lengths_proportions.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    12883 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/np2_transition_probs_per_position_igag.csv
+-rw-r--r--   0 s1404341   (501) staff       (20)    12925 2022-12-16 13:44:11.000000 airrship-0.1.5/airrship/data/np2_transition_probs_per_position_igdm.csv
+drwxr-xr-x   0 s1404341   (501) staff       (20)        0 2023-05-03 10:37:26.000000 airrship-0.1.5/airrship.egg-info/
+-rw-r--r--   0 s1404341   (501) staff       (20)    41786 2023-05-03 10:37:26.000000 airrship-0.1.5/airrship.egg-info/PKG-INFO
+-rw-r--r--   0 s1404341   (501) staff       (20)     1569 2023-05-03 10:37:26.000000 airrship-0.1.5/airrship.egg-info/SOURCES.txt
+-rw-r--r--   0 s1404341   (501) staff       (20)        1 2023-05-03 10:37:26.000000 airrship-0.1.5/airrship.egg-info/dependency_links.txt
+-rw-r--r--   0 s1404341   (501) staff       (20)       61 2023-05-03 10:37:26.000000 airrship-0.1.5/airrship.egg-info/entry_points.txt
+-rw-r--r--   0 s1404341   (501) staff       (20)        9 2023-05-03 10:37:26.000000 airrship-0.1.5/airrship.egg-info/top_level.txt
+-rw-r--r--   0 s1404341   (501) staff       (20)      957 2023-05-03 10:37:07.000000 airrship-0.1.5/pyproject.toml
+-rw-r--r--   0 s1404341   (501) staff       (20)      213 2023-05-03 10:37:26.000000 airrship-0.1.5/setup.cfg
+-rw-r--r--   0 s1404341   (501) staff       (20)       37 2022-12-19 16:04:00.000000 airrship-0.1.5/setup.py
```

### Comparing `airrship-0.1.4/LICENSE` & `airrship-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/PKG-INFO` & `airrship-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airrship
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simulation of B cell receptor repertoires
 Author-email: Catherine Sutherland <catherine.sutherland@ed.ac.uk>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `airrship-0.1.4/README.md` & `airrship-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/create_repertoire.py` & `airrship-0.1.5/airrship/create_repertoire.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 import csv
 import time
 import warnings
 import re
 import argparse
 import sys
 import importlib.resources
-from importlib.metadata import version
+
+from airrship import __version__
+
 
 
 
 # Classes
 
 
 class Allele:
@@ -2096,15 +2098,15 @@
 def main(args=None):
     if args is None:
         args = sys.argv[1:]
 
     parser = argparse.ArgumentParser(allow_abbrev=False)
 
     parser.add_argument('-v', '--version',
-                        action='version', version=version('airrship'))
+                        action='version', version=__version__)
     parser.add_argument("-o",
                         "--outfname",  # specify prefix to name files
                         action="store",
                         help="Output file name.",
                         dest="out_name",
                         required=True)
     parser.add_argument("--outdir",
```

### Comparing `airrship-0.1.4/airrship/data/D_3_family_trimming_proportions.csv` & `airrship-0.1.5/airrship/data/D_3_family_trimming_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/D_5_family_trimming_proportions.csv` & `airrship-0.1.5/airrship/data/D_5_family_trimming_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/IGHD_usage_gene.csv` & `airrship-0.1.5/airrship/data/IGHD_usage_gene.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/IGHV_usage_gene.csv` & `airrship-0.1.5/airrship/data/IGHV_usage_gene.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/J_family_trimming_proportions.csv` & `airrship-0.1.5/airrship/data/J_family_trimming_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/V_family_trimming_proportions.csv` & `airrship-0.1.5/airrship/data/V_family_trimming_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/cdr1_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/cdr1_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/cdr2_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/cdr2_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/cdr3_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/cdr3_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/cdr_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/cdr_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/fwr1_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/fwr1_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/fwr2_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/fwr2_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/fwr3_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/fwr3_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/fwr4_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/fwr4_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/fwr_kmer_base_usage.csv` & `airrship-0.1.5/airrship/data/fwr_kmer_base_usage.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/imgt_human_IGHD.fasta` & `airrship-0.1.5/airrship/data/imgt_human_IGHD.fasta`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/imgt_human_IGHJ.fasta` & `airrship-0.1.5/airrship/data/imgt_human_IGHJ.fasta`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/imgt_human_IGHV.fasta` & `airrship-0.1.5/airrship/data/imgt_human_IGHV.fasta`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/mut_freq_per_seq_per_family.csv` & `airrship-0.1.5/airrship/data/mut_freq_per_seq_per_family.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/np1_lengths_proportions.csv` & `airrship-0.1.5/airrship/data/np1_lengths_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/np1_transition_probs_per_position_igag.csv` & `airrship-0.1.5/airrship/data/np1_transition_probs_per_position_igag.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/np1_transition_probs_per_position_igdm.csv` & `airrship-0.1.5/airrship/data/np1_transition_probs_per_position_igdm.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/np2_lengths_proportions.csv` & `airrship-0.1.5/airrship/data/np2_lengths_proportions.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/np2_transition_probs_per_position_igag.csv` & `airrship-0.1.5/airrship/data/np2_transition_probs_per_position_igag.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship/data/np2_transition_probs_per_position_igdm.csv` & `airrship-0.1.5/airrship/data/np2_transition_probs_per_position_igdm.csv`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/airrship.egg-info/PKG-INFO` & `airrship-0.1.5/airrship.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airrship
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simulation of B cell receptor repertoires
 Author-email: Catherine Sutherland <catherine.sutherland@ed.ac.uk>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `airrship-0.1.4/airrship.egg-info/SOURCES.txt` & `airrship-0.1.5/airrship.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `airrship-0.1.4/pyproject.toml` & `airrship-0.1.5/pyproject.toml`

 * *Files identical despite different names*

