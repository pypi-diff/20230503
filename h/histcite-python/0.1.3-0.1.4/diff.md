# Comparing `tmp/histcite-python-0.1.3.tar.gz` & `tmp/histcite-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "histcite-python-0.1.3.tar", last modified: Mon Apr 24 10:17:09 2023, max compression
+gzip compressed data, was "histcite-python-0.1.4.tar", last modified: Wed May  3 12:18:45 2023, max compression
```

## Comparing `histcite-python-0.1.3.tar` & `histcite-python-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:17:09.505904 histcite-python-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-24 10:16:58.000000 histcite-python-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-24 10:17:09.505904 histcite-python-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6081 2023-04-24 10:16:58.000000 histcite-python-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:17:09.505904 histcite-python-0.1.3/histcite/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/parse_citation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-04-24 10:16:58.000000 histcite-python-0.1.3/histcite/process_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:17:09.505904 histcite-python-0.1.3/histcite_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-24 10:17:09.000000 histcite-python-0.1.3/histcite_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 10:17:09.505904 histcite-python-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-24 10:16:58.000000 histcite-python-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 10:17:09.505904 histcite-python-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-24 10:16:58.000000 histcite-python-0.1.3/tests/test_compute_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-24 10:16:58.000000 histcite-python-0.1.3/tests/test_network_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-04-24 10:16:58.000000 histcite-python-0.1.3/tests/test_parse_citation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:18:45.771508 histcite-python-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-03 12:18:32.000000 histcite-python-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-03 12:18:45.771508 histcite-python-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-03 12:18:32.000000 histcite-python-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:18:45.771508 histcite-python-0.1.4/histcite/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/parse_citation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-03 12:18:32.000000 histcite-python-0.1.4/histcite/process_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:18:45.771508 histcite-python-0.1.4/histcite_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 12:18:45.000000 histcite-python-0.1.4/histcite_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 12:18:45.771508 histcite-python-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 12:18:32.000000 histcite-python-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 12:18:45.771508 histcite-python-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-03 12:18:32.000000 histcite-python-0.1.4/tests/test_compute_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-03 12:18:32.000000 histcite-python-0.1.4/tests/test_network_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-05-03 12:18:32.000000 histcite-python-0.1.4/tests/test_parse_citation.py
```

### Comparing `histcite-python-0.1.3/LICENSE` & `histcite-python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.3/PKG-INFO` & `histcite-python-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -35,55 +35,56 @@
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
 - Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 
 ## 快速开始
-> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后放在某个文件夹内；    
-
+> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后不要修改文件名，放在某个文件夹内；  
 ```console
-# 需要 Python 3.8 或以上版本
+# 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
-| 简写参数 | 参数 | 说明 |
-| :-: | :-: | --- |
+|  | 参数 | 说明 |
+| :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+
 ```console
 $ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
 $ histcite -f /Users/.../downloads/dataset -n 100
 ```
 
 > 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
-对应的节点信息：
-| doc_index |      AU       |  PY  | SO                                               |  VL  |  BP  |
+对应的文献节点信息：
+
+|  |      AU       |  PY  | SO                                               |  VL  |  BP  |
 | :-------: | :-----------: | :--: | :----------------------------------------------- | :--: | :--: |
 |    31     |    Iyer R     | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |  4   | 221  |
 |    58     |    Iyer RM    | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  7   |  30  |
 |    68     |    Iver R     | 1999 | COMPUTER SPEECH AND LANGUAGE                     |  13  | 267  |
 |    77     | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  8   |  76  |
 |    82     | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |  88  | 1279 |
 |    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
-from histcite.parse_table import ParseTable
+from histcite.process_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
 process = ProcessTable(folder_path)
 process.concat_table() # 合并多个文件
```

### Comparing `histcite-python-0.1.3/README.md` & `histcite-python-0.1.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,55 +12,56 @@
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
 - Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 
 ## 快速开始
-> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后放在某个文件夹内；    
-
+> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后不要修改文件名，放在某个文件夹内；  
 ```console
-# 需要 Python 3.8 或以上版本
+# 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
-| 简写参数 | 参数 | 说明 |
-| :-: | :-: | --- |
+|  | 参数 | 说明 |
+| :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+
 ```console
 $ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
 $ histcite -f /Users/.../downloads/dataset -n 100
 ```
 
 > 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
-对应的节点信息：
-| doc_index |      AU       |  PY  | SO                                               |  VL  |  BP  |
+对应的文献节点信息：
+
+|  |      AU       |  PY  | SO                                               |  VL  |  BP  |
 | :-------: | :-----------: | :--: | :----------------------------------------------- | :--: | :--: |
 |    31     |    Iyer R     | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |  4   | 221  |
 |    58     |    Iyer RM    | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  7   |  30  |
 |    68     |    Iver R     | 1999 | COMPUTER SPEECH AND LANGUAGE                     |  13  | 267  |
 |    77     | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  8   |  76  |
 |    82     | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |  88  | 1279 |
 |    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
-from histcite.parse_table import ParseTable
+from histcite.process_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
 process = ProcessTable(folder_path)
 process.concat_table() # 合并多个文件
```

### Comparing `histcite-python-0.1.3/histcite/cli.py` & `histcite-python-0.1.4/histcite/cli.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.3/histcite/compute_metrics.py` & `histcite-python-0.1.4/histcite/compute_metrics.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,20 +9,18 @@
         self.reference_table = reference_table
 
     def __generate_table(self,use_cols:list,col:str,split_char=None)->pd.DataFrame:
         
         df = self.docs_table[use_cols]
         # 如果字段包含多个值，则进行拆分
         if split_char:
-            try:
-                df = df.dropna(subset=[col])
-                df[col] = df[col].str.split(split_char)
-            except NotImplementedError:
-                df = df.astype({col:'str'})
-                df[col] = df[col].str.split(split_char)
+            
+            df = df.dropna(subset=[col])
+            df = df.astype({col:'str'})
+            df[col] = df[col].str.split(split_char)
             df = df.explode(col)
             df = df.reset_index(drop=True)
         
         if 'LCS' in use_cols:
             grouped_df = df.groupby(col).agg({col: 'count', 'LCS': 'sum', 'TC': 'sum'})
             grouped_df = grouped_df.rename(columns={col: 'Recs', 'LCS': 'TLCS', 'TC': 'TGCS'})
         else:
```

### Comparing `histcite-python-0.1.3/histcite/network_graph.py` & `histcite-python-0.1.4/histcite/network_graph.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.3/histcite/parse_citation.py` & `histcite-python-0.1.4/histcite/parse_citation.py`

 * *Files identical despite different names*

### Comparing `histcite-python-0.1.3/histcite/process_table.py` & `histcite-python-0.1.4/histcite/process_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,63 +18,69 @@
         use_cols = ['AU','TI','SO','DT','CR','DE','C3','NR','TC','Z9','J9','PY','VL','BP','DI','UT']
         file_path = os.path.join(self.folder_path,file_name)
         df = pd.read_csv(
             file_path,sep='\t',
             header=0,
             on_bad_lines='skip',
             usecols=use_cols,
-            dtype_backend="pyarrow") # type: ignore
-                              
+            dtype_backend="pyarrow") # type: ignore                    
         return df
    
     @staticmethod
     def __extract_first_author(au_cell:str):
         """提取一作"""
         return au_cell.split(';',1)[0].replace(',','')
     
     def concat_table(self):
         """合并多个dataframe"""
