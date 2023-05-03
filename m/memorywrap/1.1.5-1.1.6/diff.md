# Comparing `tmp/memorywrap-1.1.5.tar.gz` & `tmp/memorywrap-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memorywrap-1.1.5.tar", last modified: Fri Aug  5 14:02:44 2022, max compression
+gzip compressed data, was "memorywrap-1.1.6.tar", last modified: Wed May  3 18:15:24 2023, max compression
```

## Comparing `memorywrap-1.1.5.tar` & `memorywrap-1.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 14:02:44.859807 memorywrap-1.1.5/
--rw-r--r--   0 root         (0) root         (0)     3798 2022-08-05 14:02:44.859807 memorywrap-1.1.5/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     3373 2022-08-05 13:55:05.000000 memorywrap-1.1.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 14:02:44.859807 memorywrap-1.1.5/memorywrap/
--rwxrwxrwx   0 root         (0) root         (0)       91 2021-06-05 20:50:47.000000 memorywrap-1.1.5/memorywrap/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7248 2022-07-14 21:08:12.000000 memorywrap-1.1.5/memorywrap/memory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-05 14:02:44.859807 memorywrap-1.1.5/memorywrap.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)     3798 2022-08-05 14:02:44.000000 memorywrap-1.1.5/memorywrap.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      241 2022-08-05 14:02:44.000000 memorywrap-1.1.5/memorywrap.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2022-08-05 14:02:44.000000 memorywrap-1.1.5/memorywrap.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       17 2022-08-05 14:02:44.000000 memorywrap-1.1.5/memorywrap.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       11 2022-08-05 14:02:44.000000 memorywrap-1.1.5/memorywrap.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2022-08-05 14:02:44.859807 memorywrap-1.1.5/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      672 2022-08-05 14:02:21.000000 memorywrap-1.1.5/setup.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2023-05-03 18:15:24.571350 memorywrap-1.1.6/
+-rw-r--r--   0 mattia    (1000) mattia    (1000)     3742 2023-05-03 18:15:24.571350 memorywrap-1.1.6/PKG-INFO
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)     3373 2022-08-05 13:55:05.000000 memorywrap-1.1.6/README.md
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2023-05-03 18:15:24.568017 memorywrap-1.1.6/memorywrap/
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)       91 2021-06-05 20:50:47.000000 memorywrap-1.1.6/memorywrap/__init__.py
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)     6890 2023-05-03 18:02:47.000000 memorywrap-1.1.6/memorywrap/memory.py
+drwxr-xr-x   0 mattia    (1000) mattia    (1000)        0 2023-05-03 18:15:24.571350 memorywrap-1.1.6/memorywrap.egg-info/
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)     3742 2023-05-03 18:15:24.000000 memorywrap-1.1.6/memorywrap.egg-info/PKG-INFO
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)      241 2023-05-03 18:15:24.000000 memorywrap-1.1.6/memorywrap.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)        1 2023-05-03 18:15:24.000000 memorywrap-1.1.6/memorywrap.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)       17 2023-05-03 18:15:24.000000 memorywrap-1.1.6/memorywrap.egg-info/requires.txt
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)       11 2023-05-03 18:15:24.000000 memorywrap-1.1.6/memorywrap.egg-info/top_level.txt
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)       38 2023-05-03 18:15:24.571350 memorywrap-1.1.6/setup.cfg
+-rwxrwxrwx   0 mattia    (1000) mattia    (1000)      672 2023-05-03 18:03:24.000000 memorywrap-1.1.6/setup.py
```

### Comparing `memorywrap-1.1.5/PKG-INFO` & `memorywrap-1.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: memorywrap
-Version: 1.1.5
+Version: 1.1.6
 Summary: Memory Wrap: an extension for image classification models
-Home-page: UNKNOWN
 Author: La Rosa Biagio
 Author-email: larosa@diag.uniroma1.it
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Description
 Memory Wrap is an extension to image classification models that improves both data-efficiency and model interpretability, adopting a sparse content-attention mechanism between the input and some memories of past training samples.
