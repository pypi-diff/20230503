# Comparing `tmp/visualimiss-0.0.6.tar.gz` & `tmp/visualimiss-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visualimiss-0.0.6.tar", last modified: Fri Apr 21 11:58:34 2023, max compression
+gzip compressed data, was "visualimiss-0.0.7.tar", last modified: Wed May  3 16:14:14 2023, max compression
```

## Comparing `visualimiss-0.0.6.tar` & `visualimiss-0.0.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 11:58:34.904872 visualimiss-0.0.6/
--rw-rw-rw-   0        0        0     1088 2023-04-14 15:05:45.000000 visualimiss-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     2646 2023-04-21 11:58:34.903861 visualimiss-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     2258 2023-04-15 15:24:07.000000 visualimiss-0.0.6/README.md
--rw-rw-rw-   0        0        0      533 2023-04-15 17:38:10.000000 visualimiss-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-21 11:58:34.904872 visualimiss-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-21 11:58:34.875172 visualimiss-0.0.6/visualimiss/
--rw-rw-rw-   0        0        0       94 2023-04-14 16:04:41.000000 visualimiss-0.0.6/visualimiss/__init__.py
--rw-rw-rw-   0        0        0      431 2023-04-13 16:51:12.000000 visualimiss-0.0.6/visualimiss/utils.py
--rw-rw-rw-   0        0        0     2467 2023-04-14 02:12:37.000000 visualimiss-0.0.6/visualimiss/visualimiss.py
-drwxrwxrwx   0        0        0        0 2023-04-21 11:58:34.902884 visualimiss-0.0.6/visualimiss.egg-info/
--rw-rw-rw-   0        0        0     2646 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-21 11:58:34.000000 visualimiss-0.0.6/visualimiss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:14.262495 visualimiss-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-03 16:13:56.000000 visualimiss-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-03 16:14:14.262495 visualimiss-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-03 16:13:56.000000 visualimiss-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-03 16:13:56.000000 visualimiss-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 16:14:14.262495 visualimiss-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:14.258495 visualimiss-0.0.7/visualimiss/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-03 16:13:56.000000 visualimiss-0.0.7/visualimiss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-03 16:13:56.000000 visualimiss-0.0.7/visualimiss/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-03 16:13:56.000000 visualimiss-0.0.7/visualimiss/visualimiss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 16:14:14.258495 visualimiss-0.0.7/visualimiss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-03 16:14:14.000000 visualimiss-0.0.7/visualimiss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-03 16:14:14.000000 visualimiss-0.0.7/visualimiss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 16:14:14.000000 visualimiss-0.0.7/visualimiss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-03 16:14:14.000000 visualimiss-0.0.7/visualimiss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 16:14:14.000000 visualimiss-0.0.7/visualimiss.egg-info/top_level.txt
```

### Comparing `visualimiss-0.0.6/LICENSE` & `visualimiss-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Duc Nguyen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Duc Nguyen
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `visualimiss-0.0.6/pyproject.toml` & `visualimiss-0.0.7/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-[build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "visualimiss"
-version = "0.0.6"
-authors = [{ name="ngntrgduc"}]
-description = "Visualize missing data"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = []
-keywords = ["data", "data visualization", "missing data"]
-dependencies = ["numpy", "pandas", "matplotlib"]
-
-[project.urls]
-"Homepage" = "https://github.com/ngntrgduc/visualimiss"
+[build-system]
+requires = ["setuptools>=61.0"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "visualimiss"
+version = "0.0.7"
+authors = [{ name="ngntrgduc"}]
+description = "Visualize missing data"
+readme = "README.md"
+requires-python = ">=3.7"
+classifiers = []
+keywords = ["data", "data visualization", "missing data"]
+dependencies = ["numpy", "pandas", "matplotlib"]
+
+[project.urls]
+"Homepage" = "https://github.com/ngntrgduc/visualimiss"
 "Bug Tracker" = "https://github.com/ngntrgduc/visualimiss/issues"
```

