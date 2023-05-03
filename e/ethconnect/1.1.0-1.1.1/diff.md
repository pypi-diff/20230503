# Comparing `tmp/ethconnect-1.1.0.tar.gz` & `tmp/ethconnect-1.1.1.tar.gz`

## Comparing `ethconnect-1.1.0.tar` & `ethconnect-1.1.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/Account.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/EllipticCurve.py
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/EthAccount.py
--rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/EthConnect.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/EthTransaction.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/Keyring.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/ZymbitEthKeyring.py
--rw-r--r--   0        0        0     3890 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/ZymbitKeyringManager.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ethconnect-1.1.0/src/ethconnect/__init__.py
--rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 ethconnect-1.1.0/tests/ABI.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ethconnect-1.1.0/tests/__init__.py
--rw-r--r--   0        0        0    17056 2020-02-02 00:00:00.000000 ethconnect-1.1.0/tests/bytecode.txt
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 ethconnect-1.1.0/tests/test_eth_account.py
--rw-r--r--   0        0        0     3856 2020-02-02 00:00:00.000000 ethconnect-1.1.0/tests/test_eth_connect.py
--rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 ethconnect-1.1.0/tests/test_zymbit_eth_keyring.py
--rw-r--r--   0        0        0     3081 2020-02-02 00:00:00.000000 ethconnect-1.1.0/tests/test_zymbit_keyring_manager.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ethconnect-1.1.0/.gitignore
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ethconnect-1.1.0/LICENSE.md
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 ethconnect-1.1.0/README.md
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ethconnect-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ethconnect-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/Account.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/EllipticCurve.py
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/EthAccount.py
+-rw-r--r--   0        0        0    11003 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/EthConnect.py
+-rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/EthTransaction.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/Keyring.py
+-rw-r--r--   0        0        0    12340 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/ZymbitEthKeyring.py
+-rw-r--r--   0        0        0     3799 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/ZymbitKeyringManager.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 ethconnect-1.1.1/src/ethconnect/__init__.py
+-rw-r--r--   0        0        0    11245 2020-02-02 00:00:00.000000 ethconnect-1.1.1/tests/ABI.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ethconnect-1.1.1/tests/__init__.py
+-rw-r--r--   0        0        0    17056 2020-02-02 00:00:00.000000 ethconnect-1.1.1/tests/bytecode.txt
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ethconnect-1.1.1/tests/test.sh
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 ethconnect-1.1.1/tests/test_eth_account.py
+-rw-r--r--   0        0        0     3823 2020-02-02 00:00:00.000000 ethconnect-1.1.1/tests/test_eth_connect.py
+-rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 ethconnect-1.1.1/tests/test_zymbit_eth_keyring.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 ethconnect-1.1.1/tests/test_zymbit_keyring_manager.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 ethconnect-1.1.1/.gitignore
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 ethconnect-1.1.1/LICENSE.md
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 ethconnect-1.1.1/README.md
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ethconnect-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 ethconnect-1.1.1/PKG-INFO
```

### Comparing `ethconnect-1.1.0/src/ethconnect/EthAccount.py` & `ethconnect-1.1.1/src/ethconnect/EthAccount.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.1.0/src/ethconnect/EthConnect.py` & `ethconnect-1.1.1/src/ethconnect/EthConnect.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.1.0/src/ethconnect/EthTransaction.py` & `ethconnect-1.1.1/src/ethconnect/EthTransaction.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.1.0/src/ethconnect/Keyring.py` & `ethconnect-1.1.1/src/ethconnect/Keyring.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,41 +5,41 @@
 import re
 
 class Keyring(ABC):
     TYPE: str
     BASE_PATH: str
     CURVE: EllipticCurve
 
-    def __init__(self, options: dict = {}) -> None:
+    def __init__(self, wallet_name: str = None, master_slot: int = None) -> None:
         if not isinstance(self.CURVE, EllipticCurve):
             raise TypeError("Invalid elliptic curve type. CURVE should be an instance of the EllipticCurve enumeration.")
         if not self._is_valid_bip44_base_path(self.BASE_PATH):
             raise TypeError("Invalid BIP44 BASE_PATH")
-        self.deserialize(options)
+        self.deserialize(wallet_name=wallet_name, master_slot=master_slot)
         if not (hasattr(self, 'wallet_name') and hasattr(self, 'master_slot')):
             raise TypeError("Subclasses of Keyring must have instance properties 'wallet_name' and 'master_slot'")
 
     @abstractmethod
     def serialize(self) -> dict:
         pass
 
     @abstractmethod
