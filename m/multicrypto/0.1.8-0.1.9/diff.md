# Comparing `tmp/multicrypto-0.1.8.tar.gz` & `tmp/multicrypto-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/multicrypto-0.1.8.tar", last modified: Tue Jun 19 15:08:22 2018, max compression
+gzip compressed data, was "dist/multicrypto-0.1.9.tar", last modified: Fri Jun 29 07:01:45 2018, max compression
```

## Comparing `multicrypto-0.1.8.tar` & `multicrypto-0.1.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 tompin    (1000) tompin    (1000)        0 2018-06-19 15:08:22.000000 multicrypto-0.1.8/
--rw-rw-r--   0 tompin    (1000) tompin    (1000)      111 2018-06-19 15:08:22.000000 multicrypto-0.1.8/setup.cfg
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     8166 2018-06-19 15:08:22.000000 multicrypto-0.1.8/PKG-INFO
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     6040 2018-06-19 15:06:19.000000 multicrypto-0.1.8/README.md
-drwxrwxr-x   0 tompin    (1000) tompin    (1000)        0 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto.egg-info/
--rw-rw-r--   0 tompin    (1000) tompin    (1000)        1 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto.egg-info/dependency_links.txt
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     8166 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto.egg-info/PKG-INFO
--rw-rw-r--   0 tompin    (1000) tompin    (1000)      719 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto.egg-info/SOURCES.txt
--rw-rw-r--   0 tompin    (1000) tompin    (1000)       12 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto.egg-info/top_level.txt
--rw-rw-r--   0 tompin    (1000) tompin    (1000)      335 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto.egg-info/entry_points.txt
--rw-rw-r--   0 tompin    (1000) tompin    (1000)       31 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto.egg-info/requires.txt
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     1682 2018-06-19 14:50:00.000000 multicrypto-0.1.8/setup.py
-drwxrwxr-x   0 tompin    (1000) tompin    (1000)        0 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto/
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     3409 2018-06-18 17:28:26.000000 multicrypto-0.1.8/multicrypto/network.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     7096 2018-06-19 14:00:10.000000 multicrypto-0.1.8/multicrypto/transaction.py
-drwxrwxr-x   0 tompin    (1000) tompin    (1000)        0 2018-06-19 15:08:22.000000 multicrypto-0.1.8/multicrypto/commands/
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     3544 2018-04-16 07:49:00.000000 multicrypto-0.1.8/multicrypto/commands/genaddress.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     2815 2018-06-13 22:21:50.000000 multicrypto-0.1.8/multicrypto/commands/transprivkey.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     3948 2018-06-19 14:21:10.000000 multicrypto-0.1.8/multicrypto/commands/sendcrypto.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     4889 2018-06-19 14:18:39.000000 multicrypto-0.1.8/multicrypto/commands/sweepaddress.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     3372 2018-06-19 11:58:59.000000 multicrypto-0.1.8/multicrypto/commands/checkaddress.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     2384 2018-03-16 16:46:26.000000 multicrypto-0.1.8/multicrypto/commands/transaddress.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)        0 2018-06-18 17:34:38.000000 multicrypto-0.1.8/multicrypto/commands/__init__.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     3419 2018-06-19 09:41:37.000000 multicrypto-0.1.8/multicrypto/utils.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     6715 2018-06-19 12:03:14.000000 multicrypto-0.1.8/multicrypto/address.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     2125 2018-06-15 16:38:39.000000 multicrypto-0.1.8/multicrypto/consts.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     6457 2018-06-16 14:28:13.000000 multicrypto-0.1.8/multicrypto/coins.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     1055 2018-04-17 09:41:06.000000 multicrypto-0.1.8/multicrypto/ethaddress.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)      173 2018-06-14 16:10:11.000000 multicrypto-0.1.8/multicrypto/log.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)     1423 2018-05-04 13:29:33.000000 multicrypto-0.1.8/multicrypto/base58.py
--rw-rw-r--   0 tompin    (1000) tompin    (1000)        0 2018-02-08 12:48:33.000000 multicrypto-0.1.8/multicrypto/__init__.py
+drwxrwxr-x   0 tompin    (1000) tompin    (1000)        0 2018-06-29 07:01:45.000000 multicrypto-0.1.9/
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)      111 2018-06-29 07:01:45.000000 multicrypto-0.1.9/setup.cfg
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     8248 2018-06-29 07:01:45.000000 multicrypto-0.1.9/PKG-INFO
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     6114 2018-06-21 22:08:51.000000 multicrypto-0.1.9/README.md
+drwxrwxr-x   0 tompin    (1000) tompin    (1000)        0 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto.egg-info/
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)        1 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto.egg-info/dependency_links.txt
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     8248 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto.egg-info/PKG-INFO
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)      719 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto.egg-info/SOURCES.txt
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)       12 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto.egg-info/top_level.txt
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)      335 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto.egg-info/entry_points.txt
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)       31 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto.egg-info/requires.txt
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     1682 2018-06-29 06:59:50.000000 multicrypto-0.1.9/setup.py
+drwxrwxr-x   0 tompin    (1000) tompin    (1000)        0 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto/
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     3409 2018-06-18 17:28:26.000000 multicrypto-0.1.9/multicrypto/network.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     9197 2018-06-28 13:29:05.000000 multicrypto-0.1.9/multicrypto/transaction.py
+drwxrwxr-x   0 tompin    (1000) tompin    (1000)        0 2018-06-29 07:01:45.000000 multicrypto-0.1.9/multicrypto/commands/
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     3611 2018-06-27 12:02:43.000000 multicrypto-0.1.9/multicrypto/commands/genaddress.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     2815 2018-06-13 22:21:50.000000 multicrypto-0.1.9/multicrypto/commands/transprivkey.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     3963 2018-06-23 17:25:38.000000 multicrypto-0.1.9/multicrypto/commands/sendcrypto.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     4904 2018-06-24 14:33:57.000000 multicrypto-0.1.9/multicrypto/commands/sweepaddress.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     3387 2018-06-23 17:25:28.000000 multicrypto-0.1.9/multicrypto/commands/checkaddress.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     2384 2018-03-16 16:46:26.000000 multicrypto-0.1.9/multicrypto/commands/transaddress.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)        0 2018-06-18 17:34:38.000000 multicrypto-0.1.9/multicrypto/commands/__init__.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     4647 2018-06-27 12:35:57.000000 multicrypto-0.1.9/multicrypto/utils.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     6411 2018-06-27 12:02:43.000000 multicrypto-0.1.9/multicrypto/address.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     2125 2018-06-15 16:38:39.000000 multicrypto-0.1.9/multicrypto/consts.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     7356 2018-06-25 14:00:42.000000 multicrypto-0.1.9/multicrypto/coins.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     1055 2018-04-17 09:41:06.000000 multicrypto-0.1.9/multicrypto/ethaddress.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)      173 2018-06-14 16:10:11.000000 multicrypto-0.1.9/multicrypto/log.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)     1423 2018-05-04 13:29:33.000000 multicrypto-0.1.9/multicrypto/base58.py
+-rw-rw-r--   0 tompin    (1000) tompin    (1000)        0 2018-02-08 12:48:33.000000 multicrypto-0.1.9/multicrypto/__init__.py
```

### Comparing `multicrypto-0.1.8/PKG-INFO` & `multicrypto-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: multicrypto
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool for translating and creating custom addresses for various cryptocurrencies
 Home-page: https://github.com/tompin/multicrypto
 Author: tompin
 Author-email: tompin@tuta.io
 License: http://opensource.org/licenses/MIT
 Description: # README
         