### Comparing `visualimiss-0.0.6/visualimiss/visualimiss.py` & `visualimiss-0.0.7/visualimiss/visualimiss.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,99 @@
-import numpy as np
-import matplotlib.pyplot as plt
-from matplotlib import ticker
-from .utils import nullity_sort
-
-def matrix(df, sort=None, figsize=(25, 10), fontsize=12, 
-           color=(60, 60, 60), show_label=True, label_rotation=45):
-    
-    df = nullity_sort(df, sort=sort)
-    height, width = df.shape
-
-    z = df.notnull().values
-    x = np.zeros((height, width, 3), dtype=np.uint32)
-    x[z < 0.5] = (255, 255, 255) # White color
-    x[z > 0.5] = color
-
-    plt.figure(figsize=figsize)
-    ax = plt.subplot()
-    ax.imshow(x, interpolation='none', aspect='auto')
-    ax.xaxis.tick_top()
-    ax.xaxis.set_ticks_position('none')
-    ax.yaxis.set_ticks_position('none')
-    ax.set_yticks([])
-    ax.spines[['top', 'right', 'bottom', 'left']].set_visible(False)
-    
-    if show_label:
-        ax.set_xticks(list(range(0, width)))
-        ax.set_xticklabels(list(df.columns), rotation=label_rotation, 
-                           ha='left', fontsize=fontsize)
-    else:
-        ax.set_xticks([])
-
-    # Add a vertical line across the grid
-    for x in [_ + 0.5 for _ in range(0, width-1)]:
-        ax.axvline(x, color='white')
-
-    return ax
-
-
-def bar(df, sort=None, figsize=(25, 10), fontsize=12, 
-        color='C0', show_label=True, label_rotation=45):
-
-    df = nullity_sort(df, sort=sort)
-        
-    ax1 = plt.gca()
-
-    plot_args = {'figsize': figsize, 'fontsize': fontsize, 'color': color, 'ax': ax1}
-    valid_counts = len(df) - df.isnull().sum()
-    (valid_counts / len(df)).plot.bar(**plot_args)
-
-    axes = [ax1]
-
-    if show_label:
-        ax1.set_xticklabels(ax1.get_xticklabels(), 
-                            rotation=label_rotation, ha='right', fontsize=fontsize)
-        ax1.set_ylim([0, 1])
-        ax1.yaxis.set_major_formatter(ticker.PercentFormatter(1.0)) # Make % format
-        
-        # Display total of valid data above the plot.
-        ax2 = ax1.twiny()
-        ax2.set_xticks(ax1.get_xticks())
-        ax2.set_xlim(ax1.get_xlim())
-        ax2.set_xticklabels(valid_counts.values, 
-                                rotation=label_rotation, ha='left', fontsize=fontsize)
-        axes.append(ax2)
-    else:
-        ax1.set_xticks([])
-        ax1.set_yticks([])
-
-    for ax in axes:
-        ax.spines[['top', 'right', 'bottom', 'left']].set_visible(False)
-        ax.xaxis.set_ticks_position('none')
-        ax.yaxis.set_ticks_position('none')
-
-    return ax1
+import numpy as np
+import pandas as pd
+import matplotlib.pyplot as plt
+from matplotlib import ticker
+from .utils import nullity_sort
+
+def matrix(df, sort=None, figsize=(25, 10), fontsize=12, 
+           color=(60, 60, 60), show_label=True, label_rotation=45):
+    
+    df = nullity_sort(df, sort=sort)
+    height, width = df.shape
+
+    z = df.notnull().values
+    x = np.zeros((height, width, 3), dtype=np.uint32)
+    x[z < 0.5] = (255, 255, 255) # White color
+    x[z > 0.5] = color
+
+    plt.figure(figsize=figsize)
+    ax = plt.subplot()
+    ax.imshow(x, interpolation='none', aspect='auto')
+    ax.xaxis.tick_top()
+    ax.xaxis.set_ticks_position('none')
+    ax.yaxis.set_ticks_position('none')
+    ax.set_yticks([])
+    ax.spines[['top', 'right', 'bottom', 'left']].set_visible(False)
+    
+    if show_label:
+        ax.set_xticks(list(range(0, width)))
+        ax.set_xticklabels(list(df.columns), rotation=label_rotation, 
+                           ha='left', fontsize=fontsize)
+    else:
+        ax.set_xticks([])
+
+    # Add a vertical line across the grid
+    for x in [_ + 0.5 for _ in range(0, width-1)]:
+        ax.axvline(x, color='white')
+
+    return ax
+
+
+def bar(df, sort=None, figsize=(25, 10), fontsize=12, 
+        color='C0', show_label=True, label_rotation=45):
+
+    df = nullity_sort(df, sort=sort)
+        
+    ax1 = plt.gca()
+    axes = [ax1]
+
+    plot_args = {'figsize': figsize, 'fontsize': fontsize, 'color': color, 'ax': ax1}
+    valid_counts = df.notnull().sum()
+    (valid_counts / len(df)).plot.bar(**plot_args)
+
+    if show_label:
+        ax1.set_xticklabels(ax1.get_xticklabels(), 
+                            rotation=label_rotation, ha='right', fontsize=fontsize)
+        ax1.set_ylim([0, 1])
+        ax1.yaxis.set_major_formatter(ticker.PercentFormatter(1.0)) # Make % format
+        
+        # Display total of valid data above the plot.
+        ax2 = ax1.twiny()
+        ax2.set_xticks(ax1.get_xticks())
+        ax2.set_xlim(ax1.get_xlim())
+        ax2.set_xticklabels(valid_counts.values, 
+                                rotation=label_rotation, ha='left', fontsize=fontsize)
+        axes.append(ax2)
+    else:
+        ax1.set_xticks([])
+        ax1.set_yticks([])
+
+    for ax in axes:
+        ax.spines[['top', 'right', 'bottom', 'left']].set_visible(False)
+        ax.xaxis.set_ticks_position('none')
+        ax.yaxis.set_ticks_position('none')
+
+    return ax1
+
+def info(df, print_null=True):
+    """This function doesn't visualize but give the information of dataframe,
+        a more readable version of pandas.DataFrame.info().
+    """
+    print(f'- DataFrame has {len(df)} rows, {len(df.columns)} columns')
+    print(f'- Memory usage: {sum(df.memory_usage())/1000000} MB')
+    
+    if print_null:
+        name = 'Null count'
+        count = df.isnull().sum()
+    else:
+        name = 'Non-Null count'
+        count = df.notnull().sum()
+
+    # if sort == 'asc':
+        # count = count.sort_values()
+    # elif sort == 'desc':
+        # count = count.sort_values(ascending=False)
+    
+    info = pd.DataFrame(data={name: count,
+                              'Dtype': df.dtypes.to_string(index=False).split()})
+    print(info)
+    pass
```