-    def deserialize(self, options: dict = {}) -> bool:
+    def deserialize(self, wallet_name: str = None, master_slot: int = None) -> bool:
         pass
 
     @abstractmethod
-    def add_account(self, index: int = 0) -> Type[Account]:
+    def add_account(self, index: int = 0) -> Account:
         pass
 
     @abstractmethod
-    def add_accounts(self, n: int = 1) -> list[Type[Account]]:
+    def add_accounts(self, n: int = 1) -> list[Account]:
         pass
 
     @abstractmethod
-    def get_accounts(self) -> list[Type[Account]]:
+    def get_accounts(self) -> list[Account]:
         pass
 
     @abstractmethod
     def remove_account(self, address: str = None, slot: int = None, path: int = None) -> bool:
         pass
 
     @staticmethod
```

### Comparing `ethconnect-1.1.0/src/ethconnect/ZymbitEthKeyring.py` & `ethconnect-1.1.1/src/ethconnect/ZymbitEthKeyring.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,43 +10,47 @@
 import re
 
 class ZymbitEthKeyring(Keyring):
     TYPE: str = "ETH"
     BASE_PATH: str = "m/44'/60'/0'/0"
     CURVE: EllipticCurve = EllipticCurve.secp256k1
 
-    def __init__(self, options: dict = {}) -> None:
-        super().__init__(options)
+    def __init__(self, wallet_name: str = None, master_slot: int = None) -> None:
+        super().__init__(wallet_name=wallet_name, master_slot=master_slot)
 
     def serialize(self) -> dict:
         serialized_keyring = {
             "wallet_name": self.wallet_name,
             "master_slot": self.master_slot,
             "type": ZymbitEthKeyring.TYPE,
+            "curve": ZymbitEthKeyring.CURVE.get_curve_type(),
             "base_path": ZymbitEthKeyring.BASE_PATH,
             "base_slot": self.base_slot,
             "accounts": [account.serialize() for account in self.accounts]
         }
         return serialized_keyring
 
-    def deserialize(self, options: dict = {}) -> bool:
-        if "wallet_name" not in options and "master_slot" not in options:
-            raise KeyError("wallet_name and master_slot properties required in options")
+    def deserialize(self, wallet_name: str = None, master_slot: int = None) -> bool:
+        if not wallet_name and not master_slot:
+            raise ValueError("wallet_name or master_slot required")
+        
+        if wallet_name and master_slot:
+            raise ValueError("Can't provide both wallet_name and master_slot")
 
-        if "wallet_name" in options:
+        if wallet_name:
             try:
-                self.master_slot: int = zymkey.client.get_wallet_key_slot('m', options["wallet_name"])
-                self.wallet_name: str = options["wallet_name"]
+                self.master_slot: int = zymkey.client.get_wallet_key_slot('m', wallet_name)
+                self.wallet_name: str = wallet_name
             except:
                 raise ValueError("Invalid wallet_name")
         else:
             try:
-                (path, wallet_name, master_slot) = zymkey.client.get_wallet_node_addr(options["master_slot"])
+                (path, wallet_name, master_slot) = zymkey.client.get_wallet_node_addr(master_slot)
                 if path == "m":
-                    self.master_slot: int = options["master_slot"]
+                    self.master_slot: int = master_slot
                     self.wallet_name: str = wallet_name
                 else:
                     raise
             except:
                 raise ValueError("Invalid master_slot")
 
         self.base_slot: int = 0
```

### Comparing `ethconnect-1.1.0/src/ethconnect/ZymbitKeyringManager.py` & `ethconnect-1.1.1/src/ethconnect/ZymbitKeyringManager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from .Keyring import Keyring
 from typing import Type
 from time import sleep
 import zymkey
 
 class ZymbitKeyringManager:
     
-    def __init__(self, keyrings: list[Type[Keyring]] = []) -> None:
+    def __init__(self, keyrings: list[Keyring] = []) -> None:
         if keyrings:
             for keyring in keyrings:
                 if not isinstance(keyring, Keyring):
                     raise TypeError(f"Invalid type: {type(keyring)}. Expected a subclass of the Keyring class")
-        self.keyrings: list[Type[Keyring]] = keyrings
+        self.keyrings: list[Keyring] = keyrings
 
     def create_keyring(self, keyring_class: Type[Keyring], wallet_name: str, master_gen_key: bytearray = bytearray()) -> tuple[int, str]:
         if not issubclass(keyring_class, Keyring):
             raise TypeError(f"Invalid type: {type(keyring_class)}. Expected a subclass of the Keyring class")
 
         if len(wallet_name) < 1 or not isinstance(wallet_name, str):
             raise ValueError("Invalid wallet_name")