@@ -26,15 +26,16 @@
         ## INSTALLATION
         
         If you don't have Python 3 install it by following instructions from python.org. 
         Supported Python versions are 3.5, 3.6, 3.7. Then Run:
         ```bash
         pip3 install multicrypto
         ```
-        The package contains four commands `sendcrypto`, `transaddress`, `transprivkey`, `genaddress`
+        The package contains six commands `sweepaddress`, `sendcrypto`, `checkaddress`, `transaddress`,
+        `transprivkey`, `genaddress`
         described below.
         ### Additional packages on Ubuntu
         ```bash
         sudo apt-get install build-essential python3-dev libgmp3-dev
         ```
         ## USAGE
         
@@ -45,20 +46,20 @@
          sweepaddress --coin_symbol=<COIN_SYMBOL> --address=<ADDRESS> --private_key=<PRIVATE KEY> --minimum_input_threshold=<INT> --maximum_input_threshold=<INT>
          ```
          After mining some currency for longer period we could end up with address having a lot of small inputs. 
          In such case it is very likely it will be not possible to send the funds in one transaction and it could
           be difficult to cope with. Let say for Zen Cash we have private key of the address which inputs 
           we want to combine, but we want only combine inputs which are smaller than 0.1 ZEN:
           ```bash
-         sweepaddress -c ZEN --private_key --maximum_input_threshold==10000000
+         sweepaddress -c ZEN -p KwDiDMtpksBAcfyHsVS5XzmirtyjKWSeaeM9U1QppugixMUeKMqp --maximum_input_threshold==10000000
          ```
          This will create appropriate number of transactions (by default one transaction for each 200 inputs, you can 
-         override this value by setting parameter --batch_size, but setting it to high will result in too big transaction error),
+         override this value by setting parameter --batch_size, but setting it too high will result in too big transaction error),
          transaction fee will be set to default 0.00001 ZEN (you can override it using --fee parameter) and the
-         funds will be sent back to original address (you can override the output address using --address parameter) 
+         funds will be sent back to original address (you can override the output address using --address parameter).
         
          2. Sending funds (P2PKH):
          ```bash
          sendcrypto --coin_symbol=<COIN_SYMBOL> --satoshis=<INT> --address=<ADDRESS> --private_key=<PRIVATE KEY> --minimum_input_threshold=<INT> --maximum_input_threshold=<INT>
          ```
          Sending 0.25 BTC to address 1BTC1NNjeiAmFqe2n1QJjkEa4aMyAhkpKG with default fee 10000 satoshis
          and only using inputs containing not more than 100000 satoshis:
```

