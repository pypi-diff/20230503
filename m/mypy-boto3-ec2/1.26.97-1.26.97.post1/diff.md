# Comparing `tmp/mypy-boto3-ec2-1.26.97.tar.gz` & `tmp/mypy-boto3-ec2-1.26.97.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-ec2-1.26.97.tar", last modified: Wed Mar 22 20:21:41 2023, max compression
+gzip compressed data, was "mypy-boto3-ec2-1.26.97.post1.tar", last modified: Thu Mar 23 01:30:37 2023, max compression
```

## Comparing `mypy-boto3-ec2-1.26.97.tar` & `mypy-boto3-ec2-1.26.97.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-22 20:21:41.795140 mypy-boto3-ec2-1.26.97/
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1070 2023-03-22 20:20:29.000000 mypy-boto3-ec2-1.26.97/LICENSE
--rw-r--r--   0 vlad      (1000) vlad      (1000)   168955 2023-03-22 20:21:41.795140 mypy-boto3-ec2-1.26.97/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)   167484 2023-03-22 20:20:29.000000 mypy-boto3-ec2-1.26.97/README.md
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-22 20:21:41.795140 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/
--rw-r--r--   0 vlad      (1000) vlad      (1000)    45547 2023-03-22 20:20:29.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/__init__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    45545 2023-03-22 20:20:29.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/__init__.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)      891 2023-03-22 20:20:29.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/__main__.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   515466 2023-03-22 20:20:35.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/client.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   514699 2023-03-22 20:20:32.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/client.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)    88156 2023-03-22 20:20:41.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/literals.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    88154 2023-03-22 20:20:40.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/literals.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   179462 2023-03-22 20:20:39.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/paginator.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   179323 2023-03-22 20:20:38.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/paginator.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)        0 2023-03-22 20:20:29.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/py.typed
--rw-r--r--   0 vlad      (1000) vlad      (1000)   269598 2023-03-22 20:20:37.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/service_resource.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   269133 2023-03-22 20:20:36.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/service_resource.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)   944025 2023-03-22 20:21:04.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/type_defs.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)   943032 2023-03-22 20:20:52.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/type_defs.pyi
--rw-r--r--   0 vlad      (1000) vlad      (1000)       61 2023-03-22 20:20:29.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/version.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    38536 2023-03-22 20:20:39.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/waiter.py
--rw-r--r--   0 vlad      (1000) vlad      (1000)    38501 2023-03-22 20:20:39.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/waiter.pyi
-drwxr-xr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-22 20:21:41.795140 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/
--rw-r--r--   0 vlad      (1000) vlad      (1000)   168955 2023-03-22 20:21:41.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/PKG-INFO
--rw-r--r--   0 vlad      (1000) vlad      (1000)      726 2023-03-22 20:21:41.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-22 20:21:41.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)        1 2023-03-22 20:21:41.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/not-zip-safe
--rw-r--r--   0 vlad      (1000) vlad      (1000)       52 2023-03-22 20:21:41.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/requires.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       15 2023-03-22 20:21:41.000000 mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/top_level.txt
--rw-r--r--   0 vlad      (1000) vlad      (1000)       38 2023-03-22 20:21:41.795140 mypy-boto3-ec2-1.26.97/setup.cfg
--rw-r--r--   0 vlad      (1000) vlad      (1000)     1957 2023-03-22 20:20:28.000000 mypy-boto3-ec2-1.26.97/setup.py
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.315125 mypy-boto3-ec2-1.26.97.post1/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1070 2023-03-23 01:29:35.000000 mypy-boto3-ec2-1.26.97.post1/LICENSE
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   168961 2023-03-23 01:30:37.311125 mypy-boto3-ec2-1.26.97.post1/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   167484 2023-03-23 01:29:35.000000 mypy-boto3-ec2-1.26.97.post1/README.md
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.311125 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    45547 2023-03-23 01:29:35.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/__init__.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    45545 2023-03-23 01:29:35.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/__init__.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      903 2023-03-23 01:29:35.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/__main__.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   515439 2023-03-23 01:29:41.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/client.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   514672 2023-03-23 01:29:38.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/client.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    88156 2023-03-23 01:29:48.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/literals.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    88154 2023-03-23 01:29:47.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/literals.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   179435 2023-03-23 01:29:45.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/paginator.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   179296 2023-03-23 01:29:44.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/paginator.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:29:35.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/py.typed
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   269571 2023-03-23 01:29:44.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/service_resource.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   269106 2023-03-23 01:29:42.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/service_resource.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   943998 2023-03-23 01:30:10.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/type_defs.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   943005 2023-03-23 01:29:59.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/type_defs.pyi
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       67 2023-03-23 01:29:35.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/version.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    38527 2023-03-23 01:29:46.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/waiter.py
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)    38492 2023-03-23 01:29:46.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/waiter.pyi
+drwxrwxr-x   0 vlad      (1000) vlad      (1000)        0 2023-03-23 01:30:37.311125 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)   168961 2023-03-23 01:30:37.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/PKG-INFO
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)      726 2023-03-23 01:30:37.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/SOURCES.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-03-23 01:30:37.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/dependency_links.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)        1 2023-03-23 01:30:37.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/not-zip-safe
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       52 2023-03-23 01:30:37.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/requires.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       15 2023-03-23 01:30:37.000000 mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/top_level.txt
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)       38 2023-03-23 01:30:37.315125 mypy-boto3-ec2-1.26.97.post1/setup.cfg
+-rw-rw-r--   0 vlad      (1000) vlad      (1000)     1963 2023-03-23 01:29:34.000000 mypy-boto3-ec2-1.26.97.post1/setup.py
```

### Comparing `mypy-boto3-ec2-1.26.97/LICENSE` & `mypy-boto3-ec2-1.26.97.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.26.97/PKG-INFO` & `mypy-boto3-ec2-1.26.97.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.26.97
-Summary: Type annotations for boto3.EC2 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.97.post1
+Summary: Type annotations for boto3.EC2 1.26.97 service generated with mypy-boto3-builder 7.14.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-1.26.97/README.md` & `mypy-boto3-ec2-1.26.97.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/__init__.py` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/__init__.pyi` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/__main__.py` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.EC2 1.26.97\nVersion:         1.26.97\nBuilder version:"
-        " 7.13.0\nDocs:           "
+        "Type annotations for boto3.EC2 1.26.97\nVersion:         1.26.97.post1\nBuilder version:"
+        " 7.14.1\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ec2.html#EC2\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.97")
+    print("1.26.97.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/client.py` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,16 @@
     from mypy_boto3_ec2.client import EC2Client
 
     session = Session()
     client: EC2Client = session.client("ec2")
     ```
 """
 import sys
-from collections.abc import Mapping, Sequence
 from datetime import datetime
-from typing import IO, Any, Dict, Type, Union, overload
+from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import (
     AccountAttributeNameType,
     AddressFamilyType,
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/client.pyi` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -10,17 +10,16 @@
     from mypy_boto3_ec2.client import EC2Client
 
     session = Session()
     client: EC2Client = session.client("ec2")
     ```
 """
 import sys
-from collections.abc import Mapping, Sequence
 from datetime import datetime
-from typing import IO, Any, Dict, Type, Union, overload
+from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
 
 from botocore.client import BaseClient, ClientMeta
 from botocore.response import StreamingBody
 
 from .literals import (
     AccountAttributeNameType,
     AddressFamilyType,
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/literals.py` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/literals.pyi` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/paginator.py` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,17 +286,16 @@
     list_images_in_recycle_bin_paginator: ListImagesInRecycleBinPaginator = client.get_paginator("list_images_in_recycle_bin")
     list_snapshots_in_recycle_bin_paginator: ListSnapshotsInRecycleBinPaginator = client.get_paginator("list_snapshots_in_recycle_bin")
     search_local_gateway_routes_paginator: SearchLocalGatewayRoutesPaginator = client.get_paginator("search_local_gateway_routes")
     search_transit_gateway_multicast_groups_paginator: SearchTransitGatewayMulticastGroupsPaginator = client.get_paginator("search_transit_gateway_multicast_groups")
     ```
 """
 import sys
-from collections.abc import Sequence
 from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ArchitectureTypeType,
     InstanceTypeType,
     IpamResourceTypeType,
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/paginator.pyi` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -286,17 +286,16 @@
     list_images_in_recycle_bin_paginator: ListImagesInRecycleBinPaginator = client.get_paginator("list_images_in_recycle_bin")
     list_snapshots_in_recycle_bin_paginator: ListSnapshotsInRecycleBinPaginator = client.get_paginator("list_snapshots_in_recycle_bin")
     search_local_gateway_routes_paginator: SearchLocalGatewayRoutesPaginator = client.get_paginator("search_local_gateway_routes")
     search_transit_gateway_multicast_groups_paginator: SearchTransitGatewayMulticastGroupsPaginator = client.get_paginator("search_transit_gateway_multicast_groups")
     ```
 """
 import sys
-from collections.abc import Sequence
 from datetime import datetime
-from typing import Generic, Iterator, TypeVar, Union
+from typing import Generic, Iterator, Sequence, TypeVar, Union
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import (
     ArchitectureTypeType,
     InstanceTypeType,
     IpamResourceTypeType,
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/service_resource.py` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/service_resource.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,16 @@
     my_volume: ec2_resources.Volume = resource.Volume(...)
     my_vpc: ec2_resources.Vpc = resource.Vpc(...)
     my_vpc_peering_connection: ec2_resources.VpcPeeringConnection = resource.VpcPeeringConnection(...)
     my_vpc_address: ec2_resources.VpcAddress = resource.VpcAddress(...)
 ```
 """
 import sys
-from collections.abc import Iterator, Sequence
 from datetime import datetime
-from typing import IO, Any, List, Union
+from typing import IO, Any, Iterator, List, Sequence, Union
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 from botocore.response import StreamingBody
 
 from .client import EC2Client
 from .literals import (
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/service_resource.pyi` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/service_resource.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,16 @@
     my_volume: ec2_resources.Volume = resource.Volume(...)
     my_vpc: ec2_resources.Vpc = resource.Vpc(...)
     my_vpc_peering_connection: ec2_resources.VpcPeeringConnection = resource.VpcPeeringConnection(...)
     my_vpc_address: ec2_resources.VpcAddress = resource.VpcAddress(...)
 ```
 """
 import sys
-from collections.abc import Iterator, Sequence
 from datetime import datetime
-from typing import IO, Any, List, Union
+from typing import IO, Any, Iterator, List, Sequence, Union
 
 from boto3.resources.base import ResourceMeta, ServiceResource
 from boto3.resources.collection import ResourceCollection
 from botocore.response import StreamingBody
 
 from .client import EC2Client
 from .literals import (
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/type_defs.py` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,16 @@
     ```python
     from mypy_boto3_ec2.type_defs import AcceleratorCountRequestTypeDef
 
     data: AcceleratorCountRequestTypeDef = {...}
     ```
 """
 import sys
-from collections.abc import Sequence
 from datetime import datetime
-from typing import IO, Any, Dict, List, Union
+from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AcceleratorManufacturerType,
     AcceleratorNameType,
     AcceleratorTypeType,
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/type_defs.pyi` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,16 @@
     ```python
     from mypy_boto3_ec2.type_defs import AcceleratorCountRequestTypeDef
 
     data: AcceleratorCountRequestTypeDef = {...}
     ```
 """
 import sys
