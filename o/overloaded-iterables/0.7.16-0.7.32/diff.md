# Comparing `tmp/overloaded-iterables-0.7.16.tar.gz` & `tmp/overloaded-iterables-0.7.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overloaded-iterables-0.7.16.tar", last modified: Mon May  1 08:08:20 2023, max compression
+gzip compressed data, was "overloaded-iterables-0.7.32.tar", last modified: Tue May  2 19:44:12 2023, max compression
```

## Comparing `overloaded-iterables-0.7.16.tar` & `overloaded-iterables-0.7.32.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 08:08:20.022153 overloaded-iterables-0.7.16/
--rw-rw-rw-   0        0        0     1097 2023-05-01 06:21:45.000000 overloaded-iterables-0.7.16/LICENSE
--rw-rw-rw-   0        0        0     7908 2023-05-01 08:08:20.023164 overloaded-iterables-0.7.16/PKG-INFO
--rw-rw-rw-   0        0        0     7194 2023-05-01 08:05:48.000000 overloaded-iterables-0.7.16/README.md
--rw-rw-rw-   0        0        0      111 2023-05-01 08:08:20.029846 overloaded-iterables-0.7.16/setup.cfg
--rw-rw-rw-   0        0        0     1497 2023-05-01 06:21:45.000000 overloaded-iterables-0.7.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:08:19.963958 overloaded-iterables-0.7.16/src/
-drwxrwxrwx   0        0        0        0 2023-05-01 08:08:19.983438 overloaded-iterables-0.7.16/src/overloaded_iterables/
--rw-rw-rw-   0        0        0        0 2023-05-01 06:21:45.000000 overloaded-iterables-0.7.16/src/overloaded_iterables/__init__.py
--rw-rw-rw-   0        0        0    14919 2023-05-01 08:06:01.000000 overloaded-iterables-0.7.16/src/overloaded_iterables/classes.py
-drwxrwxrwx   0        0        0        0 2023-05-01 08:08:20.020985 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/
--rw-rw-rw-   0        0        0     7908 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-01 08:08:19.000000 overloaded-iterables-0.7.16/src/overloaded_iterables.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-02 19:44:12.993371 overloaded-iterables-0.7.32/
+-rw-rw-rw-   0        0        0     1097 2023-04-29 23:58:34.000000 overloaded-iterables-0.7.32/LICENSE
+-rw-rw-rw-   0        0        0    12615 2023-05-02 19:44:12.994464 overloaded-iterables-0.7.32/PKG-INFO
+-rw-rw-rw-   0        0        0    11888 2023-05-02 19:40:10.000000 overloaded-iterables-0.7.32/README.md
+-rw-rw-rw-   0        0        0      111 2023-05-02 19:44:12.996476 overloaded-iterables-0.7.32/setup.cfg
+-rw-rw-rw-   0        0        0     1645 2023-05-02 19:44:01.000000 overloaded-iterables-0.7.32/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:44:12.942295 overloaded-iterables-0.7.32/src/
+drwxrwxrwx   0        0        0        0 2023-05-02 19:44:12.974550 overloaded-iterables-0.7.32/src/overloaded_iterables/
+-rw-rw-rw-   0        0        0      676 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.32/src/overloaded_iterables/__init__.py
+-rw-rw-rw-   0        0        0    17338 2023-05-02 19:40:38.000000 overloaded-iterables-0.7.32/src/overloaded_iterables/classes.py
+-rw-rw-rw-   0        0        0     1905 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.32/src/overloaded_iterables/exceptions.py
+-rw-rw-rw-   0        0        0      921 2023-05-02 18:49:58.000000 overloaded-iterables-0.7.32/src/overloaded_iterables/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-02 19:44:12.992374 overloaded-iterables-0.7.32/src/overloaded_iterables.egg-info/
+-rw-rw-rw-   0        0        0    12615 2023-05-02 19:44:12.000000 overloaded-iterables-0.7.32/src/overloaded_iterables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-05-02 19:44:12.000000 overloaded-iterables-0.7.32/src/overloaded_iterables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-02 19:44:12.000000 overloaded-iterables-0.7.32/src/overloaded_iterables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-02 19:44:12.000000 overloaded-iterables-0.7.32/src/overloaded_iterables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-02 19:44:12.000000 overloaded-iterables-0.7.32/src/overloaded_iterables.egg-info/top_level.txt
```

### Comparing `overloaded-iterables-0.7.16/LICENSE` & `overloaded-iterables-0.7.32/LICENSE`

 * *Files identical despite different names*

### Comparing `overloaded-iterables-0.7.16/src/overloaded_iterables/classes.py` & `overloaded-iterables-0.7.32/src/overloaded_iterables/classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class OverloadedList(list):
     """
     Overloaded <list> class to add additional methods.
     """
     iZERO: int = 0
     fZERO: float = 0.0