### Comparing `multicrypto-0.1.8/README.md` & `multicrypto-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 ## INSTALLATION
 
 If you don't have Python 3 install it by following instructions from python.org. 
 Supported Python versions are 3.5, 3.6, 3.7. Then Run:
 ```bash
 pip3 install multicrypto
 ```
-The package contains four commands `sendcrypto`, `transaddress`, `transprivkey`, `genaddress`
+The package contains six commands `sweepaddress`, `sendcrypto`, `checkaddress`, `transaddress`,
+`transprivkey`, `genaddress`
 described below.
 ### Additional packages on Ubuntu
 ```bash
 sudo apt-get install build-essential python3-dev libgmp3-dev
 ```
 ## USAGE
 
@@ -37,20 +38,20 @@
  sweepaddress --coin_symbol=<COIN_SYMBOL> --address=<ADDRESS> --private_key=<PRIVATE KEY> --minimum_input_threshold=<INT> --maximum_input_threshold=<INT>
  ```
  After mining some currency for longer period we could end up with address having a lot of small inputs. 
  In such case it is very likely it will be not possible to send the funds in one transaction and it could
   be difficult to cope with. Let say for Zen Cash we have private key of the address which inputs 
   we want to combine, but we want only combine inputs which are smaller than 0.1 ZEN:
   ```bash
- sweepaddress -c ZEN --private_key --maximum_input_threshold==10000000
+ sweepaddress -c ZEN -p KwDiDMtpksBAcfyHsVS5XzmirtyjKWSeaeM9U1QppugixMUeKMqp --maximum_input_threshold==10000000
  ```
  This will create appropriate number of transactions (by default one transaction for each 200 inputs, you can 
- override this value by setting parameter --batch_size, but setting it to high will result in too big transaction error),
+ override this value by setting parameter --batch_size, but setting it too high will result in too big transaction error),
  transaction fee will be set to default 0.00001 ZEN (you can override it using --fee parameter) and the
- funds will be sent back to original address (you can override the output address using --address parameter) 
+ funds will be sent back to original address (you can override the output address using --address parameter).
 
  2. Sending funds (P2PKH):
  ```bash
  sendcrypto --coin_symbol=<COIN_SYMBOL> --satoshis=<INT> --address=<ADDRESS> --private_key=<PRIVATE KEY> --minimum_input_threshold=<INT> --maximum_input_threshold=<INT>
  ```
  Sending 0.25 BTC to address 1BTC1NNjeiAmFqe2n1QJjkEa4aMyAhkpKG with default fee 10000 satoshis
  and only using inputs containing not more than 100000 satoshis:
```

### Comparing `multicrypto-0.1.8/multicrypto.egg-info/PKG-INFO` & `multicrypto-0.1.9/multicrypto.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: multicrypto
-Version: 0.1.8
+Version: 0.1.9
 Summary: Tool for translating and creating custom addresses for various cryptocurrencies
 Home-page: https://github.com/tompin/multicrypto
 Author: tompin
 Author-email: tompin@tuta.io
 License: http://opensource.org/licenses/MIT
 Description: # README
         
@@ -26,15 +26,16 @@
         ## INSTALLATION
         
         If you don't have Python 3 install it by following instructions from python.org. 
         Supported Python versions are 3.5, 3.6, 3.7. Then Run:
         ```bash
         pip3 install multicrypto
         ```
-        The package contains four commands `sendcrypto`, `transaddress`, `transprivkey`, `genaddress`
+        The package contains six commands `sweepaddress`, `sendcrypto`, `checkaddress`, `transaddress`,
+        `transprivkey`, `genaddress`
         described below.
         ### Additional packages on Ubuntu
         ```bash
         sudo apt-get install build-essential python3-dev libgmp3-dev
         ```
         ## USAGE
         
