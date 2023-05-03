# Comparing `tmp/open-aea-ledger-ethereum-flashbots-1.32.0.tar.gz` & `tmp/open-aea-ledger-ethereum-flashbots-1.33.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-aea-ledger-ethereum-flashbots-1.32.0.tar", last modified: Tue Apr 11 12:20:29 2023, max compression
+gzip compressed data, was "open-aea-ledger-ethereum-flashbots-1.33.0.tar", last modified: Wed May  3 04:23:51 2023, max compression
```

## Comparing `open-aea-ledger-ethereum-flashbots-1.32.0.tar` & `open-aea-ledger-ethereum-flashbots-1.33.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:29.116811 open-aea-ledger-ethereum-flashbots-1.32.0/
--rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-04-11 12:20:29.116811 open-aea-ledger-ethereum-flashbots-1.32.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:29.112811 open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/
--rw-r--r--   0 runner    (1001) docker     (122)      943 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9630 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:29.112811 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      538 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-04-11 12:20:29.000000 open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       90 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-11 12:20:29.116811 open-aea-ledger-ethereum-flashbots-1.32.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-11 12:20:29.112811 open-aea-ledger-ethereum-flashbots-1.32.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      843 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9419 2023-04-11 12:19:43.000000 open-aea-ledger-ethereum-flashbots-1.32.0/tests/test_ethereum.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 04:23:51.376526 open-aea-ledger-ethereum-flashbots-1.33.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    11339 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-03 04:23:51.376526 open-aea-ledger-ethereum-flashbots-1.33.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 04:23:51.376526 open-aea-ledger-ethereum-flashbots-1.33.0/aea_ledger_ethereum_flashbots/
+-rw-r--r--   0 runner    (1001) docker     (122)      943 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/aea_ledger_ethereum_flashbots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10252 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 04:23:51.376526 open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1122 2023-05-03 04:23:51.000000 open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      538 2023-05-03 04:23:51.000000 open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-03 04:23:51.000000 open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-03 04:23:51.000000 open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-03 04:23:51.000000 open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-05-03 04:23:51.000000 open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       90 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-03 04:23:51.376526 open-aea-ledger-ethereum-flashbots-1.33.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2686 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-03 04:23:51.376526 open-aea-ledger-ethereum-flashbots-1.33.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10646 2023-05-03 04:23:03.000000 open-aea-ledger-ethereum-flashbots-1.33.0/tests/test_ethereum.py
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/LICENSE` & `open-aea-ledger-ethereum-flashbots-1.33.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/PKG-INFO` & `open-aea-ledger-ethereum-flashbots-1.33.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.32.0
+Version: 1.33.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/__init__.py` & `open-aea-ledger-ethereum-flashbots-1.33.0/aea_ledger_ethereum_flashbots/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py` & `open-aea-ledger-ethereum-flashbots-1.33.0/aea_ledger_ethereum_flashbots/ethereum_flashbots.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,15 +105,18 @@
 
         :param bundle: the bundle to simulate.
         :param target_block: the target block for the transaction, the current block if not provided.
         :return: True if the simulation went through, False otherwise.
         """
         _default_logger.debug(f"Simulating bundle: {bundle}")
         try:
-            self.flashbots.simulate(bundle, target_block)
+            simulation_response = self.flashbots.simulate(bundle, target_block)
+            _default_logger.info(
+                f"Flashbots simulation response: {simulation_response}"
+            )
             _default_logger.debug(f"Simulation successful for bundle {bundle}.")
             return True
         except Exception as e:  # pylint: disable=broad-except
             _default_logger.warning(f"Simulation failed for bundle {bundle}: {e}")
         return False
 
     def send_bundle(
@@ -133,25 +136,34 @@
 
         :param bundle: the signed transactions to bundle together and send.
         :param target_blocks: the target blocks for the transactions.
         :param raise_on_failed_simulation: whether to raise an exception if the simulation fails.
         :return: the transaction digest if the transaction went through, None otherwise.
         """
         for target_block in target_blocks:
