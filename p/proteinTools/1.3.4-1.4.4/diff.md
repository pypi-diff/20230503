# Comparing `tmp/proteinTools-1.3.4.tar.gz` & `tmp/proteinTools-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-1.3.4.tar", last modified: Wed Apr 26 01:41:49 2023, max compression
+gzip compressed data, was "proteinTools-1.4.4.tar", last modified: Wed May  3 04:09:01 2023, max compression
```

## Comparing `proteinTools-1.3.4.tar` & `proteinTools-1.4.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-26 01:41:49.117251 proteinTools-1.3.4/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.3.4/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-26 01:41:49.113927 proteinTools-1.3.4/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.3.4/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-26 01:41:48.995367 proteinTools-1.3.4/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    53271 2023-04-26 01:32:02.000000 proteinTools-1.3.4/proteinTools/PT.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.3.4/proteinTools/__init__.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-26 01:41:49.100507 proteinTools-1.3.4/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/requires.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-26 01:41:48.000000 proteinTools-1.3.4/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-26 01:41:49.121290 proteinTools-1.3.4/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-04-26 01:41:41.000000 proteinTools-1.3.4/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-03 04:09:01.046785 proteinTools-1.4.4/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-1.4.4/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-03 04:09:01.038872 proteinTools-1.4.4/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-1.4.4/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-03 04:09:00.902194 proteinTools-1.4.4/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    53271 2023-05-03 03:59:01.000000 proteinTools-1.4.4/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-1.4.4/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-05-03 04:09:00.999945 proteinTools-1.4.4/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      483 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       58 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-05-03 04:09:00.000000 proteinTools-1.4.4/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-05-03 04:09:01.083979 proteinTools-1.4.4/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      555 2023-05-03 04:08:43.000000 proteinTools-1.4.4/setup.py
```

### Comparing `proteinTools-1.3.4/LICENSE` & `proteinTools-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-1.3.4/proteinTools/PT.py` & `proteinTools-1.4.4/proteinTools/PT.py`

 * *Files 0% similar despite different names*

```diff
@@ -468,15 +468,15 @@
                                 current_ligand_index += 1
                         element = line[76:80].strip()
                         if element not in atom_keys:
                             e = element[:1]
                             if e not in atom_keys:
                                 e = element[1:]
                             element = e
-                        atm = atom(element, float(line[30:38].strip()), float(line[38:47].strip()), float(line[47:56].strip()), data = line, number = int(numconv.sub('', line[6:13])))
+                        atm = atom(element, float(line[30:38].strip()), float(line[38:46].strip()), float(line[46:56].strip()), data = line, number = int(numconv.sub('', line[6:13])))
                         try:
                             self.ligand_list[current_ligand_index].atoms.append(atm)
                         except:
                             try:
                                  self.ligand_list[current_ligand_index + 1].atoms.append(atm)
                             except:
                                  continue
```

### Comparing `proteinTools-1.3.4/setup.py` & `proteinTools-1.4.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setuptools.setup(
     name = "proteinTools",
-    version = "1.3.4",
+    version = "1.4.4",
     author = "Christian de Frondeville",
     description = "Lightweight, object-oriented bioinformatics package which simplifies interacting with proteins.",
     long_description = long_description,
     packages = ["proteinTools"],
     install_requires=['pandas','urllib3','chembl-webresource-client','mygene', 'pubchempy']
 )
```