@@ -50,9 +47,7 @@
 The last argument of the Memory Wrap's call function is a boolean flag controlling the number of outputs returned. If the flag is True, then the layer returns both the output and the sparse attention weight associated to each memory sample; if the flag is False, then the layer return only the output.
 
 # Additional information
 Here you can find link to additional source of information about Memory Wrap:
 - <a href="https://trebuchet.public.springernature.app/get_content/809bb246-b0f1-4f37-b640-270d7413ebdc">Paper</a>
 - <a href="https://github.com/KRLGroup/memory-wrap">GitHub repo</a>
 - <a href="https://colab.research.google.com/drive/1OPjcpTH7X8EV1ev361iuhVzd2Jfp9kFA">Jupyter notebook</a>
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,37 @@
-Metadata-Version: 2.1 Name: memorywrap Version: 1.1.5 Summary: Memory Wrap: an
-extension for image classification models Home-page: UNKNOWN Author: La Rosa
-Biagio Author-email: larosa@diag.uniroma1.it License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown # Description Memory Wrap is an
-extension to image classification models that improves both data-efficiency and
-model interpretability, adopting a sparse content-attention mechanism between
-the input and some memories of past training samples. # Installation This is a
-PyTorch implementation of Memory Wrap. To install Memory Wrap run the following
-command: ``` pip install memorywrap ``` The library contains two main classes:
-- *MemoryWrapLayer*: it is the Memory Wrap variant described in the paper that
-uses both the input encoding and the memory encoding to compute the output; -
-*BaselineMemory*: it is the baseline that uses only the memory encoding to
-compute the output. # Usage ## Instantiate the layer ```python memorywrap =
-MemoryWrapLayer(encoder_output_dim, output_dim, head=None, classifier=None,
-distance='cosine') ``` or, for the baseline that uses only the memory to output
-the prediction: ```python memorywrap = BaselineMemory(encoder_output_dim,
-output_dim, head=None, classifier=None, distance='cosine') ``` where -
-*encoder_output_dim* (int) is the output dimension of the last layer of the
-encoder - *output_dim* (int) is the desired output dimensione. In the case of
-the paper *output_dim* is equal to the **number of classes**; - *head*
-(torch.nn.Module): Read head used to project the key and query. It can be a
-linear or non-linear layer. Input dimensions must be equal to
-encoder_output_dim (in this case 1280). If None, it is fixed as a linear layer
-with input and output dimension equal to the input dimension of MemoryWrap
-(encoder_output_dim). (See https://www.nature.com/articles/nature20101 for
-further information) - classifier (torch.nn.Module): Classifier on top of
-MemoryWrap. Inputs dimensions must be equal at encoder_output_dim\*2 for
-MemoryWrapLayer and encoder_output_dim for BaselineMemory. By default is an MLP
-as described in the paper. An alternative is to use a linear layer. (e.g.
+Metadata-Version: 2.1 Name: memorywrap Version: 1.1.6 Summary: Memory Wrap: an
+extension for image classification models Author: La Rosa Biagio Author-email:
+larosa@diag.uniroma1.it Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Description-Content-Type: text/markdown # Description Memory
+Wrap is an extension to image classification models that improves both data-
+efficiency and model interpretability, adopting a sparse content-attention
+mechanism between the input and some memories of past training samples. #
+Installation This is a PyTorch implementation of Memory Wrap. To install Memory
+Wrap run the following command: ``` pip install memorywrap ``` The library
+contains two main classes: - *MemoryWrapLayer*: it is the Memory Wrap variant
+described in the paper that uses both the input encoding and the memory
+encoding to compute the output; - *BaselineMemory*: it is the baseline that
+uses only the memory encoding to compute the output. # Usage ## Instantiate the
+layer ```python memorywrap = MemoryWrapLayer(encoder_output_dim, output_dim,
+head=None, classifier=None, distance='cosine') ``` or, for the baseline that
+uses only the memory to output the prediction: ```python memorywrap =
+BaselineMemory(encoder_output_dim, output_dim, head=None, classifier=None,
+distance='cosine') ``` where - *encoder_output_dim* (int) is the output
+dimension of the last layer of the encoder - *output_dim* (int) is the desired
+output dimensione. In the case of the paper *output_dim* is equal to the
+**number of classes**; - *head* (torch.nn.Module): Read head used to project
+the key and query. It can be a linear or non-linear layer. Input dimensions
+must be equal to encoder_output_dim (in this case 1280). If None, it is fixed
+as a linear layer with input and output dimension equal to the input dimension
+of MemoryWrap(encoder_output_dim). (See https://www.nature.com/articles/
+nature20101 for further information) - classifier (torch.nn.Module): Classifier
+on top of MemoryWrap. Inputs dimensions must be equal at encoder_output_dim\*2
+for MemoryWrapLayer and encoder_output_dim for BaselineMemory. By default is an
+MLP as described in the paper. An alternative is to use a linear layer. (e.g.
 torch.nn.Linear(encoder_output_dim\*2, output_dim). Default:
 torch.nn.Sequential( torch.nn.Linear(encoder_output_dim*2,
 encoder_output_dim\*4), torch.nn.ReLU(), torch.nn.Linear(encoder_output_dim\*4,
 output_dim) - distance (str): Distance to use to compute the similarity between
 input and memory set. Allowed values are: cosine, l2 and dot for respectively
 cosine similarity, l2 distance and dot product distance. Default=cosine ##
 Forward call Add the forward call to your forward function. ```python