-    TIME_FORMAT:str = '%Y-%m-%dT%H-%M-%S.%fZ%z'
+    TIME_FORMAT: str = '%Y-%m-%dT%H-%M-%S.%fZ%z'
 
     def mean(self) -> float:
         """
         Returns the arithmetic mean of the values in the OverloadedList.
         """
         return self.sum()/self.len
 
@@ -107,16 +107,16 @@
         color: str = '#0f0f0f',
         file_name: str = None,
         histtype: str = 'step',
         align: str = 'mid',
         orientation: str = 'vertical',
         log_scale: bool = False,
         show: bool = False,
-        dpi: int=300,
-        pad_inches: float=1,
+        dpi: int = 300,
+        pad_inches: float = 1,
         *args,
         **kwargs
     ) -> bool:
         """
         Draws and saves if required, the histogram of the frequency distribution of the elements of the OverloadedList object.
         """
         try:
@@ -151,15 +151,15 @@
                 raise AttributeError(
                     "Both `show` and `save_dir` cannot be defined."
                 )
             elif not show and not save_dir:
                 pass
             else:
                 raise ValueError("Something went wrong.")
-            
+
             plt.clf()
             return True
         except Exception as ex:
             raise ex
 
     def plot(
             self,
@@ -170,16 +170,16 @@
             file_name: str = None,
             color: str = '#000000',
             linewidth: float = 1,
             marker: str = ',',
             markerfacecolor: str = '#252525',
             marker_size: float = 1.0,
             show: bool = False,
-            dpi: int=300,
-            pad_inches: float=1,
+            dpi: int = 300,
+            pad_inches: float = 1,
             *args,
             **kwargs
     ):
         """
         Draws and saves if required, the line-plot of the frequency distribution of the elements of the OverloadedList object.
         """
         try:
@@ -192,29 +192,29 @@
             plt.xlabel(x_label)
             plt.ylabel(y_label)
             plt.grid(visible=True, which='both', axis='both')
 
             if save_dir and not show:
                 file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__plot__{datetime.utcnow().strftime(self.TIME_FORMAT)}.PNG"
                 save_path = path.join(save_dir, file_name)
-                
+
                 plt.savefig(fname=save_path, dpi=dpi, pad_inches=pad_inches)
 
                 return file_name
             elif show and not save_dir:
                 plt.show()
             elif save_dir and show:
                 raise AttributeError(
                     "Both `show` and `save_dir` cannot be defined."
                 )
             elif not show and not save_dir:
                 pass
             else:
                 raise ValueError("Something went wrong.")
-            
+
             plt.clf()
             return True
         except Exception as ex:
             raise ex
 
     def scatter(
             self,
@@ -224,50 +224,51 @@
             save_dir: str = None,
             file_name: str = None,
             size: List[float] = [1.25],
             color: str = '#000000',
             marker: str = ',',
             line_width: float = 2,
             show: bool = False,
-            dpi: int=300,
-            pad_inches: float=1,
+            dpi: int = 300,
+            pad_inches: float = 1,
             *args,
             **kwargs
     ):
         """
         Draws and saves if required, the scatter-plot of the frequency distribution of the elements of the OverloadedList object.
         """
         try:
             x_axis, y_axis = self.frequencies
             x_axis = array(x_axis)
             y_axis = array(y_axis)
