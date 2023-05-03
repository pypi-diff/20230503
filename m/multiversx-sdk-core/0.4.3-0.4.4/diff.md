# Comparing `tmp/multiversx_sdk_core-0.4.3.tar.gz` & `tmp/multiversx_sdk_core-0.4.4.tar.gz`

## Comparing `multiversx_sdk_core-0.4.3.tar` & `multiversx_sdk_core-0.4.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/.flake8
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/py.typed
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/pyrightconfig.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/requirements-dev.txt
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/requirements.txt
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/.github/workflows/linter-flake8.yml
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/.github/workflows/linter-pyright.yml
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/.vscode/settings.json
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/__init__.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/account.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/account_test.py
--rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/address.py
--rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/address_test.py
--rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/bech32.py
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/code_metadata.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/code_metadata_test.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/constants.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/contract_query.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/contract_query_builder.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/contract_query_builder_test.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/errors.py
--rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/interfaces.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/messages.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/messages_test.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/serializer.py
--rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/token_payment.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/token_payment_test.py
--rw-r--r--   0        0        0     3512 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction.py
--rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_payload.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_test.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/typecheck.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/__init__.py
--rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/contract_builders.py
--rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/contract_builders_test.py
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/default_configuration.py
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/default_configuration_test.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/esdt_builders.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/esdt_builders_test.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/other_builders.py
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/relayed_builders.py
--rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/transaction_builder.py
--rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/transfers_builders.py
--rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/transfers_builders_test.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/LICENSE
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/README.md
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/.flake8
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/py.typed
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/pyrightconfig.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/requirements-dev.txt
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/requirements.txt
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/.github/workflows/linter-flake8.yml
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/.github/workflows/linter-pyright.yml
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/.vscode/settings.json
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/__init__.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/account.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/account_test.py
+-rw-r--r--   0        0        0     4478 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/address.py
+-rw-r--r--   0        0        0     4037 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/address_test.py
+-rw-r--r--   0        0        0     4747 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/bech32.py
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/code_metadata.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/code_metadata_test.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/constants.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/contract_query.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/contract_query_builder.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/contract_query_builder_test.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/errors.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/interfaces.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/messages.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/messages_test.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/serializer.py
+-rw-r--r--   0        0        0     3833 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/token_payment.py
+-rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/token_payment_test.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_payload.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_test.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/typecheck.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/__init__.py
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/contract_builders.py
+-rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/contract_builders_test.py
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/default_configuration.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/default_configuration_test.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/esdt_builders.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/esdt_builders_test.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/other_builders.py
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/relayed_builders.py
+-rw-r--r--   0        0        0     3927 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/transaction_builder.py
+-rw-r--r--   0        0        0     5680 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/transfers_builders.py
+-rw-r--r--   0        0        0     4373 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/transfers_builders_test.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/LICENSE
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/README.md
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 multiversx_sdk_core-0.4.4/PKG-INFO
```

### Comparing `multiversx_sdk_core-0.4.3/.github/workflows/linter-flake8.yml` & `multiversx_sdk_core-0.4.4/.github/workflows/linter-flake8.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/.github/workflows/linter-pyright.yml` & `multiversx_sdk_core-0.4.4/.github/workflows/linter-pyright.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/.github/workflows/python-publish.yml` & `multiversx_sdk_core-0.4.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/.github/workflows/test.yml` & `multiversx_sdk_core-0.4.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/__init__.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/address.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/address.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/address_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/address_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/bech32.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/bech32.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/code_metadata.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/code_metadata.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/code_metadata_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/code_metadata_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/contract_query.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/contract_query.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/contract_query_builder.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/contract_query_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/contract_query_builder_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/contract_query_builder_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/interfaces.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/interfaces.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/messages.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/messages.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/messages_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/messages_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/serializer.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/serializer.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/token_payment.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/token_payment.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/token_payment_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/token_payment_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         version: Optional[ITransactionVersion] = None,
         options: Optional[ITransactionOptions] = None,
         guardian: Optional[IAddress] = None
     ):
         self.chainID: IChainID = chain_id
         self.sender: IAddress = sender
         self.receiver: IAddress = receiver
-        self.guardian = guardian
+        self.guardian: Optional[IAddress] = guardian
 
         self.gas_limit: IGasLimit = gas_limit
         self.gas_price: IGasPrice = gas_price or TRANSACTION_MIN_GAS_PRICE
 
         self.nonce: INonce = nonce or 0
         self.value: ITransactionValue = value or 0
         self.data: ITransactionPayload = data or TransactionPayload.empty()
```

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_payload.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_payload.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/typecheck.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/typecheck.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/__init__.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/__init__.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/contract_builders.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/contract_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/contract_builders_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/contract_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/default_configuration.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/default_configuration.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/esdt_builders.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/esdt_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/esdt_builders_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/esdt_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/transaction_builder.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/transfers_builders.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/transfers_builders.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/multiversx_sdk_core/transaction_builders/transfers_builders_test.py` & `multiversx_sdk_core-0.4.4/multiversx_sdk_core/transaction_builders/transfers_builders_test.py`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/.gitignore` & `multiversx_sdk_core-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/LICENSE` & `multiversx_sdk_core-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/README.md` & `multiversx_sdk_core-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `multiversx_sdk_core-0.4.3/pyproject.toml` & `multiversx_sdk_core-0.4.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multiversx-sdk-core"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="MultiversX" },
 ]
 license = "MIT"
 description = "Core components of the MultiversX Python SDK."
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `multiversx_sdk_core-0.4.3/PKG-INFO` & `multiversx_sdk_core-0.4.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiversx-sdk-core
-Version: 0.4.3
+Version: 0.4.4
 Summary: Core components of the MultiversX Python SDK.
 Project-URL: Homepage, https://github.com/multiversx/mx-sdk-py-core
 Author: MultiversX
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