@@ -25,43 +25,40 @@
         master_key_slot: int = 0
         try:
             use_bip39_recovery = zymkey.RecoveryStrategyBIP39()
             key_type: str = keyring_class.CURVE.get_curve_type()
             master_key: tuple[int, str] = zymkey.client.gen_wallet_master_seed(key_type=key_type, master_gen_key=master_gen_key, wallet_name=wallet_name, recovery_strategy=use_bip39_recovery)
             master_key_slot = master_key[0]
 
-            options = {
-                "wallet_name": wallet_name
-            }
-            keyring: keyring_class = keyring_class(options)
+            keyring: keyring_class = keyring_class(master_slot=master_key_slot)
             self.keyrings.append(keyring)
             return master_key
         except Exception as e:
             if master_key_slot:
                 zymkey.client.remove_key(master_key_slot)
 
             raise ValueError("Failed to create keyring")
         
-    def add_keyring(self, keyring: Type[Keyring]) -> bool:
+    def add_keyring(self, keyring: Keyring) -> bool:
         if not isinstance(keyring, Keyring):
             raise TypeError(f"Invalid type: {type(keyring)}. Expected a subclass of the Keyring class")
         self.keyrings.append(keyring)
         return True
           
-    def get_keyring(self, wallet_name: str = None, master_slot: int = None) -> Type[Keyring]:
+    def get_keyring(self, wallet_name: str = None, master_slot: int = None) -> Keyring:
         if not (wallet_name or master_slot):
             raise ValueError("wallet_name or master_slot are required")
         
         for keyring in self.keyrings:
             if keyring.wallet_name == wallet_name or keyring.master_slot == master_slot:
                 return keyring
             
         raise ValueError("Keyring does not exist in KeyringManager")
 
-    def get_keyrings(self) -> list[Type[Keyring]]:
+    def get_keyrings(self) -> list[Keyring]:
         return self.keyrings
     
     def remove_keyring(self, wallet_name: str = None, master_slot: int = None, remove_master: bool = False) -> bool:
         if not (wallet_name or master_slot) or (wallet_name and master_slot):
             raise ValueError("1 of wallet_name or master_slot are required")
         
         for keyring in self.keyrings:
```

### Comparing `ethconnect-1.1.0/src/ethconnect/__init__.py` & `ethconnect-1.1.1/src/ethconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `ethconnect-1.1.0/tests/ABI.json` & `ethconnect-1.1.1/tests/ABI.json`

 * *Files identical despite different names*

### Comparing `ethconnect-1.1.0/tests/bytecode.txt` & `ethconnect-1.1.1/tests/bytecode.txt`

 * *Files identical despite different names*

### Comparing `ethconnect-1.1.0/tests/test_eth_connect.py` & `ethconnect-1.1.1/tests/test_eth_connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     def setUpClass(cls):
         slots: list[int] = zymkey.client.get_slot_alloc_list()[0]
         cls.slots = list(filter(lambda slot: slot > 15, slots))
         cls.wallet_name = "test_wallet"
         use_bip39_recovery = zymkey.RecoveryStrategyBIP39()
         (master_slot, mnemonic) = zymkey.client.gen_wallet_master_seed(key_type=ZymbitEthKeyring.CURVE.get_curve_type(), master_gen_key=bytearray(), wallet_name=cls.wallet_name, recovery_strategy=use_bip39_recovery)
         cls.master_slot = master_slot
-        cls.keyring = ZymbitEthKeyring({"wallet_name": cls.wallet_name, "master_slot": master_slot})
+        cls.keyring = ZymbitEthKeyring(wallet_name=cls.wallet_name)
         cls.keyring.add_accounts(5)
 
     @classmethod
     def tearDownClass(cls):
         slots: list[int] = zymkey.client.get_slot_alloc_list()[0]
         slots = list(filter(lambda slot: slot > 15, slots))
         diff = set(slots) - set(cls.slots)
```

### Comparing `ethconnect-1.1.0/tests/test_zymbit_eth_keyring.py` & `ethconnect-1.1.1/tests/test_zymbit_eth_keyring.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,27 +13,27 @@
     def setUpClass(cls):
         slots: list[int] = zymkey.client.get_slot_alloc_list()[0]
         cls.slots = list(filter(lambda slot: slot > 15, slots))
         cls.wallet_name = "test_wallet"
         use_bip39_recovery = zymkey.RecoveryStrategyBIP39()
         (master_slot, mnemonic) = zymkey.client.gen_wallet_master_seed(key_type=ZymbitEthKeyring.CURVE.get_curve_type(), master_gen_key=bytearray(), wallet_name=cls.wallet_name, recovery_strategy=use_bip39_recovery)
         cls.master_slot = master_slot