-            if not self.simulate(bundle, target_block):
-                msg = f"Simulation failed for bundle {bundle} targeting block {target_block}."
+            current_block = self.api.eth.blockNumber
+            if current_block >= target_block:
+                # we can only target future blocks
+                _default_logger.debug(
+                    f"Current block {current_block} >= target block {target_block}"
+                )
+                continue
+            # we simulate the bundle against the current block
+            if not self.simulate(bundle, current_block):
+                msg = f"Simulation failed for bundle {bundle} on block {current_block}."
                 if raise_on_failed_simulation:
                     raise ValueError(msg)
                 _default_logger.warning(msg)
                 continue
 
             replacement_uuid = str(uuid4())
             _default_logger.debug(
                 f"Sending bundle {bundle} with replacement_uuid {replacement_uuid} targeting block {target_block}"
             )
+            # we try to send the bundle on the target block, which MUST be greater than the current block
             response = self.flashbots.send_bundle(
                 bundle, target_block, opts={"replacementUuid": replacement_uuid}
             )
             _default_logger.debug(
                 f"Response from bundle with replacement uuid {replacement_uuid}: {response}"
             )
             response.wait()
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO` & `open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-aea-ledger-ethereum-flashbots
-Version: 1.32.0
+Version: 1.33.0
 Summary: Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.
 Author: Valory AG
 License: Apache-2.0
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt` & `open-aea-ledger-ethereum-flashbots-1.33.0/open_aea_ledger_ethereum_flashbots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/setup.py` & `open-aea-ledger-ethereum-flashbots-1.33.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 """Setup script for "aea_ledger_ethereum_flashbots" package."""
 
 from setuptools import find_packages, setup
 
 
 setup(
     name="open-aea-ledger-ethereum-flashbots",
-    version="1.32.0",
+    version="1.33.0",
     author="Valory AG",
     license="Apache-2.0",
     description="Python package extending the default open-aea ethereum ledger plugin to add support for flashbots.",
     long_description=(
         "Python package extending the default open-aea ethereum ledger plugin to add support for flashbots."
     ),
     long_description_content_type="text/markdown",
@@ -37,15 +37,15 @@
     package_data={
         "aea_ledger_ethereum_flashbots": [
             "py.typed",
         ]
     },
     python_requires=">=3.9,<4.0",
     install_requires=[
-        "open-aea-ledger-ethereum~=1.32.0",
+        "open-aea-ledger-ethereum~=1.33.0",
         "flashbots==1.1.1",
     ],
     tests_require=["pytest"],
     entry_points={
         "aea.cryptos": [
             "ethereum_flashbots = aea_ledger_ethereum_flashbots:EthereumFlashbotCrypto"
         ],
```

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/tests/__init__.py` & `open-aea-ledger-ethereum-flashbots-1.33.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `open-aea-ledger-ethereum-flashbots-1.32.0/tests/test_ethereum.py` & `open-aea-ledger-ethereum-flashbots-1.33.0/tests/test_ethereum.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,31 +100,37 @@
     # check
     ethereum_flashbot_api.flashbots.simulate.assert_called_once_with(bundle, 123)
     assert not success
 
 
 def test_send_bundle_with_successful_transaction(ethereum_flashbot_api) -> None:
     """Test send bundle with successful transaction."""
+    current_block = 122
     send_bundle = [FlashbotsBundleRawTx(signed_transaction=HexBytes("0x1234"))]
     res_bundle = [{"hash": b"0x1234"}]
     response_mock = MagicMock()
     response_mock.wait = MagicMock()
     response_mock.receipts = MagicMock(return_value=[TxReceipt(blockNumber=1)])
     response_mock.bundle = res_bundle
+    ethereum_flashbot_api.api.eth.get_block_number = MagicMock(
+        return_value=current_block
+    )
     ethereum_flashbot_api.flashbots.simulate = MagicMock(return_value=True)
     ethereum_flashbot_api.flashbots.send_bundle = MagicMock(return_value=response_mock)
 
     # run
     target_blocks = [123]
     tx_hashes = ethereum_flashbot_api.send_bundle(send_bundle, target_blocks)
 
     # check
-    ethereum_flashbot_api.flashbots.simulate.assert_called_once_with(send_bundle, 123)
+    ethereum_flashbot_api.flashbots.simulate.assert_called_once_with(
+        send_bundle, current_block
+    )
     ethereum_flashbot_api.flashbots.send_bundle.assert_called_once_with(
-        send_bundle, 123, opts={"replacementUuid": ANY}
+        send_bundle, target_blocks[0], opts={"replacementUuid": ANY}
     )
     assert response_mock.wait.called
     assert tx_hashes == [tx["hash"].hex() for tx in response_mock.bundle]
 
 
 def test_bundle_transactions_with_empty_list(ethereum_flashbot_api) -> None:
     """Test bundle transactions with an empty list of signed transactions."""
@@ -153,14 +159,15 @@
     response_mock = MagicMock()
     response_mock.wait = MagicMock()
     response_mock.receipts = MagicMock(
         return_value=[TxReceipt(blockNumber=1), TxReceipt(blockNumber=2)]
     )
     response_mock.bundle = [{"hash": b"0x1234"}, {"hash": b"0x5678"}]
     ethereum_flashbot_api._get_next_blocks = MagicMock(return_value=1)
+    ethereum_flashbot_api.api.eth.get_block_number = MagicMock(return_value=1)
     ethereum_flashbot_api.flashbots.simulate = MagicMock(return_value=True)
     ethereum_flashbot_api.flashbots.send_bundle = MagicMock(return_value=response_mock)
 
     # run
     signed_transactions = [
         dict(raw_transaction="0x1234"),
         dict(raw_transaction="0x5678"),
@@ -182,14 +189,15 @@
     """Test bundle and send with failed simulation."""
     # mock
     response_mock = MagicMock()
     response_mock.wait = MagicMock()
     response_mock.bundle_hash = MagicMock()
     response_mock.receipts = MagicMock(side_effect=TransactionNotFound)
     ethereum_flashbot_api._get_next_blocks = MagicMock(return_value=1)
+    ethereum_flashbot_api.api.eth.get_block_number = MagicMock(return_value=1)
     ethereum_flashbot_api.flashbots.simulate = MagicMock(return_value=True)
     ethereum_flashbot_api.flashbots.send_bundle = MagicMock(return_value=response_mock)
     ethereum_flashbot_api.flashbots.cancel_bundles = MagicMock()
     ethereum_flashbot_api.api.toHex = MagicMock()
     ethereum_flashbot_api.flashbots.get_bundle_stats_v2 = MagicMock(
         return_value=response_mock
     )
@@ -215,14 +223,15 @@
 def test_send_bundle_with_failed_simulation(ethereum_flashbot_api) -> None:
     """Test send bundle with failed simulation."""
     # mock
     response_mock = MagicMock()
     response_mock.wait = MagicMock()
     response_mock.bundle_hash = MagicMock()
     response_mock.receipts = MagicMock(side_effect=TransactionNotFound)
+    ethereum_flashbot_api.api.eth.get_block_number = MagicMock(return_value=1)
     ethereum_flashbot_api.simulate = MagicMock(return_value=False)
     target_blocks = [0]
 
     # run
     tx_hashes = ethereum_flashbot_api.send_bundle(MagicMock(), target_blocks)
 
     # check
@@ -232,16 +241,36 @@
 def test_send_bundle_with_failed_simulation_and_raise(ethereum_flashbot_api) -> None:
     """Test send bundle with failed simulation and should raise."""
     # mock
     response_mock = MagicMock()
     response_mock.wait = MagicMock()
     response_mock.bundle_hash = MagicMock()
     response_mock.receipts = MagicMock(side_effect=TransactionNotFound)
+    ethereum_flashbot_api.api.eth.get_block_number = MagicMock(return_value=0)
     ethereum_flashbot_api.simulate = MagicMock(return_value=False)
     raise_on_failed_simulation = True
-    target_blocks = [0]
+    target_blocks = [1]
 
     # run
     with pytest.raises(ValueError):
         ethereum_flashbot_api.send_bundle(
             MagicMock(), target_blocks, raise_on_failed_simulation
         )
+
+
+def test_send_bundle_with_bad_target_block(ethereum_flashbot_api) -> None:
+    """Test send bundle with an old target block should return None."""
+    # mock
+    response_mock = MagicMock()
+    response_mock.wait = MagicMock()
+    response_mock.bundle_hash = MagicMock()
+    response_mock.receipts = MagicMock(side_effect=TransactionNotFound)
+    ethereum_flashbot_api.api.eth.get_block_number = MagicMock(return_value=1)
+    ethereum_flashbot_api.simulate = MagicMock(return_value=True)
+    raise_on_failed_simulation = True
+    target_blocks = [0]
+
+    # run
+    res = ethereum_flashbot_api.send_bundle(
+        MagicMock(), target_blocks, raise_on_failed_simulation
+    )
+    assert res is None, "Should return None if target block is old"
```