@@ -45,20 +46,20 @@
          sweepaddress --coin_symbol=<COIN_SYMBOL> --address=<ADDRESS> --private_key=<PRIVATE KEY> --minimum_input_threshold=<INT> --maximum_input_threshold=<INT>
          ```
          After mining some currency for longer period we could end up with address having a lot of small inputs. 
          In such case it is very likely it will be not possible to send the funds in one transaction and it could
           be difficult to cope with. Let say for Zen Cash we have private key of the address which inputs 
           we want to combine, but we want only combine inputs which are smaller than 0.1 ZEN:
           ```bash
-         sweepaddress -c ZEN --private_key --maximum_input_threshold==10000000
+         sweepaddress -c ZEN -p KwDiDMtpksBAcfyHsVS5XzmirtyjKWSeaeM9U1QppugixMUeKMqp --maximum_input_threshold==10000000
          ```
          This will create appropriate number of transactions (by default one transaction for each 200 inputs, you can 
-         override this value by setting parameter --batch_size, but setting it to high will result in too big transaction error),
+         override this value by setting parameter --batch_size, but setting it too high will result in too big transaction error),
          transaction fee will be set to default 0.00001 ZEN (you can override it using --fee parameter) and the
-         funds will be sent back to original address (you can override the output address using --address parameter) 
+         funds will be sent back to original address (you can override the output address using --address parameter).
         
          2. Sending funds (P2PKH):
          ```bash
          sendcrypto --coin_symbol=<COIN_SYMBOL> --satoshis=<INT> --address=<ADDRESS> --private_key=<PRIVATE KEY> --minimum_input_threshold=<INT> --maximum_input_threshold=<INT>
          ```
          Sending 0.25 BTC to address 1BTC1NNjeiAmFqe2n1QJjkEa4aMyAhkpKG with default fee 10000 satoshis
          and only using inputs containing not more than 100000 satoshis:
```