-        cls.keyring = ZymbitEthKeyring({"wallet_name": cls.wallet_name, "master_slot": master_slot})
+        cls.keyring = ZymbitEthKeyring(master_slot=master_slot)
 
     @classmethod
     def tearDownClass(cls):
         slots: list[int] = zymkey.client.get_slot_alloc_list()[0]
         slots = list(filter(lambda slot: slot > 15, slots))
         diff = set(slots) - set(cls.slots)
         for slot in list(diff):
             zymkey.client.remove_key(slot)
         
     def test_serialize_deserialize(self):
         serialized = self.keyring.serialize()
-        keyring = ZymbitEthKeyring(serialized)
+        keyring = ZymbitEthKeyring(wallet_name=serialized['wallet_name'])
         self.assertEqual(self.keyring.TYPE, keyring.TYPE)
         self.assertEqual(self.keyring.BASE_PATH, keyring.BASE_PATH)
         self.assertEqual(self.keyring.wallet_name, keyring.wallet_name)
         self.assertEqual(self.keyring.master_slot, keyring.master_slot)
         self.assertEqual(self.keyring.base_slot, keyring.base_slot)
         self.assertEqual(len(self.keyring.accounts), len(keyring.accounts))
```

### Comparing `ethconnect-1.1.0/tests/test_zymbit_keyring_manager.py` & `ethconnect-1.1.1/tests/test_zymbit_keyring_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         self.keyring_manager.remove_keyring(wallet_name_2, remove_master=True)
 
     def test_add_and_remove_keyring(self):
         # create a new keyring and add it to the manager
         wallet_name = "test_wallet_3"
         use_bip39_recovery = zymkey.RecoveryStrategyBIP39()
         zymkey.client.gen_wallet_master_seed(key_type=ZymbitEthKeyring.CURVE.get_curve_type(), master_gen_key=bytearray(), wallet_name=wallet_name, recovery_strategy=use_bip39_recovery)
-        keyring = ZymbitEthKeyring({"wallet_name": wallet_name})
+        keyring = ZymbitEthKeyring(wallet_name=wallet_name)
         self.keyring_manager.add_keyring(keyring)
 
         # test that the keyring was added successfully
         added_keyring = self.keyring_manager.get_keyring(wallet_name)
         self.assertIsInstance(added_keyring, ZymbitEthKeyring)
         self.assertEqual(added_keyring.wallet_name, wallet_name)
```

### Comparing `ethconnect-1.1.0/LICENSE.md` & `ethconnect-1.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ethconnect-1.1.0/README.md` & `ethconnect-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,8 +6,12 @@
 
 **NOTE:** Only compatible with [HSM6](https://www.zymbit.com/hsm6/), [SCM](https://www.zymbit.com/scm/), and [SEN](https://www.zymbit.com/secure-compute-node/)
 
 ## Installation
 
 ```
 pip install ethconnect
-```
+```
+
+## Documentation:
+
+[ETH-Connect Python SDK Documentation](https://docs.zymbit.com/eth-connect/eth-connect-py/)
```

### Comparing `ethconnect-1.1.0/pyproject.toml` & `ethconnect-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ethconnect"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Shivaansh Kapoor", email="shiv@zymbit.com" },
 ]
 description = "ETH-Connect Python SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `ethconnect-1.1.0/PKG-INFO` & `ethconnect-1.1.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethconnect
-Version: 1.1.0
+Version: 1.1.1
 Summary: ETH-Connect Python SDK
 Project-URL: Homepage, https://github.com/Zymbit-Wallet/ETH-Connect-PY
 Author-email: Shivaansh Kapoor <shiv@zymbit.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -19,8 +19,12 @@
 
 **NOTE:** Only compatible with [HSM6](https://www.zymbit.com/hsm6/), [SCM](https://www.zymbit.com/scm/), and [SEN](https://www.zymbit.com/secure-compute-node/)
 
 ## Installation
 
 ```
 pip install ethconnect
-```
+```
+
+## Documentation:
+
+[ETH-Connect Python SDK Documentation](https://docs.zymbit.com/eth-connect/eth-connect-py/)
```

