# Comparing `tmp/aptos_brownie-3.0.2-py3-none-any.whl.zip` & `tmp/aptos_brownie-3.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 7612 bytes, number of entries: 5
--rw-r--r--  2.0 unx    34213 b- defN 23-Apr-28 08:43 aptos_brownie.py
--rw-r--r--  2.0 unx      911 b- defN 23-Apr-28 09:49 aptos_brownie-3.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 09:49 aptos_brownie-3.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-28 09:49 aptos_brownie-3.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      395 b- defN 23-Apr-28 09:49 aptos_brownie-3.0.2.dist-info/RECORD
-5 files, 35625 bytes uncompressed, 6874 bytes compressed:  80.7%
+Zip file size: 7679 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    34925 b- defN 23-May-03 07:16 aptos_brownie.py
+-rw-r--r--  2.0 unx      891 b- defN 23-May-03 07:18 aptos_brownie-3.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-03 07:18 aptos_brownie-3.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-03 07:18 aptos_brownie-3.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      395 b- defN 23-May-03 07:18 aptos_brownie-3.0.3.dist-info/RECORD
+5 files, 36317 bytes uncompressed, 6941 bytes compressed:  80.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: aptos_brownie.py
 Comment: 
 
-Filename: aptos_brownie-3.0.2.dist-info/METADATA
+Filename: aptos_brownie-3.0.3.dist-info/METADATA
 Comment: 
 
-Filename: aptos_brownie-3.0.2.dist-info/WHEEL
+Filename: aptos_brownie-3.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: aptos_brownie-3.0.2.dist-info/top_level.txt
+Filename: aptos_brownie-3.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: aptos_brownie-3.0.2.dist-info/RECORD
+Filename: aptos_brownie-3.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aptos_brownie.py

```diff
@@ -514,14 +514,27 @@
                         args[i]), f"Param {function_arg} not match"
                     value = StructTag.from_str(args[i])
                 elif function_arg.type_tag == AccountAddressTag:
                     if isinstance(args[i], str):
                         value = function_arg.type_tag(AccountAddress.from_hex(args[i]))
                     else:
                         value = function_arg.type_tag(args[i])
+                elif function_arg.type_tag == VectorAccountAddressTag:
+                    value = []
+                    for j in range(len(args[i])):
+                        if isinstance(args[i][j], str):
+                            value.append(AccountAddressTag(AccountAddress.from_hex(args[i][j])))
+                        else:
+                            value.append(AccountAddressTag(args[i][j]))
+                    value = function_arg.type_tag(value)
+                elif function_arg.type_tag == VectorBoolTag:
+                    value = []
+                    for j in range(len(args[i])):
+                        value.append(args[i][j])
+                    value = function_arg.type_tag(value)
                 else:
                     assert function_arg.type_tag(
                         args[i]), f"Param {function_arg} not match"
                     value = function_arg.type_tag(args[i])
 
                 normal_args.append({
                     "value": value,
```

## Comparing `aptos_brownie-3.0.2.dist-info/METADATA` & `aptos_brownie-3.0.3.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: aptos-brownie
-Version: 3.0.2
+Version: 3.0.3
 Summary: Aptos Package Tool
 Home-page: https://github.com/OmniBTC/OmniSwap/blob/main/utils
 Author: DaiWei
 Author-email: dw1253464613@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: System :: Logging
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
@@ -20,9 +19,7 @@
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Requires-Dist: aptos-sdk
 Requires-Dist: pyyaml
 Requires-Dist: toml
 
 This is an aptos python tool to quickly implement aptos calls
-
-
```