-            plt.scatter(x=x_axis, y=y_axis, s=array(size), color=color, marker=marker, linewidths=line_width)
+            plt.scatter(x=x_axis, y=y_axis, s=array(size),
+                        color=color, marker=marker, linewidths=line_width)
             plt.title(title)
             plt.xlabel(x_label)
             plt.ylabel(y_label)
             plt.grid(visible=True, which='both', axis='both')
 
             if save_dir and not show:
                 file_name = f"{file_name.lower().strip()}.PNG" if file_name else f"{title.lower().strip()}__scatter__{datetime.utcnow().strftime(self.TIME_FORMAT)}.PNG"
                 save_path = path.join(save_dir, file_name)
-                
+
                 plt.savefig(fname=save_path, dpi=dpi, pad_inches=pad_inches)
 
                 return file_name
             elif show and not save_dir:
                 plt.show()
             elif save_dir and show:
                 raise AttributeError(
                     "Both `show` and `save_dir` cannot be defined."
                 )
             elif not show and not save_dir:
                 pass
             else:
                 raise ValueError("Something went wrong.")
-            
+
             plt.clf()
             return True
         except Exception as ex:
             raise ex
 
     @property
     def _type(self):
@@ -312,14 +313,89 @@
                 frequencies.append(self.count(item))
 
             return values, frequencies
         except Exception:
             return type(self)(), type(self)()
 
 
+class Queue(OverloadedList):
+    """
+    Queue implementation of `OverloadedList`.
+
+    Follows first-in-first-out (fifo).
+    """
+
+    def insert(self, value: any = None) -> None:
+        """
+        Insert a single or sequence of values to the end of the Queue object.
+        """
+        type_check = (type(value) == list or type(value) == set or type(value) == OverloadedList or type(value) == OverloadedSet or type(value) == tuple)
+        if value is not None and not type_check:
+            self.append(value)
+        elif value is not None and type_check:
+            self.extend(value)
+
+    def pop(self, num: int = 1) -> None:
+        """
+        Remove the first `num: int | default: 1` elements of the Queue.
+        """
+        if num > self.len:
+            raise ValueError(
+                f"Not enough items ({num}) in <Stack> object"
+            )
+        elif num < self.len:
+            try:
+                new_queue = self._type(self[num::1])
+                self.clear()
+                self.extend(new_queue)
+            except Exception as ex:
+                raise ex
+        else:
+            ## i.e, `num` == `self.len`
+            self.clear()
+
+
+class Stack(OverloadedList):
+    """
+    Stack implementation of `OverloadedList`.
+
+    Follows first-in-last-out (filo).
+    """
+
+    def insert(self, value:any=None)->None:
+        """
+        Insert a single or sequence of values to the end of the Stack object.
+        """
+        type_check = (type(value) == list or type(value) == set or type(value) == OverloadedList or type(value) == OverloadedSet or type(value) == tuple)
+        if value is not None and not type_check:
+            self.append(value)
+        elif value is not None and type_check:
+            self.extend(value)
+
+    def pop(self, num:int=1):
+        """
+        Remove the latest `num: int | default: 1` elements from the top (highest index) of the stack
+        """
+        if num > self.len:
+            raise ValueError(
+                f"Not enough items ({num}) in <Stack> object"
+            )
+        elif num < self.len:
+            try:
+                new_stack = self._type(self[:(0-num):1])
+                self.clear()
+                self.extend(new_stack)
+            except Exception as ex:
+                raise ex
+
+        else:
+            ## i.e, `num` == `self.len`
+            self = self.clear()
+
+
 class OverloadedSet(set):
     """
     Overloaded <set> class to add additional methods.
     """
     iZERO: int = 0
     fZERO: float = 0.0
```