### Comparing `multicrypto-0.1.8/multicrypto.egg-info/SOURCES.txt` & `multicrypto-0.1.9/multicrypto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multicrypto-0.1.8/setup.py` & `multicrypto-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='multicrypto',
-    version='0.1.8',
+    version='0.1.9',
     description='Tool for translating and creating custom addresses for various cryptocurrencies',
     long_description=long_description,
     author='tompin',
     author_email='tompin@tuta.io',
     url='https://github.com/tompin/multicrypto',
     license='http://opensource.org/licenses/MIT',
     classifiers=[
```

### Comparing `multicrypto-0.1.8/multicrypto/network.py` & `multicrypto-0.1.9/multicrypto/network.py`

 * *Files identical despite different names*

### Comparing `multicrypto-0.1.8/multicrypto/transaction.py` & `multicrypto-0.1.9/multicrypto/transaction.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
+import time
 from binascii import hexlify
 
 from fastecdsa.curve import secp256k1
 from fastecdsa.ecdsa import sign
 
-from multicrypto.address import get_public_key_hash, get_encoded_point, calculate_public_key_hash
+from multicrypto.address import get_public_key_hash, encode_point, calculate_public_key_hash
 from multicrypto.consts import OP_DUP, OP_HASH160, OP_PUSH_20, OP_CHECKSIG, OP_EQUALVERIFY, OP_0
 from multicrypto.utils import int_to_bytes, hex_to_bytes, der_encode_signature, double_sha256_hex, \
     reverse_byte_hex
 
 logger = logging.getLogger(__name__)
 
 
@@ -30,15 +31,15 @@
         self.private_key = private_key
         self.public_key = private_key * secp256k1.G
         compressed_public_key_hash = calculate_public_key_hash(self.public_key, compressed=True)
         if compressed_public_key_hash.hex() in script:
             compressed_public_key = True
         else:
             compressed_public_key = False
-        self.encoded_public_key = get_encoded_point(
+        self.encoded_public_key = encode_point(
             self.public_key, compressed=compressed_public_key)
         self.public_key_len = len(self.encoded_public_key).to_bytes(1, byteorder='little')
 
     def get_encoded(self, with_script):
         input_data = self.transaction_id + self.output_index
         if with_script:
             input_data += self.script_length + self.script
@@ -101,17 +102,16 @@
                 height_bytes = int_to_bytes(self.last_block['height'], byteorder='little')
                 script += len(height_bytes).to_bytes(1, byteorder='big') + height_bytes + b'\xb4'
             output_block += output.satoshis.to_bytes(8, byteorder='little')
             output_block += int_to_bytes(len(script), byteorder='little')
             output_block += script
         return output_block
 
-    def sign_input(self, position):
-        input = self.inputs[position]
-        message = (
+    def get_data_to_sign(self, position):
+        data = (
             # Four-byte version field
             self.version +
 
             # One-byte varint specifying the number of inputs
             self.inputs_counter +
 
             # Inputs
@@ -125,14 +125,19 @@
 
             # Four-byte "lock time" field
             self.lock_time +
 
             # Four-byte "hash code type"
             self.hash_type
         )
+        return data
+
+    def sign_input(self, position):
+        input = self.inputs[position]
+        message = self.get_data_to_sign(position)
         #  ECDSA signing is done as follows:
         #  given a message 'm', a sign-secret 'k', a private key 'x'
         #  calculate point R = G * k
         #  r = xcoordinate(R)
         #  s = (m + x * r) / k (mod q)
         #  q is the group order of secp256k1 = 2**256 - 432420386565659656852420866394968145599
         sig = sign(message.hex(), input.private_key, curve=secp256k1, hashfunc=double_sha256_hex)
@@ -157,11 +162,70 @@
             self.inputs_counter +
             self.get_encoded_inputs(position=range(len(self.inputs))) +
             self.outputs_counter +
             self.get_encoded_outputs() +
             self.lock_time
         )
         self.id = reverse_byte_hex(double_sha256_hex(raw_transaction_data).hexdigest())
+        self.raw = raw_transaction_data.decode()
+        logger.info('Created transaction with id: {}\nRaw data: {}'.format(
+            self.id, self.raw))
+        return self.raw
+
+
+class POSTransaction(Transaction):
+    def __init__(self, coin, inputs, outputs, transaction_time=None, **params):
+        if transaction_time is None:
+            self.transaction_time = int(time.time()).to_bytes(4, byteorder='little')
+        else:
+            self.transaction_time = transaction_time
+        for input in inputs:
+            input['transaction_id'] = reverse_byte_hex(input['transaction_id'])
+        super().__init__(coin, inputs, outputs, **params)
+
+    def get_data_to_sign(self, position):
+        data = (
+            # Four-byte version field
+            self.version +
+
+            # Transaction creation time
+            self.transaction_time +
+
+            # One-byte varint specifying the number of inputs
+            self.inputs_counter +
+
+            # Inputs
+            self.get_encoded_inputs([position]) +
+
+            # One-byte varint containing the number of outputs in our new transaction
+            self.outputs_counter +
+
+            # Outputs
+            self.get_encoded_outputs() +
+
+            # Four-byte "lock time" field
+            self.lock_time +
+
+            # Four-byte "hash code type"
+            self.hash_type
+        )
+        return data
+
+    def create(self):
+        if self.id:
+            raise Exception('Transaction id {} already created'.format(self.id))
+        for i in range(len(self.inputs)):
+            self.sign_input(i)
+        raw_transaction_data = hexlify(
+            self.version +
+            self.transaction_time +
+            self.inputs_counter +
+            self.get_encoded_inputs(position=range(len(self.inputs))) +
+            self.outputs_counter +
+            self.get_encoded_outputs() +
+            self.lock_time
+        )
+        self.id = reverse_byte_hex(double_sha256_hex(raw_transaction_data).hexdigest())
         self.raw = raw_transaction_data.decode()
         logger.info('Created transaction with id: {}\nRaw data: {}'.format(
             self.id, self.raw))
         return self.raw
```

### Comparing `multicrypto-0.1.8/multicrypto/commands/genaddress.py` & `multicrypto-0.1.9/multicrypto/commands/genaddress.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 import logging
 import multiprocessing
 import sys
 
 from fastecdsa.curve import secp256k1
 from fastecdsa.keys import gen_private_key
 
-from multicrypto.address import convert_public_key_to_address, N, G, \
-    convert_private_key_to_wif_format, validate_pattern
+from multicrypto.address import convert_public_key_to_address, convert_private_key_to_wif_format, \
+    validate_pattern
 from multicrypto.coins import coins, validate_coin_symbol
 
 
 logger = logging.getLogger(__name__)
+N = secp256k1.q  # order of the curve
+G = secp256k1.G  # generator point
 
 
 def generate_address(worker_num, coin_settings, pattern, compressed, segwit, found, quit):
     if segwit:
         prefix_bytes = coin_settings['script_prefix_bytes']
     else:
         prefix_bytes = coin_settings['address_prefix_bytes']
```

### Comparing `multicrypto-0.1.8/multicrypto/commands/transprivkey.py` & `multicrypto-0.1.9/multicrypto/commands/transprivkey.py`

 * *Files identical despite different names*

### Comparing `multicrypto-0.1.8/multicrypto/commands/sendcrypto.py` & `multicrypto-0.1.9/multicrypto/commands/sendcrypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,14 +57,15 @@
         for wif_private_key in wif_private_keys:
             validate_wif_private_key(wif_private_key, coin_symbol)
     except Exception as e:
         logger.error(e)
         return
     if not coins[coin_symbol].get('api'):
         logger.error('No api has been defined for the coin {}'.format(coin_symbol))
+        return
 
     try:
         result = send(coins[coin_symbol], wif_private_keys, address, satoshis, fee,
                       minimum_input_threshold, maximum_input_threshold, limit_inputs)
     except Exception as e:
         logger.error(e)
         return
```

### Comparing `multicrypto-0.1.8/multicrypto/commands/sweepaddress.py` & `multicrypto-0.1.9/multicrypto/commands/sweepaddress.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,15 @@
             address = convert_wif_private_key_to_address(
                 wif_private_key, coin['address_prefix_bytes'])
     except Exception as e:
         logger.error(e)
         return
     if not coin.get('api'):
         logger.error('No api has been defined for the coin {}'.format(coin_symbol))
+        return
     try:
         utxos = get_utxo_from_private_keys(
             coin=coin,
             wif_private_keys=[wif_private_key],
             minimum_input_threshold=minimum_input_threshold,
             maximum_input_threshold=maximum_input_threshold)
         utxos = [utxo for _, _, utxo in utxos]
```

### Comparing `multicrypto-0.1.8/multicrypto/commands/checkaddress.py` & `multicrypto-0.1.9/multicrypto/commands/checkaddress.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         validate_coin_symbol(coin_symbol)
         validate_address(address, coin_symbol)
     except Exception as e:
         logger.error(e)
         return
     if not coins[coin_symbol].get('api'):
         logger.error('No api has been defined for the coin {}'.format(coin_symbol))
+        return
 
     try:
         utxos = get_utxo_from_address(coins[coin_symbol], address, minimum_input_threshold,
                                       maximum_input_threshold, limit_inputs)
     except Exception as e:
         logger.error(e)
         return
```

### Comparing `multicrypto-0.1.8/multicrypto/commands/transaddress.py` & `multicrypto-0.1.9/multicrypto/commands/transaddress.py`

 * *Files identical despite different names*

### Comparing `multicrypto-0.1.8/multicrypto/utils.py` & `multicrypto-0.1.9/multicrypto/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,48 @@
 import argparse
 import hashlib
 from binascii import unhexlify
 
 from fastecdsa.curve import secp256k1
+from fastecdsa.point import Point
+
+P = secp256k1.p  # curve prime value
+A = secp256k1.a  # curve coefficient
+B = secp256k1.b  # curve coefficient
+
+
+def decode_point(encoded_point):
+    if isinstance(encoded_point, bytes):
+        encoded_point = encoded_point.hex()
+    if len(encoded_point) == 130:  # uncompressed
+        x = int(encoded_point[2:66], 16)
+        y = int(encoded_point[66:130], 16)
+        return Point(x=x, y=y, curve=secp256k1)
+    elif len(encoded_point) == 66:  # compressed
+        x = int(encoded_point[2:66], 16)
+        beta = pow(x**3 + A * x + B, (P + 1) // 4, P)
+        if (beta + int(encoded_point[:2], 16)) % 2:
+            y = P - beta
+        else:
+            y = beta
+        return Point(x=x, y=y, curve=secp256k1)
+    else:
+        raise Exception('Unrecognized point format')
+
+
+def encode_point(point, compressed, output_format='bytes'):
+    if compressed:
+        encoded_point = bytes([2 + (point.y % 2)]) + point.x.to_bytes(32, byteorder='big')
+    else:
+        encoded_point = b'\x04' + point.x.to_bytes(32, byteorder='big') + \
+            point.y.to_bytes(32, byteorder='big')
+    if output_format == 'hex':
+        return encoded_point.hex()
+    else:
+        return encoded_point
 
 
 def int_to_bytes(integer, byteorder):
     return integer.to_bytes((integer.bit_length() + 7) // 8, byteorder=byteorder)
 
 
 def hex_to_bytes(hex_value, byteorder):
```

### Comparing `multicrypto-0.1.8/multicrypto/address.py` & `multicrypto-0.1.9/multicrypto/address.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,16 @@
 import hashlib
 
 from fastecdsa.curve import secp256k1
 
 from multicrypto.base58 import bytes_to_base58, base58_to_int, base58_to_bytes, validate_base58
 from multicrypto.coins import coins
-from multicrypto.utils import double_sha256
+from multicrypto.utils import double_sha256, encode_point
 
 G = secp256k1.G  # generator point
-N = secp256k1.q  # order of the curve
-
-
-def get_encoded_point(point, compressed):
-    if compressed:
-        return bytes([2 + (point.y % 2)]) + point.x.to_bytes(32, byteorder='big')
-    else:
-        return b'\x04' + point.x.to_bytes(32, byteorder='big') + \
-               point.y.to_bytes(32, byteorder='big')
 
 
 def convert_private_key_to_address(private_key, address_prefix_bytes, compressed=True):
     public_key = G * private_key
     return convert_public_key_to_address(public_key, address_prefix_bytes, compressed)
 
 
@@ -42,15 +33,15 @@
     if not input_data.startswith(address_prefix_bytes):
         raise Exception('Incorrect address prefix')
     digest = input_data[len(address_prefix_bytes):]
     return digest
 
 
 def calculate_public_key_hash(public_key, compressed=True, segwit=False):
-    encoded_public_key = get_encoded_point(public_key, compressed)
+    encoded_public_key = encode_point(public_key, compressed)
     hashed_public_key = hashlib.sha256(encoded_public_key).digest()
     digest = hashlib.new('ripemd160', hashed_public_key).digest()
     if segwit:
         redeem_script = b'\x00\x14' + digest
         hashed_script = hashlib.sha256(redeem_script).digest()
         digest = hashlib.new('ripemd160', hashed_script).digest()
     return digest
```

### Comparing `multicrypto-0.1.8/multicrypto/consts.py` & `multicrypto-0.1.9/multicrypto/consts.py`

 * *Files identical despite different names*

### Comparing `multicrypto-0.1.8/multicrypto/coins.py` & `multicrypto-0.1.9/multicrypto/coins.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,28 +3,31 @@
              'script_prefix_bytes': b'\x1c'},
     'BTC': {'name': 'bitcoin', 'address_prefix_bytes': b'\x00', 'secret_prefix_bytes': b'\x80',
             'script_prefix_bytes': b'\x05', 'api': [
                 {'utxo': 'https://insight.bitpay.com/api/addr/{}/utxo',
                  'send': 'https://insight.bitpay.com/api/tx/send'}]
             },
     'BTG': {'name': 'bitcoin gold', 'address_prefix_bytes': b'\x26', 'secret_prefix_bytes': b'\x80',
-            'script_prefix_bytes': b'\x17'},
+            'script_prefix_bytes': b'\x17', 'sig_hash': b'\x41', 'api': [
+                {'utxo': 'https://explorer.bitcoingold.org/insight-api/addr/{}/utxo',
+                 'send': 'https://explorer.bitcoingold.org/insight-api/tx/send'}]
+            },
     'BITS': {'name': 'bitstar', 'address_prefix_bytes': b'\x19', 'secret_prefix_bytes': b'\x99',
              'script_prefix_bytes': b'\x08'},
     'BTCH': {'name': 'bitcoin hush', 'address_prefix_bytes': b'\x3c',
              'secret_prefix_bytes': b'\xbc', 'script_prefix_bytes': b'\x55'},
     'BTCP': {'name': 'bitcoin private', 'address_prefix_bytes': b'\x13\x25',
              'secret_prefix_bytes': b'\x80', 'script_prefix_bytes': b'\x13\xaf',
-             'sig_hash': b'x\41', 'api': [
-                 {'utxo': 'https://explorer.btcprivate.org/api/addr{}/utxo',
+             'sig_hash': b'\x41', 'api': [
+                 {'utxo': 'https://explorer.btcprivate.org/api/addr/{}/utxo',
                   'send': 'https://explorer.btcprivate.org/api/tx/send'}]
              },
     'BTCZ': {'name': 'bitcoinz', 'address_prefix_bytes': b'\x1c\xb8',
              'secret_prefix_bytes': b'\x80', 'script_prefix_bytes': b'\x1c\xbd', 'api': [
-                 {'utxo': 'https://explorer.btcz.rocks/api/addr{}/utxo',
+                 {'utxo': 'https://explorer.btcz.rocks/api/addr/{}/utxo',
                   'send': 'https://explorer.btcz.rocks/api/tx/send'}]
              },
     'BUCK': {'name': 'buck', 'address_prefix_bytes': b'\x1c\xb8',
              'secret_prefix_bytes': b'\x80', 'script_prefix_bytes': b'\x1c\xbd'},
     'CRAVE': {'name': 'crave', 'address_prefix_bytes': b'\x46', 'secret_prefix_bytes': b'\x99',
               'script_prefix_bytes': b'\x55'},
     'DASH': {'name': 'dash', 'address_prefix_bytes': b'\x4c', 'secret_prefix_bytes': b'\xcc',
@@ -37,15 +40,18 @@
              'script_prefix_bytes': b'\x1c\xbd', 'api': [
                  {'utxo': 'https://explorer.myhush.org/api/addr/{}/utxo',
                   'send': 'https://explorer.myhush.org/api/tx/send'}]
              },
     'KMD': {'name': 'komodo', 'address_prefix_bytes': b'\x3c', 'secret_prefix_bytes': b'\xbc',
             'script_prefix_bytes': b'\x55'},
     'LTC': {'name': 'litecoin', 'address_prefix_bytes': b'\x30', 'secret_prefix_bytes': b'\xb0',
-            'script_prefix_bytes': b'\x05'},
+            'script_prefix_bytes': b'\x05', 'api': [
+                {'utxo': 'https://insight.litecore.io/api/addr/{}/utxo',
+                 'send': 'https://insight.litecore.io/api/tx/send'}]
+            },
     'LTZ': {'name': 'litecoinz', 'address_prefix_bytes': b'\x0a\xb3',
             'secret_prefix_bytes': b'\xb0', 'script_prefix_bytes': b'\x0a\xb8'},
     'MOON': {'name': 'mooncoin', 'address_prefix_bytes': b'\x03', 'secret_prefix_bytes': b'\x83',
              'script_prefix_bytes': b'\x32'},
     'QTUM': {'name': 'qtum', 'address_prefix_bytes': b'\x3a', 'secret_prefix_bytes': b'\x80',
              'script_prefix_bytes': b'\x32'},
     'SAFE': {'name': 'safecoin', 'address_prefix_bytes': b'\x3d', 'secret_prefix_bytes': b'\xbd',
@@ -62,18 +68,26 @@
              'script_prefix_bytes': b'\x32'},
     'SMART': {'name': 'smartcash', 'address_prefix_bytes': b'\x3f', 'secret_prefix_bytes': b'\xbf',
               'script_prefix_bytes': b'\x12'},
     'UNIFY': {'name': 'unify', 'address_prefix_bytes': b'\x44', 'secret_prefix_bytes': b'\x80',
               'script_prefix_bytes': b'\x05'},
     'UNO': {'name': 'unobtanium', 'address_prefix_bytes': b'\x82', 'secret_prefix_bytes': b'\xe0',
             'script_prefix_bytes': b'\x1e'},
+    'VOT': {'name': 'votecoin', 'address_prefix_bytes': b'\x1c\xb8', 'secret_prefix_bytes': b'\x80',
+            'script_prefix_bytes': b'\x1c\xbd', 'api': [
+                {'utxo': 'http://explorer.votecoin.site/insight-api-zcash/addr/{}/utxo',
+                 'send': 'http://explorer.votecoin.site/insight-api-zcash/tx/send'}]
+            },
     'VTC': {'name': 'vertcoin', 'address_prefix_bytes': b'\x47', 'secret_prefix_bytes': b'\x80',
             'script_prefix_bytes': b'\x05'},
     'ZEC': {'name': 'zcash', 'address_prefix_bytes': b'\x1c\xb8', 'secret_prefix_bytes': b'\x80',
-            'script_prefix_bytes': b'\x1c\xbd'},
+            'script_prefix_bytes': b'\x1c\xbd', 'api': [
+                {'utxo': 'https://zcash.blockexplorer.com/api/addr/{}/utxo',
+                 'send': 'https://zcash.blockexplorer.com/api/tx/send'}]
+            },
     'ZCL': {'name': 'zclassic', 'address_prefix_bytes': b'\x1c\xb8',
             'secret_prefix_bytes': b'\x80', 'script_prefix_bytes': b'\x1c\xbd', 'api': [
                 {'utxo': 'http://explorer.zclmine.pro/insight-api-zcash/addr/{}/utxo',
                  'send': 'http://explorer.zclmine.pro/insight-api-zcash/tx/send'}]
             },
     'ZEIT': {'name': 'zeit', 'address_prefix_bytes': b'\x33', 'secret_prefix_bytes': b'\x80',
              'script_prefix_bytes': b'\x08'},
```

### Comparing `multicrypto-0.1.8/multicrypto/ethaddress.py` & `multicrypto-0.1.9/multicrypto/ethaddress.py`

 * *Files identical despite different names*

### Comparing `multicrypto-0.1.8/multicrypto/base58.py` & `multicrypto-0.1.9/multicrypto/base58.py`

 * *Files identical despite different names*

