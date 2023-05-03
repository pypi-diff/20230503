# Comparing `tmp/algokit_utils-1.1.0b5-py3-none-any.whl.zip` & `tmp/algokit_utils-1.1.1b1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 33635 bytes, number of entries: 15
+Zip file size: 33780 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     3697 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    53906 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
--rw-r--r--  2.0 unx    32431 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
+-rw-r--r--  2.0 unx    32559 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     1981 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
--rw-r--r--  2.0 unx     3930 b- defN 80-Jan-01 00:00 algokit_utils/models.py
+-rw-r--r--  2.0 unx     4309 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.1.0b5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.1.0b5.dist-info/RECORD
-15 files, 128059 bytes uncompressed, 31543 bytes compressed:  75.4%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.1.1b1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.1.1b1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.1.1b1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.1.1b1.dist-info/RECORD
+15 files, 128566 bytes uncompressed, 31688 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.1.0b5.dist-info/LICENSE
+Filename: algokit_utils-1.1.1b1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.1.0b5.dist-info/METADATA
+Filename: algokit_utils-1.1.1b1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.1.0b5.dist-info/WHEEL
+Filename: algokit_utils-1.1.1b1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.1.0b5.dist-info/RECORD
+Filename: algokit_utils-1.1.1b1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/deploy.py

```diff
@@ -704,26 +704,28 @@
         )
         self.app_client.compose_create(
             atc,
             create_method,
             create_parameters,
             **create_abi_args,
         )
+        create_txn_index = len(atc.txn_list) - 1
         delete_method, delete_abi_args, delete_parameters = _convert_deploy_args(
             self.delete_args, self.new_app_metadata, self.signer, self.sender
         )
         self.app_client.compose_delete(
             atc,
             delete_method,
             delete_parameters,
             **delete_abi_args,
         )
+        delete_txn_index = len(atc.txn_list) - 1
         create_delete_response = self.app_client.execute_atc(atc)
-        create_response = TransactionResponse.from_atr(create_delete_response, 0)
-        delete_response = TransactionResponse.from_atr(create_delete_response, 1)
+        create_response = TransactionResponse.from_atr(create_delete_response, create_txn_index)
+        delete_response = TransactionResponse.from_atr(create_delete_response, delete_txn_index)
         self.app_client.app_id = get_app_id_from_tx_id(self.app_client.algod_client, create_response.tx_id)
         logger.info(
             f"{self.new_app_metadata.name} ({self.new_app_metadata.version}) deployed successfully, "
             f"with app id {self.app_client.app_id}."
         )
         logger.info(
             f"{self.existing_app_metadata_or_reference.name} "
```

## algokit_utils/models.py

```diff
@@ -21,15 +21,20 @@
 
     tx_id: str
     """Transaction Id"""
     confirmed_round: int | None
     """Round transaction was confirmed, `None` if call was a from a dry-run"""
 
     @staticmethod
-    def from_atr(result: AtomicTransactionResponse, transaction_index: int = 0) -> "TransactionResponse":
+    def from_atr(result: AtomicTransactionResponse, transaction_index: int = -1) -> "TransactionResponse":
+        """Returns either an ABITransactionResponse or a TransactionResponse based on the type of the transaction
+        referred to by transaction_index
+        :param AtomicTransactionResponse result: Result containing one or more transactions
+        :param int transaction_index: Which transaction in the result to return, defaults to -1 (the last transaction)
+        """
         tx_id = result.tx_ids[transaction_index]
         abi_result = next((r for r in result.abi_results if r.tx_id == tx_id), None)
         if abi_result:
             return ABITransactionResponse(
                 tx_id=tx_id,
                 raw_value=abi_result.raw_value,
                 return_value=abi_result.return_value,
```

## Comparing `algokit_utils-1.1.0b5.dist-info/LICENSE` & `algokit_utils-1.1.1b1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.1.0b5.dist-info/METADATA` & `algokit_utils-1.1.1b1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.1.0b5
+Version: 1.1.1b1
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.1.0b5.dist-info/RECORD` & `algokit_utils-1.1.1b1.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 algokit_utils/__init__.py,sha256=XFpWqRXQgnT9JCh6ZOlI2strJgbaZeaykfM2JZgBz9E,3697
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=3oON9YJ-fU3rFhxacSPNxrpmnHUgG349oMH_Id9NdIA,53906
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
-algokit_utils/deploy.py,sha256=Qdlfos3AcgkxoS69cx3TzTf210nn3dssKWwEjb_vJok,32431
+algokit_utils/deploy.py,sha256=qJDgrHpoZMZA0upQ8QnriO62b5OnRkJHBULpRdQ4khc,32559
 algokit_utils/logic_error.py,sha256=ypu2DSyus-Kjy51_1oE8T3LHVhRSOrc21Gpbau_WjAc,1981
-algokit_utils/models.py,sha256=46vPWFNMowMyNOhmlInq58gVtOg91xgPhQ0w-bIMacw,3930
+algokit_utils/models.py,sha256=_0vVN1qW1VxyqjkhuxLpxcrOfVtw2LtCcOeQXJSv-4A,4309
 algokit_utils/network_clients.py,sha256=0cbUHCEWycFnduEu5cJ4dY6pfDOOzvHO1cXmcxAe83M,4841
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.1.0b5.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.1.0b5.dist-info/METADATA,sha256=6qnF1yeiIqemWiqhQvI0ZVWCPuKdBpSWBX-B_6xSxoc,2037
-algokit_utils-1.1.0b5.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.1.0b5.dist-info/RECORD,,
+algokit_utils-1.1.1b1.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.1.1b1.dist-info/METADATA,sha256=KUDTOD_b7RvUJ2xNXZW8DuhqRhntSmoL1GLXAQuGrII,2037
+algokit_utils-1.1.1b1.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+algokit_utils-1.1.1b1.dist-info/RECORD,,
```