```

### Comparing `memorywrap-1.1.5/README.md` & `memorywrap-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `memorywrap-1.1.5/memorywrap/memory.py` & `memorywrap-1.1.6/memorywrap/memory.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,22 +67,21 @@
         relu = self.relu(hidden)
         output = self.fc2(relu)
         return output
 
 
 class MemoryWrapLayer(nn.Module):
 
-    def __init__(self, encoder_output_dim:int, output_dim:int, head: torch.nn.Module=None, classifier:torch.nn.Module=None,distance:str='cosine'):
+    def __init__(self, encoder_output_dim:int, output_dim:int, classifier:torch.nn.Module=None,distance:str='cosine'):
         """ Initialize a Memory Wrap layer
 
         Args:
             encoder_output_dim (int): Dimensions of the last layer of the encoder
             output_dim (int): Number of desired output units.
-            head (torch.nn.Module, optional): Module to use as read head. Input dimensions must be equal to encoder_output_dim. Default: torch.nn.Linear.
-            classifier (torch.nn.Module, optional): Module to use as classifier head. Input dimensions must be equal to output dimensions*2 of the read head. Default: Multi-layer perceptron of dimensions [encoder_output_dim*2,encoder_output_dim*4,output_dim]
+            classifier (torch.nn.Module, optional): Module to use as classifier. Input dimensions must be equal to output dimensions*2 of the last layer of the encoder. Default: Multi-layer perceptron of dimensions [encoder_output_dim*2,encoder_output_dim*4,output_dim]
         """
         super(MemoryWrapLayer, self).__init__()
 
         self.distance_name = distance
 
         self.classifier = classifier or MLP(encoder_output_dim*2, encoder_output_dim*4, output_dim)
     
@@ -119,26 +118,24 @@
         else: 
             return output
 
 
 
 class BaselineMemory(nn.Module):
 
-    def __init__(self, encoder_output_dim:int, output_dim:int,head: torch.nn.Module=None, classifier:torch.nn.Module=None,distance:str='cosine'):
+    def __init__(self, encoder_output_dim:int, output_dim:int, classifier:torch.nn.Module=None,distance:str='cosine'):
         """ Initialize the layer opf the baseline that uses only the memory set to compute the output
 
         Args:
             encoder_output_dim (int): Dimensions of the last layer of the encoder
             output_dim (int): Number of desired output units.
-            head (torch.nn.Module, optional): Module to use as read head. Input dimensions must be equal to encoder_output_dim. Default: torch.nn.Linear.
-            classifier (torch.nn.Module, optional): Module to use as classifier head. Input dimensions must be equal to output dimensions of the read head. Default: Multi-layer perceptron of dimensions [encoder_output_dim,encoder_output_dim*2,output_dim]
+            classifier (torch.nn.Module, optional): Module to use as a classifier. Input dimensions must be equal to output dimensions of the last layer of the encoder. Default: Multi-layer perceptron of dimensions [encoder_output_dim,encoder_output_dim*2,output_dim]
         """
         super(BaselineMemory, self).__init__()
 
-        # Red Head
         self.distance = distance
         self.classifier = classifier or MLP(encoder_output_dim, encoder_output_dim*2, output_dim)
         
     def forward(self, encoder_output:torch.Tensor, memory_set:torch.Tensor, return_weights:bool=False)->torch.Tensor:
         """Forward call of MemoryWrap.
         Args:
             input: A tensor of dimensions [b,dim] where dim is the dimension required by the encoder
```

