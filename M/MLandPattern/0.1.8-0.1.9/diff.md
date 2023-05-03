# Comparing `tmp/MLandPattern-0.1.8.tar.gz` & `tmp/MLandPattern-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MLandPattern-0.1.8.tar", last modified: Thu Apr 27 14:06:44 2023, max compression
+gzip compressed data, was "MLandPattern-0.1.9.tar", last modified: Wed May  3 19:29:09 2023, max compression
```

## Comparing `MLandPattern-0.1.8.tar` & `MLandPattern-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-27 14:06:44.963662 MLandPattern-0.1.8/
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-27 14:06:44.961127 MLandPattern-0.1.8/MLandPattern/
--rw-r--r--   0 pablomunoz   (501) staff       (20)    16656 2023-04-27 14:06:27.000000 MLandPattern-0.1.8/MLandPattern/MLandPattern.py
--rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.1.8/MLandPattern/__init__.py
-drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-04-27 14:06:44.962756 MLandPattern-0.1.8/MLandPattern.egg-info/
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-04-27 14:06:44.000000 MLandPattern-0.1.8/MLandPattern.egg-info/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-04-27 14:06:44.000000 MLandPattern-0.1.8/MLandPattern.egg-info/SOURCES.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-04-27 14:06:44.000000 MLandPattern-0.1.8/MLandPattern.egg-info/dependency_links.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-04-27 14:06:44.000000 MLandPattern-0.1.8/MLandPattern.egg-info/top_level.txt
--rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-04-27 14:06:44.963364 MLandPattern-0.1.8/PKG-INFO
--rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.1.8/README.md
--rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-04-27 14:06:44.963793 MLandPattern-0.1.8/setup.cfg
--rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-04-27 14:06:41.000000 MLandPattern-0.1.8/setup.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-03 19:29:09.635215 MLandPattern-0.1.9/
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-03 19:29:09.629397 MLandPattern-0.1.9/MLandPattern/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)    16780 2023-04-28 06:57:12.000000 MLandPattern-0.1.9/MLandPattern/MLandPattern.py
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       27 2023-03-29 18:22:32.000000 MLandPattern-0.1.9/MLandPattern/__init__.py
+drwxr-xr-x   0 pablomunoz   (501) staff       (20)        0 2023-05-03 19:29:09.633597 MLandPattern-0.1.9/MLandPattern.egg-info/
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-05-03 19:29:09.000000 MLandPattern-0.1.9/MLandPattern.egg-info/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      216 2023-05-03 19:29:09.000000 MLandPattern-0.1.9/MLandPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        1 2023-05-03 19:29:09.000000 MLandPattern-0.1.9/MLandPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       13 2023-05-03 19:29:09.000000 MLandPattern-0.1.9/MLandPattern.egg-info/top_level.txt
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      235 2023-05-03 19:29:09.634724 MLandPattern-0.1.9/PKG-INFO
+-rw-r--r--   0 pablomunoz   (501) staff       (20)        0 2023-03-28 08:17:35.000000 MLandPattern-0.1.9/README.md
+-rw-r--r--   0 pablomunoz   (501) staff       (20)       38 2023-05-03 19:29:09.635567 MLandPattern-0.1.9/setup.cfg
+-rw-r--r--   0 pablomunoz   (501) staff       (20)      276 2023-05-03 19:27:46.000000 MLandPattern-0.1.9/setup.py
```

### Comparing `MLandPattern-0.1.8/MLandPattern/MLandPattern.py` & `MLandPattern-0.1.9/MLandPattern/MLandPattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -300,16 +300,17 @@
 
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
+        acc = round(acc*100, 2)
         print(f'Accuracy: {acc}')
-        print(f'Error: {1 - acc}')
+        print(f'Error: {(100 - acc)}%')
 
     return SPost, predictions
 
 
 def MVG_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the MultiVariate Gaussian classifier on the logarithm dimension for a set of data, and applyes it to a test dataset
@@ -338,16 +339,17 @@
 
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
+        acc = round(acc*100, 2)
         print(f'Accuracy: {acc}')
-        print(f'Error: {1 - acc}')
+        print(f'Error: {(100 - acc)}%')
 
     return SPost, predictions
 
 
 def Naive_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the Naive classifier for a set of data, and applyes it to a test dataset
@@ -377,16 +379,17 @@
 
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
-        print(f'Accuracy: {acc*100}%')
-        print(f'Error: {(1 - acc)*100}%')
+        acc = round(acc*100, 2)
+        print(f'Accuracy: {acc}')
+        print(f'Error: {(100 - acc)}%')
 
     return SPost, predictions
 
 
 def Naive_log_classifier(train_data, train_labels, test_data, prior_probability, test_label=[]):
     """
     Calculates the model of the Naive classifier on the logarithm realm for a set of data, and applyes it to a test dataset
@@ -417,11 +420,12 @@
 
     if(len(test_label) != 0):
         acc = 0
         for i in range(len(test_label)):
             if predictions[i] == test_label[i]:
                 acc += 1
         acc/=len(test_label)
-        print(f'Accuracy: {acc*100}%')
-        print(f'Error: {(1 - acc)*100}%')
+        acc = round(acc*100, 2)
+        print(f'Accuracy: {acc}')
+        print(f'Error: {(100 - acc)}%')
 
     return SPost, predictions
```

