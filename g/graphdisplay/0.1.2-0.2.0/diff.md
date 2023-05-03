# Comparing `tmp/graphdisplay-0.1.2.tar.gz` & `tmp/graphdisplay-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphdisplay-0.1.2.tar", last modified: Tue May  2 21:05:13 2023, max compression
+gzip compressed data, was "graphdisplay-0.2.0.tar", last modified: Wed May  3 20:23:24 2023, max compression
```

## Comparing `graphdisplay-0.1.2.tar` & `graphdisplay-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 21:05:13.439128 graphdisplay-0.1.2/
--rw-rw-rw-   0        0        0     1051 2023-05-02 21:05:13.438130 graphdisplay-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      394 2023-05-02 18:43:09.000000 graphdisplay-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 21:05:13.420178 graphdisplay-0.1.2/graphdisplay/
--rw-rw-rw-   0        0        0       34 2023-04-24 21:08:03.000000 graphdisplay-0.1.2/graphdisplay/__init__.py
--rw-rw-rw-   0        0        0     4927 2023-05-02 21:02:58.000000 graphdisplay-0.1.2/graphdisplay/graph.py
--rw-rw-rw-   0        0        0    10026 2023-05-02 21:02:40.000000 graphdisplay-0.1.2/graphdisplay/graphdisplay.py
-drwxrwxrwx   0        0        0        0 2023-05-02 21:05:13.437157 graphdisplay-0.1.2/graphdisplay.egg-info/
--rw-rw-rw-   0        0        0     1051 2023-05-02 21:05:13.000000 graphdisplay-0.1.2/graphdisplay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2023-05-02 21:05:13.000000 graphdisplay-0.1.2/graphdisplay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 21:05:13.000000 graphdisplay-0.1.2/graphdisplay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-02 21:05:13.000000 graphdisplay-0.1.2/graphdisplay.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 21:05:13.439128 graphdisplay-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1842 2023-05-02 21:02:40.000000 graphdisplay-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:23:24.628969 graphdisplay-0.2.0/
+-rw-rw-rw-   0        0        0     1051 2023-05-03 20:23:24.627970 graphdisplay-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      394 2023-05-02 18:43:09.000000 graphdisplay-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 20:23:24.614008 graphdisplay-0.2.0/graphdisplay/
+-rw-rw-rw-   0        0        0       34 2023-04-24 21:08:03.000000 graphdisplay-0.2.0/graphdisplay/__init__.py
+-rw-rw-rw-   0        0        0     5991 2023-05-03 20:21:36.000000 graphdisplay-0.2.0/graphdisplay/graph.py
+-rw-rw-rw-   0        0        0    12719 2023-05-03 20:16:02.000000 graphdisplay-0.2.0/graphdisplay/graphdisplay.py
+drwxrwxrwx   0        0        0        0 2023-05-03 20:23:24.626973 graphdisplay-0.2.0/graphdisplay.egg-info/
+-rw-rw-rw-   0        0        0     1051 2023-05-03 20:23:24.000000 graphdisplay-0.2.0/graphdisplay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2023-05-03 20:23:24.000000 graphdisplay-0.2.0/graphdisplay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 20:23:24.000000 graphdisplay-0.2.0/graphdisplay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-03 20:23:24.000000 graphdisplay-0.2.0/graphdisplay.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 20:23:24.628969 graphdisplay-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1842 2023-05-03 20:23:01.000000 graphdisplay-0.2.0/setup.py
```

### Comparing `graphdisplay-0.1.2/PKG-INFO` & `graphdisplay-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.1.2
+Version: 0.2.0
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.1.2/graphdisplay/graphdisplay.py` & `graphdisplay-0.2.0/graphdisplay/graphdisplay.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import tkinter as tk
+import json
 import math
 
 class GraphGUI:
     def __init__(self, graph, node_radius: int = 40, scr_width: int = 600, scr_height: int = 600):
         """
         Creates a GraphGUI object, which will display the graph in a external window. Nodes can be moved with the mouse.
         The creation of the window will stop the execution of the program until the window is closed. Thus, it is recommended
@@ -19,60 +20,107 @@
         if node_radius < 10 or node_radius > 100:
             raise ValueError("The parameter node_radius must be a value between 10 and 100")
         if scr_width < 200 or scr_height < 200:
             raise ValueError("The parameters scr_width and scr_height must be values greater than 200")
         if scr_width > 1000 or scr_height > 1000:
             raise ValueError("The parameters scr_width and scr_height must be values less than 1000")
 
-        self.graph = graph
+        self.__graph = graph
+        self.__node_radius = node_radius
+        self.__scr_width = scr_width
+        self.__scr_height = scr_height
+        self.nodes = []
+        self.edges = []
+
         # create the main window and start the GUI
-        root = tk.Tk()
-        root.title('GraphGUI')
-        root.resizable(False, False)
+        self.root = tk.Tk()
+        self.root.title('GraphGUI')
+        self.root.resizable(False, False)
+
+        # Closing protocol
+        self.root.protocol("WM_DELETE_WINDOW", self.__on_closing)
+
+        # Data recovery
+        data = self.__get_data()
 
         # Create the canvas
-        self.canvas = tk.Canvas(root, width=scr_width, height=scr_height)
+        self.canvas = tk.Canvas(self.root, width=scr_width, height=scr_height)
         self.canvas.pack(padx=10, pady=10)
 
+        # Reset button
+        self.reset_button = tk.Button(self.root, text="Reset", bg="#ede4cc", command=self.__display_reset)
+        self.reset_button.pack()
+
+        # Main display
+        self.__display(data)
+
+        self.canvas.tag_bind("movil", "<ButtonPress-1>", self.on_press)
+        self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
+        self.selected_node = None
+
+        self.root.mainloop()
+
+    def __display_reset(self):
+        for node in self.nodes:
+            node.terminate()
+            print("terminado!")
+        for edge in self.edges:
+            edge.terminate()
+        self.__display()
+
+    def __display(self, data: dict = None):
         # Preparation for the nodes display
-        scr_center = (scr_width//2, scr_height//2)
-        display_radius = min(scr_width, scr_height)//2 - node_radius - 10
-        arch_angle = 360/len(graph._vertices)
-        first_node_pos = (scr_center[0] - node_radius, scr_center[1] - node_radius)
+        scr_center = (self.__scr_width // 2, self.__scr_height // 2)
+        display_radius = min(self.__scr_width, self.__scr_height) // 2 - self.__node_radius - 10
+        arch_angle = 360 / len(self.__graph._vertices)
+        first_node_pos = (scr_center[0] - self.__node_radius, scr_center[1] - self.__node_radius)
 
         # Display the nodes
-        self.nodes =[]
+        self.nodes = []
         i = 0
         angle = 0
-        for vertex in self.graph._vertices:
+        for vertex in self.__graph._vertices:
             if i == 0:
-                self.nodes.append(Node(self.canvas, node_radius, first_node_pos[0], first_node_pos[1], text=str(vertex)))
+                if data and vertex in data and data[vertex][0] < self.__scr_width and data[vertex][
+                    1] < self.__scr_height:
+                    self.nodes.append(
+                        Node(self.canvas, self.__node_radius, data[vertex][0], data[vertex][1], text=str(vertex)))
+                else:
+                    self.nodes.append(
+                        Node(self.canvas, self.__node_radius, first_node_pos[0], first_node_pos[1], text=str(vertex)))
             else:
-                self.nodes.append(Node(self.canvas,
-                                       node_radius,
-                                       scr_center[0] - node_radius - display_radius*math.sin(math.radians(angle)),
-                                       scr_center[1] - node_radius - display_radius*math.cos(math.radians(angle)),
-                                       text=str(vertex)))
+                if data and vertex in data and data[vertex][0] < self.__scr_width and data[vertex][
+                    1] < self.__scr_height:
+                    self.nodes.append(
+                        Node(self.canvas, self.__node_radius, data[vertex][0], data[vertex][1], text=str(vertex)))
+                else:
+                    self.nodes.append(Node(self.canvas,
+                                           self.__node_radius,
+                                           int(scr_center[0] - self.__node_radius - display_radius * math.sin(
+                                               math.radians(angle))),
+                                           int(scr_center[1] - self.__node_radius - display_radius * math.cos(
+                                               math.radians(angle))),
+                                           text=str(vertex)))
             i += 1
             angle += arch_angle
 
         # Create the edges
         i = 0
         self.edges = []
-        for vertex in self.graph._vertices:
-            for adj in self.graph._vertices[vertex]:
+        for vertex in self.__graph._vertices:
+            for adj in self.__graph._vertices[vertex]:
                 for node in self.nodes:
                     if node.id == str(adj.vertex):
                         self.edges.append(Edge(self.canvas, self.nodes[i], node, adj.weight))
                         node.asociated_edges_IN.append(self.edges[-1])
                         self.nodes[i].asociated_edges_OUT.append(self.edges[-1])
             i += 1
 
         # Display the edges
-        if self.graph._directed:
+        if self.__graph._directed:
             for edge in self.edges:
                 edge_start_node = edge.start_node
                 edge_end_node = edge.end_node
                 found = False
                 for i in edge_start_node.asociated_edges_IN:
                     if i.start_node == edge_end_node:
                         found = True
@@ -81,22 +129,33 @@
                         break
                 if not found:
                     edge.show()
         else:
             for edge in self.edges:
                 edge.show()
 
-        self.canvas.tag_bind("movil", "<ButtonPress-1>", self.on_press)
-        self.canvas.tag_bind("movil", "<Button1-Motion>", self.move)
-        self.selected_node = None
-
-        """label =  tk.Label(self.canvas, text="Ventana de prueba", background="Red")
-        self.window = self.canvas.create_window(10,10, window=label)"""
-
-        root.mainloop()
+        # Display author
+        self.canvas.create_text(self.__scr_width - 60, 10, text="by @seniorbeto", fill="#695210",
+                                font=("Courier", 10))
+
+    def __on_closing(self):
+        data = {}
+        for node in self.nodes:
+            data[node.id] = (node.pos_x, node.pos_y)
+        with open("save.json", "w", encoding="utf-8", newline="") as file:
+            json.dump(data, file, indent=2)
+        self.root.destroy()
+
+    def __get_data(self):
+        try:
+            with open("save.json", "r", encoding="utf-8", newline="") as file:
+                data = json.load(file)
+        except FileNotFoundError:
+            data = None
+        return data
 
     def on_press(self, event):
         node = self.canvas.find_withtag(tk.CURRENT)
         self.selected_node = (node, event.x, event.y)
 
     def move(self, event):
         x, y = event.x, event.y
@@ -114,15 +173,15 @@
                     i.asociated_edges_IN.remove(edge)
                     self.canvas.delete(edge.line)
                     self.canvas.delete(edge.window)
                     del edge
                     edge = Edge(self.canvas, edge_start, i, weight, overlaped=overlaped)
                     edge.show()
                     i.asociated_edges_IN.append(edge)
-                for adj in self.graph._vertices[i.id]:
+                for adj in self.__graph._vertices[i.id]:
                     for nd in self.nodes:
                         if nd.id == str(adj.vertex):
                             for edge in nd.asociated_edges_IN:
                                 if edge.start_node == i:
                                     edge_end = edge.end_node
                                     weight = edge.weight
                                     overlaped = edge.overlaped
@@ -146,24 +205,36 @@
         self.radius = radius
         self.pos_x = posx
         self.pos_y = posy
         self.circle = canvas.create_oval(self.pos_x, self.pos_y, self.pos_x + self.radius*2, self.pos_y + self.radius*2, fill=bg, width=2)
         self.text = canvas.create_text(self.pos_x + self.radius, self.pos_y + self.radius, text=text)
         canvas.addtag_enclosed("movil", self.pos_x - 3, self.pos_y - 3, self.pos_x + self.radius * 2 + 3, self.pos_y + self.radius * 2 + 3)
 
+    def terminate(self):
+        for edge in self.asociated_edges_IN:
+            edge.terminate()
+        for edge in self.asociated_edges_OUT:
+            edge.terminate()
+        self.canvas.delete(self.circle)
+        self.canvas.delete(self.text)
+
 class Edge:
     def __init__(self, canvas: tk.Canvas, start: Node, end: Node, weight: int = 1, overlaped: bool = False):
         self.canvas = canvas
         self.overlaped = overlaped
         self.start_node = start
         self.end_node = end
         self.weight = weight
         self.start = self.__calculate_start(start, end)
         self.end = self.__calculate_end(start, end)
 
+    def terminate(self):
+        self.canvas.delete(self.line)
+        self.canvas.delete(self.window)
+
     def show(self):
         self.line = self.canvas.create_line(self.start[0], self.start[1], self.end[0], self.end[1], arrow=tk.LAST, width=1.5)
         if not self.overlaped:
             self.window = self.canvas.create_window((self.start[0] + self.end[0]) // 2, (self.start[1] + self.end[1]) // 2,
                                                window=tk.Label(self.canvas, text=str(self.weight)))
         else:
             self.window = self.canvas.create_window((self.start[0] * 0.2 + self.end[0] * 0.8),
```

### Comparing `graphdisplay-0.1.2/graphdisplay.egg-info/PKG-INFO` & `graphdisplay-0.2.0/graphdisplay.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphdisplay
-Version: 0.1.2
+Version: 0.2.0
 Summary: Librería para representar visualmente grafos de tipo diccionario
 Home-page: https://github.com/seniorbeto
 Author: Alberto Penas Díaz
 Author-email: albertopenasdiaz@gmail.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `graphdisplay-0.1.2/setup.py` & `graphdisplay-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.2' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.2.0' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'graphdisplay' #Debe coincidir con el nombre de la carpeta
 AUTHOR = 'Alberto Penas Díaz' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'albertopenasdiaz@gmail.com' #Modificar con vuestros datos
 URL = 'https://github.com/seniorbeto' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = 'Librería para representar visualmente grafos de tipo diccionario' #Descripción corta
```

