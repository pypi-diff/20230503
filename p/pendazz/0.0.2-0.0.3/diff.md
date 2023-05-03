# Comparing `tmp/pendazz-0.0.2.tar.gz` & `tmp/pendazz-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pendazz-0.0.2.tar", last modified: Wed May  3 05:15:33 2023, max compression
+gzip compressed data, was "pendazz-0.0.3.tar", last modified: Wed May  3 05:27:35 2023, max compression
```

## Comparing `pendazz-0.0.2.tar` & `pendazz-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 05:15:33.741888 pendazz-0.0.2/
--rw-rw-rw-   0        0        0      269 2023-05-03 05:15:33.741888 pendazz-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-03 05:15:33.732441 pendazz-0.0.2/pendazz/
--rw-rw-rw-   0        0        0    16212 2023-05-03 05:15:07.000000 pendazz-0.0.2/pendazz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 05:15:33.739884 pendazz-0.0.2/pendazz.egg-info/
--rw-rw-rw-   0        0        0      269 2023-05-03 05:15:33.000000 pendazz-0.0.2/pendazz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-05-03 05:15:33.000000 pendazz-0.0.2/pendazz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 05:15:33.000000 pendazz-0.0.2/pendazz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-03 05:15:33.000000 pendazz-0.0.2/pendazz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 05:15:33.743885 pendazz-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      453 2023-05-03 05:12:54.000000 pendazz-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 05:27:35.910647 pendazz-0.0.3/
+-rw-rw-rw-   0        0        0      269 2023-05-03 05:27:35.910647 pendazz-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-03 05:27:35.893758 pendazz-0.0.3/pendazz/
+-rw-rw-rw-   0        0        0    18796 2023-05-03 05:26:51.000000 pendazz-0.0.3/pendazz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 05:27:35.909137 pendazz-0.0.3/pendazz.egg-info/
+-rw-rw-rw-   0        0        0      269 2023-05-03 05:27:35.000000 pendazz-0.0.3/pendazz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-05-03 05:27:35.000000 pendazz-0.0.3/pendazz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 05:27:35.000000 pendazz-0.0.3/pendazz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-03 05:27:35.000000 pendazz-0.0.3/pendazz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 05:27:35.913117 pendazz-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      453 2023-05-03 05:26:59.000000 pendazz-0.0.3/setup.py
```

### Comparing `pendazz-0.0.2/pendazz/__init__.py` & `pendazz-0.0.3/pendazz/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,91 @@
     factorial_prolog()
     boxsolver_prolog()
     list_prolog()
     sum_prolog()
     monkey_prolog()
     classification_12()
     regression_13()
+    puzzle_8()
+    '''
+
+def puzzle_8():
+    return '''
+    import copy
+
+    def get_states(state: list) -> list:
+        states = list()
+        
+        for row in range(0, len(state)):
+            for col in range(0, len(state[row])):
+                if(state[row][col] == 0):
+                    if(row==0 or row==1):
+                        tmp_state = copy.deepcopy(state)
+                        tmp_state[row][col], tmp_state[row+1][col] = tmp_state[row+1][col], tmp_state[row][col]
+                        states.append(tmp_state)
+
+                    if(row==1 or row==2):
+                        tmp_state = copy.deepcopy(state)
+                        tmp_state[row][col], tmp_state[row-1][col] = tmp_state[row-1][col], tmp_state[row][col]
+                        states.append(tmp_state)
+                    
+                    if(col==0 or col==1):
+                        tmp_state = copy.deepcopy(state)
+                        tmp_state[row][col], tmp_state[row][col+1] = tmp_state[row][col+1], tmp_state[row][col]
+                        states.append(tmp_state)
+
+                    if(col==1 or col==2):
+                        tmp_state = copy.deepcopy(state)
+                        tmp_state[row][col], tmp_state[row][col-1] = tmp_state[row][col-1], tmp_state[row][col]
+                        states.append(tmp_state)
+        return states
+
+    def get_heuristic(states: list) -> list:
+        costs={}
+        for state in states:
+            if state not in closed:
+                cost = 0
+                for row in range(0, len(state)):
+                    for col in range(0, len(state[row])):
+                        if(state[row][col] != goal[row][col]):
+                            cost = cost + 1
+                costs[cost]=state
+        lst = list(costs.items())
+        lst.sort()
+        costs = dict(lst)
+        return list(costs.values())
+
+    def ASTAR() -> None:
+        while(len(open)>0):
+            node = open.pop(0)
+            if node not in closed:
+                print(node)
+                if(node == goal):
+                    break
+                closed.append(node)
+                open[:0]= get_heuristic(get_states(node))
+
+    if __name__ == "__main__":
+        goal = [
+            [1, 2, 3],
+            [8, 0, 4],
+            [7, 6, 5]
+        ]
+        
+        puzzle = [
+            [2, 8, 1],
+            [0, 4, 3],
+            [7, 6, 5]
+        ]
+
+        open = list()
+        open.append(puzzle)
+        closed = list()
+
+        ASTAR()
     '''
 
 def classification_12():
     return '''
     data=pd.read_csv("/content/drive/MyDrive/Re_Car_Purchasing_Data.csv",encoding="ISO-8859-1")
     data.head()
```