-
-        docs_table = pd.concat([self._read_table(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
+        if len(self.file_name_list)>1:
+            docs_table = pd.concat([self._read_table(file_name) for file_name in self.file_name_list],ignore_index=True,copy=False)
+        elif len(self.file_name_list)==1:
+            docs_table = self._read_table(self.file_name_list[0])
+        else:
+            raise ValueError('No valid file in the folder')
+        
         # 根据入藏号删除重复数据，一般不会有重复数据
         docs_table.drop_duplicates(subset='UT',ignore_index=True,inplace=True)
 
         # 转换数据类型
         docs_table['BP'] = docs_table['BP'].apply(pd.to_numeric,errors='coerce')
         docs_table['VL'] = docs_table['VL'].apply(pd.to_numeric,errors='coerce')
         docs_table = docs_table.astype({'BP':'int64[pyarrow]', 'VL':'int64[pyarrow]'})
         
         # 提取一作
-        docs_table['AU'] = docs_table['AU'].apply(lambda x:self.__extract_first_author(x))
+        first_au = docs_table['AU'].apply(lambda x:self.__extract_first_author(x))
+        docs_table.insert(1,'first_AU',first_au)
         
         # 按照年份进行排序
         docs_table = docs_table.sort_values(by='PY',ignore_index=True)
         docs_table.insert(0,'doc_index',docs_table.index)
         self.docs_table = docs_table
         return docs_table
     
     def __generate_reference_table(self,cr_series:pd.Series):
         """生成参考文献表格"""
         parsed_cr_cells = [ParseCitation(doc_index,cell).parse_cr_cell() for doc_index,cell in cr_series.items()]
         reference_table = pd.concat([pd.DataFrame.from_dict(cell) for cell in parsed_cr_cells if cell],ignore_index=True)
         reference_table = reference_table.astype({'PY':'int64[pyarrow]', 'VL':'int64[pyarrow]', 'BP':'int64[pyarrow]'})
+        reference_table.rename(columns={'AU':'first_AU'},inplace=True)
         self.reference_table = reference_table
     
     def __recognize_reference(self,row_index,merge_startegy=False)->list:
         """识别一篇文献的本地参考文献"""
         local_ref_list = []
         child_reference_table = self.reference_table[self.reference_table['doc_index']==row_index]
             
         # 存在DOI
         child_reference_table_doi = child_reference_table[child_reference_table['DI'].notna()]['DI']
         child_docs_table_doi = self.docs_table[self.docs_table['DI'].notna()]['DI']
         local_ref_list.extend(child_docs_table_doi[child_docs_table_doi.isin(child_reference_table_doi)].index.tolist())
         
         # 不存在DOI
-        compare_cols = ['AU','PY','J9','BP']
+        compare_cols = ['first_AU','PY','J9','BP']
         child_reference_table_left = child_reference_table[child_reference_table['DI'].isna()].dropna(subset=compare_cols)
         child_reference_py = child_reference_table_left['PY']
         child_reference_bp = child_reference_table_left['BP']
 
         # 年份符合，页码符合，doi为空
         child_docs_table_left = self.docs_table[(self.docs_table['PY'].isin(child_reference_py))&(self.docs_table['BP'].isin(child_reference_bp)&self.docs_table['DI'].isna())].dropna(subset=compare_cols)
```

### Comparing `histcite-python-0.1.3/histcite_python.egg-info/PKG-INFO` & `histcite-python-0.1.4/histcite_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: histcite-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python interface to histcite.
 Home-page: https://github.com/doublessay/histcite-python
 Author: WangK2
 Author-email: kw221225@gmail.com
 License: MIT
 Keywords: histcite,web of science,citation network
 Classifier: Intended Audience :: Developers
@@ -35,55 +35,56 @@
 - `GCR`, Global Cited References，表示一篇文献所有参考文献的数量；
 - `LCR`, Local Cited References，表示一篇文献所有本地参考文献的数量；
 - `T*`, Total，表示给定作者、机构、期刊等相应分数之和。例如`TLCS` = 总本地引文分数；
 - `Recs`， 记录数；
 - Web of science题录数据 [字段说明](https://images.webofknowledge.com/WOKRS5132R4.2/help/zh_CN/WOS/hs_wos_fieldtags.html)；
 
 ## 快速开始
-> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后放在某个文件夹内；    
-
+> 适用于本工具的数据集，来源Web of Science核心合集，<b> Tab delimited file/制表符分隔文件</b> 格式，导出内容选择 <b>Full Record and Cited References/全记录与引用的参考文献</b> 或者是 <b>Custome selection/自定义选择项</b>，全选字段，下载之后不要修改文件名，放在某个文件夹内；  
 ```console
-# 需要 Python 3.8 或以上版本
+# 需要 Python3.8 或以上版本
 pip install histcite-python
 ```
 
 ## 使用方法
 1、使用命令行工具，可用参数如下：
-| 简写参数 | 参数 | 说明 |
-| :-: | :-: | --- |
+|  | 参数 | 说明 |
+| :---: | :---: | --- |
 | -f | --folder_path | 下载的题录数据存放的文件夹路径，必须指定 |
 | -n | --node_num | 引文网络图中包含的节点数量，默认为 `50`，即 `LCS` 最高的 `50` 篇文献 |
 | -g | --graph | 是否仅生成图文件，指定该参数表示 `True`, 无需传值 |
+
 ```console
 $ 假设下载的wos文件夹路径为 /Users/.../downloads/dataset，引文网络图包含的节点数设置为 100
 $ histcite -f /Users/.../downloads/dataset -n 100
 ```
 
 > 结果保存在指定的 `folder_path` 下的 `result` 文件夹内，包含 `statistics.xlsx`, `graph.node.xlsx`, `graph.dot` 三个文件，第一个是描述统计表，第二个是引文网络图节点信息表，最后一个为引文网络图的数据文件，可以使用 [Graphviz在线编辑器](http://magjac.com/graphviz-visual-editor/) 或本地的 [Graphviz工具](https://graphviz.org/) 生成引文网络图。具体文件内容可以参考 [examples文件夹](examples)。 
 
 生成的引文网络图：
 
 <img src="examples/graph.svg">
 
-对应的节点信息：
-| doc_index |      AU       |  PY  | SO                                               |  VL  |  BP  |
+对应的文献节点信息：
+
+|  |      AU       |  PY  | SO                                               |  VL  |  BP  |
 | :-------: | :-----------: | :--: | :----------------------------------------------- | :--: | :--: |
 |    31     |    Iyer R     | 1997 | IEEE SIGNAL PROCESSING LETTERS                   |  4   | 221  |
 |    58     |    Iyer RM    | 1999 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  7   |  30  |
 |    68     |    Iver R     | 1999 | COMPUTER SPEECH AND LANGUAGE                     |  13  | 267  |
 |    77     | Bellegarda JR | 2000 | IEEE TRANSACTIONS ON SPEECH AND AUDIO PROCESSING |  8   |  76  |
 |    82     | Bellegarda JR | 2000 | PROCEEDINGS OF THE IEEE                          |  88  | 1279 |
 |    ...    |               |      |                                                  |      |      |
 
 2、函数调用，相比命令行工具，函数调用更加灵活，可以自定义更多参数，参考 [demo.ipynb](demo.ipynb)
 
 ```python
 import os
 import pandas as pd
-from histcite.parse_table import ParseTable
+from histcite.process_table import ParseTable
 from histcite.compute_metrics import ComputeMetrics
 from histcite.network_graph import Graphviz
 
 # 读取数据，解析引文
 folder_path = '/Users/.../downloads/dataset' # 下载的题录数据存放的文件夹路径
 process = ProcessTable(folder_path)
 process.concat_table() # 合并多个文件
```

### Comparing `histcite-python-0.1.3/setup.py` & `histcite-python-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 setup(
     name="histcite-python",
     author = "WangK2",
     author_email = "kw221225@gmail.com",
-    version="0.1.3",
+    version="0.1.4",
     description="A Python interface to histcite.",
     long_description = open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords = ["histcite","web of science","citation network"],
     license="MIT",
     url="https://github.com/doublessay/histcite-python",
     packages=["histcite"],
```

### Comparing `histcite-python-0.1.3/tests/test_parse_citation.py` & `histcite-python-0.1.4/tests/test_parse_citation.py`

 * *Files identical despite different names*