-from collections.abc import Sequence
 from datetime import datetime
-from typing import IO, Any, Dict, List, Union
+from typing import IO, Any, Dict, List, Sequence, Union
 
 from botocore.response import StreamingBody
 
 from .literals import (
     AcceleratorManufacturerType,
     AcceleratorNameType,
     AcceleratorTypeType,
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/waiter.py` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/waiter.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
     vpc_peering_connection_deleted_waiter: VpcPeeringConnectionDeletedWaiter = client.get_waiter("vpc_peering_connection_deleted")
     vpc_peering_connection_exists_waiter: VpcPeeringConnectionExistsWaiter = client.get_waiter("vpc_peering_connection_exists")
     vpn_connection_available_waiter: VpnConnectionAvailableWaiter = client.get_waiter("vpn_connection_available")
     vpn_connection_deleted_waiter: VpnConnectionDeletedWaiter = client.get_waiter("vpn_connection_deleted")
     ```
 """
-from collections.abc import Sequence
+from typing import Sequence
 
 from botocore.waiter import Waiter
 
 from .type_defs import FilterTypeDef, WaiterConfigTypeDef
 
 __all__ = (
     "BundleTaskCompleteWaiter",
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2/waiter.pyi` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2/waiter.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     vpc_exists_waiter: VpcExistsWaiter = client.get_waiter("vpc_exists")
     vpc_peering_connection_deleted_waiter: VpcPeeringConnectionDeletedWaiter = client.get_waiter("vpc_peering_connection_deleted")
     vpc_peering_connection_exists_waiter: VpcPeeringConnectionExistsWaiter = client.get_waiter("vpc_peering_connection_exists")
     vpn_connection_available_waiter: VpnConnectionAvailableWaiter = client.get_waiter("vpn_connection_available")
     vpn_connection_deleted_waiter: VpnConnectionDeletedWaiter = client.get_waiter("vpn_connection_deleted")
     ```
 """
-from collections.abc import Sequence
+from typing import Sequence
 
 from botocore.waiter import Waiter
 
 from .type_defs import FilterTypeDef, WaiterConfigTypeDef
 
 __all__ = (
     "BundleTaskCompleteWaiter",
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/PKG-INFO` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-ec2
-Version: 1.26.97
-Summary: Type annotations for boto3.EC2 1.26.97 service generated with mypy-boto3-builder 7.13.0
+Version: 1.26.97.post1
+Summary: Type annotations for boto3.EC2 1.26.97 service generated with mypy-boto3-builder 7.14.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -47,15 +47,15 @@
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.13.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-ec2 docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_ec2/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-ec2-1.26.97/mypy_boto3_ec2.egg-info/SOURCES.txt` & `mypy-boto3-ec2-1.26.97.post1/mypy_boto3_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-ec2-1.26.97/setup.py` & `mypy-boto3-ec2-1.26.97.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-ec2",
-    version="1.26.97",
+    version="1.26.97.post1",
     packages=["mypy_boto3_ec2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.EC2 1.26.97 service generated with mypy-boto3-builder 7.13.0"
+        "Type annotations for boto3.EC2 1.26.97 service generated with mypy-boto3-builder 7.14.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
```