### Comparing `memorywrap-1.1.5/memorywrap.egg-info/PKG-INFO` & `memorywrap-1.1.6/memorywrap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 Metadata-Version: 2.1
 Name: memorywrap
-Version: 1.1.5
+Version: 1.1.6
 Summary: Memory Wrap: an extension for image classification models
-Home-page: UNKNOWN
 Author: La Rosa Biagio
 Author-email: larosa@diag.uniroma1.it
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
 # Description
 Memory Wrap is an extension to image classification models that improves both data-efficiency and model interpretability, adopting a sparse content-attention mechanism between the input and some memories of past training samples.
@@ -50,9 +47,7 @@
 The last argument of the Memory Wrap's call function is a boolean flag controlling the number of outputs returned. If the flag is True, then the layer returns both the output and the sparse attention weight associated to each memory sample; if the flag is False, then the layer return only the output.
 
 # Additional information
 Here you can find link to additional source of information about Memory Wrap:
 - <a href="https://trebuchet.public.springernature.app/get_content/809bb246-b0f1-4f37-b640-270d7413ebdc">Paper</a>
 - <a href="https://github.com/KRLGroup/memory-wrap">GitHub repo</a>
 - <a href="https://colab.research.google.com/drive/1OPjcpTH7X8EV1ev361iuhVzd2Jfp9kFA">Jupyter notebook</a>
