# Comparing `tmp/xjet-0.1.1.tar.gz` & `tmp/xjet-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xjet-0.1.1.tar", max compression
+gzip compressed data, was "xjet-0.1.2.tar", max compression
```

## Comparing `xjet-0.1.1.tar` & `xjet-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-01-15 16:26:30.059724 xjet-0.1.1/LICENSE
--rw-r--r--   0        0        0     1143 2023-01-15 16:26:30.059812 xjet-0.1.1/README.md
--rw-r--r--   0        0        0      798 2023-01-29 08:52:16.538115 xjet-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1909 2023-01-29 08:53:55.423251 xjet-0.1.1/xjet/__init__.py
--rw-r--r--   0        0        0     4975 2023-01-15 17:04:08.533858 xjet-0.1.1/xjet/api.py
--rw-r--r--   0        0        0      256 2023-01-15 16:42:40.104778 xjet-0.1.1/xjet/constants.py
--rw-r--r--   0        0        0     1228 2023-01-15 16:42:40.142189 xjet-0.1.1/xjet/sync.py
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 xjet-0.1.1/setup.py
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 xjet-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-01-15 16:26:30.059724 xjet-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1296 2023-05-03 09:38:23.542817 xjet-0.1.2/README.md
+-rw-r--r--   0        0        0      798 2023-05-03 09:36:57.069787 xjet-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1918 2023-05-03 09:23:09.871940 xjet-0.1.2/xjet/__init__.py
+-rw-r--r--   0        0        0     5738 2023-05-03 10:45:04.960289 xjet-0.1.2/xjet/api.py
+-rw-r--r--   0        0        0      256 2023-01-15 16:42:40.104778 xjet-0.1.2/xjet/constants.py
+-rw-r--r--   0        0        0     1228 2023-01-15 16:42:40.142189 xjet-0.1.2/xjet/sync.py
+-rw-r--r--   0        0        0     1996 1970-01-01 00:00:00.000000 xjet-0.1.2/setup.py
+-rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 xjet-0.1.2/PKG-INFO
```

### Comparing `xjet-0.1.1/LICENSE` & `xjet-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xjet-0.1.1/README.md` & `xjet-0.1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # pyxJetAPI
 
 ## Authors
 - [@xJetLabs](https://github.com/xJetLabs) (forked from)
 - [@nik-1x](https://www.github.com/nik-1x)
  
 ## Usage/Examples  
+
+[Live example](https://replit.com/@delpydoc/xJetAPI)
+
 ```python
 api = pyxJet(
     api_key="API_KEY",
     private_key="PRIVATE_KEY", 
     mainnet=xJetNet.TESTNET # or xJetNet.MAINNET
 )
 ```
@@ -32,9 +35,15 @@
 ```python
 # Invoice methods
 await api.invoice_create(currency, amount, description, max_payments) # create invoice
 await api.invoice_status(invoice_status) # get invoice status
 await api.invoice_list() # get invoices on account
 ```
 
+```python
+# NFT methods
+await api.nft_list()
+await api.nft_transfer(nft_address, to_address)
+```
+
 ## License
 [GNUv3](https://github.com/nik-1x/pyxJetAPI/blob/main/LICENSE)
```

### Comparing `xjet-0.1.1/pyproject.toml` & `xjet-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xjet"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python SDK for t.me/xJetSwapBot"
 readme = "README.md"
 authors = [
     "delpydoc <delpydoc@proton.me>",
 ]
 maintainers = []
 repository = "https://github.com/xJetLabs/python-sdk"
```

### Comparing `xjet-0.1.1/xjet/__init__.py` & `xjet-0.1.2/xjet/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import time
 import json
 
 from .constants import xJetNet
-from .api import Account, Cheques, Invoices, System
+from .api import Account, Cheques, Invoices, System, NFT
 
 from nacl.signing import SigningKey
 from httpx import AsyncClient
 
 
-class JetAPI(Account, Cheques, Invoices, System):
-
+class JetAPI(Account, Cheques, Invoices, System, NFT):
     """
     Class for working with t.me/xJetSwapBot API.
 
     :author: Nick [t.me/crypt_nick]
     :author: Doc. Delpy [t.me/delpydoc]
 
     :license: GNUv3
```

### Comparing `xjet-0.1.1/xjet/api.py` & `xjet-0.1.2/xjet/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -135,36 +135,68 @@
     
     * invoice_create()
     * invoice_status()
     * invoice_list()
 
     """
 
-    async def invoice_create(self, currency: str, amount: int, description: str = None, max_payments: int = 1):
+    async def invoice_create(self, currency: str, amount: int, description: str = None, max_payments: int = 1, expires: int = None):
         """ Create invoice 
         
         :param `currency` [str]: Currency of invoice
         :param `amount` [int]: Amount of invoice
         :param `description` [str]: Description of invoice
         :param `max_payments` [int]: Max payments
         """
         return await self.request(
             method = 'invoice.create', 
             json = {
                 'currency': currency.lower(),
                 'amount': amount,
                 'description': description,
-                'max_payments': max_payments
+                'max_payments': max_payments,
+                'expires': expires
             }
         )
 
     async def invoice_status(self, invoice_id: str):
         """ Get invoice status
         
         :param `invoice_id` [str]: Invoice id
         """
         return await self.request(method = 'invoice.status', params = {'invoice_id': invoice_id})
 
     async def invoice_list(self):
         """ Get invoice list """
         return await self.request(method = 'invoice.list')
 
+
+class NFT:
+
+    """ NFT methods wrapper. 
+    
+    Available methods:
+    
+    * nft_list()
+    * nft_transfer()
+
+    """
+
+    async def nft_list(self):
+        """ List your NFTs """
+        return await self.request(method = 'nft.list')
+
+    async def nft_transfer(self, nft_address: str, to_address: str):
+        """nft_transfer
+
+        Args:
+            nft_address (str): NFT Item contract address
+            to_address (str): Transfer recipient address
+        """
+        return await self.request(
+            method = 'nft.transfer',
+            json = self.sign_message({
+                'nft_address': nft_address,
+                'to_address': to_address
+            }) 
+        )
+
```

### Comparing `xjet-0.1.1/xjet/sync.py` & `xjet-0.1.2/xjet/sync.py`

 * *Files identical despite different names*

### Comparing `xjet-0.1.1/setup.py` & `xjet-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['PyNaCl>=1.5.0', 'httpx>=0.23.1']
 
 setup_kwargs = {
     'name': 'xjet',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Python SDK for t.me/xJetSwapBot',
-    'long_description': '# pyxJetAPI\n\n## Authors\n- [@xJetLabs](https://github.com/xJetLabs) (forked from)\n- [@nik-1x](https://www.github.com/nik-1x)\n \n## Usage/Examples  \n```python\napi = pyxJet(\n    api_key="API_KEY",\n    private_key="PRIVATE_KEY", \n    mainnet=xJetNet.TESTNET # or xJetNet.MAINNET\n)\n```\n\n```python\n# Account methods\nawait api.me() # get API Application information.\nawait api.balance() # get balance\nawait api.submit_deposit() # check for deposit\nawait api.withdraw(ton_address, currency, amount) # check for deposit\n```\n\n```python\n# Cheques methods\nawait api.cheque_create(currency, amount, expires, description, activates_count, groups_id, personal_id, password) # create cheque\nawait api.cheque_status(cheque_id) # get cheque status\nawait api.cheque_list() # get cheques on account\nawait api.cheque_cancel(cheque_id) # delete cheque\n```\n\n```python\n# Invoice methods\nawait api.invoice_create(currency, amount, description, max_payments) # create invoice\nawait api.invoice_status(invoice_status) # get invoice status\nawait api.invoice_list() # get invoices on account\n```\n\n## License\n[GNUv3](https://github.com/nik-1x/pyxJetAPI/blob/main/LICENSE)  \n',
+    'long_description': '# pyxJetAPI\n\n## Authors\n- [@xJetLabs](https://github.com/xJetLabs) (forked from)\n- [@nik-1x](https://www.github.com/nik-1x)\n \n## Usage/Examples  \n\n[Live example](https://replit.com/@delpydoc/xJetAPI)\n\n```python\napi = pyxJet(\n    api_key="API_KEY",\n    private_key="PRIVATE_KEY", \n    mainnet=xJetNet.TESTNET # or xJetNet.MAINNET\n)\n```\n\n```python\n# Account methods\nawait api.me() # get API Application information.\nawait api.balance() # get balance\nawait api.submit_deposit() # check for deposit\nawait api.withdraw(ton_address, currency, amount) # check for deposit\n```\n\n```python\n# Cheques methods\nawait api.cheque_create(currency, amount, expires, description, activates_count, groups_id, personal_id, password) # create cheque\nawait api.cheque_status(cheque_id) # get cheque status\nawait api.cheque_list() # get cheques on account\nawait api.cheque_cancel(cheque_id) # delete cheque\n```\n\n```python\n# Invoice methods\nawait api.invoice_create(currency, amount, description, max_payments) # create invoice\nawait api.invoice_status(invoice_status) # get invoice status\nawait api.invoice_list() # get invoices on account\n```\n\n```python\n# NFT methods\nawait api.nft_list()\nawait api.nft_transfer(nft_address, to_address)\n```\n\n## License\n[GNUv3](https://github.com/nik-1x/pyxJetAPI/blob/main/LICENSE)  \n',
     'author': 'delpydoc',
     'author_email': 'delpydoc@proton.me',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/xJetLabs/python-sdk',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `xjet-0.1.1/PKG-INFO` & `xjet-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xjet
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python SDK for t.me/xJetSwapBot
 Home-page: https://github.com/xJetLabs/python-sdk
 Keywords: ton,the open network,xjet,xjetswap,sdk
 Author: delpydoc
 Author-email: delpydoc@proton.me
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -26,14 +26,17 @@
 # pyxJetAPI
 
 ## Authors
 - [@xJetLabs](https://github.com/xJetLabs) (forked from)
 - [@nik-1x](https://www.github.com/nik-1x)
  
 ## Usage/Examples  
+
+[Live example](https://replit.com/@delpydoc/xJetAPI)
+
 ```python
 api = pyxJet(
     api_key="API_KEY",
     private_key="PRIVATE_KEY", 
     mainnet=xJetNet.TESTNET # or xJetNet.MAINNET
 )
 ```
@@ -57,10 +60,16 @@
 ```python
 # Invoice methods
 await api.invoice_create(currency, amount, description, max_payments) # create invoice
 await api.invoice_status(invoice_status) # get invoice status
 await api.invoice_list() # get invoices on account
 ```
 
+```python
+# NFT methods
+await api.nft_list()
+await api.nft_transfer(nft_address, to_address)
+```
+
 ## License
 [GNUv3](https://github.com/nik-1x/pyxJetAPI/blob/main/LICENSE)
```