-
-
```

#### html2text {}

```diff
@@ -1,38 +1,37 @@
-Metadata-Version: 2.1 Name: memorywrap Version: 1.1.5 Summary: Memory Wrap: an
-extension for image classification models Home-page: UNKNOWN Author: La Rosa
-Biagio Author-email: larosa@diag.uniroma1.it License: UNKNOWN Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown # Description Memory Wrap is an
-extension to image classification models that improves both data-efficiency and
-model interpretability, adopting a sparse content-attention mechanism between
-the input and some memories of past training samples. # Installation This is a
-PyTorch implementation of Memory Wrap. To install Memory Wrap run the following
-command: ``` pip install memorywrap ``` The library contains two main classes:
-- *MemoryWrapLayer*: it is the Memory Wrap variant described in the paper that
-uses both the input encoding and the memory encoding to compute the output; -
-*BaselineMemory*: it is the baseline that uses only the memory encoding to
-compute the output. # Usage ## Instantiate the layer ```python memorywrap =
-MemoryWrapLayer(encoder_output_dim, output_dim, head=None, classifier=None,
-distance='cosine') ``` or, for the baseline that uses only the memory to output
-the prediction: ```python memorywrap = BaselineMemory(encoder_output_dim,
-output_dim, head=None, classifier=None, distance='cosine') ``` where -
-*encoder_output_dim* (int) is the output dimension of the last layer of the
-encoder - *output_dim* (int) is the desired output dimensione. In the case of
-the paper *output_dim* is equal to the **number of classes**; - *head*
-(torch.nn.Module): Read head used to project the key and query. It can be a
-linear or non-linear layer. Input dimensions must be equal to
-encoder_output_dim (in this case 1280). If None, it is fixed as a linear layer
-with input and output dimension equal to the input dimension of MemoryWrap
-(encoder_output_dim). (See https://www.nature.com/articles/nature20101 for
-further information) - classifier (torch.nn.Module): Classifier on top of
-MemoryWrap. Inputs dimensions must be equal at encoder_output_dim\*2 for
-MemoryWrapLayer and encoder_output_dim for BaselineMemory. By default is an MLP
-as described in the paper. An alternative is to use a linear layer. (e.g.
+Metadata-Version: 2.1 Name: memorywrap Version: 1.1.6 Summary: Memory Wrap: an
+extension for image classification models Author: La Rosa Biagio Author-email:
+larosa@diag.uniroma1.it Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Description-Content-Type: text/markdown # Description Memory
+Wrap is an extension to image classification models that improves both data-
+efficiency and model interpretability, adopting a sparse content-attention
+mechanism between the input and some memories of past training samples. #
+Installation This is a PyTorch implementation of Memory Wrap. To install Memory
+Wrap run the following command: ``` pip install memorywrap ``` The library
+contains two main classes: - *MemoryWrapLayer*: it is the Memory Wrap variant
+described in the paper that uses both the input encoding and the memory
+encoding to compute the output; - *BaselineMemory*: it is the baseline that
+uses only the memory encoding to compute the output. # Usage ## Instantiate the
+layer ```python memorywrap = MemoryWrapLayer(encoder_output_dim, output_dim,
+head=None, classifier=None, distance='cosine') ``` or, for the baseline that
+uses only the memory to output the prediction: ```python memorywrap =
+BaselineMemory(encoder_output_dim, output_dim, head=None, classifier=None,
+distance='cosine') ``` where - *encoder_output_dim* (int) is the output
+dimension of the last layer of the encoder - *output_dim* (int) is the desired
+output dimensione. In the case of the paper *output_dim* is equal to the
+**number of classes**; - *head* (torch.nn.Module): Read head used to project
+the key and query. It can be a linear or non-linear layer. Input dimensions
+must be equal to encoder_output_dim (in this case 1280). If None, it is fixed
+as a linear layer with input and output dimension equal to the input dimension
+of MemoryWrap(encoder_output_dim). (See https://www.nature.com/articles/
+nature20101 for further information) - classifier (torch.nn.Module): Classifier
+on top of MemoryWrap. Inputs dimensions must be equal at encoder_output_dim\*2
+for MemoryWrapLayer and encoder_output_dim for BaselineMemory. By default is an
+MLP as described in the paper. An alternative is to use a linear layer. (e.g.
 torch.nn.Linear(encoder_output_dim\*2, output_dim). Default:
 torch.nn.Sequential( torch.nn.Linear(encoder_output_dim*2,
 encoder_output_dim\*4), torch.nn.ReLU(), torch.nn.Linear(encoder_output_dim\*4,
 output_dim) - distance (str): Distance to use to compute the similarity between
 input and memory set. Allowed values are: cosine, l2 and dot for respectively
 cosine similarity, l2 distance and dot product distance. Default=cosine ##
 Forward call Add the forward call to your forward function. ```python
```

### Comparing `memorywrap-1.1.5/setup.py` & `memorywrap-1.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="memorywrap",
-    version="1.1.5",
+    version="1.1.6",
     author="La Rosa Biagio",
     author_email="larosa@diag.uniroma1.it",
     description="Memory Wrap: an extension for image classification models",
     install_requires=[
           'entmax',
           'torch>1.5'
       ],
```

