# Comparing `tmp/dexhub-0.6.5.tar.gz` & `tmp/dexhub-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexhub-0.6.5.tar", last modified: Tue May  2 19:52:01 2023, max compression
+gzip compressed data, was "dexhub-0.6.6.tar", last modified: Tue May  2 22:19:46 2023, max compression
```

## Comparing `dexhub-0.6.5.tar` & `dexhub-0.6.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.819816 dexhub-0.6.5/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-02 19:52:01.819671 dexhub-0.6.5/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.6.5/README.md
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.815917 dexhub-0.6.5/dexhub/
--rw-r--r--   0 czhong     (501) staff       (20)     1207 2023-05-02 19:50:21.000000 dexhub-0.6.5/dexhub/__init__.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.817914 dexhub-0.6.5/dexhub/abi/
--rw-r--r--   0 czhong     (501) staff       (20)      250 2023-05-01 18:43:45.000000 dexhub-0.6.5/dexhub/abi/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.6.5/dexhub/abi/arbitrum_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.6.5/dexhub/abi/avax_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    22419 2023-03-03 18:30:32.000000 dexhub-0.6.5/dexhub/abi/dfk_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.6.5/dexhub/abi/eth_abi.py
--rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.6.5/dexhub/abi/klay_abi.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.818778 dexhub-0.6.5/dexhub/address/
--rw-r--r--   0 czhong     (501) staff       (20)      482 2023-05-01 18:42:42.000000 dexhub-0.6.5/dexhub/address/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.6.5/dexhub/address/arbitrum_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.6.5/dexhub/address/avax_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     4539 2023-03-09 16:49:05.000000 dexhub-0.6.5/dexhub/address/dfk_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.6.5/dexhub/address/eth_address.py
--rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.6.5/dexhub/address/klay_address.py
--rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.6.5/dexhub/address/polygon_address.py
--rw-r--r--   0 czhong     (501) staff       (20)   141917 2023-04-01 13:32:00.000000 dexhub-0.6.5/dexhub/dex.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.819032 dexhub-0.6.5/dexhub/interface/
--rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.6.5/dexhub/interface/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.6.5/dexhub/interface/joe.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.819454 dexhub-0.6.5/dexhub/util/
--rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.6.5/dexhub/util/__init__.py
--rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.6.5/dexhub/util/helper.py
--rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.6.5/dexhub/util/joe_v2.py
-drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 19:52:01.816674 dexhub-0.6.5/dexhub.egg-info/
--rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/PKG-INFO
--rw-r--r--   0 czhong     (501) staff       (20)      679 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/SOURCES.txt
--rw-r--r--   0 czhong     (501) staff       (20)        1 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/dependency_links.txt
--rw-r--r--   0 czhong     (501) staff       (20)        5 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/requires.txt
--rw-r--r--   0 czhong     (501) staff       (20)        7 2023-05-02 19:52:01.000000 dexhub-0.6.5/dexhub.egg-info/top_level.txt
--rw-r--r--   0 czhong     (501) staff       (20)       38 2023-05-02 19:52:01.819862 dexhub-0.6.5/setup.cfg
--rw-r--r--   0 czhong     (501) staff       (20)      609 2023-05-02 19:51:23.000000 dexhub-0.6.5/setup.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 22:19:46.971001 dexhub-0.6.6/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-02 22:19:46.970375 dexhub-0.6.6/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      175 2022-09-19 20:57:53.000000 dexhub-0.6.6/README.md
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 22:19:46.959412 dexhub-0.6.6/dexhub/
+-rw-r--r--   0 czhong     (501) staff       (20)     1207 2023-05-02 19:50:21.000000 dexhub-0.6.6/dexhub/__init__.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 22:19:46.966274 dexhub-0.6.6/dexhub/abi/
+-rw-r--r--   0 czhong     (501) staff       (20)      250 2023-05-01 18:43:45.000000 dexhub-0.6.6/dexhub/abi/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66121 2023-05-01 18:41:59.000000 dexhub-0.6.6/dexhub/abi/arbitrum_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)   120303 2023-05-02 03:17:30.000000 dexhub-0.6.6/dexhub/abi/avax_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    22419 2023-03-03 18:30:32.000000 dexhub-0.6.6/dexhub/abi/dfk_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    44719 2023-04-13 14:46:59.000000 dexhub-0.6.6/dexhub/abi/eth_abi.py
+-rw-r--r--   0 czhong     (501) staff       (20)    32710 2023-03-03 18:30:54.000000 dexhub-0.6.6/dexhub/abi/klay_abi.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 22:19:46.968360 dexhub-0.6.6/dexhub/address/
+-rw-r--r--   0 czhong     (501) staff       (20)      482 2023-05-01 18:42:42.000000 dexhub-0.6.6/dexhub/address/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1333 2023-05-01 18:38:02.000000 dexhub-0.6.6/dexhub/address/arbitrum_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1763 2023-05-01 18:23:53.000000 dexhub-0.6.6/dexhub/address/avax_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     4539 2023-03-09 16:49:05.000000 dexhub-0.6.6/dexhub/address/dfk_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      963 2023-04-10 17:04:00.000000 dexhub-0.6.6/dexhub/address/eth_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)     1339 2023-03-23 18:27:21.000000 dexhub-0.6.6/dexhub/address/klay_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)      709 2023-03-14 13:50:18.000000 dexhub-0.6.6/dexhub/address/polygon_address.py
+-rw-r--r--   0 czhong     (501) staff       (20)   142189 2023-05-02 22:19:30.000000 dexhub-0.6.6/dexhub/dex.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 22:19:46.969075 dexhub-0.6.6/dexhub/interface/
+-rw-r--r--   0 czhong     (501) staff       (20)       88 2023-04-27 19:25:48.000000 dexhub-0.6.6/dexhub/interface/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    66768 2023-04-27 19:19:07.000000 dexhub-0.6.6/dexhub/interface/joe.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 22:19:46.969910 dexhub-0.6.6/dexhub/util/
+-rw-r--r--   0 czhong     (501) staff       (20)       83 2023-05-02 19:50:16.000000 dexhub-0.6.6/dexhub/util/__init__.py
+-rw-r--r--   0 czhong     (501) staff       (20)    14052 2023-05-01 20:35:46.000000 dexhub-0.6.6/dexhub/util/helper.py
+-rw-r--r--   0 czhong     (501) staff       (20)      471 2023-05-02 19:50:10.000000 dexhub-0.6.6/dexhub/util/joe_v2.py
+drwxr-xr-x   0 czhong     (501) staff       (20)        0 2023-05-02 22:19:46.960075 dexhub-0.6.6/dexhub.egg-info/
+-rw-r--r--   0 czhong     (501) staff       (20)      515 2023-05-02 22:19:46.000000 dexhub-0.6.6/dexhub.egg-info/PKG-INFO
+-rw-r--r--   0 czhong     (501) staff       (20)      679 2023-05-02 22:19:46.000000 dexhub-0.6.6/dexhub.egg-info/SOURCES.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        1 2023-05-02 22:19:46.000000 dexhub-0.6.6/dexhub.egg-info/dependency_links.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        5 2023-05-02 22:19:46.000000 dexhub-0.6.6/dexhub.egg-info/requires.txt
+-rw-r--r--   0 czhong     (501) staff       (20)        7 2023-05-02 22:19:46.000000 dexhub-0.6.6/dexhub.egg-info/top_level.txt
+-rw-r--r--   0 czhong     (501) staff       (20)       38 2023-05-02 22:19:46.971059 dexhub-0.6.6/setup.cfg
+-rw-r--r--   0 czhong     (501) staff       (20)      609 2023-05-02 22:19:43.000000 dexhub-0.6.6/setup.py
```

### Comparing `dexhub-0.6.5/PKG-INFO` & `dexhub-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.6.5
+Version: 0.6.6
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.6.5/dexhub/__init__.py` & `dexhub-0.6.6/dexhub/__init__.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/abi/arbitrum_abi.py` & `dexhub-0.6.6/dexhub/abi/arbitrum_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/abi/avax_abi.py` & `dexhub-0.6.6/dexhub/abi/avax_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/abi/dfk_abi.py` & `dexhub-0.6.6/dexhub/abi/dfk_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/abi/eth_abi.py` & `dexhub-0.6.6/dexhub/abi/eth_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/abi/klay_abi.py` & `dexhub-0.6.6/dexhub/abi/klay_abi.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/address/arbitrum_address.py` & `dexhub-0.6.6/dexhub/address/arbitrum_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/address/avax_address.py` & `dexhub-0.6.6/dexhub/address/avax_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/address/dfk_address.py` & `dexhub-0.6.6/dexhub/address/dfk_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/address/eth_address.py` & `dexhub-0.6.6/dexhub/address/eth_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/address/klay_address.py` & `dexhub-0.6.6/dexhub/address/klay_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/address/polygon_address.py` & `dexhub-0.6.6/dexhub/address/polygon_address.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/dex.py` & `dexhub-0.6.6/dexhub/dex.py`

 * *Files 0% similar despite different names*

```diff
@@ -2816,6055 +2816,6072 @@
 0000aff0: 5469 6d65 5374 616d 703d 7061 6972 436f  TimeStamp=pairCo
 0000b000: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
 0000b010: 2e67 6574 5265 7365 7276 6573 2829 2e63  .getReserves().c
 0000b020: 616c 6c28 290a 2020 2020 2020 2020 7265  all().        re
 0000b030: 7475 726e 2072 6573 6572 7665 302c 7265  turn reserve0,re
 0000b040: 7365 7276 6531 2c62 6c6f 636b 5469 6d65  serve1,blockTime
 0000b050: 5374 616d 700a 0a20 2020 2064 6566 2067  Stamp..    def g
-0000b060: 6574 5f70 6169 725f 696e 666f 2873 656c  et_pair_info(sel
-0000b070: 662c 7061 6972 5f61 6464 7265 7373 293a  f,pair_address):
-0000b080: 0a20 2020 2020 2020 2070 6169 7243 6f6e  .        pairCon
-0000b090: 7472 6163 743d 7365 6c66 2e77 6562 332e  tract=self.web3.
-0000b0a0: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
-0000b0b0: 7265 7373 3d70 6169 725f 6164 6472 6573  ress=pair_addres
-0000b0c0: 732c 2061 6269 3d73 656c 662e 7061 6972  s, abi=self.pair
-0000b0d0: 5f61 6269 290a 2020 2020 2020 2020 746f  _abi).        to
-0000b0e0: 6b65 6e30 4164 6472 6573 733d 7061 6972  ken0Address=pair
-0000b0f0: 436f 6e74 7261 6374 2e66 756e 6374 696f  Contract.functio
-0000b100: 6e73 2e74 6f6b 656e 3028 292e 6361 6c6c  ns.token0().call
-0000b110: 2829 0a20 2020 2020 2020 2074 6f6b 656e  ().        token
-0000b120: 3141 6464 7265 7373 3d70 6169 7243 6f6e  1Address=pairCon
-0000b130: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
-0000b140: 746f 6b65 6e31 2829 2e63 616c 6c28 290a  token1().call().
-0000b150: 2020 2020 2020 2020 7265 7365 7276 6530          reserve0
-0000b160: 2c72 6573 6572 7665 312c 626c 6f63 6b54  ,reserve1,blockT
-0000b170: 696d 6553 7461 6d70 3d70 6169 7243 6f6e  imeStamp=pairCon
-0000b180: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
-0000b190: 6765 7452 6573 6572 7665 7328 292e 6361  getReserves().ca
-0000b1a0: 6c6c 2829 0a20 2020 2020 2020 2023 2074  ll().        # t
-0000b1b0: 6f6b 656e 305f 636f 6e74 7261 6374 3d73  oken0_contract=s
-0000b1c0: 656c 662e 7765 6233 2e65 7468 2e63 6f6e  elf.web3.eth.con
-0000b1d0: 7472 6163 7428 6164 6472 6573 733d 746f  tract(address=to
-0000b1e0: 6b65 6e30 4164 6472 6573 732c 2061 6269  ken0Address, abi
-0000b1f0: 3d73 656c 662e 6572 6332 305f 6162 6929  =self.erc20_abi)
-0000b200: 0a20 2020 2020 2020 2023 2074 6f6b 656e  .        # token
-0000b210: 315f 636f 6e74 7261 6374 3d73 656c 662e  1_contract=self.
-0000b220: 7765 6233 2e65 7468 2e63 6f6e 7472 6163  web3.eth.contrac
-0000b230: 7428 6164 6472 6573 733d 746f 6b65 6e31  t(address=token1
-0000b240: 4164 6472 6573 732c 2061 6269 3d73 656c  Address, abi=sel
-0000b250: 662e 6572 6332 305f 6162 6929 0a20 2020  f.erc20_abi).   
-0000b260: 2020 2020 2023 2074 6f6b 656e 305f 6e61       # token0_na
-0000b270: 6d65 3d74 6f6b 656e 305f 636f 6e74 7261  me=token0_contra
-0000b280: 6374 2e66 756e 6374 696f 6e73 2e6e 616d  ct.functions.nam
-0000b290: 6528 292e 6361 6c6c 2829 0a20 2020 2020  e().call().     
-0000b2a0: 2020 2023 2074 6f6b 656e 315f 6e61 6d65     # token1_name
-0000b2b0: 3d74 6f6b 656e 315f 636f 6e74 7261 6374  =token1_contract
-0000b2c0: 2e66 756e 6374 696f 6e73 2e6e 616d 6528  .functions.name(
-0000b2d0: 292e 6361 6c6c 2829 0a20 2020 2020 2020  ).call().       
-0000b2e0: 2070 7269 6365 303d 7265 7365 7276 6531   price0=reserve1
-0000b2f0: 2f72 6573 6572 7665 300a 2020 2020 2020  /reserve0.      
-0000b300: 2020 7072 6963 6531 3d72 6573 6572 7665    price1=reserve
-0000b310: 302f 7265 7365 7276 6531 0a20 2020 2020  0/reserve1.     
-0000b320: 2020 2023 2070 7269 6e74 2822 746f 6b65     # print("toke
-0000b330: 6e30 3a22 2c73 7472 2874 6f6b 656e 3041  n0:",str(token0A
-0000b340: 6464 7265 7373 292c 222d 2d6e 616d 653a  ddress),"--name:
-0000b350: 222c 7374 7228 746f 6b65 6e30 5f6e 616d  ",str(token0_nam
-0000b360: 6529 2c22 2d2d 7072 6963 653a 222c 7374  e),"--price:",st
-0000b370: 7228 7072 6963 6530 2929 0a20 2020 2020  r(price0)).     
-0000b380: 2020 2023 2070 7269 6e74 2822 746f 6b65     # print("toke
-0000b390: 6e31 3a22 2c73 7472 2874 6f6b 656e 3141  n1:",str(token1A
-0000b3a0: 6464 7265 7373 292c 222d 2d6e 616d 653a  ddress),"--name:
-0000b3b0: 222c 7374 7228 746f 6b65 6e31 5f6e 616d  ",str(token1_nam
-0000b3c0: 6529 2c22 2d2d 7072 6963 653a 222c 7374  e),"--price:",st
-0000b3d0: 7228 7072 6963 6531 2929 0a20 2020 2020  r(price1)).     
-0000b3e0: 2020 2023 2070 7269 6e74 2822 7265 7365     # print("rese
-0000b3f0: 7276 6530 222c 7374 7228 7265 7365 7276  rve0",str(reserv
-0000b400: 6530 2929 0a20 2020 2020 2020 2023 2070  e0)).        # p
-0000b410: 7269 6e74 2822 7265 7365 7276 6531 222c  rint("reserve1",
-0000b420: 7374 7228 7265 7365 7276 6531 2929 0a20  str(reserve1)). 
-0000b430: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
-0000b440: 626c 6f63 6b54 696d 6553 7461 6d70 222c  blockTimeStamp",
-0000b450: 7374 7228 626c 6f63 6b54 696d 6553 7461  str(blockTimeSta
-0000b460: 6d70 2929 0a20 2020 2020 2020 2072 6574  mp)).        ret
-0000b470: 7572 6e20 746f 6b65 6e30 4164 6472 6573  urn token0Addres
-0000b480: 732c 7265 7365 7276 6530 2c74 6f6b 656e  s,reserve0,token
-0000b490: 3141 6464 7265 7373 2c72 6573 6572 7665  1Address,reserve
-0000b4a0: 312c 626c 6f63 6b54 696d 6553 7461 6d70  1,blockTimeStamp
-0000b4b0: 2c70 7269 6365 302c 7072 6963 6531 0a0a  ,price0,price1..
-0000b4c0: 636c 6173 7320 556e 6973 7761 7056 333a  class UniswapV3:
-0000b4d0: 0a20 2020 2023 6874 7470 733a 2f2f 6574  .    #https://et
-0000b4e0: 6865 7273 6361 6e2e 696f 2f61 6464 7265  herscan.io/addre
-0000b4f0: 7373 2f30 7831 6639 3834 3331 6338 6164  ss/0x1f98431c8ad
-0000b500: 3938 3532 3336 3331 6165 3461 3539 6632  98523631ae4a59f2
-0000b510: 3637 3334 3665 6133 3166 3938 340a 2020  67346ea31f984.  
-0000b520: 2020 756e 6973 7761 705f 7633 5f66 6163    uniswap_v3_fac
-0000b530: 746f 7279 5f61 6269 3d27 5b7b 2269 6e70  tory_abi='[{"inp
-0000b540: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
-0000b550: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
-0000b560: 7961 626c 6522 2c22 7479 7065 223a 2263  yable","type":"c
-0000b570: 6f6e 7374 7275 6374 6f72 227d 2c7b 2261  onstructor"},{"a
-0000b580: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
-0000b590: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
-0000b5a0: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
-0000b5b0: 6e61 6c54 7970 6522 3a22 7569 6e74 3234  nalType":"uint24
-0000b5c0: 222c 226e 616d 6522 3a22 6665 6522 2c22  ","name":"fee","
-0000b5d0: 7479 7065 223a 2275 696e 7432 3422 7d2c  type":"uint24"},
-0000b5e0: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
-0000b5f0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000b600: 696e 7432 3422 2c22 6e61 6d65 223a 2274  int24","name":"t
-0000b610: 6963 6b53 7061 6369 6e67 222c 2274 7970  ickSpacing","typ
-0000b620: 6522 3a22 696e 7432 3422 7d5d 2c22 6e61  e":"int24"}],"na
-0000b630: 6d65 223a 2246 6565 416d 6f75 6e74 456e  me":"FeeAmountEn
-0000b640: 6162 6c65 6422 2c22 7479 7065 223a 2265  abled","type":"e
-0000b650: 7665 6e74 227d 2c7b 2261 6e6f 6e79 6d6f  vent"},{"anonymo
-0000b660: 7573 223a 6661 6c73 652c 2269 6e70 7574  us":false,"input
-0000b670: 7322 3a5b 7b22 696e 6465 7865 6422 3a74  s":[{"indexed":t
-0000b680: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
-0000b690: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0000b6a0: 6d65 223a 226f 6c64 4f77 6e65 7222 2c22  me":"oldOwner","
-0000b6b0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0000b6c0: 2c7b 2269 6e64 6578 6564 223a 7472 7565  ,{"indexed":true
-0000b6d0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0000b6e0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0000b6f0: 3a22 6e65 774f 776e 6572 222c 2274 7970  :"newOwner","typ
-0000b700: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-0000b710: 6e61 6d65 223a 224f 776e 6572 4368 616e  name":"OwnerChan
-0000b720: 6765 6422 2c22 7479 7065 223a 2265 7665  ged","type":"eve
-0000b730: 6e74 227d 2c7b 2261 6e6f 6e79 6d6f 7573  nt"},{"anonymous
-0000b740: 223a 6661 6c73 652c 2269 6e70 7574 7322  ":false,"inputs"
-0000b750: 3a5b 7b22 696e 6465 7865 6422 3a74 7275  :[{"indexed":tru
-0000b760: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0000b770: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-0000b780: 223a 2274 6f6b 656e 3022 2c22 7479 7065  ":"token0","type
-0000b790: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0000b7a0: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
-0000b7b0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0000b7c0: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
-0000b7d0: 6b65 6e31 222c 2274 7970 6522 3a22 6164  ken1","type":"ad
-0000b7e0: 6472 6573 7322 7d2c 7b22 696e 6465 7865  dress"},{"indexe
-0000b7f0: 6422 3a74 7275 652c 2269 6e74 6572 6e61  d":true,"interna
-0000b800: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
-0000b810: 226e 616d 6522 3a22 6665 6522 2c22 7479  "name":"fee","ty
-0000b820: 7065 223a 2275 696e 7432 3422 7d2c 7b22  pe":"uint24"},{"
-0000b830: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
-0000b840: 696e 7465 726e 616c 5479 7065 223a 2269  internalType":"i
-0000b850: 6e74 3234 222c 226e 616d 6522 3a22 7469  nt24","name":"ti
-0000b860: 636b 5370 6163 696e 6722 2c22 7479 7065  ckSpacing","type
-0000b870: 223a 2269 6e74 3234 227d 2c7b 2269 6e64  ":"int24"},{"ind
-0000b880: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-0000b890: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0000b8a0: 6573 7322 2c22 6e61 6d65 223a 2270 6f6f  ess","name":"poo
-0000b8b0: 6c22 2c22 7479 7065 223a 2261 6464 7265  l","type":"addre
-0000b8c0: 7373 227d 5d2c 226e 616d 6522 3a22 506f  ss"}],"name":"Po
-0000b8d0: 6f6c 4372 6561 7465 6422 2c22 7479 7065  olCreated","type
-0000b8e0: 223a 2265 7665 6e74 227d 2c7b 2269 6e70  ":"event"},{"inp
-0000b8f0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0000b900: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-0000b910: 226e 616d 6522 3a22 746f 6b65 6e41 222c  "name":"tokenA",
-0000b920: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0000b930: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0000b940: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0000b950: 6522 3a22 746f 6b65 6e42 222c 2274 7970  e":"tokenB","typ
-0000b960: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0000b970: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0000b980: 696e 7432 3422 2c22 6e61 6d65 223a 2266  int24","name":"f
-0000b990: 6565 222c 2274 7970 6522 3a22 7569 6e74  ee","type":"uint
-0000b9a0: 3234 227d 5d2c 226e 616d 6522 3a22 6372  24"}],"name":"cr
-0000b9b0: 6561 7465 506f 6f6c 222c 226f 7574 7075  eatePool","outpu
-0000b9c0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0000b9d0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0000b9e0: 6e61 6d65 223a 2270 6f6f 6c22 2c22 7479  name":"pool","ty
-0000b9f0: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
-0000ba00: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000ba10: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
-0000ba20: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-0000ba30: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-0000ba40: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0000ba50: 6e74 3234 222c 226e 616d 6522 3a22 6665  nt24","name":"fe
-0000ba60: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
-0000ba70: 3422 7d2c 7b22 696e 7465 726e 616c 5479  4"},{"internalTy
-0000ba80: 7065 223a 2269 6e74 3234 222c 226e 616d  pe":"int24","nam
-0000ba90: 6522 3a22 7469 636b 5370 6163 696e 6722  e":"tickSpacing"
-0000baa0: 2c22 7479 7065 223a 2269 6e74 3234 227d  ,"type":"int24"}
-0000bab0: 5d2c 226e 616d 6522 3a22 656e 6162 6c65  ],"name":"enable
-0000bac0: 4665 6541 6d6f 756e 7422 2c22 6f75 7470  FeeAmount","outp
-0000bad0: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
-0000bae0: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
-0000baf0: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-0000bb00: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-0000bb10: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0000bb20: 7970 6522 3a22 7569 6e74 3234 222c 226e  ype":"uint24","n
-0000bb30: 616d 6522 3a22 222c 2274 7970 6522 3a22  ame":"","type":"
-0000bb40: 7569 6e74 3234 227d 5d2c 226e 616d 6522  uint24"}],"name"
-0000bb50: 3a22 6665 6541 6d6f 756e 7454 6963 6b53  :"feeAmountTickS
-0000bb60: 7061 6369 6e67 222c 226f 7574 7075 7473  pacing","outputs
-0000bb70: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0000bb80: 6522 3a22 696e 7432 3422 2c22 6e61 6d65  e":"int24","name
-0000bb90: 223a 2222 2c22 7479 7065 223a 2269 6e74  ":"","type":"int
-0000bba0: 3234 227d 5d2c 2273 7461 7465 4d75 7461  24"}],"stateMuta
-0000bbb0: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-0000bbc0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-0000bbd0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-0000bbe0: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-0000bbf0: 6472 6573 7322 2c22 6e61 6d65 223a 2222  dress","name":""
-0000bc00: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0000bc10: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0000bc20: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0000bc30: 6d65 223a 2222 2c22 7479 7065 223a 2261  me":"","type":"a
-0000bc40: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-0000bc50: 6e61 6c54 7970 6522 3a22 7569 6e74 3234  nalType":"uint24
-0000bc60: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-0000bc70: 6522 3a22 7569 6e74 3234 227d 5d2c 226e  e":"uint24"}],"n
-0000bc80: 616d 6522 3a22 6765 7450 6f6f 6c22 2c22  ame":"getPool","
-0000bc90: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-0000bca0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0000bcb0: 7373 222c 226e 616d 6522 3a22 222c 2274  ss","name":"","t
-0000bcc0: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
-0000bcd0: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-0000bce0: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
-0000bcf0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-0000bd00: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-0000bd10: 3a22 6f77 6e65 7222 2c22 6f75 7470 7574  :"owner","output
-0000bd20: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0000bd30: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0000bd40: 616d 6522 3a22 222c 2274 7970 6522 3a22  ame":"","type":"
-0000bd50: 6164 6472 6573 7322 7d5d 2c22 7374 6174  address"}],"stat
-0000bd60: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
-0000bd70: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
-0000bd80: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-0000bd90: 3a5b 5d2c 226e 616d 6522 3a22 7061 7261  :[],"name":"para
-0000bda0: 6d65 7465 7273 222c 226f 7574 7075 7473  meters","outputs
-0000bdb0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0000bdc0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0000bdd0: 6d65 223a 2266 6163 746f 7279 222c 2274  me":"factory","t
-0000bde0: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-0000bdf0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0000be00: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0000be10: 3a22 746f 6b65 6e30 222c 2274 7970 6522  :"token0","type"
-0000be20: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0000be30: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0000be40: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
-0000be50: 6b65 6e31 222c 2274 7970 6522 3a22 6164  ken1","type":"ad
-0000be60: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0000be70: 616c 5479 7065 223a 2275 696e 7432 3422  alType":"uint24"
-0000be80: 2c22 6e61 6d65 223a 2266 6565 222c 2274  ,"name":"fee","t
-0000be90: 7970 6522 3a22 7569 6e74 3234 227d 2c7b  ype":"uint24"},{
-0000bea0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000beb0: 696e 7432 3422 2c22 6e61 6d65 223a 2274  int24","name":"t
-0000bec0: 6963 6b53 7061 6369 6e67 222c 2274 7970  ickSpacing","typ
-0000bed0: 6522 3a22 696e 7432 3422 7d5d 2c22 7374  e":"int24"}],"st
-0000bee0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-0000bef0: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
-0000bf00: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-0000bf10: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0000bf20: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0000bf30: 616d 6522 3a22 5f6f 776e 6572 222c 2274  ame":"_owner","t
-0000bf40: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
-0000bf50: 2c22 6e61 6d65 223a 2273 6574 4f77 6e65  ,"name":"setOwne
-0000bf60: 7222 2c22 6f75 7470 7574 7322 3a5b 5d2c  r","outputs":[],
-0000bf70: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000bf80: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
-0000bf90: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-0000bfa0: 7d5d 270a 2020 2020 756e 6973 7761 705f  }]'.    uniswap_
-0000bfb0: 7633 5f70 6169 725f 6162 693d 275b 207b  v3_pair_abi='[ {
-0000bfc0: 2022 616e 6f6e 796d 6f75 7322 3a20 6661   "anonymous": fa
-0000bfd0: 6c73 652c 2022 696e 7075 7473 223a 205b  lse, "inputs": [
-0000bfe0: 207b 2022 696e 6465 7865 6422 3a20 7472   { "indexed": tr
-0000bff0: 7565 2c20 2269 6e74 6572 6e61 6c54 7970  ue, "internalTyp
-0000c000: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000c010: 6e61 6d65 223a 2022 6f77 6e65 7222 2c20  name": "owner", 
-0000c020: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-0000c030: 2220 7d2c 207b 2022 696e 6465 7865 6422  " }, { "indexed"
-0000c040: 3a20 7472 7565 2c20 2269 6e74 6572 6e61  : true, "interna
-0000c050: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
-0000c060: 222c 2022 6e61 6d65 223a 2022 7370 656e  ", "name": "spen
-0000c070: 6465 7222 2c20 2274 7970 6522 3a20 2261  der", "type": "a
-0000c080: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
-0000c090: 6465 7865 6422 3a20 6661 6c73 652c 2022  dexed": false, "
-0000c0a0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000c0b0: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
-0000c0c0: 3a20 2276 616c 7565 222c 2022 7479 7065  : "value", "type
-0000c0d0: 223a 2022 7569 6e74 3235 3622 207d 205d  ": "uint256" } ]
-0000c0e0: 2c20 226e 616d 6522 3a20 2241 7070 726f  , "name": "Appro
-0000c0f0: 7661 6c22 2c20 2274 7970 6522 3a20 2265  val", "type": "e
-0000c100: 7665 6e74 2220 7d2c 207b 2022 616e 6f6e  vent" }, { "anon
-0000c110: 796d 6f75 7322 3a20 6661 6c73 652c 2022  ymous": false, "
-0000c120: 696e 7075 7473 223a 205b 207b 2022 696e  inputs": [ { "in
-0000c130: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
-0000c140: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
-0000c150: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
-0000c160: 2022 7365 6e64 6572 222c 2022 7479 7065   "sender", "type
-0000c170: 223a 2022 6164 6472 6573 7322 207d 2c20  ": "address" }, 
-0000c180: 7b20 2269 6e64 6578 6564 223a 2066 616c  { "indexed": fal
-0000c190: 7365 2c20 2269 6e74 6572 6e61 6c54 7970  se, "internalTyp
-0000c1a0: 6522 3a20 2275 696e 7432 3536 222c 2022  e": "uint256", "
-0000c1b0: 6e61 6d65 223a 2022 616d 6f75 6e74 3022  name": "amount0"
-0000c1c0: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
-0000c1d0: 3536 2220 7d2c 207b 2022 696e 6465 7865  56" }, { "indexe
-0000c1e0: 6422 3a20 6661 6c73 652c 2022 696e 7465  d": false, "inte
-0000c1f0: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
-0000c200: 3235 3622 2c20 226e 616d 6522 3a20 2261  256", "name": "a
-0000c210: 6d6f 756e 7431 222c 2022 7479 7065 223a  mount1", "type":
-0000c220: 2022 7569 6e74 3235 3622 207d 2c20 7b20   "uint256" }, { 
-0000c230: 2269 6e64 6578 6564 223a 2074 7275 652c  "indexed": true,
-0000c240: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000c250: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
-0000c260: 6522 3a20 2274 6f22 2c20 2274 7970 6522  e": "to", "type"
-0000c270: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
-0000c280: 2022 6e61 6d65 223a 2022 4275 726e 222c   "name": "Burn",
-0000c290: 2022 7479 7065 223a 2022 6576 656e 7422   "type": "event"
-0000c2a0: 207d 2c20 7b20 2261 6e6f 6e79 6d6f 7573   }, { "anonymous
-0000c2b0: 223a 2066 616c 7365 2c20 2269 6e70 7574  ": false, "input
-0000c2c0: 7322 3a20 5b20 7b20 2269 6e64 6578 6564  s": [ { "indexed
-0000c2d0: 223a 2074 7275 652c 2022 696e 7465 726e  ": true, "intern
-0000c2e0: 616c 5479 7065 223a 2022 6164 6472 6573  alType": "addres
-0000c2f0: 7322 2c20 226e 616d 6522 3a20 2273 656e  s", "name": "sen
-0000c300: 6465 7222 2c20 2274 7970 6522 3a20 2261  der", "type": "a
-0000c310: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
-0000c320: 6465 7865 6422 3a20 6661 6c73 652c 2022  dexed": false, "
-0000c330: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000c340: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
-0000c350: 3a20 2261 6d6f 756e 7430 222c 2022 7479  : "amount0", "ty
-0000c360: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
-0000c370: 2c20 7b20 2269 6e64 6578 6564 223a 2066  , { "indexed": f
-0000c380: 616c 7365 2c20 2269 6e74 6572 6e61 6c54  alse, "internalT
-0000c390: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
-0000c3a0: 2022 6e61 6d65 223a 2022 616d 6f75 6e74   "name": "amount
-0000c3b0: 3122 2c20 2274 7970 6522 3a20 2275 696e  1", "type": "uin
-0000c3c0: 7432 3536 2220 7d20 5d2c 2022 6e61 6d65  t256" } ], "name
-0000c3d0: 223a 2022 4d69 6e74 222c 2022 7479 7065  ": "Mint", "type
-0000c3e0: 223a 2022 6576 656e 7422 207d 2c20 7b20  ": "event" }, { 
-0000c3f0: 2261 6e6f 6e79 6d6f 7573 223a 2066 616c  "anonymous": fal
-0000c400: 7365 2c20 2269 6e70 7574 7322 3a20 5b20  se, "inputs": [ 
-0000c410: 7b20 2269 6e64 6578 6564 223a 2074 7275  { "indexed": tru
-0000c420: 652c 2022 696e 7465 726e 616c 5479 7065  e, "internalType
-0000c430: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
-0000c440: 616d 6522 3a20 2273 656e 6465 7222 2c20  ame": "sender", 
-0000c450: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-0000c460: 2220 7d2c 207b 2022 696e 6465 7865 6422  " }, { "indexed"
-0000c470: 3a20 6661 6c73 652c 2022 696e 7465 726e  : false, "intern
-0000c480: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
-0000c490: 3622 2c20 226e 616d 6522 3a20 2261 6d6f  6", "name": "amo
-0000c4a0: 756e 7430 496e 222c 2022 7479 7065 223a  unt0In", "type":
-0000c4b0: 2022 7569 6e74 3235 3622 207d 2c20 7b20   "uint256" }, { 
-0000c4c0: 2269 6e64 6578 6564 223a 2066 616c 7365  "indexed": false
-0000c4d0: 2c20 2269 6e74 6572 6e61 6c54 7970 6522  , "internalType"
-0000c4e0: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
-0000c4f0: 6d65 223a 2022 616d 6f75 6e74 3149 6e22  me": "amount1In"
-0000c500: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
-0000c510: 3536 2220 7d2c 207b 2022 696e 6465 7865  56" }, { "indexe
-0000c520: 6422 3a20 6661 6c73 652c 2022 696e 7465  d": false, "inte
-0000c530: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
-0000c540: 3235 3622 2c20 226e 616d 6522 3a20 2261  256", "name": "a
-0000c550: 6d6f 756e 7430 4f75 7422 2c20 2274 7970  mount0Out", "typ
-0000c560: 6522 3a20 2275 696e 7432 3536 2220 7d2c  e": "uint256" },
-0000c570: 207b 2022 696e 6465 7865 6422 3a20 6661   { "indexed": fa
-0000c580: 6c73 652c 2022 696e 7465 726e 616c 5479  lse, "internalTy
-0000c590: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
-0000c5a0: 226e 616d 6522 3a20 2261 6d6f 756e 7431  "name": "amount1
-0000c5b0: 4f75 7422 2c20 2274 7970 6522 3a20 2275  Out", "type": "u
-0000c5c0: 696e 7432 3536 2220 7d2c 207b 2022 696e  int256" }, { "in
-0000c5d0: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
-0000c5e0: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
-0000c5f0: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
-0000c600: 2022 746f 222c 2022 7479 7065 223a 2022   "to", "type": "
-0000c610: 6164 6472 6573 7322 207d 205d 2c20 226e  address" } ], "n
-0000c620: 616d 6522 3a20 2253 7761 7022 2c20 2274  ame": "Swap", "t
-0000c630: 7970 6522 3a20 2265 7665 6e74 2220 7d2c  ype": "event" },
-0000c640: 207b 2022 616e 6f6e 796d 6f75 7322 3a20   { "anonymous": 
-0000c650: 6661 6c73 652c 2022 696e 7075 7473 223a  false, "inputs":
-0000c660: 205b 207b 2022 696e 6465 7865 6422 3a20   [ { "indexed": 
-0000c670: 6661 6c73 652c 2022 696e 7465 726e 616c  false, "internal
-0000c680: 5479 7065 223a 2022 7569 6e74 3131 3222  Type": "uint112"
-0000c690: 2c20 226e 616d 6522 3a20 2272 6573 6572  , "name": "reser
-0000c6a0: 7665 3022 2c20 2274 7970 6522 3a20 2275  ve0", "type": "u
-0000c6b0: 696e 7431 3132 2220 7d2c 207b 2022 696e  int112" }, { "in
-0000c6c0: 6465 7865 6422 3a20 6661 6c73 652c 2022  dexed": false, "
-0000c6d0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000c6e0: 7569 6e74 3131 3222 2c20 226e 616d 6522  uint112", "name"
-0000c6f0: 3a20 2272 6573 6572 7665 3122 2c20 2274  : "reserve1", "t
-0000c700: 7970 6522 3a20 2275 696e 7431 3132 2220  ype": "uint112" 
-0000c710: 7d20 5d2c 2022 6e61 6d65 223a 2022 5379  } ], "name": "Sy
-0000c720: 6e63 222c 2022 7479 7065 223a 2022 6576  nc", "type": "ev
-0000c730: 656e 7422 207d 2c20 7b20 2261 6e6f 6e79  ent" }, { "anony
-0000c740: 6d6f 7573 223a 2066 616c 7365 2c20 2269  mous": false, "i
-0000c750: 6e70 7574 7322 3a20 5b20 7b20 2269 6e64  nputs": [ { "ind
-0000c760: 6578 6564 223a 2074 7275 652c 2022 696e  exed": true, "in
-0000c770: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-0000c780: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-0000c790: 2266 726f 6d22 2c20 2274 7970 6522 3a20  "from", "type": 
-0000c7a0: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
-0000c7b0: 696e 6465 7865 6422 3a20 7472 7565 2c20  indexed": true, 
-0000c7c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-0000c7d0: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
-0000c7e0: 223a 2022 746f 222c 2022 7479 7065 223a  ": "to", "type":
-0000c7f0: 2022 6164 6472 6573 7322 207d 2c20 7b20   "address" }, { 
-0000c800: 2269 6e64 6578 6564 223a 2066 616c 7365  "indexed": false
-0000c810: 2c20 2269 6e74 6572 6e61 6c54 7970 6522  , "internalType"
-0000c820: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
-0000c830: 6d65 223a 2022 7661 6c75 6522 2c20 2274  me": "value", "t
-0000c840: 7970 6522 3a20 2275 696e 7432 3536 2220  ype": "uint256" 
-0000c850: 7d20 5d2c 2022 6e61 6d65 223a 2022 5472  } ], "name": "Tr
-0000c860: 616e 7366 6572 222c 2022 7479 7065 223a  ansfer", "type":
-0000c870: 2022 6576 656e 7422 207d 2c20 7b20 2269   "event" }, { "i
-0000c880: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
-0000c890: 6522 3a20 2244 4f4d 4149 4e5f 5345 5041  e": "DOMAIN_SEPA
-0000c8a0: 5241 544f 5222 2c20 226f 7574 7075 7473  RATOR", "outputs
-0000c8b0: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-0000c8c0: 5479 7065 223a 2022 6279 7465 7333 3222  Type": "bytes32"
-0000c8d0: 2c20 226e 616d 6522 3a20 2222 2c20 2274  , "name": "", "t
-0000c8e0: 7970 6522 3a20 2262 7974 6573 3332 2220  ype": "bytes32" 
-0000c8f0: 7d20 5d2c 2022 7374 6174 654d 7574 6162  } ], "stateMutab
-0000c900: 696c 6974 7922 3a20 2276 6965 7722 2c20  ility": "view", 
-0000c910: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
-0000c920: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
-0000c930: 3a20 5b5d 2c20 226e 616d 6522 3a20 224d  : [], "name": "M
-0000c940: 494e 494d 554d 5f4c 4951 5549 4449 5459  INIMUM_LIQUIDITY
-0000c950: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
-0000c960: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000c970: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
-0000c980: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
-0000c990: 2022 7569 6e74 3235 3622 207d 205d 2c20   "uint256" } ], 
-0000c9a0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000c9b0: 223a 2022 7075 7265 222c 2022 7479 7065  ": "pure", "type
-0000c9c0: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
-0000c9d0: 207b 2022 696e 7075 7473 223a 205b 5d2c   { "inputs": [],
-0000c9e0: 2022 6e61 6d65 223a 2022 5045 524d 4954   "name": "PERMIT
-0000c9f0: 5f54 5950 4548 4153 4822 2c20 226f 7574  _TYPEHASH", "out
-0000ca00: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
-0000ca10: 726e 616c 5479 7065 223a 2022 6279 7465  rnalType": "byte
-0000ca20: 7333 3222 2c20 226e 616d 6522 3a20 2222  s32", "name": ""
-0000ca30: 2c20 2274 7970 6522 3a20 2262 7974 6573  , "type": "bytes
-0000ca40: 3332 2220 7d20 5d2c 2022 7374 6174 654d  32" } ], "stateM
-0000ca50: 7574 6162 696c 6974 7922 3a20 2270 7572  utability": "pur
-0000ca60: 6522 2c20 2274 7970 6522 3a20 2266 756e  e", "type": "fun
-0000ca70: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
-0000ca80: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
-0000ca90: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
-0000caa0: 7373 222c 2022 6e61 6d65 223a 2022 6f77  ss", "name": "ow
-0000cab0: 6e65 7222 2c20 2274 7970 6522 3a20 2261  ner", "type": "a
-0000cac0: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
-0000cad0: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-0000cae0: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-0000caf0: 2273 7065 6e64 6572 222c 2022 7479 7065  "spender", "type
-0000cb00: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
-0000cb10: 2c20 226e 616d 6522 3a20 2261 6c6c 6f77  , "name": "allow
-0000cb20: 616e 6365 222c 2022 6f75 7470 7574 7322  ance", "outputs"
-0000cb30: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-0000cb40: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
-0000cb50: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
-0000cb60: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
-0000cb70: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
-0000cb80: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
-0000cb90: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
-0000cba0: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
-0000cbb0: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-0000cbc0: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
-0000cbd0: 226e 616d 6522 3a20 2273 7065 6e64 6572  "name": "spender
-0000cbe0: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
-0000cbf0: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
-0000cc00: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
-0000cc10: 3536 222c 2022 6e61 6d65 223a 2022 7661  56", "name": "va
-0000cc20: 6c75 6522 2c20 2274 7970 6522 3a20 2275  lue", "type": "u
-0000cc30: 696e 7432 3536 2220 7d20 5d2c 2022 6e61  int256" } ], "na
-0000cc40: 6d65 223a 2022 6170 7072 6f76 6522 2c20  me": "approve", 
-0000cc50: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
-0000cc60: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000cc70: 626f 6f6c 222c 2022 6e61 6d65 223a 2022  bool", "name": "
-0000cc80: 222c 2022 7479 7065 223a 2022 626f 6f6c  ", "type": "bool
-0000cc90: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
-0000cca0: 6162 696c 6974 7922 3a20 226e 6f6e 7061  ability": "nonpa
-0000ccb0: 7961 626c 6522 2c20 2274 7970 6522 3a20  yable", "type": 
-0000ccc0: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
-0000ccd0: 2269 6e70 7574 7322 3a20 5b20 7b20 2269  "inputs": [ { "i
-0000cce0: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
-0000ccf0: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
-0000cd00: 2022 6f77 6e65 7222 2c20 2274 7970 6522   "owner", "type"
-0000cd10: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
-0000cd20: 2022 6e61 6d65 223a 2022 6261 6c61 6e63   "name": "balanc
-0000cd30: 654f 6622 2c20 226f 7574 7075 7473 223a  eOf", "outputs":
-0000cd40: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-0000cd50: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
-0000cd60: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-0000cd70: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
-0000cd80: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-0000cd90: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
-0000cda0: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
-0000cdb0: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-0000cdc0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000cdd0: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000cde0: 6e61 6d65 223a 2022 746f 222c 2022 7479  name": "to", "ty
-0000cdf0: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
-0000ce00: 205d 2c20 226e 616d 6522 3a20 2262 7572   ], "name": "bur
-0000ce10: 6e22 2c20 226f 7574 7075 7473 223a 205b  n", "outputs": [
-0000ce20: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000ce30: 223a 2022 7569 6e74 3235 3622 2c20 226e  ": "uint256", "n
-0000ce40: 616d 6522 3a20 2261 6d6f 756e 7430 222c  ame": "amount0",
-0000ce50: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
-0000ce60: 3622 207d 2c20 7b20 2269 6e74 6572 6e61  6" }, { "interna
-0000ce70: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
-0000ce80: 222c 2022 6e61 6d65 223a 2022 616d 6f75  ", "name": "amou
-0000ce90: 6e74 3122 2c20 2274 7970 6522 3a20 2275  nt1", "type": "u
-0000cea0: 696e 7432 3536 2220 7d20 5d2c 2022 7374  int256" } ], "st
-0000ceb0: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
-0000cec0: 226e 6f6e 7061 7961 626c 6522 2c20 2274  "nonpayable", "t
-0000ced0: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
-0000cee0: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-0000cef0: 5b5d 2c20 226e 616d 6522 3a20 2264 6563  [], "name": "dec
-0000cf00: 696d 616c 7322 2c20 226f 7574 7075 7473  imals", "outputs
-0000cf10: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-0000cf20: 5479 7065 223a 2022 7569 6e74 3822 2c20  Type": "uint8", 
-0000cf30: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-0000cf40: 6522 3a20 2275 696e 7438 2220 7d20 5d2c  e": "uint8" } ],
-0000cf50: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-0000cf60: 7922 3a20 2270 7572 6522 2c20 2274 7970  y": "pure", "typ
-0000cf70: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
-0000cf80: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
-0000cf90: 2c20 226e 616d 6522 3a20 2266 6163 746f  , "name": "facto
-0000cfa0: 7279 222c 2022 6f75 7470 7574 7322 3a20  ry", "outputs": 
-0000cfb0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000cfc0: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000cfd0: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-0000cfe0: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
-0000cff0: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
-0000d000: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
-0000d010: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-0000d020: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000d030: 5d2c 2022 6e61 6d65 223a 2022 6765 7452  ], "name": "getR
-0000d040: 6573 6572 7665 7322 2c20 226f 7574 7075  eserves", "outpu
-0000d050: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
-0000d060: 616c 5479 7065 223a 2022 7569 6e74 3131  alType": "uint11
-0000d070: 3222 2c20 226e 616d 6522 3a20 2272 6573  2", "name": "res
-0000d080: 6572 7665 3022 2c20 2274 7970 6522 3a20  erve0", "type": 
-0000d090: 2275 696e 7431 3132 2220 7d2c 207b 2022  "uint112" }, { "
-0000d0a0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000d0b0: 7569 6e74 3131 3222 2c20 226e 616d 6522  uint112", "name"
-0000d0c0: 3a20 2272 6573 6572 7665 3122 2c20 2274  : "reserve1", "t
-0000d0d0: 7970 6522 3a20 2275 696e 7431 3132 2220  ype": "uint112" 
-0000d0e0: 7d2c 207b 2022 696e 7465 726e 616c 5479  }, { "internalTy
-0000d0f0: 7065 223a 2022 7569 6e74 3332 222c 2022  pe": "uint32", "
-0000d100: 6e61 6d65 223a 2022 626c 6f63 6b54 696d  name": "blockTim
-0000d110: 6573 7461 6d70 4c61 7374 222c 2022 7479  estampLast", "ty
-0000d120: 7065 223a 2022 7569 6e74 3332 2220 7d20  pe": "uint32" } 
-0000d130: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-0000d140: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
-0000d150: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
-0000d160: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-0000d170: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000d180: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000d190: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-0000d1a0: 223a 2022 6164 6472 6573 7322 207d 2c20  ": "address" }, 
-0000d1b0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000d1c0: 3a20 2261 6464 7265 7373 222c 2022 6e61  : "address", "na
-0000d1d0: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
-0000d1e0: 2022 6164 6472 6573 7322 207d 205d 2c20   "address" } ], 
-0000d1f0: 226e 616d 6522 3a20 2269 6e69 7469 616c  "name": "initial
-0000d200: 697a 6522 2c20 226f 7574 7075 7473 223a  ize", "outputs":
-0000d210: 205b 5d2c 2022 7374 6174 654d 7574 6162   [], "stateMutab
-0000d220: 696c 6974 7922 3a20 226e 6f6e 7061 7961  ility": "nonpaya
-0000d230: 626c 6522 2c20 2274 7970 6522 3a20 2266  ble", "type": "f
-0000d240: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
-0000d250: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
-0000d260: 6522 3a20 226b 4c61 7374 222c 2022 6f75  e": "kLast", "ou
-0000d270: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
-0000d280: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
-0000d290: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
-0000d2a0: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
-0000d2b0: 3235 3622 207d 205d 2c20 2273 7461 7465  256" } ], "state
-0000d2c0: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
-0000d2d0: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
-0000d2e0: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
-0000d2f0: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
-0000d300: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
-0000d310: 6573 7322 2c20 226e 616d 6522 3a20 2274  ess", "name": "t
-0000d320: 6f22 2c20 2274 7970 6522 3a20 2261 6464  o", "type": "add
-0000d330: 7265 7373 2220 7d20 5d2c 2022 6e61 6d65  ress" } ], "name
-0000d340: 223a 2022 6d69 6e74 222c 2022 6f75 7470  ": "mint", "outp
-0000d350: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
-0000d360: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
-0000d370: 3536 222c 2022 6e61 6d65 223a 2022 6c69  56", "name": "li
-0000d380: 7175 6964 6974 7922 2c20 2274 7970 6522  quidity", "type"
-0000d390: 3a20 2275 696e 7432 3536 2220 7d20 5d2c  : "uint256" } ],
-0000d3a0: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-0000d3b0: 7922 3a20 226e 6f6e 7061 7961 626c 6522  y": "nonpayable"
-0000d3c0: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
-0000d3d0: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
-0000d3e0: 7322 3a20 5b5d 2c20 226e 616d 6522 3a20  s": [], "name": 
-0000d3f0: 226e 616d 6522 2c20 226f 7574 7075 7473  "name", "outputs
-0000d400: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-0000d410: 5479 7065 223a 2022 7374 7269 6e67 222c  Type": "string",
-0000d420: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
-0000d430: 7065 223a 2022 7374 7269 6e67 2220 7d20  pe": "string" } 
-0000d440: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-0000d450: 6974 7922 3a20 2270 7572 6522 2c20 2274  ity": "pure", "t
-0000d460: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
-0000d470: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-0000d480: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000d490: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000d4a0: 6e61 6d65 223a 2022 6f77 6e65 7222 2c20  name": "owner", 
-0000d4b0: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-0000d4c0: 2220 7d20 5d2c 2022 6e61 6d65 223a 2022  " } ], "name": "
-0000d4d0: 6e6f 6e63 6573 222c 2022 6f75 7470 7574  nonces", "output
-0000d4e0: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000d4f0: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
-0000d500: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
-0000d510: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
-0000d520: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
-0000d530: 6269 6c69 7479 223a 2022 7669 6577 222c  bility": "view",
-0000d540: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
-0000d550: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
-0000d560: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-0000d570: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
-0000d580: 2c20 226e 616d 6522 3a20 226f 776e 6572  , "name": "owner
-0000d590: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
-0000d5a0: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
-0000d5b0: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
-0000d5c0: 7373 222c 2022 6e61 6d65 223a 2022 7370  ss", "name": "sp
-0000d5d0: 656e 6465 7222 2c20 2274 7970 6522 3a20  ender", "type": 
-0000d5e0: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
-0000d5f0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000d600: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
-0000d610: 3a20 2276 616c 7565 222c 2022 7479 7065  : "value", "type
-0000d620: 223a 2022 7569 6e74 3235 3622 207d 2c20  ": "uint256" }, 
-0000d630: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000d640: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
-0000d650: 6d65 223a 2022 6465 6164 6c69 6e65 222c  me": "deadline",
-0000d660: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
-0000d670: 3622 207d 2c20 7b20 2269 6e74 6572 6e61  6" }, { "interna
-0000d680: 6c54 7970 6522 3a20 2275 696e 7438 222c  lType": "uint8",
-0000d690: 2022 6e61 6d65 223a 2022 7622 2c20 2274   "name": "v", "t
-0000d6a0: 7970 6522 3a20 2275 696e 7438 2220 7d2c  ype": "uint8" },
-0000d6b0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000d6c0: 223a 2022 6279 7465 7333 3222 2c20 226e  ": "bytes32", "n
-0000d6d0: 616d 6522 3a20 2272 222c 2022 7479 7065  ame": "r", "type
-0000d6e0: 223a 2022 6279 7465 7333 3222 207d 2c20  ": "bytes32" }, 
-0000d6f0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000d700: 3a20 2262 7974 6573 3332 222c 2022 6e61  : "bytes32", "na
-0000d710: 6d65 223a 2022 7322 2c20 2274 7970 6522  me": "s", "type"
-0000d720: 3a20 2262 7974 6573 3332 2220 7d20 5d2c  : "bytes32" } ],
-0000d730: 2022 6e61 6d65 223a 2022 7065 726d 6974   "name": "permit
-0000d740: 222c 2022 6f75 7470 7574 7322 3a20 5b5d  ", "outputs": []
-0000d750: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
-0000d760: 7479 223a 2022 6e6f 6e70 6179 6162 6c65  ty": "nonpayable
-0000d770: 222c 2022 7479 7065 223a 2022 6675 6e63  ", "type": "func
-0000d780: 7469 6f6e 2220 7d2c 207b 2022 696e 7075  tion" }, { "inpu
-0000d790: 7473 223a 205b 5d2c 2022 6e61 6d65 223a  ts": [], "name":
-0000d7a0: 2022 7072 6963 6530 4375 6d75 6c61 7469   "price0Cumulati
-0000d7b0: 7665 4c61 7374 222c 2022 6f75 7470 7574  veLast", "output
-0000d7c0: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000d7d0: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
-0000d7e0: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
-0000d7f0: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
-0000d800: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
-0000d810: 6269 6c69 7479 223a 2022 7669 6577 222c  bility": "view",
-0000d820: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
-0000d830: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
-0000d840: 223a 205b 5d2c 2022 6e61 6d65 223a 2022  ": [], "name": "
-0000d850: 7072 6963 6531 4375 6d75 6c61 7469 7665  price1Cumulative
-0000d860: 4c61 7374 222c 2022 6f75 7470 7574 7322  Last", "outputs"
-0000d870: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-0000d880: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
-0000d890: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
-0000d8a0: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
-0000d8b0: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
-0000d8c0: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
-0000d8d0: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
-0000d8e0: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
-0000d8f0: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-0000d900: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
-0000d910: 226e 616d 6522 3a20 2274 6f22 2c20 2274  "name": "to", "t
-0000d920: 7970 6522 3a20 2261 6464 7265 7373 2220  ype": "address" 
-0000d930: 7d20 5d2c 2022 6e61 6d65 223a 2022 736b  } ], "name": "sk
-0000d940: 696d 222c 2022 6f75 7470 7574 7322 3a20  im", "outputs": 
-0000d950: 5b5d 2c20 2273 7461 7465 4d75 7461 6269  [], "stateMutabi
-0000d960: 6c69 7479 223a 2022 6e6f 6e70 6179 6162  lity": "nonpayab
-0000d970: 6c65 222c 2022 7479 7065 223a 2022 6675  le", "type": "fu
-0000d980: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
-0000d990: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
-0000d9a0: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
-0000d9b0: 3235 3622 2c20 226e 616d 6522 3a20 2261  256", "name": "a
-0000d9c0: 6d6f 756e 7430 4f75 7422 2c20 2274 7970  mount0Out", "typ
-0000d9d0: 6522 3a20 2275 696e 7432 3536 2220 7d2c  e": "uint256" },
-0000d9e0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
-0000d9f0: 223a 2022 7569 6e74 3235 3622 2c20 226e  ": "uint256", "n
-0000da00: 616d 6522 3a20 2261 6d6f 756e 7431 4f75  ame": "amount1Ou
-0000da10: 7422 2c20 2274 7970 6522 3a20 2275 696e  t", "type": "uin
-0000da20: 7432 3536 2220 7d2c 207b 2022 696e 7465  t256" }, { "inte
-0000da30: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
-0000da40: 6573 7322 2c20 226e 616d 6522 3a20 2274  ess", "name": "t
-0000da50: 6f22 2c20 2274 7970 6522 3a20 2261 6464  o", "type": "add
-0000da60: 7265 7373 2220 7d2c 207b 2022 696e 7465  ress" }, { "inte
-0000da70: 726e 616c 5479 7065 223a 2022 6279 7465  rnalType": "byte
-0000da80: 7322 2c20 226e 616d 6522 3a20 2264 6174  s", "name": "dat
-0000da90: 6122 2c20 2274 7970 6522 3a20 2262 7974  a", "type": "byt
-0000daa0: 6573 2220 7d20 5d2c 2022 6e61 6d65 223a  es" } ], "name":
-0000dab0: 2022 7377 6170 222c 2022 6f75 7470 7574   "swap", "output
-0000dac0: 7322 3a20 5b5d 2c20 2273 7461 7465 4d75  s": [], "stateMu
-0000dad0: 7461 6269 6c69 7479 223a 2022 6e6f 6e70  tability": "nonp
-0000dae0: 6179 6162 6c65 222c 2022 7479 7065 223a  ayable", "type":
-0000daf0: 2022 6675 6e63 7469 6f6e 2220 7d2c 207b   "function" }, {
-0000db00: 2022 696e 7075 7473 223a 205b 5d2c 2022   "inputs": [], "
-0000db10: 6e61 6d65 223a 2022 7379 6d62 6f6c 222c  name": "symbol",
-0000db20: 2022 6f75 7470 7574 7322 3a20 5b20 7b20   "outputs": [ { 
-0000db30: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-0000db40: 2273 7472 696e 6722 2c20 226e 616d 6522  "string", "name"
-0000db50: 3a20 2222 2c20 2274 7970 6522 3a20 2273  : "", "type": "s
-0000db60: 7472 696e 6722 207d 205d 2c20 2273 7461  tring" } ], "sta
-0000db70: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
-0000db80: 7075 7265 222c 2022 7479 7065 223a 2022  pure", "type": "
-0000db90: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
-0000dba0: 696e 7075 7473 223a 205b 5d2c 2022 6e61  inputs": [], "na
-0000dbb0: 6d65 223a 2022 7379 6e63 222c 2022 6f75  me": "sync", "ou
-0000dbc0: 7470 7574 7322 3a20 5b5d 2c20 2273 7461  tputs": [], "sta
-0000dbd0: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
-0000dbe0: 6e6f 6e70 6179 6162 6c65 222c 2022 7479  nonpayable", "ty
-0000dbf0: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-0000dc00: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000dc10: 5d2c 2022 6e61 6d65 223a 2022 746f 6b65  ], "name": "toke
-0000dc20: 6e30 222c 2022 6f75 7470 7574 7322 3a20  n0", "outputs": 
-0000dc30: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000dc40: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000dc50: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-0000dc60: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
-0000dc70: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
-0000dc80: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
-0000dc90: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-0000dca0: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000dcb0: 5d2c 2022 6e61 6d65 223a 2022 746f 6b65  ], "name": "toke
-0000dcc0: 6e31 222c 2022 6f75 7470 7574 7322 3a20  n1", "outputs": 
-0000dcd0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000dce0: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000dcf0: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-0000dd00: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
-0000dd10: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
-0000dd20: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
-0000dd30: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
-0000dd40: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
-0000dd50: 5d2c 2022 6e61 6d65 223a 2022 746f 7461  ], "name": "tota
-0000dd60: 6c53 7570 706c 7922 2c20 226f 7574 7075  lSupply", "outpu
-0000dd70: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
-0000dd80: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
-0000dd90: 3622 2c20 226e 616d 6522 3a20 2222 2c20  6", "name": "", 
-0000dda0: 2274 7970 6522 3a20 2275 696e 7432 3536  "type": "uint256
-0000ddb0: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
-0000ddc0: 6162 696c 6974 7922 3a20 2276 6965 7722  ability": "view"
-0000ddd0: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
-0000dde0: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
-0000ddf0: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000de00: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
-0000de10: 222c 2022 6e61 6d65 223a 2022 746f 222c  ", "name": "to",
-0000de20: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
-0000de30: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
-0000de40: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
-0000de50: 222c 2022 6e61 6d65 223a 2022 7661 6c75  ", "name": "valu
-0000de60: 6522 2c20 2274 7970 6522 3a20 2275 696e  e", "type": "uin
-0000de70: 7432 3536 2220 7d20 5d2c 2022 6e61 6d65  t256" } ], "name
-0000de80: 223a 2022 7472 616e 7366 6572 222c 2022  ": "transfer", "
-0000de90: 6f75 7470 7574 7322 3a20 5b20 7b20 2269  outputs": [ { "i
-0000dea0: 6e74 6572 6e61 6c54 7970 6522 3a20 2262  nternalType": "b
-0000deb0: 6f6f 6c22 2c20 226e 616d 6522 3a20 2222  ool", "name": ""
-0000dec0: 2c20 2274 7970 6522 3a20 2262 6f6f 6c22  , "type": "bool"
-0000ded0: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
-0000dee0: 6269 6c69 7479 223a 2022 6e6f 6e70 6179  bility": "nonpay
-0000def0: 6162 6c65 222c 2022 7479 7065 223a 2022  able", "type": "
-0000df00: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
-0000df10: 696e 7075 7473 223a 205b 207b 2022 696e  inputs": [ { "in
-0000df20: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-0000df30: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-0000df40: 2266 726f 6d22 2c20 2274 7970 6522 3a20  "from", "type": 
-0000df50: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
-0000df60: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000df70: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
-0000df80: 3a20 2274 6f22 2c20 2274 7970 6522 3a20  : "to", "type": 
-0000df90: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
-0000dfa0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000dfb0: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
-0000dfc0: 3a20 2276 616c 7565 222c 2022 7479 7065  : "value", "type
-0000dfd0: 223a 2022 7569 6e74 3235 3622 207d 205d  ": "uint256" } ]
-0000dfe0: 2c20 226e 616d 6522 3a20 2274 7261 6e73  , "name": "trans
-0000dff0: 6665 7246 726f 6d22 2c20 226f 7574 7075  ferFrom", "outpu
-0000e000: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
-0000e010: 616c 5479 7065 223a 2022 626f 6f6c 222c  alType": "bool",
-0000e020: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
-0000e030: 7065 223a 2022 626f 6f6c 2220 7d20 5d2c  pe": "bool" } ],
-0000e040: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-0000e050: 7922 3a20 226e 6f6e 7061 7961 626c 6522  y": "nonpayable"
-0000e060: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
-0000e070: 696f 6e22 207d 205d 270a 2020 2020 756e  ion" } ]'.    un
-0000e080: 6973 7761 705f 7633 5f65 7263 3230 5f61  iswap_v3_erc20_a
-0000e090: 6269 3d27 5b20 7b20 2261 6e6f 6e79 6d6f  bi='[ { "anonymo
-0000e0a0: 7573 223a 2066 616c 7365 2c20 2269 6e70  us": false, "inp
-0000e0b0: 7574 7322 3a20 5b20 7b20 2269 6e64 6578  uts": [ { "index
-0000e0c0: 6564 223a 2074 7275 652c 2022 696e 7465  ed": true, "inte
-0000e0d0: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
-0000e0e0: 6573 7322 2c20 226e 616d 6522 3a20 226f  ess", "name": "o
-0000e0f0: 776e 6572 222c 2022 7479 7065 223a 2022  wner", "type": "
-0000e100: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
-0000e110: 6e64 6578 6564 223a 2074 7275 652c 2022  ndexed": true, "
-0000e120: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000e130: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
-0000e140: 3a20 2273 7065 6e64 6572 222c 2022 7479  : "spender", "ty
-0000e150: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
-0000e160: 2c20 7b20 2269 6e64 6578 6564 223a 2066  , { "indexed": f
-0000e170: 616c 7365 2c20 2269 6e74 6572 6e61 6c54  alse, "internalT
-0000e180: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
-0000e190: 2022 6e61 6d65 223a 2022 7661 6c75 6522   "name": "value"
-0000e1a0: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
-0000e1b0: 3536 2220 7d20 5d2c 2022 6e61 6d65 223a  56" } ], "name":
-0000e1c0: 2022 4170 7072 6f76 616c 222c 2022 7479   "Approval", "ty
-0000e1d0: 7065 223a 2022 6576 656e 7422 207d 2c20  pe": "event" }, 
-0000e1e0: 7b20 2261 6e6f 6e79 6d6f 7573 223a 2066  { "anonymous": f
-0000e1f0: 616c 7365 2c20 2269 6e70 7574 7322 3a20  alse, "inputs": 
-0000e200: 5b20 7b20 2269 6e64 6578 6564 223a 2074  [ { "indexed": t
-0000e210: 7275 652c 2022 696e 7465 726e 616c 5479  rue, "internalTy
-0000e220: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
-0000e230: 226e 616d 6522 3a20 2266 726f 6d22 2c20  "name": "from", 
-0000e240: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-0000e250: 2220 7d2c 207b 2022 696e 6465 7865 6422  " }, { "indexed"
-0000e260: 3a20 7472 7565 2c20 2269 6e74 6572 6e61  : true, "interna
-0000e270: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
-0000e280: 222c 2022 6e61 6d65 223a 2022 746f 222c  ", "name": "to",
-0000e290: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
-0000e2a0: 7322 207d 2c20 7b20 2269 6e64 6578 6564  s" }, { "indexed
-0000e2b0: 223a 2066 616c 7365 2c20 2269 6e74 6572  ": false, "inter
-0000e2c0: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
-0000e2d0: 3536 222c 2022 6e61 6d65 223a 2022 7661  56", "name": "va
-0000e2e0: 6c75 6522 2c20 2274 7970 6522 3a20 2275  lue", "type": "u
-0000e2f0: 696e 7432 3536 2220 7d20 5d2c 2022 6e61  int256" } ], "na
-0000e300: 6d65 223a 2022 5472 616e 7366 6572 222c  me": "Transfer",
-0000e310: 2022 7479 7065 223a 2022 6576 656e 7422   "type": "event"
-0000e320: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-0000e330: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
-0000e340: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
-0000e350: 6e61 6d65 223a 2022 6f77 6e65 7222 2c20  name": "owner", 
-0000e360: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
-0000e370: 2220 7d2c 207b 2022 696e 7465 726e 616c  " }, { "internal
-0000e380: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
-0000e390: 2c20 226e 616d 6522 3a20 2273 7065 6e64  , "name": "spend
-0000e3a0: 6572 222c 2022 7479 7065 223a 2022 6164  er", "type": "ad
-0000e3b0: 6472 6573 7322 207d 205d 2c20 226e 616d  dress" } ], "nam
-0000e3c0: 6522 3a20 2261 6c6c 6f77 616e 6365 222c  e": "allowance",
-0000e3d0: 2022 6f75 7470 7574 7322 3a20 5b20 7b20   "outputs": [ { 
-0000e3e0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-0000e3f0: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
-0000e400: 223a 2022 222c 2022 7479 7065 223a 2022  ": "", "type": "
-0000e410: 7569 6e74 3235 3622 207d 205d 2c20 2273  uint256" } ], "s
-0000e420: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-0000e430: 2022 7669 6577 222c 2022 7479 7065 223a   "view", "type":
-0000e440: 2022 6675 6e63 7469 6f6e 2220 7d2c 207b   "function" }, {
-0000e450: 2022 696e 7075 7473 223a 205b 207b 2022   "inputs": [ { "
-0000e460: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000e470: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
-0000e480: 3a20 2273 7065 6e64 6572 222c 2022 7479  : "spender", "ty
-0000e490: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
-0000e4a0: 2c20 7b20 2269 6e74 6572 6e61 6c54 7970  , { "internalTyp
-0000e4b0: 6522 3a20 2275 696e 7432 3536 222c 2022  e": "uint256", "
-0000e4c0: 6e61 6d65 223a 2022 7661 6c75 6522 2c20  name": "value", 
-0000e4d0: 2274 7970 6522 3a20 2275 696e 7432 3536  "type": "uint256
-0000e4e0: 2220 7d20 5d2c 2022 6e61 6d65 223a 2022  " } ], "name": "
-0000e4f0: 6170 7072 6f76 6522 2c20 226f 7574 7075  approve", "outpu
-0000e500: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
-0000e510: 616c 5479 7065 223a 2022 626f 6f6c 222c  alType": "bool",
-0000e520: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
-0000e530: 7065 223a 2022 626f 6f6c 2220 7d20 5d2c  pe": "bool" } ],
-0000e540: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-0000e550: 7922 3a20 226e 6f6e 7061 7961 626c 6522  y": "nonpayable"
-0000e560: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
-0000e570: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
-0000e580: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
-0000e590: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
-0000e5a0: 222c 2022 6e61 6d65 223a 2022 6f77 6e65  ", "name": "owne
-0000e5b0: 7222 2c20 2274 7970 6522 3a20 2261 6464  r", "type": "add
-0000e5c0: 7265 7373 2220 7d20 5d2c 2022 6e61 6d65  ress" } ], "name
-0000e5d0: 223a 2022 6261 6c61 6e63 654f 6622 2c20  ": "balanceOf", 
-0000e5e0: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
-0000e5f0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-0000e600: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
-0000e610: 3a20 2222 2c20 2274 7970 6522 3a20 2275  : "", "type": "u
-0000e620: 696e 7432 3536 2220 7d20 5d2c 2022 7374  int256" } ], "st
-0000e630: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
-0000e640: 2276 6965 7722 2c20 2274 7970 6522 3a20  "view", "type": 
-0000e650: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
-0000e660: 2269 6e70 7574 7322 3a20 5b5d 2c20 226e  "inputs": [], "n
-0000e670: 616d 6522 3a20 2264 6563 696d 616c 7322  ame": "decimals"
-0000e680: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
-0000e690: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000e6a0: 2022 7569 6e74 3822 2c20 226e 616d 6522   "uint8", "name"
-0000e6b0: 3a20 2222 2c20 2274 7970 6522 3a20 2275  : "", "type": "u
-0000e6c0: 696e 7438 2220 7d20 5d2c 2022 7374 6174  int8" } ], "stat
-0000e6d0: 654d 7574 6162 696c 6974 7922 3a20 2276  eMutability": "v
-0000e6e0: 6965 7722 2c20 2274 7970 6522 3a20 2266  iew", "type": "f
-0000e6f0: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
-0000e700: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
-0000e710: 6522 3a20 226e 616d 6522 2c20 226f 7574  e": "name", "out
-0000e720: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
-0000e730: 726e 616c 5479 7065 223a 2022 7374 7269  rnalType": "stri
-0000e740: 6e67 222c 2022 6e61 6d65 223a 2022 222c  ng", "name": "",
-0000e750: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
-0000e760: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
-0000e770: 6162 696c 6974 7922 3a20 2276 6965 7722  ability": "view"
-0000e780: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
-0000e790: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
-0000e7a0: 7322 3a20 5b5d 2c20 226e 616d 6522 3a20  s": [], "name": 
-0000e7b0: 2273 796d 626f 6c22 2c20 226f 7574 7075  "symbol", "outpu
-0000e7c0: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
-0000e7d0: 616c 5479 7065 223a 2022 7374 7269 6e67  alType": "string
-0000e7e0: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
-0000e7f0: 7479 7065 223a 2022 7374 7269 6e67 2220  type": "string" 
-0000e800: 7d20 5d2c 2022 7374 6174 654d 7574 6162  } ], "stateMutab
-0000e810: 696c 6974 7922 3a20 2276 6965 7722 2c20  ility": "view", 
-0000e820: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
-0000e830: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
-0000e840: 3a20 5b5d 2c20 226e 616d 6522 3a20 2274  : [], "name": "t
-0000e850: 6f74 616c 5375 7070 6c79 222c 2022 6f75  otalSupply", "ou
-0000e860: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
-0000e870: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
-0000e880: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
-0000e890: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
-0000e8a0: 3235 3622 207d 205d 2c20 2273 7461 7465  256" } ], "state
-0000e8b0: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
-0000e8c0: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
-0000e8d0: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
-0000e8e0: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
-0000e8f0: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
-0000e900: 6573 7322 2c20 226e 616d 6522 3a20 2274  ess", "name": "t
-0000e910: 6f22 2c20 2274 7970 6522 3a20 2261 6464  o", "type": "add
-0000e920: 7265 7373 2220 7d2c 207b 2022 696e 7465  ress" }, { "inte
-0000e930: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
-0000e940: 3235 3622 2c20 226e 616d 6522 3a20 2276  256", "name": "v
-0000e950: 616c 7565 222c 2022 7479 7065 223a 2022  alue", "type": "
-0000e960: 7569 6e74 3235 3622 207d 205d 2c20 226e  uint256" } ], "n
-0000e970: 616d 6522 3a20 2274 7261 6e73 6665 7222  ame": "transfer"
-0000e980: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
-0000e990: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-0000e9a0: 2022 626f 6f6c 222c 2022 6e61 6d65 223a   "bool", "name":
-0000e9b0: 2022 222c 2022 7479 7065 223a 2022 626f   "", "type": "bo
-0000e9c0: 6f6c 2220 7d20 5d2c 2022 7374 6174 654d  ol" } ], "stateM
-0000e9d0: 7574 6162 696c 6974 7922 3a20 226e 6f6e  utability": "non
-0000e9e0: 7061 7961 626c 6522 2c20 2274 7970 6522  payable", "type"
-0000e9f0: 3a20 2266 756e 6374 696f 6e22 207d 2c20  : "function" }, 
-0000ea00: 7b20 2269 6e70 7574 7322 3a20 5b20 7b20  { "inputs": [ { 
-0000ea10: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-0000ea20: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
-0000ea30: 223a 2022 6672 6f6d 222c 2022 7479 7065  ": "from", "type
-0000ea40: 223a 2022 6164 6472 6573 7322 207d 2c20  ": "address" }, 
-0000ea50: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000ea60: 3a20 2261 6464 7265 7373 222c 2022 6e61  : "address", "na
-0000ea70: 6d65 223a 2022 746f 222c 2022 7479 7065  me": "to", "type
-0000ea80: 223a 2022 6164 6472 6573 7322 207d 2c20  ": "address" }, 
-0000ea90: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-0000eaa0: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
-0000eab0: 6d65 223a 2022 7661 6c75 6522 2c20 2274  me": "value", "t
-0000eac0: 7970 6522 3a20 2275 696e 7432 3536 2220  ype": "uint256" 
-0000ead0: 7d20 5d2c 2022 6e61 6d65 223a 2022 7472  } ], "name": "tr
-0000eae0: 616e 7366 6572 4672 6f6d 222c 2022 6f75  ansferFrom", "ou
-0000eaf0: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
-0000eb00: 6572 6e61 6c54 7970 6522 3a20 2262 6f6f  ernalType": "boo
-0000eb10: 6c22 2c20 226e 616d 6522 3a20 2222 2c20  l", "name": "", 
-0000eb20: 2274 7970 6522 3a20 2262 6f6f 6c22 207d  "type": "bool" }
-0000eb30: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
-0000eb40: 6c69 7479 223a 2022 6e6f 6e70 6179 6162  lity": "nonpayab
-0000eb50: 6c65 222c 2022 7479 7065 223a 2022 6675  le", "type": "fu
-0000eb60: 6e63 7469 6f6e 2220 7d20 5d27 0a20 2020  nction" } ]'.   
-0000eb70: 2023 6874 7470 733a 2f2f 6574 6865 7273   #https://ethers
-0000eb80: 6361 6e2e 696f 2f61 6464 7265 7373 2f30  can.io/address/0
-0000eb90: 7865 3539 3234 3237 6130 6165 6365 3932  xe592427a0aece92
-0000eba0: 6465 3365 6465 6531 6631 3865 3031 3537  de3edee1f18e0157
-0000ebb0: 6330 3538 3631 3536 3423 636f 6465 0a20  c05861564#code. 
-0000ebc0: 2020 2075 6e69 7377 6170 5f76 335f 726f     uniswap_v3_ro
-0000ebd0: 7574 655f 6162 693d 275b 7b22 696e 7075  ute_abi='[{"inpu
-0000ebe0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0000ebf0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0000ec00: 6e61 6d65 223a 225f 6661 6374 6f72 7922  name":"_factory"
-0000ec10: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0000ec20: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0000ec30: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0000ec40: 6d65 223a 225f 5745 5448 3922 2c22 7479  me":"_WETH9","ty
-0000ec50: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
-0000ec60: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-0000ec70: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
-0000ec80: 7479 7065 223a 2263 6f6e 7374 7275 6374  type":"construct
-0000ec90: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-0000eca0: 5d2c 226e 616d 6522 3a22 5745 5448 3922  ],"name":"WETH9"
-0000ecb0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-0000ecc0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0000ecd0: 7265 7373 222c 226e 616d 6522 3a22 222c  ress","name":"",
-0000ece0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0000ecf0: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
-0000ed00: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
-0000ed10: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-0000ed20: 2269 6e70 7574 7322 3a5b 7b22 636f 6d70  "inputs":[{"comp
-0000ed30: 6f6e 656e 7473 223a 5b7b 2269 6e74 6572  onents":[{"inter
-0000ed40: 6e61 6c54 7970 6522 3a22 6279 7465 7322  nalType":"bytes"
-0000ed50: 2c22 6e61 6d65 223a 2270 6174 6822 2c22  ,"name":"path","
-0000ed60: 7479 7065 223a 2262 7974 6573 227d 2c7b  type":"bytes"},{
-0000ed70: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000ed80: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0000ed90: 2272 6563 6970 6965 6e74 222c 2274 7970  "recipient","typ
-0000eda0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0000edb0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0000edc0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0000edd0: 6465 6164 6c69 6e65 222c 2274 7970 6522  deadline","type"
-0000ede0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0000edf0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0000ee00: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
-0000ee10: 6f75 6e74 496e 222c 2274 7970 6522 3a22  ountIn","type":"
-0000ee20: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0000ee30: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0000ee40: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0000ee50: 6e74 4f75 744d 696e 696d 756d 222c 2274  ntOutMinimum","t
-0000ee60: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-0000ee70: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0000ee80: 2273 7472 7563 7420 4953 7761 7052 6f75  "struct ISwapRou
-0000ee90: 7465 722e 4578 6163 7449 6e70 7574 5061  ter.ExactInputPa
-0000eea0: 7261 6d73 222c 226e 616d 6522 3a22 7061  rams","name":"pa
-0000eeb0: 7261 6d73 222c 2274 7970 6522 3a22 7475  rams","type":"tu
-0000eec0: 706c 6522 7d5d 2c22 6e61 6d65 223a 2265  ple"}],"name":"e
-0000eed0: 7861 6374 496e 7075 7422 2c22 6f75 7470  xactInput","outp
-0000eee0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0000eef0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0000ef00: 226e 616d 6522 3a22 616d 6f75 6e74 4f75  "name":"amountOu
-0000ef10: 7422 2c22 7479 7065 223a 2275 696e 7432  t","type":"uint2
-0000ef20: 3536 227d 5d2c 2273 7461 7465 4d75 7461  56"}],"stateMuta
-0000ef30: 6269 6c69 7479 223a 2270 6179 6162 6c65  bility":"payable
-0000ef40: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-0000ef50: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-0000ef60: 7b22 636f 6d70 6f6e 656e 7473 223a 5b7b  {"components":[{
-0000ef70: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000ef80: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0000ef90: 2274 6f6b 656e 496e 222c 2274 7970 6522  "tokenIn","type"
-0000efa0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0000efb0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0000efc0: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
-0000efd0: 6b65 6e4f 7574 222c 2274 7970 6522 3a22  kenOut","type":"
-0000efe0: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-0000eff0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0000f000: 3422 2c22 6e61 6d65 223a 2266 6565 222c  4","name":"fee",
-0000f010: 2274 7970 6522 3a22 7569 6e74 3234 227d  "type":"uint24"}
-0000f020: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0000f030: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-0000f040: 223a 2272 6563 6970 6965 6e74 222c 2274  ":"recipient","t
-0000f050: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-0000f060: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0000f070: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0000f080: 3a22 6465 6164 6c69 6e65 222c 2274 7970  :"deadline","typ
-0000f090: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0000f0a0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0000f0b0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0000f0c0: 616d 6f75 6e74 496e 222c 2274 7970 6522  amountIn","type"
-0000f0d0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0000f0e0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0000f0f0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
-0000f100: 6f75 6e74 4f75 744d 696e 696d 756d 222c  ountOutMinimum",
-0000f110: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0000f120: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0000f130: 223a 2275 696e 7431 3630 222c 226e 616d  ":"uint160","nam
-0000f140: 6522 3a22 7371 7274 5072 6963 654c 696d  e":"sqrtPriceLim
-0000f150: 6974 5839 3622 2c22 7479 7065 223a 2275  itX96","type":"u
-0000f160: 696e 7431 3630 227d 5d2c 2269 6e74 6572  int160"}],"inter
-0000f170: 6e61 6c54 7970 6522 3a22 7374 7275 6374  nalType":"struct
-0000f180: 2049 5377 6170 526f 7574 6572 2e45 7861   ISwapRouter.Exa
-0000f190: 6374 496e 7075 7453 696e 676c 6550 6172  ctInputSinglePar
-0000f1a0: 616d 7322 2c22 6e61 6d65 223a 2270 6172  ams","name":"par
-0000f1b0: 616d 7322 2c22 7479 7065 223a 2274 7570  ams","type":"tup
-0000f1c0: 6c65 227d 5d2c 226e 616d 6522 3a22 6578  le"}],"name":"ex
-0000f1d0: 6163 7449 6e70 7574 5369 6e67 6c65 222c  actInputSingle",
-0000f1e0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-0000f1f0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0000f200: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0000f210: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
-0000f220: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
-0000f230: 654d 7574 6162 696c 6974 7922 3a22 7061  eMutability":"pa
-0000f240: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-0000f250: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-0000f260: 7473 223a 5b7b 2263 6f6d 706f 6e65 6e74  ts":[{"component
-0000f270: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0000f280: 7065 223a 2262 7974 6573 222c 226e 616d  pe":"bytes","nam
-0000f290: 6522 3a22 7061 7468 222c 2274 7970 6522  e":"path","type"
-0000f2a0: 3a22 6279 7465 7322 7d2c 7b22 696e 7465  :"bytes"},{"inte
-0000f2b0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0000f2c0: 7373 222c 226e 616d 6522 3a22 7265 6369  ss","name":"reci
-0000f2d0: 7069 656e 7422 2c22 7479 7065 223a 2261  pient","type":"a
-0000f2e0: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-0000f2f0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0000f300: 3622 2c22 6e61 6d65 223a 2264 6561 646c  6","name":"deadl
-0000f310: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
-0000f320: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-0000f330: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0000f340: 2c22 6e61 6d65 223a 2261 6d6f 756e 744f  ,"name":"amountO
-0000f350: 7574 222c 2274 7970 6522 3a22 7569 6e74  ut","type":"uint
-0000f360: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0000f370: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0000f380: 226e 616d 6522 3a22 616d 6f75 6e74 496e  "name":"amountIn
-0000f390: 4d61 7869 6d75 6d22 2c22 7479 7065 223a  Maximum","type":
-0000f3a0: 2275 696e 7432 3536 227d 5d2c 2269 6e74  "uint256"}],"int
-0000f3b0: 6572 6e61 6c54 7970 6522 3a22 7374 7275  ernalType":"stru
-0000f3c0: 6374 2049 5377 6170 526f 7574 6572 2e45  ct ISwapRouter.E
-0000f3d0: 7861 6374 4f75 7470 7574 5061 7261 6d73  xactOutputParams
-0000f3e0: 222c 226e 616d 6522 3a22 7061 7261 6d73  ","name":"params
-0000f3f0: 222c 2274 7970 6522 3a22 7475 706c 6522  ","type":"tuple"
-0000f400: 7d5d 2c22 6e61 6d65 223a 2265 7861 6374  }],"name":"exact
-0000f410: 4f75 7470 7574 222c 226f 7574 7075 7473  Output","outputs
-0000f420: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0000f430: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0000f440: 6d65 223a 2261 6d6f 756e 7449 6e22 2c22  me":"amountIn","
-0000f450: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0000f460: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-0000f470: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
-0000f480: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-0000f490: 2c7b 2269 6e70 7574 7322 3a5b 7b22 636f  ,{"inputs":[{"co
-0000f4a0: 6d70 6f6e 656e 7473 223a 5b7b 2269 6e74  mponents":[{"int
-0000f4b0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0000f4c0: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
-0000f4d0: 656e 496e 222c 2274 7970 6522 3a22 6164  enIn","type":"ad
-0000f4e0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0000f4f0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-0000f500: 222c 226e 616d 6522 3a22 746f 6b65 6e4f  ","name":"tokenO
-0000f510: 7574 222c 2274 7970 6522 3a22 6164 6472  ut","type":"addr
-0000f520: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0000f530: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
-0000f540: 6e61 6d65 223a 2266 6565 222c 2274 7970  name":"fee","typ
-0000f550: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
-0000f560: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-0000f570: 6472 6573 7322 2c22 6e61 6d65 223a 2272  dress","name":"r
-0000f580: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
-0000f590: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0000f5a0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0000f5b0: 7432 3536 222c 226e 616d 6522 3a22 6465  t256","name":"de
-0000f5c0: 6164 6c69 6e65 222c 2274 7970 6522 3a22  adline","type":"
-0000f5d0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0000f5e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0000f5f0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0000f600: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
-0000f610: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0000f620: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0000f630: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-0000f640: 7449 6e4d 6178 696d 756d 222c 2274 7970  tInMaximum","typ
-0000f650: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0000f660: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0000f670: 696e 7431 3630 222c 226e 616d 6522 3a22  int160","name":"
-0000f680: 7371 7274 5072 6963 654c 696d 6974 5839  sqrtPriceLimitX9
-0000f690: 3622 2c22 7479 7065 223a 2275 696e 7431  6","type":"uint1
-0000f6a0: 3630 227d 5d2c 2269 6e74 6572 6e61 6c54  60"}],"internalT
-0000f6b0: 7970 6522 3a22 7374 7275 6374 2049 5377  ype":"struct ISw
-0000f6c0: 6170 526f 7574 6572 2e45 7861 6374 4f75  apRouter.ExactOu
-0000f6d0: 7470 7574 5369 6e67 6c65 5061 7261 6d73  tputSingleParams
-0000f6e0: 222c 226e 616d 6522 3a22 7061 7261 6d73  ","name":"params
-0000f6f0: 222c 2274 7970 6522 3a22 7475 706c 6522  ","type":"tuple"
-0000f700: 7d5d 2c22 6e61 6d65 223a 2265 7861 6374  }],"name":"exact
-0000f710: 4f75 7470 7574 5369 6e67 6c65 222c 226f  OutputSingle","o
-0000f720: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0000b060: 6574 5f70 6169 725f 6461 7461 285f 7765  et_pair_data(_we
+0000b070: 6233 3a57 6562 332c 5f70 6169 725f 6164  b3:Web3,_pair_ad
+0000b080: 6472 6573 732c 5f70 6169 725f 6162 6929  dress,_pair_abi)
+0000b090: 3a0a 2020 2020 2020 2020 7061 6972 5f63  :.        pair_c
+0000b0a0: 6f6e 7472 6163 743d 5f77 6562 332e 6574  ontract=_web3.et
+0000b0b0: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
+0000b0c0: 7373 3d5f 7061 6972 5f61 6464 7265 7373  ss=_pair_address
+0000b0d0: 2c61 6269 3d5f 7061 6972 5f61 6269 290a  ,abi=_pair_abi).
+0000b0e0: 2020 2020 2020 2020 7265 7365 7276 6530          reserve0
+0000b0f0: 2c72 6573 6572 7665 312c 626c 6f63 6b54  ,reserve1,blockT
+0000b100: 696d 6553 7461 6d70 3d70 6169 725f 636f  imeStamp=pair_co
+0000b110: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
+0000b120: 2e67 6574 5265 7365 7276 6573 2829 2e63  .getReserves().c
+0000b130: 616c 6c28 290a 2020 2020 2020 2020 7265  all().        re
+0000b140: 7475 726e 2072 6573 6572 7665 302c 7265  turn reserve0,re
+0000b150: 7365 7276 6531 2c62 6c6f 636b 5469 6d65  serve1,blockTime
+0000b160: 5374 616d 700a 0a20 2020 2064 6566 2067  Stamp..    def g
+0000b170: 6574 5f70 6169 725f 696e 666f 2873 656c  et_pair_info(sel
+0000b180: 662c 7061 6972 5f61 6464 7265 7373 293a  f,pair_address):
+0000b190: 0a20 2020 2020 2020 2070 6169 7243 6f6e  .        pairCon
+0000b1a0: 7472 6163 743d 7365 6c66 2e77 6562 332e  tract=self.web3.
+0000b1b0: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
+0000b1c0: 7265 7373 3d70 6169 725f 6164 6472 6573  ress=pair_addres
+0000b1d0: 732c 2061 6269 3d73 656c 662e 7061 6972  s, abi=self.pair
+0000b1e0: 5f61 6269 290a 2020 2020 2020 2020 746f  _abi).        to
+0000b1f0: 6b65 6e30 4164 6472 6573 733d 7061 6972  ken0Address=pair
+0000b200: 436f 6e74 7261 6374 2e66 756e 6374 696f  Contract.functio
+0000b210: 6e73 2e74 6f6b 656e 3028 292e 6361 6c6c  ns.token0().call
+0000b220: 2829 0a20 2020 2020 2020 2074 6f6b 656e  ().        token
+0000b230: 3141 6464 7265 7373 3d70 6169 7243 6f6e  1Address=pairCon
+0000b240: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
+0000b250: 746f 6b65 6e31 2829 2e63 616c 6c28 290a  token1().call().
+0000b260: 2020 2020 2020 2020 7265 7365 7276 6530          reserve0
+0000b270: 2c72 6573 6572 7665 312c 626c 6f63 6b54  ,reserve1,blockT
+0000b280: 696d 6553 7461 6d70 3d70 6169 7243 6f6e  imeStamp=pairCon
+0000b290: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
+0000b2a0: 6765 7452 6573 6572 7665 7328 292e 6361  getReserves().ca
+0000b2b0: 6c6c 2829 0a20 2020 2020 2020 2023 2074  ll().        # t
+0000b2c0: 6f6b 656e 305f 636f 6e74 7261 6374 3d73  oken0_contract=s
+0000b2d0: 656c 662e 7765 6233 2e65 7468 2e63 6f6e  elf.web3.eth.con
+0000b2e0: 7472 6163 7428 6164 6472 6573 733d 746f  tract(address=to
+0000b2f0: 6b65 6e30 4164 6472 6573 732c 2061 6269  ken0Address, abi
+0000b300: 3d73 656c 662e 6572 6332 305f 6162 6929  =self.erc20_abi)
+0000b310: 0a20 2020 2020 2020 2023 2074 6f6b 656e  .        # token
+0000b320: 315f 636f 6e74 7261 6374 3d73 656c 662e  1_contract=self.
+0000b330: 7765 6233 2e65 7468 2e63 6f6e 7472 6163  web3.eth.contrac
+0000b340: 7428 6164 6472 6573 733d 746f 6b65 6e31  t(address=token1
+0000b350: 4164 6472 6573 732c 2061 6269 3d73 656c  Address, abi=sel
+0000b360: 662e 6572 6332 305f 6162 6929 0a20 2020  f.erc20_abi).   
+0000b370: 2020 2020 2023 2074 6f6b 656e 305f 6e61       # token0_na
+0000b380: 6d65 3d74 6f6b 656e 305f 636f 6e74 7261  me=token0_contra
+0000b390: 6374 2e66 756e 6374 696f 6e73 2e6e 616d  ct.functions.nam
+0000b3a0: 6528 292e 6361 6c6c 2829 0a20 2020 2020  e().call().     
+0000b3b0: 2020 2023 2074 6f6b 656e 315f 6e61 6d65     # token1_name
+0000b3c0: 3d74 6f6b 656e 315f 636f 6e74 7261 6374  =token1_contract
+0000b3d0: 2e66 756e 6374 696f 6e73 2e6e 616d 6528  .functions.name(
+0000b3e0: 292e 6361 6c6c 2829 0a20 2020 2020 2020  ).call().       
+0000b3f0: 2070 7269 6365 303d 7265 7365 7276 6531   price0=reserve1
+0000b400: 2f72 6573 6572 7665 300a 2020 2020 2020  /reserve0.      
+0000b410: 2020 7072 6963 6531 3d72 6573 6572 7665    price1=reserve
+0000b420: 302f 7265 7365 7276 6531 0a20 2020 2020  0/reserve1.     
+0000b430: 2020 2023 2070 7269 6e74 2822 746f 6b65     # print("toke
+0000b440: 6e30 3a22 2c73 7472 2874 6f6b 656e 3041  n0:",str(token0A
+0000b450: 6464 7265 7373 292c 222d 2d6e 616d 653a  ddress),"--name:
+0000b460: 222c 7374 7228 746f 6b65 6e30 5f6e 616d  ",str(token0_nam
+0000b470: 6529 2c22 2d2d 7072 6963 653a 222c 7374  e),"--price:",st
+0000b480: 7228 7072 6963 6530 2929 0a20 2020 2020  r(price0)).     
+0000b490: 2020 2023 2070 7269 6e74 2822 746f 6b65     # print("toke
+0000b4a0: 6e31 3a22 2c73 7472 2874 6f6b 656e 3141  n1:",str(token1A
+0000b4b0: 6464 7265 7373 292c 222d 2d6e 616d 653a  ddress),"--name:
+0000b4c0: 222c 7374 7228 746f 6b65 6e31 5f6e 616d  ",str(token1_nam
+0000b4d0: 6529 2c22 2d2d 7072 6963 653a 222c 7374  e),"--price:",st
+0000b4e0: 7228 7072 6963 6531 2929 0a20 2020 2020  r(price1)).     
+0000b4f0: 2020 2023 2070 7269 6e74 2822 7265 7365     # print("rese
+0000b500: 7276 6530 222c 7374 7228 7265 7365 7276  rve0",str(reserv
+0000b510: 6530 2929 0a20 2020 2020 2020 2023 2070  e0)).        # p
+0000b520: 7269 6e74 2822 7265 7365 7276 6531 222c  rint("reserve1",
+0000b530: 7374 7228 7265 7365 7276 6531 2929 0a20  str(reserve1)). 
+0000b540: 2020 2020 2020 2023 2070 7269 6e74 2822         # print("
+0000b550: 626c 6f63 6b54 696d 6553 7461 6d70 222c  blockTimeStamp",
+0000b560: 7374 7228 626c 6f63 6b54 696d 6553 7461  str(blockTimeSta
+0000b570: 6d70 2929 0a20 2020 2020 2020 2072 6574  mp)).        ret
+0000b580: 7572 6e20 746f 6b65 6e30 4164 6472 6573  urn token0Addres
+0000b590: 732c 7265 7365 7276 6530 2c74 6f6b 656e  s,reserve0,token
+0000b5a0: 3141 6464 7265 7373 2c72 6573 6572 7665  1Address,reserve
+0000b5b0: 312c 626c 6f63 6b54 696d 6553 7461 6d70  1,blockTimeStamp
+0000b5c0: 2c70 7269 6365 302c 7072 6963 6531 0a0a  ,price0,price1..
+0000b5d0: 636c 6173 7320 556e 6973 7761 7056 333a  class UniswapV3:
+0000b5e0: 0a20 2020 2023 6874 7470 733a 2f2f 6574  .    #https://et
+0000b5f0: 6865 7273 6361 6e2e 696f 2f61 6464 7265  herscan.io/addre
+0000b600: 7373 2f30 7831 6639 3834 3331 6338 6164  ss/0x1f98431c8ad
+0000b610: 3938 3532 3336 3331 6165 3461 3539 6632  98523631ae4a59f2
+0000b620: 3637 3334 3665 6133 3166 3938 340a 2020  67346ea31f984.  
+0000b630: 2020 756e 6973 7761 705f 7633 5f66 6163    uniswap_v3_fac
+0000b640: 746f 7279 5f61 6269 3d27 5b7b 2269 6e70  tory_abi='[{"inp
+0000b650: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
+0000b660: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
+0000b670: 7961 626c 6522 2c22 7479 7065 223a 2263  yable","type":"c
+0000b680: 6f6e 7374 7275 6374 6f72 227d 2c7b 2261  onstructor"},{"a
+0000b690: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
+0000b6a0: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
+0000b6b0: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
+0000b6c0: 6e61 6c54 7970 6522 3a22 7569 6e74 3234  nalType":"uint24
+0000b6d0: 222c 226e 616d 6522 3a22 6665 6522 2c22  ","name":"fee","
+0000b6e0: 7479 7065 223a 2275 696e 7432 3422 7d2c  type":"uint24"},
+0000b6f0: 7b22 696e 6465 7865 6422 3a74 7275 652c  {"indexed":true,
+0000b700: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000b710: 696e 7432 3422 2c22 6e61 6d65 223a 2274  int24","name":"t
+0000b720: 6963 6b53 7061 6369 6e67 222c 2274 7970  ickSpacing","typ
+0000b730: 6522 3a22 696e 7432 3422 7d5d 2c22 6e61  e":"int24"}],"na
+0000b740: 6d65 223a 2246 6565 416d 6f75 6e74 456e  me":"FeeAmountEn
+0000b750: 6162 6c65 6422 2c22 7479 7065 223a 2265  abled","type":"e
+0000b760: 7665 6e74 227d 2c7b 2261 6e6f 6e79 6d6f  vent"},{"anonymo
+0000b770: 7573 223a 6661 6c73 652c 2269 6e70 7574  us":false,"input
+0000b780: 7322 3a5b 7b22 696e 6465 7865 6422 3a74  s":[{"indexed":t
+0000b790: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
+0000b7a0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+0000b7b0: 6d65 223a 226f 6c64 4f77 6e65 7222 2c22  me":"oldOwner","
+0000b7c0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+0000b7d0: 2c7b 2269 6e64 6578 6564 223a 7472 7565  ,{"indexed":true
+0000b7e0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0000b7f0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0000b800: 3a22 6e65 774f 776e 6572 222c 2274 7970  :"newOwner","typ
+0000b810: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+0000b820: 6e61 6d65 223a 224f 776e 6572 4368 616e  name":"OwnerChan
+0000b830: 6765 6422 2c22 7479 7065 223a 2265 7665  ged","type":"eve
+0000b840: 6e74 227d 2c7b 2261 6e6f 6e79 6d6f 7573  nt"},{"anonymous
+0000b850: 223a 6661 6c73 652c 2269 6e70 7574 7322  ":false,"inputs"
+0000b860: 3a5b 7b22 696e 6465 7865 6422 3a74 7275  :[{"indexed":tru
+0000b870: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0000b880: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0000b890: 223a 2274 6f6b 656e 3022 2c22 7479 7065  ":"token0","type
+0000b8a0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0000b8b0: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
+0000b8c0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0000b8d0: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
+0000b8e0: 6b65 6e31 222c 2274 7970 6522 3a22 6164  ken1","type":"ad
+0000b8f0: 6472 6573 7322 7d2c 7b22 696e 6465 7865  dress"},{"indexe
+0000b900: 6422 3a74 7275 652c 2269 6e74 6572 6e61  d":true,"interna
+0000b910: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
+0000b920: 226e 616d 6522 3a22 6665 6522 2c22 7479  "name":"fee","ty
+0000b930: 7065 223a 2275 696e 7432 3422 7d2c 7b22  pe":"uint24"},{"
+0000b940: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
+0000b950: 696e 7465 726e 616c 5479 7065 223a 2269  internalType":"i
+0000b960: 6e74 3234 222c 226e 616d 6522 3a22 7469  nt24","name":"ti
+0000b970: 636b 5370 6163 696e 6722 2c22 7479 7065  ckSpacing","type
+0000b980: 223a 2269 6e74 3234 227d 2c7b 2269 6e64  ":"int24"},{"ind
+0000b990: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+0000b9a0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0000b9b0: 6573 7322 2c22 6e61 6d65 223a 2270 6f6f  ess","name":"poo
+0000b9c0: 6c22 2c22 7479 7065 223a 2261 6464 7265  l","type":"addre
+0000b9d0: 7373 227d 5d2c 226e 616d 6522 3a22 506f  ss"}],"name":"Po
+0000b9e0: 6f6c 4372 6561 7465 6422 2c22 7479 7065  olCreated","type
+0000b9f0: 223a 2265 7665 6e74 227d 2c7b 2269 6e70  ":"event"},{"inp
+0000ba00: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+0000ba10: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0000ba20: 226e 616d 6522 3a22 746f 6b65 6e41 222c  "name":"tokenA",
+0000ba30: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0000ba40: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000ba50: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0000ba60: 6522 3a22 746f 6b65 6e42 222c 2274 7970  e":"tokenB","typ
+0000ba70: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0000ba80: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0000ba90: 696e 7432 3422 2c22 6e61 6d65 223a 2266  int24","name":"f
+0000baa0: 6565 222c 2274 7970 6522 3a22 7569 6e74  ee","type":"uint
+0000bab0: 3234 227d 5d2c 226e 616d 6522 3a22 6372  24"}],"name":"cr
+0000bac0: 6561 7465 506f 6f6c 222c 226f 7574 7075  eatePool","outpu
+0000bad0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0000bae0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0000baf0: 6e61 6d65 223a 2270 6f6f 6c22 2c22 7479  name":"pool","ty
+0000bb00: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
+0000bb10: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0000bb20: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+0000bb30: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+0000bb40: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0000bb50: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0000bb60: 6e74 3234 222c 226e 616d 6522 3a22 6665  nt24","name":"fe
+0000bb70: 6522 2c22 7479 7065 223a 2275 696e 7432  e","type":"uint2
+0000bb80: 3422 7d2c 7b22 696e 7465 726e 616c 5479  4"},{"internalTy
+0000bb90: 7065 223a 2269 6e74 3234 222c 226e 616d  pe":"int24","nam
+0000bba0: 6522 3a22 7469 636b 5370 6163 696e 6722  e":"tickSpacing"
+0000bbb0: 2c22 7479 7065 223a 2269 6e74 3234 227d  ,"type":"int24"}
+0000bbc0: 5d2c 226e 616d 6522 3a22 656e 6162 6c65  ],"name":"enable
+0000bbd0: 4665 6541 6d6f 756e 7422 2c22 6f75 7470  FeeAmount","outp
+0000bbe0: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
+0000bbf0: 7461 6269 6c69 7479 223a 226e 6f6e 7061  tability":"nonpa
+0000bc00: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
+0000bc10: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+0000bc20: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0000bc30: 7970 6522 3a22 7569 6e74 3234 222c 226e  ype":"uint24","n
+0000bc40: 616d 6522 3a22 222c 2274 7970 6522 3a22  ame":"","type":"
+0000bc50: 7569 6e74 3234 227d 5d2c 226e 616d 6522  uint24"}],"name"
+0000bc60: 3a22 6665 6541 6d6f 756e 7454 6963 6b53  :"feeAmountTickS
+0000bc70: 7061 6369 6e67 222c 226f 7574 7075 7473  pacing","outputs
+0000bc80: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0000bc90: 6522 3a22 696e 7432 3422 2c22 6e61 6d65  e":"int24","name
+0000bca0: 223a 2222 2c22 7479 7065 223a 2269 6e74  ":"","type":"int
+0000bcb0: 3234 227d 5d2c 2273 7461 7465 4d75 7461  24"}],"stateMuta
+0000bcc0: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
+0000bcd0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+0000bce0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0000bcf0: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+0000bd00: 6472 6573 7322 2c22 6e61 6d65 223a 2222  dress","name":""
+0000bd10: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0000bd20: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0000bd30: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+0000bd40: 6d65 223a 2222 2c22 7479 7065 223a 2261  me":"","type":"a
+0000bd50: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+0000bd60: 6e61 6c54 7970 6522 3a22 7569 6e74 3234  nalType":"uint24
+0000bd70: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
+0000bd80: 6522 3a22 7569 6e74 3234 227d 5d2c 226e  e":"uint24"}],"n
+0000bd90: 616d 6522 3a22 6765 7450 6f6f 6c22 2c22  ame":"getPool","
+0000bda0: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+0000bdb0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0000bdc0: 7373 222c 226e 616d 6522 3a22 222c 2274  ss","name":"","t
+0000bdd0: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+0000bde0: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0000bdf0: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+0000be00: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0000be10: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0000be20: 3a22 6f77 6e65 7222 2c22 6f75 7470 7574  :"owner","output
+0000be30: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0000be40: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+0000be50: 616d 6522 3a22 222c 2274 7970 6522 3a22  ame":"","type":"
+0000be60: 6164 6472 6573 7322 7d5d 2c22 7374 6174  address"}],"stat
+0000be70: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
+0000be80: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
+0000be90: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0000bea0: 3a5b 5d2c 226e 616d 6522 3a22 7061 7261  :[],"name":"para
+0000beb0: 6d65 7465 7273 222c 226f 7574 7075 7473  meters","outputs
+0000bec0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0000bed0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+0000bee0: 6d65 223a 2266 6163 746f 7279 222c 2274  me":"factory","t
+0000bef0: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+0000bf00: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0000bf10: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0000bf20: 3a22 746f 6b65 6e30 222c 2274 7970 6522  :"token0","type"
+0000bf30: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0000bf40: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0000bf50: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
+0000bf60: 6b65 6e31 222c 2274 7970 6522 3a22 6164  ken1","type":"ad
+0000bf70: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0000bf80: 616c 5479 7065 223a 2275 696e 7432 3422  alType":"uint24"
+0000bf90: 2c22 6e61 6d65 223a 2266 6565 222c 2274  ,"name":"fee","t
+0000bfa0: 7970 6522 3a22 7569 6e74 3234 227d 2c7b  ype":"uint24"},{
+0000bfb0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000bfc0: 696e 7432 3422 2c22 6e61 6d65 223a 2274  int24","name":"t
+0000bfd0: 6963 6b53 7061 6369 6e67 222c 2274 7970  ickSpacing","typ
+0000bfe0: 6522 3a22 696e 7432 3422 7d5d 2c22 7374  e":"int24"}],"st
+0000bff0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+0000c000: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+0000c010: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+0000c020: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0000c030: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+0000c040: 616d 6522 3a22 5f6f 776e 6572 222c 2274  ame":"_owner","t
+0000c050: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+0000c060: 2c22 6e61 6d65 223a 2273 6574 4f77 6e65  ,"name":"setOwne
+0000c070: 7222 2c22 6f75 7470 7574 7322 3a5b 5d2c  r","outputs":[],
+0000c080: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0000c090: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+0000c0a0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+0000c0b0: 7d5d 270a 2020 2020 756e 6973 7761 705f  }]'.    uniswap_
+0000c0c0: 7633 5f70 6169 725f 6162 693d 275b 207b  v3_pair_abi='[ {
+0000c0d0: 2022 616e 6f6e 796d 6f75 7322 3a20 6661   "anonymous": fa
+0000c0e0: 6c73 652c 2022 696e 7075 7473 223a 205b  lse, "inputs": [
+0000c0f0: 207b 2022 696e 6465 7865 6422 3a20 7472   { "indexed": tr
+0000c100: 7565 2c20 2269 6e74 6572 6e61 6c54 7970  ue, "internalTyp
+0000c110: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000c120: 6e61 6d65 223a 2022 6f77 6e65 7222 2c20  name": "owner", 
+0000c130: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+0000c140: 2220 7d2c 207b 2022 696e 6465 7865 6422  " }, { "indexed"
+0000c150: 3a20 7472 7565 2c20 2269 6e74 6572 6e61  : true, "interna
+0000c160: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
+0000c170: 222c 2022 6e61 6d65 223a 2022 7370 656e  ", "name": "spen
+0000c180: 6465 7222 2c20 2274 7970 6522 3a20 2261  der", "type": "a
+0000c190: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+0000c1a0: 6465 7865 6422 3a20 6661 6c73 652c 2022  dexed": false, "
+0000c1b0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000c1c0: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
+0000c1d0: 3a20 2276 616c 7565 222c 2022 7479 7065  : "value", "type
+0000c1e0: 223a 2022 7569 6e74 3235 3622 207d 205d  ": "uint256" } ]
+0000c1f0: 2c20 226e 616d 6522 3a20 2241 7070 726f  , "name": "Appro
+0000c200: 7661 6c22 2c20 2274 7970 6522 3a20 2265  val", "type": "e
+0000c210: 7665 6e74 2220 7d2c 207b 2022 616e 6f6e  vent" }, { "anon
+0000c220: 796d 6f75 7322 3a20 6661 6c73 652c 2022  ymous": false, "
+0000c230: 696e 7075 7473 223a 205b 207b 2022 696e  inputs": [ { "in
+0000c240: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
+0000c250: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+0000c260: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+0000c270: 2022 7365 6e64 6572 222c 2022 7479 7065   "sender", "type
+0000c280: 223a 2022 6164 6472 6573 7322 207d 2c20  ": "address" }, 
+0000c290: 7b20 2269 6e64 6578 6564 223a 2066 616c  { "indexed": fal
+0000c2a0: 7365 2c20 2269 6e74 6572 6e61 6c54 7970  se, "internalTyp
+0000c2b0: 6522 3a20 2275 696e 7432 3536 222c 2022  e": "uint256", "
+0000c2c0: 6e61 6d65 223a 2022 616d 6f75 6e74 3022  name": "amount0"
+0000c2d0: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
+0000c2e0: 3536 2220 7d2c 207b 2022 696e 6465 7865  56" }, { "indexe
+0000c2f0: 6422 3a20 6661 6c73 652c 2022 696e 7465  d": false, "inte
+0000c300: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
+0000c310: 3235 3622 2c20 226e 616d 6522 3a20 2261  256", "name": "a
+0000c320: 6d6f 756e 7431 222c 2022 7479 7065 223a  mount1", "type":
+0000c330: 2022 7569 6e74 3235 3622 207d 2c20 7b20   "uint256" }, { 
+0000c340: 2269 6e64 6578 6564 223a 2074 7275 652c  "indexed": true,
+0000c350: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000c360: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
+0000c370: 6522 3a20 2274 6f22 2c20 2274 7970 6522  e": "to", "type"
+0000c380: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
+0000c390: 2022 6e61 6d65 223a 2022 4275 726e 222c   "name": "Burn",
+0000c3a0: 2022 7479 7065 223a 2022 6576 656e 7422   "type": "event"
+0000c3b0: 207d 2c20 7b20 2261 6e6f 6e79 6d6f 7573   }, { "anonymous
+0000c3c0: 223a 2066 616c 7365 2c20 2269 6e70 7574  ": false, "input
+0000c3d0: 7322 3a20 5b20 7b20 2269 6e64 6578 6564  s": [ { "indexed
+0000c3e0: 223a 2074 7275 652c 2022 696e 7465 726e  ": true, "intern
+0000c3f0: 616c 5479 7065 223a 2022 6164 6472 6573  alType": "addres
+0000c400: 7322 2c20 226e 616d 6522 3a20 2273 656e  s", "name": "sen
+0000c410: 6465 7222 2c20 2274 7970 6522 3a20 2261  der", "type": "a
+0000c420: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+0000c430: 6465 7865 6422 3a20 6661 6c73 652c 2022  dexed": false, "
+0000c440: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000c450: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
+0000c460: 3a20 2261 6d6f 756e 7430 222c 2022 7479  : "amount0", "ty
+0000c470: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
+0000c480: 2c20 7b20 2269 6e64 6578 6564 223a 2066  , { "indexed": f
+0000c490: 616c 7365 2c20 2269 6e74 6572 6e61 6c54  alse, "internalT
+0000c4a0: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
+0000c4b0: 2022 6e61 6d65 223a 2022 616d 6f75 6e74   "name": "amount
+0000c4c0: 3122 2c20 2274 7970 6522 3a20 2275 696e  1", "type": "uin
+0000c4d0: 7432 3536 2220 7d20 5d2c 2022 6e61 6d65  t256" } ], "name
+0000c4e0: 223a 2022 4d69 6e74 222c 2022 7479 7065  ": "Mint", "type
+0000c4f0: 223a 2022 6576 656e 7422 207d 2c20 7b20  ": "event" }, { 
+0000c500: 2261 6e6f 6e79 6d6f 7573 223a 2066 616c  "anonymous": fal
+0000c510: 7365 2c20 2269 6e70 7574 7322 3a20 5b20  se, "inputs": [ 
+0000c520: 7b20 2269 6e64 6578 6564 223a 2074 7275  { "indexed": tru
+0000c530: 652c 2022 696e 7465 726e 616c 5479 7065  e, "internalType
+0000c540: 223a 2022 6164 6472 6573 7322 2c20 226e  ": "address", "n
+0000c550: 616d 6522 3a20 2273 656e 6465 7222 2c20  ame": "sender", 
+0000c560: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+0000c570: 2220 7d2c 207b 2022 696e 6465 7865 6422  " }, { "indexed"
+0000c580: 3a20 6661 6c73 652c 2022 696e 7465 726e  : false, "intern
+0000c590: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
+0000c5a0: 3622 2c20 226e 616d 6522 3a20 2261 6d6f  6", "name": "amo
+0000c5b0: 756e 7430 496e 222c 2022 7479 7065 223a  unt0In", "type":
+0000c5c0: 2022 7569 6e74 3235 3622 207d 2c20 7b20   "uint256" }, { 
+0000c5d0: 2269 6e64 6578 6564 223a 2066 616c 7365  "indexed": false
+0000c5e0: 2c20 2269 6e74 6572 6e61 6c54 7970 6522  , "internalType"
+0000c5f0: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+0000c600: 6d65 223a 2022 616d 6f75 6e74 3149 6e22  me": "amount1In"
+0000c610: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
+0000c620: 3536 2220 7d2c 207b 2022 696e 6465 7865  56" }, { "indexe
+0000c630: 6422 3a20 6661 6c73 652c 2022 696e 7465  d": false, "inte
+0000c640: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
+0000c650: 3235 3622 2c20 226e 616d 6522 3a20 2261  256", "name": "a
+0000c660: 6d6f 756e 7430 4f75 7422 2c20 2274 7970  mount0Out", "typ
+0000c670: 6522 3a20 2275 696e 7432 3536 2220 7d2c  e": "uint256" },
+0000c680: 207b 2022 696e 6465 7865 6422 3a20 6661   { "indexed": fa
+0000c690: 6c73 652c 2022 696e 7465 726e 616c 5479  lse, "internalTy
+0000c6a0: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
+0000c6b0: 226e 616d 6522 3a20 2261 6d6f 756e 7431  "name": "amount1
+0000c6c0: 4f75 7422 2c20 2274 7970 6522 3a20 2275  Out", "type": "u
+0000c6d0: 696e 7432 3536 2220 7d2c 207b 2022 696e  int256" }, { "in
+0000c6e0: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
+0000c6f0: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+0000c700: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+0000c710: 2022 746f 222c 2022 7479 7065 223a 2022   "to", "type": "
+0000c720: 6164 6472 6573 7322 207d 205d 2c20 226e  address" } ], "n
+0000c730: 616d 6522 3a20 2253 7761 7022 2c20 2274  ame": "Swap", "t
+0000c740: 7970 6522 3a20 2265 7665 6e74 2220 7d2c  ype": "event" },
+0000c750: 207b 2022 616e 6f6e 796d 6f75 7322 3a20   { "anonymous": 
+0000c760: 6661 6c73 652c 2022 696e 7075 7473 223a  false, "inputs":
+0000c770: 205b 207b 2022 696e 6465 7865 6422 3a20   [ { "indexed": 
+0000c780: 6661 6c73 652c 2022 696e 7465 726e 616c  false, "internal
+0000c790: 5479 7065 223a 2022 7569 6e74 3131 3222  Type": "uint112"
+0000c7a0: 2c20 226e 616d 6522 3a20 2272 6573 6572  , "name": "reser
+0000c7b0: 7665 3022 2c20 2274 7970 6522 3a20 2275  ve0", "type": "u
+0000c7c0: 696e 7431 3132 2220 7d2c 207b 2022 696e  int112" }, { "in
+0000c7d0: 6465 7865 6422 3a20 6661 6c73 652c 2022  dexed": false, "
+0000c7e0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000c7f0: 7569 6e74 3131 3222 2c20 226e 616d 6522  uint112", "name"
+0000c800: 3a20 2272 6573 6572 7665 3122 2c20 2274  : "reserve1", "t
+0000c810: 7970 6522 3a20 2275 696e 7431 3132 2220  ype": "uint112" 
+0000c820: 7d20 5d2c 2022 6e61 6d65 223a 2022 5379  } ], "name": "Sy
+0000c830: 6e63 222c 2022 7479 7065 223a 2022 6576  nc", "type": "ev
+0000c840: 656e 7422 207d 2c20 7b20 2261 6e6f 6e79  ent" }, { "anony
+0000c850: 6d6f 7573 223a 2066 616c 7365 2c20 2269  mous": false, "i
+0000c860: 6e70 7574 7322 3a20 5b20 7b20 2269 6e64  nputs": [ { "ind
+0000c870: 6578 6564 223a 2074 7275 652c 2022 696e  exed": true, "in
+0000c880: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
+0000c890: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
+0000c8a0: 2266 726f 6d22 2c20 2274 7970 6522 3a20  "from", "type": 
+0000c8b0: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
+0000c8c0: 696e 6465 7865 6422 3a20 7472 7565 2c20  indexed": true, 
+0000c8d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000c8e0: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
+0000c8f0: 223a 2022 746f 222c 2022 7479 7065 223a  ": "to", "type":
+0000c900: 2022 6164 6472 6573 7322 207d 2c20 7b20   "address" }, { 
+0000c910: 2269 6e64 6578 6564 223a 2066 616c 7365  "indexed": false
+0000c920: 2c20 2269 6e74 6572 6e61 6c54 7970 6522  , "internalType"
+0000c930: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+0000c940: 6d65 223a 2022 7661 6c75 6522 2c20 2274  me": "value", "t
+0000c950: 7970 6522 3a20 2275 696e 7432 3536 2220  ype": "uint256" 
+0000c960: 7d20 5d2c 2022 6e61 6d65 223a 2022 5472  } ], "name": "Tr
+0000c970: 616e 7366 6572 222c 2022 7479 7065 223a  ansfer", "type":
+0000c980: 2022 6576 656e 7422 207d 2c20 7b20 2269   "event" }, { "i
+0000c990: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
+0000c9a0: 6522 3a20 2244 4f4d 4149 4e5f 5345 5041  e": "DOMAIN_SEPA
+0000c9b0: 5241 544f 5222 2c20 226f 7574 7075 7473  RATOR", "outputs
+0000c9c0: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+0000c9d0: 5479 7065 223a 2022 6279 7465 7333 3222  Type": "bytes32"
+0000c9e0: 2c20 226e 616d 6522 3a20 2222 2c20 2274  , "name": "", "t
+0000c9f0: 7970 6522 3a20 2262 7974 6573 3332 2220  ype": "bytes32" 
+0000ca00: 7d20 5d2c 2022 7374 6174 654d 7574 6162  } ], "stateMutab
+0000ca10: 696c 6974 7922 3a20 2276 6965 7722 2c20  ility": "view", 
+0000ca20: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
+0000ca30: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
+0000ca40: 3a20 5b5d 2c20 226e 616d 6522 3a20 224d  : [], "name": "M
+0000ca50: 494e 494d 554d 5f4c 4951 5549 4449 5459  INIMUM_LIQUIDITY
+0000ca60: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
+0000ca70: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000ca80: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+0000ca90: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
+0000caa0: 2022 7569 6e74 3235 3622 207d 205d 2c20   "uint256" } ], 
+0000cab0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0000cac0: 223a 2022 7075 7265 222c 2022 7479 7065  ": "pure", "type
+0000cad0: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
+0000cae0: 207b 2022 696e 7075 7473 223a 205b 5d2c   { "inputs": [],
+0000caf0: 2022 6e61 6d65 223a 2022 5045 524d 4954   "name": "PERMIT
+0000cb00: 5f54 5950 4548 4153 4822 2c20 226f 7574  _TYPEHASH", "out
+0000cb10: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+0000cb20: 726e 616c 5479 7065 223a 2022 6279 7465  rnalType": "byte
+0000cb30: 7333 3222 2c20 226e 616d 6522 3a20 2222  s32", "name": ""
+0000cb40: 2c20 2274 7970 6522 3a20 2262 7974 6573  , "type": "bytes
+0000cb50: 3332 2220 7d20 5d2c 2022 7374 6174 654d  32" } ], "stateM
+0000cb60: 7574 6162 696c 6974 7922 3a20 2270 7572  utability": "pur
+0000cb70: 6522 2c20 2274 7970 6522 3a20 2266 756e  e", "type": "fun
+0000cb80: 6374 696f 6e22 207d 2c20 7b20 2269 6e70  ction" }, { "inp
+0000cb90: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000cba0: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000cbb0: 7373 222c 2022 6e61 6d65 223a 2022 6f77  ss", "name": "ow
+0000cbc0: 6e65 7222 2c20 2274 7970 6522 3a20 2261  ner", "type": "a
+0000cbd0: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+0000cbe0: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
+0000cbf0: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
+0000cc00: 2273 7065 6e64 6572 222c 2022 7479 7065  "spender", "type
+0000cc10: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
+0000cc20: 2c20 226e 616d 6522 3a20 2261 6c6c 6f77  , "name": "allow
+0000cc30: 616e 6365 222c 2022 6f75 7470 7574 7322  ance", "outputs"
+0000cc40: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
+0000cc50: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
+0000cc60: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
+0000cc70: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
+0000cc80: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
+0000cc90: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
+0000cca0: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
+0000ccb0: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
+0000ccc0: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+0000ccd0: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
+0000cce0: 226e 616d 6522 3a20 2273 7065 6e64 6572  "name": "spender
+0000ccf0: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
+0000cd00: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
+0000cd10: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
+0000cd20: 3536 222c 2022 6e61 6d65 223a 2022 7661  56", "name": "va
+0000cd30: 6c75 6522 2c20 2274 7970 6522 3a20 2275  lue", "type": "u
+0000cd40: 696e 7432 3536 2220 7d20 5d2c 2022 6e61  int256" } ], "na
+0000cd50: 6d65 223a 2022 6170 7072 6f76 6522 2c20  me": "approve", 
+0000cd60: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+0000cd70: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000cd80: 626f 6f6c 222c 2022 6e61 6d65 223a 2022  bool", "name": "
+0000cd90: 222c 2022 7479 7065 223a 2022 626f 6f6c  ", "type": "bool
+0000cda0: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+0000cdb0: 6162 696c 6974 7922 3a20 226e 6f6e 7061  ability": "nonpa
+0000cdc0: 7961 626c 6522 2c20 2274 7970 6522 3a20  yable", "type": 
+0000cdd0: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
+0000cde0: 2269 6e70 7574 7322 3a20 5b20 7b20 2269  "inputs": [ { "i
+0000cdf0: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+0000ce00: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+0000ce10: 2022 6f77 6e65 7222 2c20 2274 7970 6522   "owner", "type"
+0000ce20: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
+0000ce30: 2022 6e61 6d65 223a 2022 6261 6c61 6e63   "name": "balanc
+0000ce40: 654f 6622 2c20 226f 7574 7075 7473 223a  eOf", "outputs":
+0000ce50: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+0000ce60: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
+0000ce70: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
+0000ce80: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
+0000ce90: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
+0000cea0: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
+0000ceb0: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+0000cec0: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+0000ced0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000cee0: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000cef0: 6e61 6d65 223a 2022 746f 222c 2022 7479  name": "to", "ty
+0000cf00: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
+0000cf10: 205d 2c20 226e 616d 6522 3a20 2262 7572   ], "name": "bur
+0000cf20: 6e22 2c20 226f 7574 7075 7473 223a 205b  n", "outputs": [
+0000cf30: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
+0000cf40: 223a 2022 7569 6e74 3235 3622 2c20 226e  ": "uint256", "n
+0000cf50: 616d 6522 3a20 2261 6d6f 756e 7430 222c  ame": "amount0",
+0000cf60: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
+0000cf70: 3622 207d 2c20 7b20 2269 6e74 6572 6e61  6" }, { "interna
+0000cf80: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000cf90: 222c 2022 6e61 6d65 223a 2022 616d 6f75  ", "name": "amou
+0000cfa0: 6e74 3122 2c20 2274 7970 6522 3a20 2275  nt1", "type": "u
+0000cfb0: 696e 7432 3536 2220 7d20 5d2c 2022 7374  int256" } ], "st
+0000cfc0: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
+0000cfd0: 226e 6f6e 7061 7961 626c 6522 2c20 2274  "nonpayable", "t
+0000cfe0: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+0000cff0: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+0000d000: 5b5d 2c20 226e 616d 6522 3a20 2264 6563  [], "name": "dec
+0000d010: 696d 616c 7322 2c20 226f 7574 7075 7473  imals", "outputs
+0000d020: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+0000d030: 5479 7065 223a 2022 7569 6e74 3822 2c20  Type": "uint8", 
+0000d040: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
+0000d050: 6522 3a20 2275 696e 7438 2220 7d20 5d2c  e": "uint8" } ],
+0000d060: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
+0000d070: 7922 3a20 2270 7572 6522 2c20 2274 7970  y": "pure", "typ
+0000d080: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
+0000d090: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
+0000d0a0: 2c20 226e 616d 6522 3a20 2266 6163 746f  , "name": "facto
+0000d0b0: 7279 222c 2022 6f75 7470 7574 7322 3a20  ry", "outputs": 
+0000d0c0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000d0d0: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000d0e0: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
+0000d0f0: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
+0000d100: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
+0000d110: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
+0000d120: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
+0000d130: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
+0000d140: 5d2c 2022 6e61 6d65 223a 2022 6765 7452  ], "name": "getR
+0000d150: 6573 6572 7665 7322 2c20 226f 7574 7075  eserves", "outpu
+0000d160: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
+0000d170: 616c 5479 7065 223a 2022 7569 6e74 3131  alType": "uint11
+0000d180: 3222 2c20 226e 616d 6522 3a20 2272 6573  2", "name": "res
+0000d190: 6572 7665 3022 2c20 2274 7970 6522 3a20  erve0", "type": 
+0000d1a0: 2275 696e 7431 3132 2220 7d2c 207b 2022  "uint112" }, { "
+0000d1b0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000d1c0: 7569 6e74 3131 3222 2c20 226e 616d 6522  uint112", "name"
+0000d1d0: 3a20 2272 6573 6572 7665 3122 2c20 2274  : "reserve1", "t
+0000d1e0: 7970 6522 3a20 2275 696e 7431 3132 2220  ype": "uint112" 
+0000d1f0: 7d2c 207b 2022 696e 7465 726e 616c 5479  }, { "internalTy
+0000d200: 7065 223a 2022 7569 6e74 3332 222c 2022  pe": "uint32", "
+0000d210: 6e61 6d65 223a 2022 626c 6f63 6b54 696d  name": "blockTim
+0000d220: 6573 7461 6d70 4c61 7374 222c 2022 7479  estampLast", "ty
+0000d230: 7065 223a 2022 7569 6e74 3332 2220 7d20  pe": "uint32" } 
+0000d240: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
+0000d250: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
+0000d260: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+0000d270: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+0000d280: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000d290: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000d2a0: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
+0000d2b0: 223a 2022 6164 6472 6573 7322 207d 2c20  ": "address" }, 
+0000d2c0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000d2d0: 3a20 2261 6464 7265 7373 222c 2022 6e61  : "address", "na
+0000d2e0: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
+0000d2f0: 2022 6164 6472 6573 7322 207d 205d 2c20   "address" } ], 
+0000d300: 226e 616d 6522 3a20 2269 6e69 7469 616c  "name": "initial
+0000d310: 697a 6522 2c20 226f 7574 7075 7473 223a  ize", "outputs":
+0000d320: 205b 5d2c 2022 7374 6174 654d 7574 6162   [], "stateMutab
+0000d330: 696c 6974 7922 3a20 226e 6f6e 7061 7961  ility": "nonpaya
+0000d340: 626c 6522 2c20 2274 7970 6522 3a20 2266  ble", "type": "f
+0000d350: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
+0000d360: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
+0000d370: 6522 3a20 226b 4c61 7374 222c 2022 6f75  e": "kLast", "ou
+0000d380: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
+0000d390: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
+0000d3a0: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
+0000d3b0: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
+0000d3c0: 3235 3622 207d 205d 2c20 2273 7461 7465  256" } ], "state
+0000d3d0: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
+0000d3e0: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
+0000d3f0: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
+0000d400: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+0000d410: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+0000d420: 6573 7322 2c20 226e 616d 6522 3a20 2274  ess", "name": "t
+0000d430: 6f22 2c20 2274 7970 6522 3a20 2261 6464  o", "type": "add
+0000d440: 7265 7373 2220 7d20 5d2c 2022 6e61 6d65  ress" } ], "name
+0000d450: 223a 2022 6d69 6e74 222c 2022 6f75 7470  ": "mint", "outp
+0000d460: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+0000d470: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
+0000d480: 3536 222c 2022 6e61 6d65 223a 2022 6c69  56", "name": "li
+0000d490: 7175 6964 6974 7922 2c20 2274 7970 6522  quidity", "type"
+0000d4a0: 3a20 2275 696e 7432 3536 2220 7d20 5d2c  : "uint256" } ],
+0000d4b0: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
+0000d4c0: 7922 3a20 226e 6f6e 7061 7961 626c 6522  y": "nonpayable"
+0000d4d0: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
+0000d4e0: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
+0000d4f0: 7322 3a20 5b5d 2c20 226e 616d 6522 3a20  s": [], "name": 
+0000d500: 226e 616d 6522 2c20 226f 7574 7075 7473  "name", "outputs
+0000d510: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+0000d520: 5479 7065 223a 2022 7374 7269 6e67 222c  Type": "string",
+0000d530: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
+0000d540: 7065 223a 2022 7374 7269 6e67 2220 7d20  pe": "string" } 
+0000d550: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
+0000d560: 6974 7922 3a20 2270 7572 6522 2c20 2274  ity": "pure", "t
+0000d570: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+0000d580: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+0000d590: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000d5a0: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000d5b0: 6e61 6d65 223a 2022 6f77 6e65 7222 2c20  name": "owner", 
+0000d5c0: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+0000d5d0: 2220 7d20 5d2c 2022 6e61 6d65 223a 2022  " } ], "name": "
+0000d5e0: 6e6f 6e63 6573 222c 2022 6f75 7470 7574  nonces", "output
+0000d5f0: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
+0000d600: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000d610: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
+0000d620: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
+0000d630: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
+0000d640: 6269 6c69 7479 223a 2022 7669 6577 222c  bility": "view",
+0000d650: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
+0000d660: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
+0000d670: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+0000d680: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
+0000d690: 2c20 226e 616d 6522 3a20 226f 776e 6572  , "name": "owner
+0000d6a0: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
+0000d6b0: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
+0000d6c0: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+0000d6d0: 7373 222c 2022 6e61 6d65 223a 2022 7370  ss", "name": "sp
+0000d6e0: 656e 6465 7222 2c20 2274 7970 6522 3a20  ender", "type": 
+0000d6f0: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
+0000d700: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000d710: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
+0000d720: 3a20 2276 616c 7565 222c 2022 7479 7065  : "value", "type
+0000d730: 223a 2022 7569 6e74 3235 3622 207d 2c20  ": "uint256" }, 
+0000d740: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000d750: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+0000d760: 6d65 223a 2022 6465 6164 6c69 6e65 222c  me": "deadline",
+0000d770: 2022 7479 7065 223a 2022 7569 6e74 3235   "type": "uint25
+0000d780: 3622 207d 2c20 7b20 2269 6e74 6572 6e61  6" }, { "interna
+0000d790: 6c54 7970 6522 3a20 2275 696e 7438 222c  lType": "uint8",
+0000d7a0: 2022 6e61 6d65 223a 2022 7622 2c20 2274   "name": "v", "t
+0000d7b0: 7970 6522 3a20 2275 696e 7438 2220 7d2c  ype": "uint8" },
+0000d7c0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
+0000d7d0: 223a 2022 6279 7465 7333 3222 2c20 226e  ": "bytes32", "n
+0000d7e0: 616d 6522 3a20 2272 222c 2022 7479 7065  ame": "r", "type
+0000d7f0: 223a 2022 6279 7465 7333 3222 207d 2c20  ": "bytes32" }, 
+0000d800: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000d810: 3a20 2262 7974 6573 3332 222c 2022 6e61  : "bytes32", "na
+0000d820: 6d65 223a 2022 7322 2c20 2274 7970 6522  me": "s", "type"
+0000d830: 3a20 2262 7974 6573 3332 2220 7d20 5d2c  : "bytes32" } ],
+0000d840: 2022 6e61 6d65 223a 2022 7065 726d 6974   "name": "permit
+0000d850: 222c 2022 6f75 7470 7574 7322 3a20 5b5d  ", "outputs": []
+0000d860: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
+0000d870: 7479 223a 2022 6e6f 6e70 6179 6162 6c65  ty": "nonpayable
+0000d880: 222c 2022 7479 7065 223a 2022 6675 6e63  ", "type": "func
+0000d890: 7469 6f6e 2220 7d2c 207b 2022 696e 7075  tion" }, { "inpu
+0000d8a0: 7473 223a 205b 5d2c 2022 6e61 6d65 223a  ts": [], "name":
+0000d8b0: 2022 7072 6963 6530 4375 6d75 6c61 7469   "price0Cumulati
+0000d8c0: 7665 4c61 7374 222c 2022 6f75 7470 7574  veLast", "output
+0000d8d0: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
+0000d8e0: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000d8f0: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
+0000d900: 7479 7065 223a 2022 7569 6e74 3235 3622  type": "uint256"
+0000d910: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
+0000d920: 6269 6c69 7479 223a 2022 7669 6577 222c  bility": "view",
+0000d930: 2022 7479 7065 223a 2022 6675 6e63 7469   "type": "functi
+0000d940: 6f6e 2220 7d2c 207b 2022 696e 7075 7473  on" }, { "inputs
+0000d950: 223a 205b 5d2c 2022 6e61 6d65 223a 2022  ": [], "name": "
+0000d960: 7072 6963 6531 4375 6d75 6c61 7469 7665  price1Cumulative
+0000d970: 4c61 7374 222c 2022 6f75 7470 7574 7322  Last", "outputs"
+0000d980: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
+0000d990: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
+0000d9a0: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
+0000d9b0: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
+0000d9c0: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
+0000d9d0: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
+0000d9e0: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
+0000d9f0: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
+0000da00: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+0000da10: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
+0000da20: 226e 616d 6522 3a20 2274 6f22 2c20 2274  "name": "to", "t
+0000da30: 7970 6522 3a20 2261 6464 7265 7373 2220  ype": "address" 
+0000da40: 7d20 5d2c 2022 6e61 6d65 223a 2022 736b  } ], "name": "sk
+0000da50: 696d 222c 2022 6f75 7470 7574 7322 3a20  im", "outputs": 
+0000da60: 5b5d 2c20 2273 7461 7465 4d75 7461 6269  [], "stateMutabi
+0000da70: 6c69 7479 223a 2022 6e6f 6e70 6179 6162  lity": "nonpayab
+0000da80: 6c65 222c 2022 7479 7065 223a 2022 6675  le", "type": "fu
+0000da90: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
+0000daa0: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+0000dab0: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
+0000dac0: 3235 3622 2c20 226e 616d 6522 3a20 2261  256", "name": "a
+0000dad0: 6d6f 756e 7430 4f75 7422 2c20 2274 7970  mount0Out", "typ
+0000dae0: 6522 3a20 2275 696e 7432 3536 2220 7d2c  e": "uint256" },
+0000daf0: 207b 2022 696e 7465 726e 616c 5479 7065   { "internalType
+0000db00: 223a 2022 7569 6e74 3235 3622 2c20 226e  ": "uint256", "n
+0000db10: 616d 6522 3a20 2261 6d6f 756e 7431 4f75  ame": "amount1Ou
+0000db20: 7422 2c20 2274 7970 6522 3a20 2275 696e  t", "type": "uin
+0000db30: 7432 3536 2220 7d2c 207b 2022 696e 7465  t256" }, { "inte
+0000db40: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+0000db50: 6573 7322 2c20 226e 616d 6522 3a20 2274  ess", "name": "t
+0000db60: 6f22 2c20 2274 7970 6522 3a20 2261 6464  o", "type": "add
+0000db70: 7265 7373 2220 7d2c 207b 2022 696e 7465  ress" }, { "inte
+0000db80: 726e 616c 5479 7065 223a 2022 6279 7465  rnalType": "byte
+0000db90: 7322 2c20 226e 616d 6522 3a20 2264 6174  s", "name": "dat
+0000dba0: 6122 2c20 2274 7970 6522 3a20 2262 7974  a", "type": "byt
+0000dbb0: 6573 2220 7d20 5d2c 2022 6e61 6d65 223a  es" } ], "name":
+0000dbc0: 2022 7377 6170 222c 2022 6f75 7470 7574   "swap", "output
+0000dbd0: 7322 3a20 5b5d 2c20 2273 7461 7465 4d75  s": [], "stateMu
+0000dbe0: 7461 6269 6c69 7479 223a 2022 6e6f 6e70  tability": "nonp
+0000dbf0: 6179 6162 6c65 222c 2022 7479 7065 223a  ayable", "type":
+0000dc00: 2022 6675 6e63 7469 6f6e 2220 7d2c 207b   "function" }, {
+0000dc10: 2022 696e 7075 7473 223a 205b 5d2c 2022   "inputs": [], "
+0000dc20: 6e61 6d65 223a 2022 7379 6d62 6f6c 222c  name": "symbol",
+0000dc30: 2022 6f75 7470 7574 7322 3a20 5b20 7b20   "outputs": [ { 
+0000dc40: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000dc50: 2273 7472 696e 6722 2c20 226e 616d 6522  "string", "name"
+0000dc60: 3a20 2222 2c20 2274 7970 6522 3a20 2273  : "", "type": "s
+0000dc70: 7472 696e 6722 207d 205d 2c20 2273 7461  tring" } ], "sta
+0000dc80: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
+0000dc90: 7075 7265 222c 2022 7479 7065 223a 2022  pure", "type": "
+0000dca0: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
+0000dcb0: 696e 7075 7473 223a 205b 5d2c 2022 6e61  inputs": [], "na
+0000dcc0: 6d65 223a 2022 7379 6e63 222c 2022 6f75  me": "sync", "ou
+0000dcd0: 7470 7574 7322 3a20 5b5d 2c20 2273 7461  tputs": [], "sta
+0000dce0: 7465 4d75 7461 6269 6c69 7479 223a 2022  teMutability": "
+0000dcf0: 6e6f 6e70 6179 6162 6c65 222c 2022 7479  nonpayable", "ty
+0000dd00: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
+0000dd10: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
+0000dd20: 5d2c 2022 6e61 6d65 223a 2022 746f 6b65  ], "name": "toke
+0000dd30: 6e30 222c 2022 6f75 7470 7574 7322 3a20  n0", "outputs": 
+0000dd40: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000dd50: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000dd60: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
+0000dd70: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
+0000dd80: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
+0000dd90: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
+0000dda0: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
+0000ddb0: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
+0000ddc0: 5d2c 2022 6e61 6d65 223a 2022 746f 6b65  ], "name": "toke
+0000ddd0: 6e31 222c 2022 6f75 7470 7574 7322 3a20  n1", "outputs": 
+0000dde0: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000ddf0: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000de00: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
+0000de10: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
+0000de20: 2c20 2273 7461 7465 4d75 7461 6269 6c69  , "stateMutabili
+0000de30: 7479 223a 2022 7669 6577 222c 2022 7479  ty": "view", "ty
+0000de40: 7065 223a 2022 6675 6e63 7469 6f6e 2220  pe": "function" 
+0000de50: 7d2c 207b 2022 696e 7075 7473 223a 205b  }, { "inputs": [
+0000de60: 5d2c 2022 6e61 6d65 223a 2022 746f 7461  ], "name": "tota
+0000de70: 6c53 7570 706c 7922 2c20 226f 7574 7075  lSupply", "outpu
+0000de80: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
+0000de90: 616c 5479 7065 223a 2022 7569 6e74 3235  alType": "uint25
+0000dea0: 3622 2c20 226e 616d 6522 3a20 2222 2c20  6", "name": "", 
+0000deb0: 2274 7970 6522 3a20 2275 696e 7432 3536  "type": "uint256
+0000dec0: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+0000ded0: 6162 696c 6974 7922 3a20 2276 6965 7722  ability": "view"
+0000dee0: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
+0000def0: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
+0000df00: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
+0000df10: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
+0000df20: 222c 2022 6e61 6d65 223a 2022 746f 222c  ", "name": "to",
+0000df30: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000df40: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
+0000df50: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+0000df60: 222c 2022 6e61 6d65 223a 2022 7661 6c75  ", "name": "valu
+0000df70: 6522 2c20 2274 7970 6522 3a20 2275 696e  e", "type": "uin
+0000df80: 7432 3536 2220 7d20 5d2c 2022 6e61 6d65  t256" } ], "name
+0000df90: 223a 2022 7472 616e 7366 6572 222c 2022  ": "transfer", "
+0000dfa0: 6f75 7470 7574 7322 3a20 5b20 7b20 2269  outputs": [ { "i
+0000dfb0: 6e74 6572 6e61 6c54 7970 6522 3a20 2262  nternalType": "b
+0000dfc0: 6f6f 6c22 2c20 226e 616d 6522 3a20 2222  ool", "name": ""
+0000dfd0: 2c20 2274 7970 6522 3a20 2262 6f6f 6c22  , "type": "bool"
+0000dfe0: 207d 205d 2c20 2273 7461 7465 4d75 7461   } ], "stateMuta
+0000dff0: 6269 6c69 7479 223a 2022 6e6f 6e70 6179  bility": "nonpay
+0000e000: 6162 6c65 222c 2022 7479 7065 223a 2022  able", "type": "
+0000e010: 6675 6e63 7469 6f6e 2220 7d2c 207b 2022  function" }, { "
+0000e020: 696e 7075 7473 223a 205b 207b 2022 696e  inputs": [ { "in
+0000e030: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
+0000e040: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
+0000e050: 2266 726f 6d22 2c20 2274 7970 6522 3a20  "from", "type": 
+0000e060: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
+0000e070: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000e080: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
+0000e090: 3a20 2274 6f22 2c20 2274 7970 6522 3a20  : "to", "type": 
+0000e0a0: 2261 6464 7265 7373 2220 7d2c 207b 2022  "address" }, { "
+0000e0b0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000e0c0: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
+0000e0d0: 3a20 2276 616c 7565 222c 2022 7479 7065  : "value", "type
+0000e0e0: 223a 2022 7569 6e74 3235 3622 207d 205d  ": "uint256" } ]
+0000e0f0: 2c20 226e 616d 6522 3a20 2274 7261 6e73  , "name": "trans
+0000e100: 6665 7246 726f 6d22 2c20 226f 7574 7075  ferFrom", "outpu
+0000e110: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
+0000e120: 616c 5479 7065 223a 2022 626f 6f6c 222c  alType": "bool",
+0000e130: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
+0000e140: 7065 223a 2022 626f 6f6c 2220 7d20 5d2c  pe": "bool" } ],
+0000e150: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
+0000e160: 7922 3a20 226e 6f6e 7061 7961 626c 6522  y": "nonpayable"
+0000e170: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
+0000e180: 696f 6e22 207d 205d 270a 2020 2020 756e  ion" } ]'.    un
+0000e190: 6973 7761 705f 7633 5f65 7263 3230 5f61  iswap_v3_erc20_a
+0000e1a0: 6269 3d27 5b20 7b20 2261 6e6f 6e79 6d6f  bi='[ { "anonymo
+0000e1b0: 7573 223a 2066 616c 7365 2c20 2269 6e70  us": false, "inp
+0000e1c0: 7574 7322 3a20 5b20 7b20 2269 6e64 6578  uts": [ { "index
+0000e1d0: 6564 223a 2074 7275 652c 2022 696e 7465  ed": true, "inte
+0000e1e0: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+0000e1f0: 6573 7322 2c20 226e 616d 6522 3a20 226f  ess", "name": "o
+0000e200: 776e 6572 222c 2022 7479 7065 223a 2022  wner", "type": "
+0000e210: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
+0000e220: 6e64 6578 6564 223a 2074 7275 652c 2022  ndexed": true, "
+0000e230: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000e240: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
+0000e250: 3a20 2273 7065 6e64 6572 222c 2022 7479  : "spender", "ty
+0000e260: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
+0000e270: 2c20 7b20 2269 6e64 6578 6564 223a 2066  , { "indexed": f
+0000e280: 616c 7365 2c20 2269 6e74 6572 6e61 6c54  alse, "internalT
+0000e290: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
+0000e2a0: 2022 6e61 6d65 223a 2022 7661 6c75 6522   "name": "value"
+0000e2b0: 2c20 2274 7970 6522 3a20 2275 696e 7432  , "type": "uint2
+0000e2c0: 3536 2220 7d20 5d2c 2022 6e61 6d65 223a  56" } ], "name":
+0000e2d0: 2022 4170 7072 6f76 616c 222c 2022 7479   "Approval", "ty
+0000e2e0: 7065 223a 2022 6576 656e 7422 207d 2c20  pe": "event" }, 
+0000e2f0: 7b20 2261 6e6f 6e79 6d6f 7573 223a 2066  { "anonymous": f
+0000e300: 616c 7365 2c20 2269 6e70 7574 7322 3a20  alse, "inputs": 
+0000e310: 5b20 7b20 2269 6e64 6578 6564 223a 2074  [ { "indexed": t
+0000e320: 7275 652c 2022 696e 7465 726e 616c 5479  rue, "internalTy
+0000e330: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
+0000e340: 226e 616d 6522 3a20 2266 726f 6d22 2c20  "name": "from", 
+0000e350: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+0000e360: 2220 7d2c 207b 2022 696e 6465 7865 6422  " }, { "indexed"
+0000e370: 3a20 7472 7565 2c20 2269 6e74 6572 6e61  : true, "interna
+0000e380: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
+0000e390: 222c 2022 6e61 6d65 223a 2022 746f 222c  ", "name": "to",
+0000e3a0: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+0000e3b0: 7322 207d 2c20 7b20 2269 6e64 6578 6564  s" }, { "indexed
+0000e3c0: 223a 2066 616c 7365 2c20 2269 6e74 6572  ": false, "inter
+0000e3d0: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
+0000e3e0: 3536 222c 2022 6e61 6d65 223a 2022 7661  56", "name": "va
+0000e3f0: 6c75 6522 2c20 2274 7970 6522 3a20 2275  lue", "type": "u
+0000e400: 696e 7432 3536 2220 7d20 5d2c 2022 6e61  int256" } ], "na
+0000e410: 6d65 223a 2022 5472 616e 7366 6572 222c  me": "Transfer",
+0000e420: 2022 7479 7065 223a 2022 6576 656e 7422   "type": "event"
+0000e430: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+0000e440: 5b20 7b20 2269 6e74 6572 6e61 6c54 7970  [ { "internalTyp
+0000e450: 6522 3a20 2261 6464 7265 7373 222c 2022  e": "address", "
+0000e460: 6e61 6d65 223a 2022 6f77 6e65 7222 2c20  name": "owner", 
+0000e470: 2274 7970 6522 3a20 2261 6464 7265 7373  "type": "address
+0000e480: 2220 7d2c 207b 2022 696e 7465 726e 616c  " }, { "internal
+0000e490: 5479 7065 223a 2022 6164 6472 6573 7322  Type": "address"
+0000e4a0: 2c20 226e 616d 6522 3a20 2273 7065 6e64  , "name": "spend
+0000e4b0: 6572 222c 2022 7479 7065 223a 2022 6164  er", "type": "ad
+0000e4c0: 6472 6573 7322 207d 205d 2c20 226e 616d  dress" } ], "nam
+0000e4d0: 6522 3a20 2261 6c6c 6f77 616e 6365 222c  e": "allowance",
+0000e4e0: 2022 6f75 7470 7574 7322 3a20 5b20 7b20   "outputs": [ { 
+0000e4f0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000e500: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
+0000e510: 223a 2022 222c 2022 7479 7065 223a 2022  ": "", "type": "
+0000e520: 7569 6e74 3235 3622 207d 205d 2c20 2273  uint256" } ], "s
+0000e530: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+0000e540: 2022 7669 6577 222c 2022 7479 7065 223a   "view", "type":
+0000e550: 2022 6675 6e63 7469 6f6e 2220 7d2c 207b   "function" }, {
+0000e560: 2022 696e 7075 7473 223a 205b 207b 2022   "inputs": [ { "
+0000e570: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000e580: 6164 6472 6573 7322 2c20 226e 616d 6522  address", "name"
+0000e590: 3a20 2273 7065 6e64 6572 222c 2022 7479  : "spender", "ty
+0000e5a0: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
+0000e5b0: 2c20 7b20 2269 6e74 6572 6e61 6c54 7970  , { "internalTyp
+0000e5c0: 6522 3a20 2275 696e 7432 3536 222c 2022  e": "uint256", "
+0000e5d0: 6e61 6d65 223a 2022 7661 6c75 6522 2c20  name": "value", 
+0000e5e0: 2274 7970 6522 3a20 2275 696e 7432 3536  "type": "uint256
+0000e5f0: 2220 7d20 5d2c 2022 6e61 6d65 223a 2022  " } ], "name": "
+0000e600: 6170 7072 6f76 6522 2c20 226f 7574 7075  approve", "outpu
+0000e610: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
+0000e620: 616c 5479 7065 223a 2022 626f 6f6c 222c  alType": "bool",
+0000e630: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
+0000e640: 7065 223a 2022 626f 6f6c 2220 7d20 5d2c  pe": "bool" } ],
+0000e650: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
+0000e660: 7922 3a20 226e 6f6e 7061 7961 626c 6522  y": "nonpayable"
+0000e670: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
+0000e680: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
+0000e690: 7322 3a20 5b20 7b20 2269 6e74 6572 6e61  s": [ { "interna
+0000e6a0: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
+0000e6b0: 222c 2022 6e61 6d65 223a 2022 6f77 6e65  ", "name": "owne
+0000e6c0: 7222 2c20 2274 7970 6522 3a20 2261 6464  r", "type": "add
+0000e6d0: 7265 7373 2220 7d20 5d2c 2022 6e61 6d65  ress" } ], "name
+0000e6e0: 223a 2022 6261 6c61 6e63 654f 6622 2c20  ": "balanceOf", 
+0000e6f0: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+0000e700: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+0000e710: 7569 6e74 3235 3622 2c20 226e 616d 6522  uint256", "name"
+0000e720: 3a20 2222 2c20 2274 7970 6522 3a20 2275  : "", "type": "u
+0000e730: 696e 7432 3536 2220 7d20 5d2c 2022 7374  int256" } ], "st
+0000e740: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
+0000e750: 2276 6965 7722 2c20 2274 7970 6522 3a20  "view", "type": 
+0000e760: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
+0000e770: 2269 6e70 7574 7322 3a20 5b5d 2c20 226e  "inputs": [], "n
+0000e780: 616d 6522 3a20 2264 6563 696d 616c 7322  ame": "decimals"
+0000e790: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
+0000e7a0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000e7b0: 2022 7569 6e74 3822 2c20 226e 616d 6522   "uint8", "name"
+0000e7c0: 3a20 2222 2c20 2274 7970 6522 3a20 2275  : "", "type": "u
+0000e7d0: 696e 7438 2220 7d20 5d2c 2022 7374 6174  int8" } ], "stat
+0000e7e0: 654d 7574 6162 696c 6974 7922 3a20 2276  eMutability": "v
+0000e7f0: 6965 7722 2c20 2274 7970 6522 3a20 2266  iew", "type": "f
+0000e800: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
+0000e810: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
+0000e820: 6522 3a20 226e 616d 6522 2c20 226f 7574  e": "name", "out
+0000e830: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+0000e840: 726e 616c 5479 7065 223a 2022 7374 7269  rnalType": "stri
+0000e850: 6e67 222c 2022 6e61 6d65 223a 2022 222c  ng", "name": "",
+0000e860: 2022 7479 7065 223a 2022 7374 7269 6e67   "type": "string
+0000e870: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+0000e880: 6162 696c 6974 7922 3a20 2276 6965 7722  ability": "view"
+0000e890: 2c20 2274 7970 6522 3a20 2266 756e 6374  , "type": "funct
+0000e8a0: 696f 6e22 207d 2c20 7b20 2269 6e70 7574  ion" }, { "input
+0000e8b0: 7322 3a20 5b5d 2c20 226e 616d 6522 3a20  s": [], "name": 
+0000e8c0: 2273 796d 626f 6c22 2c20 226f 7574 7075  "symbol", "outpu
+0000e8d0: 7473 223a 205b 207b 2022 696e 7465 726e  ts": [ { "intern
+0000e8e0: 616c 5479 7065 223a 2022 7374 7269 6e67  alType": "string
+0000e8f0: 222c 2022 6e61 6d65 223a 2022 222c 2022  ", "name": "", "
+0000e900: 7479 7065 223a 2022 7374 7269 6e67 2220  type": "string" 
+0000e910: 7d20 5d2c 2022 7374 6174 654d 7574 6162  } ], "stateMutab
+0000e920: 696c 6974 7922 3a20 2276 6965 7722 2c20  ility": "view", 
+0000e930: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
+0000e940: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
+0000e950: 3a20 5b5d 2c20 226e 616d 6522 3a20 2274  : [], "name": "t
+0000e960: 6f74 616c 5375 7070 6c79 222c 2022 6f75  otalSupply", "ou
+0000e970: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
+0000e980: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
+0000e990: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
+0000e9a0: 222c 2022 7479 7065 223a 2022 7569 6e74  ", "type": "uint
+0000e9b0: 3235 3622 207d 205d 2c20 2273 7461 7465  256" } ], "state
+0000e9c0: 4d75 7461 6269 6c69 7479 223a 2022 7669  Mutability": "vi
+0000e9d0: 6577 222c 2022 7479 7065 223a 2022 6675  ew", "type": "fu
+0000e9e0: 6e63 7469 6f6e 2220 7d2c 207b 2022 696e  nction" }, { "in
+0000e9f0: 7075 7473 223a 205b 207b 2022 696e 7465  puts": [ { "inte
+0000ea00: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+0000ea10: 6573 7322 2c20 226e 616d 6522 3a20 2274  ess", "name": "t
+0000ea20: 6f22 2c20 2274 7970 6522 3a20 2261 6464  o", "type": "add
+0000ea30: 7265 7373 2220 7d2c 207b 2022 696e 7465  ress" }, { "inte
+0000ea40: 726e 616c 5479 7065 223a 2022 7569 6e74  rnalType": "uint
+0000ea50: 3235 3622 2c20 226e 616d 6522 3a20 2276  256", "name": "v
+0000ea60: 616c 7565 222c 2022 7479 7065 223a 2022  alue", "type": "
+0000ea70: 7569 6e74 3235 3622 207d 205d 2c20 226e  uint256" } ], "n
+0000ea80: 616d 6522 3a20 2274 7261 6e73 6665 7222  ame": "transfer"
+0000ea90: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
+0000eaa0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+0000eab0: 2022 626f 6f6c 222c 2022 6e61 6d65 223a   "bool", "name":
+0000eac0: 2022 222c 2022 7479 7065 223a 2022 626f   "", "type": "bo
+0000ead0: 6f6c 2220 7d20 5d2c 2022 7374 6174 654d  ol" } ], "stateM
+0000eae0: 7574 6162 696c 6974 7922 3a20 226e 6f6e  utability": "non
+0000eaf0: 7061 7961 626c 6522 2c20 2274 7970 6522  payable", "type"
+0000eb00: 3a20 2266 756e 6374 696f 6e22 207d 2c20  : "function" }, 
+0000eb10: 7b20 2269 6e70 7574 7322 3a20 5b20 7b20  { "inputs": [ { 
+0000eb20: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+0000eb30: 2261 6464 7265 7373 222c 2022 6e61 6d65  "address", "name
+0000eb40: 223a 2022 6672 6f6d 222c 2022 7479 7065  ": "from", "type
+0000eb50: 223a 2022 6164 6472 6573 7322 207d 2c20  ": "address" }, 
+0000eb60: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000eb70: 3a20 2261 6464 7265 7373 222c 2022 6e61  : "address", "na
+0000eb80: 6d65 223a 2022 746f 222c 2022 7479 7065  me": "to", "type
+0000eb90: 223a 2022 6164 6472 6573 7322 207d 2c20  ": "address" }, 
+0000eba0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+0000ebb0: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+0000ebc0: 6d65 223a 2022 7661 6c75 6522 2c20 2274  me": "value", "t
+0000ebd0: 7970 6522 3a20 2275 696e 7432 3536 2220  ype": "uint256" 
+0000ebe0: 7d20 5d2c 2022 6e61 6d65 223a 2022 7472  } ], "name": "tr
+0000ebf0: 616e 7366 6572 4672 6f6d 222c 2022 6f75  ansferFrom", "ou
+0000ec00: 7470 7574 7322 3a20 5b20 7b20 2269 6e74  tputs": [ { "int
+0000ec10: 6572 6e61 6c54 7970 6522 3a20 2262 6f6f  ernalType": "boo
+0000ec20: 6c22 2c20 226e 616d 6522 3a20 2222 2c20  l", "name": "", 
+0000ec30: 2274 7970 6522 3a20 2262 6f6f 6c22 207d  "type": "bool" }
+0000ec40: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
+0000ec50: 6c69 7479 223a 2022 6e6f 6e70 6179 6162  lity": "nonpayab
+0000ec60: 6c65 222c 2022 7479 7065 223a 2022 6675  le", "type": "fu
+0000ec70: 6e63 7469 6f6e 2220 7d20 5d27 0a20 2020  nction" } ]'.   
+0000ec80: 2023 6874 7470 733a 2f2f 6574 6865 7273   #https://ethers
+0000ec90: 6361 6e2e 696f 2f61 6464 7265 7373 2f30  can.io/address/0
+0000eca0: 7865 3539 3234 3237 6130 6165 6365 3932  xe592427a0aece92
+0000ecb0: 6465 3365 6465 6531 6631 3865 3031 3537  de3edee1f18e0157
+0000ecc0: 6330 3538 3631 3536 3423 636f 6465 0a20  c05861564#code. 
+0000ecd0: 2020 2075 6e69 7377 6170 5f76 335f 726f     uniswap_v3_ro
+0000ece0: 7574 655f 6162 693d 275b 7b22 696e 7075  ute_abi='[{"inpu
+0000ecf0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0000ed00: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0000ed10: 6e61 6d65 223a 225f 6661 6374 6f72 7922  name":"_factory"
+0000ed20: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0000ed30: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0000ed40: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+0000ed50: 6d65 223a 225f 5745 5448 3922 2c22 7479  me":"_WETH9","ty
+0000ed60: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
+0000ed70: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+0000ed80: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+0000ed90: 7479 7065 223a 2263 6f6e 7374 7275 6374  type":"construct
+0000eda0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0000edb0: 5d2c 226e 616d 6522 3a22 5745 5448 3922  ],"name":"WETH9"
+0000edc0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+0000edd0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0000ede0: 7265 7373 222c 226e 616d 6522 3a22 222c  ress","name":"",
+0000edf0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0000ee00: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
+0000ee10: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
+0000ee20: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+0000ee30: 2269 6e70 7574 7322 3a5b 7b22 636f 6d70  "inputs":[{"comp
+0000ee40: 6f6e 656e 7473 223a 5b7b 2269 6e74 6572  onents":[{"inter
+0000ee50: 6e61 6c54 7970 6522 3a22 6279 7465 7322  nalType":"bytes"
+0000ee60: 2c22 6e61 6d65 223a 2270 6174 6822 2c22  ,"name":"path","
+0000ee70: 7479 7065 223a 2262 7974 6573 227d 2c7b  type":"bytes"},{
+0000ee80: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000ee90: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+0000eea0: 2272 6563 6970 6965 6e74 222c 2274 7970  "recipient","typ
+0000eeb0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0000eec0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0000eed0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0000eee0: 6465 6164 6c69 6e65 222c 2274 7970 6522  deadline","type"
+0000eef0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0000ef00: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0000ef10: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0000ef20: 6f75 6e74 496e 222c 2274 7970 6522 3a22  ountIn","type":"
+0000ef30: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0000ef40: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0000ef50: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+0000ef60: 6e74 4f75 744d 696e 696d 756d 222c 2274  ntOutMinimum","t
+0000ef70: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0000ef80: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0000ef90: 2273 7472 7563 7420 4953 7761 7052 6f75  "struct ISwapRou
+0000efa0: 7465 722e 4578 6163 7449 6e70 7574 5061  ter.ExactInputPa
+0000efb0: 7261 6d73 222c 226e 616d 6522 3a22 7061  rams","name":"pa
+0000efc0: 7261 6d73 222c 2274 7970 6522 3a22 7475  rams","type":"tu
+0000efd0: 706c 6522 7d5d 2c22 6e61 6d65 223a 2265  ple"}],"name":"e
+0000efe0: 7861 6374 496e 7075 7422 2c22 6f75 7470  xactInput","outp
+0000eff0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+0000f000: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0000f010: 226e 616d 6522 3a22 616d 6f75 6e74 4f75  "name":"amountOu
+0000f020: 7422 2c22 7479 7065 223a 2275 696e 7432  t","type":"uint2
+0000f030: 3536 227d 5d2c 2273 7461 7465 4d75 7461  56"}],"stateMuta
+0000f040: 6269 6c69 7479 223a 2270 6179 6162 6c65  bility":"payable
+0000f050: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+0000f060: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+0000f070: 7b22 636f 6d70 6f6e 656e 7473 223a 5b7b  {"components":[{
+0000f080: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000f090: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+0000f0a0: 2274 6f6b 656e 496e 222c 2274 7970 6522  "tokenIn","type"
+0000f0b0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0000f0c0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0000f0d0: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
+0000f0e0: 6b65 6e4f 7574 222c 2274 7970 6522 3a22  kenOut","type":"
+0000f0f0: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+0000f100: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0000f110: 3422 2c22 6e61 6d65 223a 2266 6565 222c  4","name":"fee",
+0000f120: 2274 7970 6522 3a22 7569 6e74 3234 227d  "type":"uint24"}
+0000f130: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0000f140: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0000f150: 223a 2272 6563 6970 6965 6e74 222c 2274  ":"recipient","t
+0000f160: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+0000f170: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0000f180: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0000f190: 3a22 6465 6164 6c69 6e65 222c 2274 7970  :"deadline","typ
+0000f1a0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0000f1b0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0000f1c0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0000f1d0: 616d 6f75 6e74 496e 222c 2274 7970 6522  amountIn","type"
+0000f1e0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0000f1f0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0000f200: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0000f210: 6f75 6e74 4f75 744d 696e 696d 756d 222c  ountOutMinimum",
+0000f220: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0000f230: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000f240: 223a 2275 696e 7431 3630 222c 226e 616d  ":"uint160","nam
+0000f250: 6522 3a22 7371 7274 5072 6963 654c 696d  e":"sqrtPriceLim
+0000f260: 6974 5839 3622 2c22 7479 7065 223a 2275  itX96","type":"u
+0000f270: 696e 7431 3630 227d 5d2c 2269 6e74 6572  int160"}],"inter
+0000f280: 6e61 6c54 7970 6522 3a22 7374 7275 6374  nalType":"struct
+0000f290: 2049 5377 6170 526f 7574 6572 2e45 7861   ISwapRouter.Exa
+0000f2a0: 6374 496e 7075 7453 696e 676c 6550 6172  ctInputSinglePar
+0000f2b0: 616d 7322 2c22 6e61 6d65 223a 2270 6172  ams","name":"par
+0000f2c0: 616d 7322 2c22 7479 7065 223a 2274 7570  ams","type":"tup
+0000f2d0: 6c65 227d 5d2c 226e 616d 6522 3a22 6578  le"}],"name":"ex
+0000f2e0: 6163 7449 6e70 7574 5369 6e67 6c65 222c  actInputSingle",
+0000f2f0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
+0000f300: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0000f310: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
+0000f320: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
+0000f330: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
+0000f340: 654d 7574 6162 696c 6974 7922 3a22 7061  eMutability":"pa
+0000f350: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
+0000f360: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+0000f370: 7473 223a 5b7b 2263 6f6d 706f 6e65 6e74  ts":[{"component
+0000f380: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0000f390: 7065 223a 2262 7974 6573 222c 226e 616d  pe":"bytes","nam
+0000f3a0: 6522 3a22 7061 7468 222c 2274 7970 6522  e":"path","type"
+0000f3b0: 3a22 6279 7465 7322 7d2c 7b22 696e 7465  :"bytes"},{"inte
+0000f3c0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0000f3d0: 7373 222c 226e 616d 6522 3a22 7265 6369  ss","name":"reci
+0000f3e0: 7069 656e 7422 2c22 7479 7065 223a 2261  pient","type":"a
+0000f3f0: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+0000f400: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0000f410: 3622 2c22 6e61 6d65 223a 2264 6561 646c  6","name":"deadl
+0000f420: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
+0000f430: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+0000f440: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0000f450: 2c22 6e61 6d65 223a 2261 6d6f 756e 744f  ,"name":"amountO
+0000f460: 7574 222c 2274 7970 6522 3a22 7569 6e74  ut","type":"uint
+0000f470: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0000f480: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0000f490: 226e 616d 6522 3a22 616d 6f75 6e74 496e  "name":"amountIn
+0000f4a0: 4d61 7869 6d75 6d22 2c22 7479 7065 223a  Maximum","type":
+0000f4b0: 2275 696e 7432 3536 227d 5d2c 2269 6e74  "uint256"}],"int
+0000f4c0: 6572 6e61 6c54 7970 6522 3a22 7374 7275  ernalType":"stru
+0000f4d0: 6374 2049 5377 6170 526f 7574 6572 2e45  ct ISwapRouter.E
+0000f4e0: 7861 6374 4f75 7470 7574 5061 7261 6d73  xactOutputParams
+0000f4f0: 222c 226e 616d 6522 3a22 7061 7261 6d73  ","name":"params
+0000f500: 222c 2274 7970 6522 3a22 7475 706c 6522  ","type":"tuple"
+0000f510: 7d5d 2c22 6e61 6d65 223a 2265 7861 6374  }],"name":"exact
+0000f520: 4f75 7470 7574 222c 226f 7574 7075 7473  Output","outputs
+0000f530: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0000f540: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0000f550: 6d65 223a 2261 6d6f 756e 7449 6e22 2c22  me":"amountIn","
+0000f560: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0000f570: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+0000f580: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
+0000f590: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+0000f5a0: 2c7b 2269 6e70 7574 7322 3a5b 7b22 636f  ,{"inputs":[{"co
+0000f5b0: 6d70 6f6e 656e 7473 223a 5b7b 2269 6e74  mponents":[{"int
+0000f5c0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0000f5d0: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
+0000f5e0: 656e 496e 222c 2274 7970 6522 3a22 6164  enIn","type":"ad
+0000f5f0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0000f600: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+0000f610: 222c 226e 616d 6522 3a22 746f 6b65 6e4f  ","name":"tokenO
+0000f620: 7574 222c 2274 7970 6522 3a22 6164 6472  ut","type":"addr
+0000f630: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0000f640: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
+0000f650: 6e61 6d65 223a 2266 6565 222c 2274 7970  name":"fee","typ
+0000f660: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
+0000f670: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+0000f680: 6472 6573 7322 2c22 6e61 6d65 223a 2272  dress","name":"r
+0000f690: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
+0000f6a0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0000f6b0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0000f6c0: 7432 3536 222c 226e 616d 6522 3a22 6465  t256","name":"de
+0000f6d0: 6164 6c69 6e65 222c 2274 7970 6522 3a22  adline","type":"
+0000f6e0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0000f6f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0000f700: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+0000f710: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
+0000f720: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
 0000f730: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
 0000f740: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-0000f750: 7449 6e22 2c22 7479 7065 223a 2275 696e  tIn","type":"uin
-0000f760: 7432 3536 227d 5d2c 2273 7461 7465 4d75  t256"}],"stateMu
-0000f770: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
-0000f780: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
-0000f790: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-0000f7a0: 3a5b 5d2c 226e 616d 6522 3a22 6661 6374  :[],"name":"fact
-0000f7b0: 6f72 7922 2c22 6f75 7470 7574 7322 3a5b  ory","outputs":[
-0000f7c0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0000f7d0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0000f7e0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
-0000f7f0: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
-0000f800: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-0000f810: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-0000f820: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-0000f830: 696e 7465 726e 616c 5479 7065 223a 2262  internalType":"b
-0000f840: 7974 6573 5b5d 222c 226e 616d 6522 3a22  ytes[]","name":"
-0000f850: 6461 7461 222c 2274 7970 6522 3a22 6279  data","type":"by
-0000f860: 7465 735b 5d22 7d5d 2c22 6e61 6d65 223a  tes[]"}],"name":
-0000f870: 226d 756c 7469 6361 6c6c 222c 226f 7574  "multicall","out
-0000f880: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0000f890: 6c54 7970 6522 3a22 6279 7465 735b 5d22  lType":"bytes[]"
-0000f8a0: 2c22 6e61 6d65 223a 2272 6573 756c 7473  ,"name":"results
-0000f8b0: 222c 2274 7970 6522 3a22 6279 7465 735b  ","type":"bytes[
-0000f8c0: 5d22 7d5d 2c22 7374 6174 654d 7574 6162  ]"}],"stateMutab
-0000f8d0: 696c 6974 7922 3a22 7061 7961 626c 6522  ility":"payable"
-0000f8e0: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-0000f8f0: 6e22 7d2c 7b22 696e 7075 7473 223a 5b5d  n"},{"inputs":[]
-0000f900: 2c22 6e61 6d65 223a 2272 6566 756e 6445  ,"name":"refundE
-0000f910: 5448 222c 226f 7574 7075 7473 223a 5b5d  TH","outputs":[]
-0000f920: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-0000f930: 7922 3a22 7061 7961 626c 6522 2c22 7479  y":"payable","ty
-0000f940: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-0000f950: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-0000f960: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0000f970: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
-0000f980: 656e 222c 2274 7970 6522 3a22 6164 6472  en","type":"addr
-0000f990: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0000f9a0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0000f9b0: 226e 616d 6522 3a22 7661 6c75 6522 2c22  "name":"value","
-0000f9c0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0000f9d0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0000f9e0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0000f9f0: 223a 2264 6561 646c 696e 6522 2c22 7479  ":"deadline","ty
-0000fa00: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-0000fa10: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0000fa20: 7569 6e74 3822 2c22 6e61 6d65 223a 2276  uint8","name":"v
-0000fa30: 222c 2274 7970 6522 3a22 7569 6e74 3822  ","type":"uint8"
-0000fa40: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0000fa50: 223a 2262 7974 6573 3332 222c 226e 616d  ":"bytes32","nam
-0000fa60: 6522 3a22 7222 2c22 7479 7065 223a 2262  e":"r","type":"b
-0000fa70: 7974 6573 3332 227d 2c7b 2269 6e74 6572  ytes32"},{"inter
-0000fa80: 6e61 6c54 7970 6522 3a22 6279 7465 7333  nalType":"bytes3
-0000fa90: 3222 2c22 6e61 6d65 223a 2273 222c 2274  2","name":"s","t
-0000faa0: 7970 6522 3a22 6279 7465 7333 3222 7d5d  ype":"bytes32"}]
-0000fab0: 2c22 6e61 6d65 223a 2273 656c 6650 6572  ,"name":"selfPer
-0000fac0: 6d69 7422 2c22 6f75 7470 7574 7322 3a5b  mit","outputs":[
-0000fad0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-0000fae0: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
-0000faf0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-0000fb00: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-0000fb10: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0000fb20: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
-0000fb30: 6b65 6e22 2c22 7479 7065 223a 2261 6464  ken","type":"add
-0000fb40: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0000fb50: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0000fb60: 2c22 6e61 6d65 223a 226e 6f6e 6365 222c  ,"name":"nonce",
-0000fb70: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0000fb80: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0000fb90: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0000fba0: 6522 3a22 6578 7069 7279 222c 2274 7970  e":"expiry","typ
-0000fbb0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0000fbc0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0000fbd0: 696e 7438 222c 226e 616d 6522 3a22 7622  int8","name":"v"
-0000fbe0: 2c22 7479 7065 223a 2275 696e 7438 227d  ,"type":"uint8"}
-0000fbf0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0000fc00: 3a22 6279 7465 7333 3222 2c22 6e61 6d65  :"bytes32","name
-0000fc10: 223a 2272 222c 2274 7970 6522 3a22 6279  ":"r","type":"by
-0000fc20: 7465 7333 3222 7d2c 7b22 696e 7465 726e  tes32"},{"intern
-0000fc30: 616c 5479 7065 223a 2262 7974 6573 3332  alType":"bytes32
-0000fc40: 222c 226e 616d 6522 3a22 7322 2c22 7479  ","name":"s","ty
-0000fc50: 7065 223a 2262 7974 6573 3332 227d 5d2c  pe":"bytes32"}],
-0000fc60: 226e 616d 6522 3a22 7365 6c66 5065 726d  "name":"selfPerm
-0000fc70: 6974 416c 6c6f 7765 6422 2c22 6f75 7470  itAllowed","outp
-0000fc80: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
-0000fc90: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
-0000fca0: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
-0000fcb0: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-0000fcc0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0000fcd0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0000fce0: 6522 3a22 746f 6b65 6e22 2c22 7479 7065  e":"token","type
-0000fcf0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0000fd00: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0000fd10: 6e74 3235 3622 2c22 6e61 6d65 223a 226e  nt256","name":"n
-0000fd20: 6f6e 6365 222c 2274 7970 6522 3a22 7569  once","type":"ui
-0000fd30: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
-0000fd40: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0000fd50: 222c 226e 616d 6522 3a22 6578 7069 7279  ","name":"expiry
-0000fd60: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0000fd70: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-0000fd80: 7065 223a 2275 696e 7438 222c 226e 616d  pe":"uint8","nam
-0000fd90: 6522 3a22 7622 2c22 7479 7065 223a 2275  e":"v","type":"u
-0000fda0: 696e 7438 227d 2c7b 2269 6e74 6572 6e61  int8"},{"interna
-0000fdb0: 6c54 7970 6522 3a22 6279 7465 7333 3222  lType":"bytes32"
-0000fdc0: 2c22 6e61 6d65 223a 2272 222c 2274 7970  ,"name":"r","typ
-0000fdd0: 6522 3a22 6279 7465 7333 3222 7d2c 7b22  e":"bytes32"},{"
-0000fde0: 696e 7465 726e 616c 5479 7065 223a 2262  internalType":"b
-0000fdf0: 7974 6573 3332 222c 226e 616d 6522 3a22  ytes32","name":"
-0000fe00: 7322 2c22 7479 7065 223a 2262 7974 6573  s","type":"bytes
-0000fe10: 3332 227d 5d2c 226e 616d 6522 3a22 7365  32"}],"name":"se
-0000fe20: 6c66 5065 726d 6974 416c 6c6f 7765 6449  lfPermitAllowedI
-0000fe30: 664e 6563 6573 7361 7279 222c 226f 7574  fNecessary","out
-0000fe40: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
-0000fe50: 7574 6162 696c 6974 7922 3a22 7061 7961  utability":"paya
-0000fe60: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
-0000fe70: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-0000fe80: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0000fe90: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0000fea0: 6d65 223a 2274 6f6b 656e 222c 2274 7970  me":"token","typ
-0000feb0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0000fec0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0000fed0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0000fee0: 7661 6c75 6522 2c22 7479 7065 223a 2275  value","type":"u
-0000fef0: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0000ff00: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0000ff10: 3622 2c22 6e61 6d65 223a 2264 6561 646c  6","name":"deadl
-0000ff20: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
-0000ff30: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-0000ff40: 6c54 7970 6522 3a22 7569 6e74 3822 2c22  lType":"uint8","
-0000ff50: 6e61 6d65 223a 2276 222c 2274 7970 6522  name":"v","type"
-0000ff60: 3a22 7569 6e74 3822 7d2c 7b22 696e 7465  :"uint8"},{"inte
-0000ff70: 726e 616c 5479 7065 223a 2262 7974 6573  rnalType":"bytes
-0000ff80: 3332 222c 226e 616d 6522 3a22 7222 2c22  32","name":"r","
-0000ff90: 7479 7065 223a 2262 7974 6573 3332 227d  type":"bytes32"}
-0000ffa0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0000ffb0: 3a22 6279 7465 7333 3222 2c22 6e61 6d65  :"bytes32","name
-0000ffc0: 223a 2273 222c 2274 7970 6522 3a22 6279  ":"s","type":"by
-0000ffd0: 7465 7333 3222 7d5d 2c22 6e61 6d65 223a  tes32"}],"name":
-0000ffe0: 2273 656c 6650 6572 6d69 7449 664e 6563  "selfPermitIfNec
-0000fff0: 6573 7361 7279 222c 226f 7574 7075 7473  essary","outputs
-00010000: 223a 5b5d 2c22 7374 6174 654d 7574 6162  ":[],"stateMutab
-00010010: 696c 6974 7922 3a22 7061 7961 626c 6522  ility":"payable"
-00010020: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-00010030: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
-00010040: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00010050: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-00010060: 2274 6f6b 656e 222c 2274 7970 6522 3a22  "token","type":"
-00010070: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-00010080: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00010090: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-000100a0: 6e74 4d69 6e69 6d75 6d22 2c22 7479 7065  ntMinimum","type
-000100b0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-000100c0: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-000100d0: 6472 6573 7322 2c22 6e61 6d65 223a 2272  dress","name":"r
-000100e0: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
-000100f0: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
-00010100: 6d65 223a 2273 7765 6570 546f 6b65 6e22  me":"sweepToken"
-00010110: 2c22 6f75 7470 7574 7322 3a5b 5d2c 2273  ,"outputs":[],"s
-00010120: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00010130: 2270 6179 6162 6c65 222c 2274 7970 6522  "payable","type"
-00010140: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00010150: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00010160: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-00010170: 222c 226e 616d 6522 3a22 746f 6b65 6e22  ","name":"token"
-00010180: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00010190: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-000101a0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-000101b0: 6d65 223a 2261 6d6f 756e 744d 696e 696d  me":"amountMinim
-000101c0: 756d 222c 2274 7970 6522 3a22 7569 6e74  um","type":"uint
-000101d0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-000101e0: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-000101f0: 226e 616d 6522 3a22 7265 6369 7069 656e  "name":"recipien
-00010200: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
-00010210: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-00010220: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00010230: 6e61 6d65 223a 2266 6565 4269 7073 222c  name":"feeBips",
-00010240: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00010250: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00010260: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-00010270: 6522 3a22 6665 6552 6563 6970 6965 6e74  e":"feeRecipient
-00010280: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00010290: 7322 7d5d 2c22 6e61 6d65 223a 2273 7765  s"}],"name":"swe
-000102a0: 6570 546f 6b65 6e57 6974 6846 6565 222c  epTokenWithFee",
-000102b0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
-000102c0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-000102d0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-000102e0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-000102f0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00010300: 6c54 7970 6522 3a22 696e 7432 3536 222c  lType":"int256",
-00010310: 226e 616d 6522 3a22 616d 6f75 6e74 3044  "name":"amount0D
-00010320: 656c 7461 222c 2274 7970 6522 3a22 696e  elta","type":"in
-00010330: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-00010340: 6c54 7970 6522 3a22 696e 7432 3536 222c  lType":"int256",
-00010350: 226e 616d 6522 3a22 616d 6f75 6e74 3144  "name":"amount1D
-00010360: 656c 7461 222c 2274 7970 6522 3a22 696e  elta","type":"in
-00010370: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-00010380: 6c54 7970 6522 3a22 6279 7465 7322 2c22  lType":"bytes","
-00010390: 6e61 6d65 223a 225f 6461 7461 222c 2274  name":"_data","t
-000103a0: 7970 6522 3a22 6279 7465 7322 7d5d 2c22  ype":"bytes"}],"
-000103b0: 6e61 6d65 223a 2275 6e69 7377 6170 5633  name":"uniswapV3
-000103c0: 5377 6170 4361 6c6c 6261 636b 222c 226f  SwapCallback","o
-000103d0: 7574 7075 7473 223a 5b5d 2c22 7374 6174  utputs":[],"stat
-000103e0: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
-000103f0: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
-00010400: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00010410: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00010420: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00010430: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
-00010440: 4d69 6e69 6d75 6d22 2c22 7479 7065 223a  Minimum","type":
-00010450: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-00010460: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-00010470: 6573 7322 2c22 6e61 6d65 223a 2272 6563  ess","name":"rec
-00010480: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
-00010490: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
-000104a0: 223a 2275 6e77 7261 7057 4554 4839 222c  ":"unwrapWETH9",
-000104b0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
-000104c0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-000104d0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-000104e0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-000104f0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00010500: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00010510: 2c22 6e61 6d65 223a 2261 6d6f 756e 744d  ,"name":"amountM
-00010520: 696e 696d 756d 222c 2274 7970 6522 3a22  inimum","type":"
-00010530: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-00010540: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-00010550: 7373 222c 226e 616d 6522 3a22 7265 6369  ss","name":"reci
-00010560: 7069 656e 7422 2c22 7479 7065 223a 2261  pient","type":"a
-00010570: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-00010580: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00010590: 3622 2c22 6e61 6d65 223a 2266 6565 4269  6","name":"feeBi
-000105a0: 7073 222c 2274 7970 6522 3a22 7569 6e74  ps","type":"uint
-000105b0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-000105c0: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-000105d0: 226e 616d 6522 3a22 6665 6552 6563 6970  "name":"feeRecip
-000105e0: 6965 6e74 222c 2274 7970 6522 3a22 6164  ient","type":"ad
-000105f0: 6472 6573 7322 7d5d 2c22 6e61 6d65 223a  dress"}],"name":
-00010600: 2275 6e77 7261 7057 4554 4839 5769 7468  "unwrapWETH9With
-00010610: 4665 6522 2c22 6f75 7470 7574 7322 3a5b  Fee","outputs":[
-00010620: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-00010630: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
-00010640: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00010650: 2c7b 2273 7461 7465 4d75 7461 6269 6c69  ,{"stateMutabili
-00010660: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
-00010670: 7970 6522 3a22 7265 6365 6976 6522 7d5d  ype":"receive"}]
-00010680: 270a 0a20 2020 2027 2727 0a20 2020 2020  '..    '''.     
-00010690: 2020 2075 7365 6420 666f 7220 756e 6973     used for unis
-000106a0: 7761 7020 7633 2062 6173 6564 2064 6578  wap v3 based dex
-000106b0: 0a20 2020 2027 2727 0a20 2020 2064 6566  .    '''.    def
-000106c0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c5f   __init__(self,_
-000106d0: 7765 6233 2c5f 6661 6374 6f72 795f 6164  web3,_factory_ad
-000106e0: 6472 6573 732c 5f72 6f75 7465 5f61 6464  dress,_route_add
-000106f0: 7265 7373 2c5f 7075 626c 6963 5f6b 6579  ress,_public_key
-00010700: 2c5f 7072 6976 6174 655f 6b65 7929 3a0a  ,_private_key):.
-00010710: 2020 2020 2020 2020 7365 6c66 2e6d 795f          self.my_
-00010720: 7075 626c 6963 5f6b 6579 3d5f 7075 626c  public_key=_publ
-00010730: 6963 5f6b 6579 0a20 2020 2020 2020 2073  ic_key.        s
-00010740: 656c 662e 6d79 5f70 7269 7661 7465 5f6b  elf.my_private_k
-00010750: 6579 3d5f 7072 6976 6174 655f 6b65 790a  ey=_private_key.
-00010760: 2020 2020 2020 2020 7365 6c66 2e66 6163          self.fac
-00010770: 746f 7279 5f61 6464 7265 7373 3d5f 6661  tory_address=_fa
-00010780: 6374 6f72 795f 6164 6472 6573 730a 2020  ctory_address.  
-00010790: 2020 2020 2020 7365 6c66 2e72 6f75 7465        self.route
-000107a0: 5f61 6464 7265 7373 3d5f 726f 7574 655f  _address=_route_
-000107b0: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
-000107c0: 7365 6c66 2e77 6562 3320 3d20 5f77 6562  self.web3 = _web
-000107d0: 330a 2020 2020 2020 2020 7365 6c66 2e77  3.        self.w
-000107e0: 6562 332e 6d69 6464 6c65 7761 7265 5f6f  eb3.middleware_o
-000107f0: 6e69 6f6e 2e69 6e6a 6563 7428 6765 7468  nion.inject(geth
-00010800: 5f70 6f61 5f6d 6964 646c 6577 6172 652c  _poa_middleware,
-00010810: 206c 6179 6572 3d30 290a 2020 2020 2020   layer=0).      
-00010820: 2020 7072 696e 7428 2723 2323 2323 2323    print('#######
-00010830: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00010840: 2323 2323 2327 290a 2020 2020 2020 2020  #####').        
-00010850: 7072 696e 7428 2263 6f6e 7472 6163 7420  print("contract 
-00010860: 636f 6e6e 6563 7469 6f6e 2069 7320 222b  connection is "+
-00010870: 7374 7228 7365 6c66 2e77 6562 332e 6973  str(self.web3.is
-00010880: 436f 6e6e 6563 7465 6428 2929 290a 2020  Connected())).  
-00010890: 2020 2020 2020 6966 2073 656c 662e 7765        if self.we
-000108a0: 6233 2e69 7343 6f6e 6e65 6374 6564 2829  b3.isConnected()
-000108b0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-000108c0: 6c66 2e6e 6f6e 6365 3d73 656c 662e 7765  lf.nonce=self.we
-000108d0: 6233 2e65 7468 2e67 6574 5f74 7261 6e73  b3.eth.get_trans
-000108e0: 6163 7469 6f6e 5f63 6f75 6e74 2873 656c  action_count(sel
-000108f0: 662e 6d79 5f70 7562 6c69 635f 6b65 7929  f.my_public_key)
-00010900: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
-00010910: 6e74 2822 6e6f 6e63 6520 3d20 222c 7365  nt("nonce = ",se
-00010920: 6c66 2e6e 6f6e 6365 290a 2020 2020 2020  lf.nonce).      
+0000f750: 7449 6e4d 6178 696d 756d 222c 2274 7970  tInMaximum","typ
+0000f760: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0000f770: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0000f780: 696e 7431 3630 222c 226e 616d 6522 3a22  int160","name":"
+0000f790: 7371 7274 5072 6963 654c 696d 6974 5839  sqrtPriceLimitX9
+0000f7a0: 3622 2c22 7479 7065 223a 2275 696e 7431  6","type":"uint1
+0000f7b0: 3630 227d 5d2c 2269 6e74 6572 6e61 6c54  60"}],"internalT
+0000f7c0: 7970 6522 3a22 7374 7275 6374 2049 5377  ype":"struct ISw
+0000f7d0: 6170 526f 7574 6572 2e45 7861 6374 4f75  apRouter.ExactOu
+0000f7e0: 7470 7574 5369 6e67 6c65 5061 7261 6d73  tputSingleParams
+0000f7f0: 222c 226e 616d 6522 3a22 7061 7261 6d73  ","name":"params
+0000f800: 222c 2274 7970 6522 3a22 7475 706c 6522  ","type":"tuple"
+0000f810: 7d5d 2c22 6e61 6d65 223a 2265 7861 6374  }],"name":"exact
+0000f820: 4f75 7470 7574 5369 6e67 6c65 222c 226f  OutputSingle","o
+0000f830: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0000f840: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0000f850: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
+0000f860: 7449 6e22 2c22 7479 7065 223a 2275 696e  tIn","type":"uin
+0000f870: 7432 3536 227d 5d2c 2273 7461 7465 4d75  t256"}],"stateMu
+0000f880: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
+0000f890: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+0000f8a0: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0000f8b0: 3a5b 5d2c 226e 616d 6522 3a22 6661 6374  :[],"name":"fact
+0000f8c0: 6f72 7922 2c22 6f75 7470 7574 7322 3a5b  ory","outputs":[
+0000f8d0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0000f8e0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0000f8f0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
+0000f900: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
+0000f910: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+0000f920: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+0000f930: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+0000f940: 696e 7465 726e 616c 5479 7065 223a 2262  internalType":"b
+0000f950: 7974 6573 5b5d 222c 226e 616d 6522 3a22  ytes[]","name":"
+0000f960: 6461 7461 222c 2274 7970 6522 3a22 6279  data","type":"by
+0000f970: 7465 735b 5d22 7d5d 2c22 6e61 6d65 223a  tes[]"}],"name":
+0000f980: 226d 756c 7469 6361 6c6c 222c 226f 7574  "multicall","out
+0000f990: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0000f9a0: 6c54 7970 6522 3a22 6279 7465 735b 5d22  lType":"bytes[]"
+0000f9b0: 2c22 6e61 6d65 223a 2272 6573 756c 7473  ,"name":"results
+0000f9c0: 222c 2274 7970 6522 3a22 6279 7465 735b  ","type":"bytes[
+0000f9d0: 5d22 7d5d 2c22 7374 6174 654d 7574 6162  ]"}],"stateMutab
+0000f9e0: 696c 6974 7922 3a22 7061 7961 626c 6522  ility":"payable"
+0000f9f0: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+0000fa00: 6e22 7d2c 7b22 696e 7075 7473 223a 5b5d  n"},{"inputs":[]
+0000fa10: 2c22 6e61 6d65 223a 2272 6566 756e 6445  ,"name":"refundE
+0000fa20: 5448 222c 226f 7574 7075 7473 223a 5b5d  TH","outputs":[]
+0000fa30: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+0000fa40: 7922 3a22 7061 7961 626c 6522 2c22 7479  y":"payable","ty
+0000fa50: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+0000fa60: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0000fa70: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0000fa80: 6573 7322 2c22 6e61 6d65 223a 2274 6f6b  ess","name":"tok
+0000fa90: 656e 222c 2274 7970 6522 3a22 6164 6472  en","type":"addr
+0000faa0: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0000fab0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0000fac0: 226e 616d 6522 3a22 7661 6c75 6522 2c22  "name":"value","
+0000fad0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0000fae0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0000faf0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0000fb00: 223a 2264 6561 646c 696e 6522 2c22 7479  ":"deadline","ty
+0000fb10: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+0000fb20: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0000fb30: 7569 6e74 3822 2c22 6e61 6d65 223a 2276  uint8","name":"v
+0000fb40: 222c 2274 7970 6522 3a22 7569 6e74 3822  ","type":"uint8"
+0000fb50: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000fb60: 223a 2262 7974 6573 3332 222c 226e 616d  ":"bytes32","nam
+0000fb70: 6522 3a22 7222 2c22 7479 7065 223a 2262  e":"r","type":"b
+0000fb80: 7974 6573 3332 227d 2c7b 2269 6e74 6572  ytes32"},{"inter
+0000fb90: 6e61 6c54 7970 6522 3a22 6279 7465 7333  nalType":"bytes3
+0000fba0: 3222 2c22 6e61 6d65 223a 2273 222c 2274  2","name":"s","t
+0000fbb0: 7970 6522 3a22 6279 7465 7333 3222 7d5d  ype":"bytes32"}]
+0000fbc0: 2c22 6e61 6d65 223a 2273 656c 6650 6572  ,"name":"selfPer
+0000fbd0: 6d69 7422 2c22 6f75 7470 7574 7322 3a5b  mit","outputs":[
+0000fbe0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+0000fbf0: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
+0000fc00: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+0000fc10: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+0000fc20: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0000fc30: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
+0000fc40: 6b65 6e22 2c22 7479 7065 223a 2261 6464  ken","type":"add
+0000fc50: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+0000fc60: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0000fc70: 2c22 6e61 6d65 223a 226e 6f6e 6365 222c  ,"name":"nonce",
+0000fc80: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0000fc90: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0000fca0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0000fcb0: 6522 3a22 6578 7069 7279 222c 2274 7970  e":"expiry","typ
+0000fcc0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0000fcd0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0000fce0: 696e 7438 222c 226e 616d 6522 3a22 7622  int8","name":"v"
+0000fcf0: 2c22 7479 7065 223a 2275 696e 7438 227d  ,"type":"uint8"}
+0000fd00: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0000fd10: 3a22 6279 7465 7333 3222 2c22 6e61 6d65  :"bytes32","name
+0000fd20: 223a 2272 222c 2274 7970 6522 3a22 6279  ":"r","type":"by
+0000fd30: 7465 7333 3222 7d2c 7b22 696e 7465 726e  tes32"},{"intern
+0000fd40: 616c 5479 7065 223a 2262 7974 6573 3332  alType":"bytes32
+0000fd50: 222c 226e 616d 6522 3a22 7322 2c22 7479  ","name":"s","ty
+0000fd60: 7065 223a 2262 7974 6573 3332 227d 5d2c  pe":"bytes32"}],
+0000fd70: 226e 616d 6522 3a22 7365 6c66 5065 726d  "name":"selfPerm
+0000fd80: 6974 416c 6c6f 7765 6422 2c22 6f75 7470  itAllowed","outp
+0000fd90: 7574 7322 3a5b 5d2c 2273 7461 7465 4d75  uts":[],"stateMu
+0000fda0: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
+0000fdb0: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+0000fdc0: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0000fdd0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0000fde0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0000fdf0: 6522 3a22 746f 6b65 6e22 2c22 7479 7065  e":"token","type
+0000fe00: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0000fe10: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0000fe20: 6e74 3235 3622 2c22 6e61 6d65 223a 226e  nt256","name":"n
+0000fe30: 6f6e 6365 222c 2274 7970 6522 3a22 7569  once","type":"ui
+0000fe40: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0000fe50: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0000fe60: 222c 226e 616d 6522 3a22 6578 7069 7279  ","name":"expiry
+0000fe70: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0000fe80: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0000fe90: 7065 223a 2275 696e 7438 222c 226e 616d  pe":"uint8","nam
+0000fea0: 6522 3a22 7622 2c22 7479 7065 223a 2275  e":"v","type":"u
+0000feb0: 696e 7438 227d 2c7b 2269 6e74 6572 6e61  int8"},{"interna
+0000fec0: 6c54 7970 6522 3a22 6279 7465 7333 3222  lType":"bytes32"
+0000fed0: 2c22 6e61 6d65 223a 2272 222c 2274 7970  ,"name":"r","typ
+0000fee0: 6522 3a22 6279 7465 7333 3222 7d2c 7b22  e":"bytes32"},{"
+0000fef0: 696e 7465 726e 616c 5479 7065 223a 2262  internalType":"b
+0000ff00: 7974 6573 3332 222c 226e 616d 6522 3a22  ytes32","name":"
+0000ff10: 7322 2c22 7479 7065 223a 2262 7974 6573  s","type":"bytes
+0000ff20: 3332 227d 5d2c 226e 616d 6522 3a22 7365  32"}],"name":"se
+0000ff30: 6c66 5065 726d 6974 416c 6c6f 7765 6449  lfPermitAllowedI
+0000ff40: 664e 6563 6573 7361 7279 222c 226f 7574  fNecessary","out
+0000ff50: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
+0000ff60: 7574 6162 696c 6974 7922 3a22 7061 7961  utability":"paya
+0000ff70: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
+0000ff80: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+0000ff90: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0000ffa0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+0000ffb0: 6d65 223a 2274 6f6b 656e 222c 2274 7970  me":"token","typ
+0000ffc0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0000ffd0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0000ffe0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0000fff0: 7661 6c75 6522 2c22 7479 7065 223a 2275  value","type":"u
+00010000: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
+00010010: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00010020: 3622 2c22 6e61 6d65 223a 2264 6561 646c  6","name":"deadl
+00010030: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
+00010040: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00010050: 6c54 7970 6522 3a22 7569 6e74 3822 2c22  lType":"uint8","
+00010060: 6e61 6d65 223a 2276 222c 2274 7970 6522  name":"v","type"
+00010070: 3a22 7569 6e74 3822 7d2c 7b22 696e 7465  :"uint8"},{"inte
+00010080: 726e 616c 5479 7065 223a 2262 7974 6573  rnalType":"bytes
+00010090: 3332 222c 226e 616d 6522 3a22 7222 2c22  32","name":"r","
+000100a0: 7479 7065 223a 2262 7974 6573 3332 227d  type":"bytes32"}
+000100b0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+000100c0: 3a22 6279 7465 7333 3222 2c22 6e61 6d65  :"bytes32","name
+000100d0: 223a 2273 222c 2274 7970 6522 3a22 6279  ":"s","type":"by
+000100e0: 7465 7333 3222 7d5d 2c22 6e61 6d65 223a  tes32"}],"name":
+000100f0: 2273 656c 6650 6572 6d69 7449 664e 6563  "selfPermitIfNec
+00010100: 6573 7361 7279 222c 226f 7574 7075 7473  essary","outputs
+00010110: 223a 5b5d 2c22 7374 6174 654d 7574 6162  ":[],"stateMutab
+00010120: 696c 6974 7922 3a22 7061 7961 626c 6522  ility":"payable"
+00010130: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+00010140: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
+00010150: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00010160: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+00010170: 2274 6f6b 656e 222c 2274 7970 6522 3a22  "token","type":"
+00010180: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+00010190: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+000101a0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+000101b0: 6e74 4d69 6e69 6d75 6d22 2c22 7479 7065  ntMinimum","type
+000101c0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+000101d0: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+000101e0: 6472 6573 7322 2c22 6e61 6d65 223a 2272  dress","name":"r
+000101f0: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
+00010200: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
+00010210: 6d65 223a 2273 7765 6570 546f 6b65 6e22  me":"sweepToken"
+00010220: 2c22 6f75 7470 7574 7322 3a5b 5d2c 2273  ,"outputs":[],"s
+00010230: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+00010240: 2270 6179 6162 6c65 222c 2274 7970 6522  "payable","type"
+00010250: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+00010260: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00010270: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+00010280: 222c 226e 616d 6522 3a22 746f 6b65 6e22  ","name":"token"
+00010290: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+000102a0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+000102b0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+000102c0: 6d65 223a 2261 6d6f 756e 744d 696e 696d  me":"amountMinim
+000102d0: 756d 222c 2274 7970 6522 3a22 7569 6e74  um","type":"uint
+000102e0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+000102f0: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+00010300: 226e 616d 6522 3a22 7265 6369 7069 656e  "name":"recipien
+00010310: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
+00010320: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+00010330: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00010340: 6e61 6d65 223a 2266 6565 4269 7073 222c  name":"feeBips",
+00010350: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00010360: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00010370: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+00010380: 6522 3a22 6665 6552 6563 6970 6965 6e74  e":"feeRecipient
+00010390: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000103a0: 7322 7d5d 2c22 6e61 6d65 223a 2273 7765  s"}],"name":"swe
+000103b0: 6570 546f 6b65 6e57 6974 6846 6565 222c  epTokenWithFee",
+000103c0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+000103d0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+000103e0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+000103f0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00010400: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00010410: 6c54 7970 6522 3a22 696e 7432 3536 222c  lType":"int256",
+00010420: 226e 616d 6522 3a22 616d 6f75 6e74 3044  "name":"amount0D
+00010430: 656c 7461 222c 2274 7970 6522 3a22 696e  elta","type":"in
+00010440: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00010450: 6c54 7970 6522 3a22 696e 7432 3536 222c  lType":"int256",
+00010460: 226e 616d 6522 3a22 616d 6f75 6e74 3144  "name":"amount1D
+00010470: 656c 7461 222c 2274 7970 6522 3a22 696e  elta","type":"in
+00010480: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00010490: 6c54 7970 6522 3a22 6279 7465 7322 2c22  lType":"bytes","
+000104a0: 6e61 6d65 223a 225f 6461 7461 222c 2274  name":"_data","t
+000104b0: 7970 6522 3a22 6279 7465 7322 7d5d 2c22  ype":"bytes"}],"
+000104c0: 6e61 6d65 223a 2275 6e69 7377 6170 5633  name":"uniswapV3
+000104d0: 5377 6170 4361 6c6c 6261 636b 222c 226f  SwapCallback","o
+000104e0: 7574 7075 7473 223a 5b5d 2c22 7374 6174  utputs":[],"stat
+000104f0: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
+00010500: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
+00010510: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+00010520: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00010530: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00010540: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
+00010550: 4d69 6e69 6d75 6d22 2c22 7479 7065 223a  Minimum","type":
+00010560: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+00010570: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+00010580: 6573 7322 2c22 6e61 6d65 223a 2272 6563  ess","name":"rec
+00010590: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
+000105a0: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+000105b0: 223a 2275 6e77 7261 7057 4554 4839 222c  ":"unwrapWETH9",
+000105c0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+000105d0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+000105e0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+000105f0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00010600: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00010610: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00010620: 2c22 6e61 6d65 223a 2261 6d6f 756e 744d  ,"name":"amountM
+00010630: 696e 696d 756d 222c 2274 7970 6522 3a22  inimum","type":"
+00010640: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+00010650: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+00010660: 7373 222c 226e 616d 6522 3a22 7265 6369  ss","name":"reci
+00010670: 7069 656e 7422 2c22 7479 7065 223a 2261  pient","type":"a
+00010680: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+00010690: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+000106a0: 3622 2c22 6e61 6d65 223a 2266 6565 4269  6","name":"feeBi
+000106b0: 7073 222c 2274 7970 6522 3a22 7569 6e74  ps","type":"uint
+000106c0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+000106d0: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+000106e0: 226e 616d 6522 3a22 6665 6552 6563 6970  "name":"feeRecip
+000106f0: 6965 6e74 222c 2274 7970 6522 3a22 6164  ient","type":"ad
+00010700: 6472 6573 7322 7d5d 2c22 6e61 6d65 223a  dress"}],"name":
+00010710: 2275 6e77 7261 7057 4554 4839 5769 7468  "unwrapWETH9With
+00010720: 4665 6522 2c22 6f75 7470 7574 7322 3a5b  Fee","outputs":[
+00010730: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+00010740: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
+00010750: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00010760: 2c7b 2273 7461 7465 4d75 7461 6269 6c69  ,{"stateMutabili
+00010770: 7479 223a 2270 6179 6162 6c65 222c 2274  ty":"payable","t
+00010780: 7970 6522 3a22 7265 6365 6976 6522 7d5d  ype":"receive"}]
+00010790: 270a 0a20 2020 2027 2727 0a20 2020 2020  '..    '''.     
+000107a0: 2020 2075 7365 6420 666f 7220 756e 6973     used for unis
+000107b0: 7761 7020 7633 2062 6173 6564 2064 6578  wap v3 based dex
+000107c0: 0a20 2020 2027 2727 0a20 2020 2064 6566  .    '''.    def
+000107d0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c5f   __init__(self,_
+000107e0: 7765 6233 2c5f 6661 6374 6f72 795f 6164  web3,_factory_ad
+000107f0: 6472 6573 732c 5f72 6f75 7465 5f61 6464  dress,_route_add
+00010800: 7265 7373 2c5f 7075 626c 6963 5f6b 6579  ress,_public_key
+00010810: 2c5f 7072 6976 6174 655f 6b65 7929 3a0a  ,_private_key):.
+00010820: 2020 2020 2020 2020 7365 6c66 2e6d 795f          self.my_
+00010830: 7075 626c 6963 5f6b 6579 3d5f 7075 626c  public_key=_publ
+00010840: 6963 5f6b 6579 0a20 2020 2020 2020 2073  ic_key.        s
+00010850: 656c 662e 6d79 5f70 7269 7661 7465 5f6b  elf.my_private_k
+00010860: 6579 3d5f 7072 6976 6174 655f 6b65 790a  ey=_private_key.
+00010870: 2020 2020 2020 2020 7365 6c66 2e66 6163          self.fac
+00010880: 746f 7279 5f61 6464 7265 7373 3d5f 6661  tory_address=_fa
+00010890: 6374 6f72 795f 6164 6472 6573 730a 2020  ctory_address.  
+000108a0: 2020 2020 2020 7365 6c66 2e72 6f75 7465        self.route
+000108b0: 5f61 6464 7265 7373 3d5f 726f 7574 655f  _address=_route_
+000108c0: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
+000108d0: 7365 6c66 2e77 6562 3320 3d20 5f77 6562  self.web3 = _web
+000108e0: 330a 2020 2020 2020 2020 7365 6c66 2e77  3.        self.w
+000108f0: 6562 332e 6d69 6464 6c65 7761 7265 5f6f  eb3.middleware_o
+00010900: 6e69 6f6e 2e69 6e6a 6563 7428 6765 7468  nion.inject(geth
+00010910: 5f70 6f61 5f6d 6964 646c 6577 6172 652c  _poa_middleware,
+00010920: 206c 6179 6572 3d30 290a 2020 2020 2020   layer=0).      
 00010930: 2020 7072 696e 7428 2723 2323 2323 2323    print('#######
 00010940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
 00010950: 2323 2323 2327 290a 2020 2020 2020 2020  #####').        
-00010960: 2320 756e 6973 7761 705f 4661 6374 6f72  # uniswap_Factor
-00010970: 790a 2020 2020 2020 2020 7365 6c66 2e66  y.        self.f
-00010980: 6163 746f 7279 5f61 6269 203d 206a 736f  actory_abi = jso
-00010990: 6e2e 6c6f 6164 7328 7365 6c66 2e75 6e69  n.loads(self.uni
-000109a0: 7377 6170 5f76 335f 6661 6374 6f72 795f  swap_v3_factory_
-000109b0: 6162 6929 0a20 2020 2020 2020 2073 656c  abi).        sel
-000109c0: 662e 7061 6972 5f61 6269 3d6a 736f 6e2e  f.pair_abi=json.
-000109d0: 6c6f 6164 7328 7365 6c66 2e75 6e69 7377  loads(self.unisw
-000109e0: 6170 5f76 335f 7061 6972 5f61 6269 290a  ap_v3_pair_abi).
-000109f0: 2020 2020 2020 2020 7365 6c66 2e65 7263          self.erc
-00010a00: 3230 5f61 6269 3d6a 736f 6e2e 6c6f 6164  20_abi=json.load
-00010a10: 7328 7365 6c66 2e75 6e69 7377 6170 5f76  s(self.uniswap_v
-00010a20: 335f 6572 6332 305f 6162 6929 0a20 2020  3_erc20_abi).   
-00010a30: 2020 2020 2073 656c 662e 726f 7574 655f       self.route_
-00010a40: 6162 693d 6a73 6f6e 2e6c 6f61 6473 2873  abi=json.loads(s
-00010a50: 656c 662e 756e 6973 7761 705f 7633 5f72  elf.uniswap_v3_r
-00010a60: 6f75 7465 5f61 6269 290a 0a20 2020 2020  oute_abi)..     
-00010a70: 2020 2073 656c 662e 6661 6374 6f72 795f     self.factory_
-00010a80: 636f 6e74 7261 6374 203d 2073 656c 662e  contract = self.
-00010a90: 7765 6233 2e65 7468 2e63 6f6e 7472 6163  web3.eth.contrac
-00010aa0: 7428 6164 6472 6573 733d 7365 6c66 2e66  t(address=self.f
-00010ab0: 6163 746f 7279 5f61 6464 7265 7373 2c20  actory_address, 
-00010ac0: 6162 693d 7365 6c66 2e66 6163 746f 7279  abi=self.factory
-00010ad0: 5f61 6269 290a 2020 2020 2020 2020 7365  _abi).        se
-00010ae0: 6c66 2e72 6f75 7465 5f63 6f6e 7472 6163  lf.route_contrac
-00010af0: 743d 7365 6c66 2e77 6562 332e 6574 682e  t=self.web3.eth.
-00010b00: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
-00010b10: 3d73 656c 662e 726f 7574 655f 6164 6472  =self.route_addr
-00010b20: 6573 732c 6162 693d 7365 6c66 2e72 6f75  ess,abi=self.rou
-00010b30: 7465 5f61 6269 290a 636c 6173 7320 556e  te_abi).class Un
-00010b40: 6973 7761 7056 3346 6163 746f 7279 3a0a  iswapV3Factory:.
-00010b50: 0a20 2020 2023 6661 6374 6f72 790a 2020  .    #factory.  
-00010b60: 2020 2372 6574 7572 6e20 6164 6472 6573    #return addres
-00010b70: 7320 6f66 2070 6f6f 6c20 666f 7220 746f  s of pool for to
-00010b80: 6b65 6e41 2061 6e64 2074 6f6b 656e 4220  kenA and tokenB 
-00010b90: 7769 7468 2073 7065 6369 6669 6320 6665  with specific fe
-00010ba0: 650a 2020 2020 2331 3030 3030 2066 6f72  e.    #10000 for
-00010bb0: 2031 2520 6665 652c 2033 3030 3020 666f   1% fee, 3000 fo
-00010bc0: 7220 302e 3325 2c20 616e 6420 3530 3020  r 0.3%, and 500 
-00010bd0: 666f 7220 302e 3035 250a 2020 2020 6465  for 0.05%.    de
-00010be0: 6620 6765 7450 6f6f 6c28 5f77 6562 333a  f getPool(_web3:
-00010bf0: 5765 6233 2c5f 6661 6374 6f72 795f 6164  Web3,_factory_ad
-00010c00: 6472 6573 732c 5f61 6269 2c5f 746f 6b65  dress,_abi,_toke
-00010c10: 6e41 3a73 7472 2c5f 746f 6b65 6e42 3a73  nA:str,_tokenB:s
-00010c20: 7472 2c5f 6665 653a 696e 7429 3a0a 2020  tr,_fee:int):.  
-00010c30: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
-00010c40: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
-00010c50: 6164 6472 6573 733d 5f66 6163 746f 7279  address=_factory
-00010c60: 5f61 6464 7265 7373 2c20 6162 693d 5f61  _address, abi=_a
-00010c70: 6269 292e 6675 6e63 7469 6f6e 732e 6765  bi).functions.ge
-00010c80: 7450 6f6f 6c28 5f74 6f6b 656e 412c 5f74  tPool(_tokenA,_t
-00010c90: 6f6b 656e 422c 5f66 6565 292e 6361 6c6c  okenB,_fee).call
-00010ca0: 2829 0a20 2020 200a 636c 6173 7320 556e  ().    .class Un
-00010cb0: 6973 7761 7056 3351 756f 7465 723a 0a20  iswapV3Quoter:. 
-00010cc0: 2020 2023 7265 7475 726e 2061 6464 7265     #return addre
-00010cd0: 7373 206f 6620 706f 6f6c 2066 6f72 2074  ss of pool for t
-00010ce0: 6f6b 656e 4120 616e 6420 746f 6b65 6e42  okenA and tokenB
-00010cf0: 2077 6974 6820 7370 6563 6966 6963 2066   with specific f
-00010d00: 6565 0a20 2020 2023 3130 3030 3020 666f  ee.    #10000 fo
-00010d10: 7220 3125 2066 6565 2c20 3330 3030 2066  r 1% fee, 3000 f
-00010d20: 6f72 2030 2e33 252c 2061 6e64 2035 3030  or 0.3%, and 500
-00010d30: 2066 6f72 2030 2e30 3525 0a20 2020 2064   for 0.05%.    d
-00010d40: 6566 2067 6574 506f 6f6c 285f 7765 6233  ef getPool(_web3
-00010d50: 3a57 6562 332c 5f71 756f 7465 725f 6164  :Web3,_quoter_ad
-00010d60: 6472 6573 732c 5f61 6269 2c5f 746f 6b65  dress,_abi,_toke
-00010d70: 6e41 3a73 7472 2c5f 746f 6b65 6e42 3a73  nA:str,_tokenB:s
-00010d80: 7472 2c5f 6665 653a 696e 7429 3a0a 2020  tr,_fee:int):.  
-00010d90: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
-00010da0: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
-00010db0: 6164 6472 6573 733d 5f71 756f 7465 725f  address=_quoter_
-00010dc0: 6164 6472 6573 732c 2061 6269 3d5f 6162  address, abi=_ab
-00010dd0: 6929 2e66 756e 6374 696f 6e73 2e67 6574  i).functions.get
-00010de0: 506f 6f6c 285f 746f 6b65 6e41 2c5f 746f  Pool(_tokenA,_to
-00010df0: 6b65 6e42 2c5f 6665 6529 2e63 616c 6c28  kenB,_fee).call(
-00010e00: 290a 2020 2020 0a20 2020 2023 2073 7472  ).    .    # str
-00010e10: 7563 7420 5175 6f74 6545 7861 6374 496e  uct QuoteExactIn
-00010e20: 7075 7453 696e 676c 6550 6172 616d 7320  putSingleParams 
-00010e30: 7b0a 2020 2020 2320 2020 2020 6164 6472  {.    #     addr
-00010e40: 6573 7320 746f 6b65 6e49 6e3b 0a20 2020  ess tokenIn;.   
-00010e50: 2023 2020 2020 2061 6464 7265 7373 2074   #     address t
-00010e60: 6f6b 656e 4f75 743b 0a20 2020 2023 2020  okenOut;.    #  
-00010e70: 2020 2075 696e 7432 3536 2061 6d6f 756e     uint256 amoun
-00010e80: 7449 6e3b 0a20 2020 2023 2020 2020 2075  tIn;.    #     u
-00010e90: 696e 7432 3420 6665 653b 0a20 2020 2023  int24 fee;.    #
-00010ea0: 2020 2020 2075 696e 7431 3630 2073 7172       uint160 sqr
-00010eb0: 7450 7269 6365 4c69 6d69 7458 3936 3b0a  tPriceLimitX96;.
-00010ec0: 2020 2020 2320 7d0a 2020 2020 6465 6620      # }.    def 
-00010ed0: 7175 6f74 6545 7861 6374 496e 7075 7453  quoteExactInputS
-00010ee0: 696e 676c 6528 5f77 6562 333a 5765 6233  ingle(_web3:Web3
-00010ef0: 2c5f 7175 6f74 6572 5f61 6464 7265 7373  ,_quoter_address
-00010f00: 2c5f 6162 692c 5f70 6172 616d 293a 0a20  ,_abi,_param):. 
-00010f10: 2020 2020 2020 2072 6574 7572 6e20 5f77         return _w
-00010f20: 6562 332e 6574 682e 636f 6e74 7261 6374  eb3.eth.contract
-00010f30: 2861 6464 7265 7373 3d5f 7175 6f74 6572  (address=_quoter
-00010f40: 5f61 6464 7265 7373 2c20 6162 693d 5f61  _address, abi=_a
-00010f50: 6269 292e 6675 6e63 7469 6f6e 732e 7175  bi).functions.qu
-00010f60: 6f74 6545 7861 6374 496e 7075 7453 696e  oteExactInputSin
-00010f70: 676c 6528 5f70 6172 616d 292e 6361 6c6c  gle(_param).call
-00010f80: 2829 0a0a 2020 2020 2370 6174 6820 7374  ()..    #path st
-00010f90: 6172 7477 6974 6820 696e 7075 7420 746f  artwith input to
-00010fa0: 6b65 6e0a 2020 2020 6465 6620 7175 6f74  ken.    def quot
-00010fb0: 6545 7861 6374 496e 7075 7428 5f77 6562  eExactInput(_web
-00010fc0: 333a 5765 6233 2c5f 7175 6f74 6572 5f61  3:Web3,_quoter_a
-00010fd0: 6464 7265 7373 2c5f 6162 692c 7061 7468  ddress,_abi,path
-00010fe0: 2c5f 616d 6f75 6e74 5f69 6e29 3a0a 2020  ,_amount_in):.  
-00010ff0: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
-00011000: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
-00011010: 6164 6472 6573 733d 5f71 756f 7465 725f  address=_quoter_
-00011020: 6164 6472 6573 732c 2061 6269 3d5f 6162  address, abi=_ab
-00011030: 6929 2e66 756e 6374 696f 6e73 2e71 756f  i).functions.quo
-00011040: 7465 4578 6163 7449 6e70 7574 2870 6174  teExactInput(pat
-00011050: 682c 5f61 6d6f 756e 745f 696e 292e 6361  h,_amount_in).ca
-00011060: 6c6c 2829 0a20 2020 200a 2020 2020 2320  ll().    .    # 
-00011070: 7374 7275 6374 2051 756f 7465 4578 6163  struct QuoteExac
-00011080: 744f 7574 7075 7453 696e 676c 6550 6172  tOutputSinglePar
-00011090: 616d 7320 7b0a 2020 2020 2320 2020 2020  ams {.    #     
-000110a0: 6164 6472 6573 7320 746f 6b65 6e49 6e3b  address tokenIn;
-000110b0: 0a20 2020 2023 2020 2020 2061 6464 7265  .    #     addre
-000110c0: 7373 2074 6f6b 656e 4f75 743b 0a20 2020  ss tokenOut;.   
-000110d0: 2023 2020 2020 2075 696e 7432 3536 2061   #     uint256 a
-000110e0: 6d6f 756e 743b 0a20 2020 2023 2020 2020  mount;.    #    
-000110f0: 2075 696e 7432 3420 6665 653b 0a20 2020   uint24 fee;.   
-00011100: 2023 2020 2020 2075 696e 7431 3630 2073   #     uint160 s
-00011110: 7172 7450 7269 6365 4c69 6d69 7458 3936  qrtPriceLimitX96
-00011120: 3b0a 2020 2020 2320 7d0a 2020 2020 6465  ;.    # }.    de
-00011130: 6620 7175 6f74 6545 7861 6374 4f75 7470  f quoteExactOutp
-00011140: 7574 5369 6e67 6c65 285f 7765 6233 3a57  utSingle(_web3:W
-00011150: 6562 332c 5f71 756f 7465 725f 6164 6472  eb3,_quoter_addr
-00011160: 6573 732c 5f61 6269 2c5f 7061 7261 6d29  ess,_abi,_param)
-00011170: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00011180: 205f 7765 6233 2e65 7468 2e63 6f6e 7472   _web3.eth.contr
-00011190: 6163 7428 6164 6472 6573 733d 5f71 756f  act(address=_quo
-000111a0: 7465 725f 6164 6472 6573 732c 2061 6269  ter_address, abi
-000111b0: 3d5f 6162 6929 2e66 756e 6374 696f 6e73  =_abi).functions
-000111c0: 2e71 756f 7465 4578 6163 744f 7574 7075  .quoteExactOutpu
-000111d0: 7453 696e 676c 6528 5f70 6172 616d 292e  tSingle(_param).
-000111e0: 6361 6c6c 2829 0a20 2020 200a 2020 2020  call().    .    
-000111f0: 2370 6174 6820 7374 6172 7420 7769 7468  #path start with
-00011200: 206f 7574 7075 7420 746f 6b65 6e0a 2020   output token.  
-00011210: 2020 6465 6620 7175 6f74 6545 7861 6374    def quoteExact
-00011220: 4f75 7470 7574 285f 7765 6233 3a57 6562  Output(_web3:Web
-00011230: 332c 5f71 756f 7465 725f 6164 6472 6573  3,_quoter_addres
-00011240: 732c 5f61 6269 2c70 6174 682c 5f61 6d6f  s,_abi,path,_amo
-00011250: 756e 745f 6f75 7429 3a0a 2020 2020 2020  unt_out):.      
-00011260: 2020 7265 7475 726e 205f 7765 6233 2e65    return _web3.e
-00011270: 7468 2e63 6f6e 7472 6163 7428 6164 6472  th.contract(addr
-00011280: 6573 733d 5f71 756f 7465 725f 6164 6472  ess=_quoter_addr
-00011290: 6573 732c 2061 6269 3d5f 6162 6929 2e66  ess, abi=_abi).f
-000112a0: 756e 6374 696f 6e73 2e71 756f 7465 4578  unctions.quoteEx
-000112b0: 6163 744f 7574 7075 7428 7061 7468 2c5f  actOutput(path,_
-000112c0: 616d 6f75 6e74 5f6f 7574 292e 6361 6c6c  amount_out).call
-000112d0: 2829 0a0a 636c 6173 7320 556e 6973 7761  ()..class Uniswa
-000112e0: 7056 3352 6f75 7465 723a 0a0a 2020 2020  pV3Router:..    
-000112f0: 2320 7374 7275 6374 2045 7861 6374 496e  # struct ExactIn
-00011300: 7075 7453 696e 676c 6550 6172 616d 7320  putSingleParams 
-00011310: 7b0a 2020 2020 2320 2020 2020 6164 6472  {.    #     addr
-00011320: 6573 7320 746f 6b65 6e49 6e3b 0a20 2020  ess tokenIn;.   
-00011330: 2023 2020 2020 2061 6464 7265 7373 2074   #     address t
-00011340: 6f6b 656e 4f75 743b 0a20 2020 2023 2020  okenOut;.    #  
-00011350: 2020 2075 696e 7432 3420 6665 653b 0a20     uint24 fee;. 
-00011360: 2020 2023 2020 2020 2061 6464 7265 7373     #     address
-00011370: 2072 6563 6970 6965 6e74 3b0a 2020 2020   recipient;.    
-00011380: 2320 2020 2020 7569 6e74 3235 3620 6465  #     uint256 de
-00011390: 6164 6c69 6e65 3b0a 2020 2020 2320 2020  adline;.    #   
-000113a0: 2020 7569 6e74 3235 3620 616d 6f75 6e74    uint256 amount
-000113b0: 496e 3b0a 2020 2020 2320 2020 2020 7569  In;.    #     ui
-000113c0: 6e74 3235 3620 616d 6f75 6e74 4f75 744d  nt256 amountOutM
-000113d0: 696e 696d 756d 3b0a 2020 2020 2320 2020  inimum;.    #   
-000113e0: 2020 7569 6e74 3136 3020 7371 7274 5072    uint160 sqrtPr
-000113f0: 6963 654c 696d 6974 5839 363b 0a20 2020  iceLimitX96;.   
-00011400: 2023 207d 0a20 2020 2064 6566 2065 7861   # }.    def exa
-00011410: 6374 496e 7075 7453 696e 676c 6528 5f77  ctInputSingle(_w
-00011420: 6562 333a 5765 6233 2c5f 726f 7574 655f  eb3:Web3,_route_
-00011430: 6164 6472 6573 732c 5f61 6269 2c5f 6e6f  address,_abi,_no
-00011440: 6e63 652c 5f70 7562 6c69 635f 6b65 792c  nce,_public_key,
-00011450: 5f70 7269 7661 7465 5f6b 6579 2c0a 2020  _private_key,.  
-00011460: 2020 2020 2020 5f74 6f6b 656e 5f69 6e2c        _token_in,
-00011470: 5f74 6f6b 656e 5f6f 7574 2c5f 6665 652c  _token_out,_fee,
-00011480: 5f72 6563 6970 6965 6e74 2c5f 6465 6164  _recipient,_dead
-00011490: 6c69 6e65 2c5f 616d 6f75 6e74 5f69 6e2c  line,_amount_in,
-000114a0: 5f61 6d6f 756e 745f 6f75 745f 6d69 6e2c  _amount_out_min,
-000114b0: 5f73 7172 745f 7072 6963 655f 6c69 6d69  _sqrt_price_limi
-000114c0: 7429 3a0a 2020 2020 2020 2020 726f 7574  t):.        rout
-000114d0: 655f 636f 6e74 7261 6374 3d5f 7765 6233  e_contract=_web3
-000114e0: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
-000114f0: 6472 6573 733d 5f72 6f75 7465 5f61 6464  dress=_route_add
-00011500: 7265 7373 2c20 6162 693d 5f61 6269 290a  ress, abi=_abi).
-00011510: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
-00011520: 5f70 6172 616d 733d 7b0a 2020 2020 2020  _params={.      
-00011530: 2020 2020 2020 2774 6f6b 656e 496e 273a        'tokenIn':
-00011540: 5f74 6f6b 656e 5f69 6e2c 0a20 2020 2020  _token_in,.     
-00011550: 2020 2020 2020 2027 746f 6b65 6e4f 7574         'tokenOut
-00011560: 273a 5f74 6f6b 656e 5f6f 7574 2c0a 2020  ':_token_out,.  
-00011570: 2020 2020 2020 2020 2020 2766 6565 273a            'fee':
-00011580: 5f66 6565 2c0a 2020 2020 2020 2020 2020  _fee,.          
-00011590: 2020 2772 6563 6970 6965 6e74 273a 5f72    'recipient':_r
-000115a0: 6563 6970 6965 6e74 2c0a 2020 2020 2020  ecipient,.      
-000115b0: 2020 2020 2020 2764 6561 646c 696e 6527        'deadline'
-000115c0: 3a5f 6465 6164 6c69 6e65 2c0a 2020 2020  :_deadline,.    
-000115d0: 2020 2020 2020 2020 2761 6d6f 756e 7449          'amountI
-000115e0: 6e27 3a5f 616d 6f75 6e74 5f69 6e2c 0a20  n':_amount_in,. 
-000115f0: 2020 2020 2020 2020 2020 2027 616d 6f75             'amou
-00011600: 6e74 4f75 744d 696e 696d 756d 273a 5f61  ntOutMinimum':_a
-00011610: 6d6f 756e 745f 6f75 745f 6d69 6e2c 0a20  mount_out_min,. 
-00011620: 2020 2020 2020 2020 2020 2027 7371 7274             'sqrt
-00011630: 5072 6963 654c 696d 6974 5839 3627 3a5f  PriceLimitX96':_
-00011640: 7371 7274 5f70 7269 6365 5f6c 696d 6974  sqrt_price_limit
-00011650: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
-00011660: 2020 2023 2066 756e 6374 696f 6e5f 7061     # function_pa
-00011670: 7261 6d73 3d28 5f74 6f6b 656e 5f69 6e2c  rams=(_token_in,
-00011680: 5f74 6f6b 656e 5f6f 7574 2c5f 6665 652c  _token_out,_fee,
-00011690: 5f72 6563 6970 6965 6e74 2c5f 6465 6164  _recipient,_dead
-000116a0: 6c69 6e65 2c5f 616d 6f75 6e74 5f69 6e2c  line,_amount_in,
-000116b0: 5f61 6d6f 756e 745f 6f75 745f 6d69 6e2c  _amount_out_min,
-000116c0: 5f73 7172 745f 7072 6963 655f 6c69 6d69  _sqrt_price_limi
-000116d0: 7429 0a20 2020 2020 2020 2073 7761 705f  t).        swap_
-000116e0: 6675 6e63 7469 6f6e 3d72 6f75 7465 5f63  function=route_c
-000116f0: 6f6e 7472 6163 742e 6675 6e63 7469 6f6e  ontract.function
-00011700: 732e 6578 6163 7449 6e70 7574 5369 6e67  s.exactInputSing
-00011710: 6c65 2866 756e 6374 696f 6e5f 7061 7261  le(function_para
-00011720: 6d73 290a 2020 2020 2020 2020 7478 5f70  ms).        tx_p
-00011730: 6172 616d 733d 7b0a 2020 2020 2020 2020  arams={.        
-00011740: 2020 2020 2766 726f 6d27 3a20 5f70 7562      'from': _pub
-00011750: 6c69 635f 6b65 792c 0a20 2020 2020 2020  lic_key,.       
-00011760: 2020 2020 2027 7661 6c75 6527 3a20 302c       'value': 0,
-00011770: 0a20 2020 2020 2020 2020 2020 2027 6e6f  .            'no
-00011780: 6e63 6527 3a20 5f6e 6f6e 6365 2c0a 2020  nce': _nonce,.  
-00011790: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
-000117a0: 3a20 2730 7832 270a 2020 2020 2020 2020  : '0x2'.        
-000117b0: 7d0a 2020 2020 2020 2020 7472 616e 7361  }.        transa
-000117c0: 6374 696f 6e3d 7377 6170 5f66 756e 6374  ction=swap_funct
-000117d0: 696f 6e2e 6275 696c 6454 7261 6e73 6163  ion.buildTransac
-000117e0: 7469 6f6e 2874 785f 7061 7261 6d73 290a  tion(tx_params).
-000117f0: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
-00011800: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
-00011810: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
-00011820: 6e5f 7472 616e 7361 6374 696f 6e28 7472  n_transaction(tr
-00011830: 616e 7361 6374 696f 6e2c 2070 7269 7661  ansaction, priva
-00011840: 7465 5f6b 6579 3d5f 7072 6976 6174 655f  te_key=_private_
-00011850: 6b65 7929 0a20 2020 2020 2020 2072 6574  key).        ret
-00011860: 7572 6e20 5f77 6562 332e 746f 4865 7828  urn _web3.toHex(
-00011870: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
-00011880: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
-00011890: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
-000118a0: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
-000118b0: 2929 0a0a 2020 2020 2320 7374 7275 6374  ))..    # struct
-000118c0: 2045 7861 6374 496e 7075 7450 6172 616d   ExactInputParam
-000118d0: 7320 7b0a 2020 2020 2320 2020 2020 6279  s {.    #     by
-000118e0: 7465 7320 7061 7468 3b0a 2020 2020 2320  tes path;.    # 
-000118f0: 2020 2020 6164 6472 6573 7320 7265 6369      address reci
-00011900: 7069 656e 743b 0a20 2020 2023 2020 2020  pient;.    #    
-00011910: 2075 696e 7432 3536 2064 6561 646c 696e   uint256 deadlin
-00011920: 653b 0a20 2020 2023 2020 2020 2075 696e  e;.    #     uin
-00011930: 7432 3536 2061 6d6f 756e 7449 6e3b 0a20  t256 amountIn;. 
-00011940: 2020 2023 2020 2020 2075 696e 7432 3536     #     uint256
-00011950: 2061 6d6f 756e 744f 7574 4d69 6e69 6d75   amountOutMinimu
-00011960: 6d3b 0a20 2020 2023 207d 0a20 2020 2064  m;.    # }.    d
-00011970: 6566 2065 7861 6374 496e 7075 7428 5f77  ef exactInput(_w
-00011980: 6562 333a 5765 6233 2c5f 726f 7574 655f  eb3:Web3,_route_
-00011990: 6164 6472 6573 732c 5f61 6269 2c5f 6e6f  address,_abi,_no
-000119a0: 6e63 652c 5f70 7562 6c69 635f 6b65 792c  nce,_public_key,
-000119b0: 5f70 7269 7661 7465 5f6b 6579 2c0a 2020  _private_key,.  
-000119c0: 2020 2020 2020 5f70 6174 682c 5f72 6563        _path,_rec
-000119d0: 6970 6965 6e74 2c5f 6465 6164 6c69 6e65  ipient,_deadline
-000119e0: 2c5f 616d 6f75 6e74 496e 2c5f 616d 6f75  ,_amountIn,_amou
-000119f0: 6e74 4f75 744d 696e 293a 0a20 2020 2020  ntOutMin):.     
-00011a00: 2020 2072 6f75 7465 5f63 6f6e 7472 6163     route_contrac
-00011a10: 743d 5f77 6562 332e 6574 682e 636f 6e74  t=_web3.eth.cont
-00011a20: 7261 6374 2861 6464 7265 7373 3d5f 726f  ract(address=_ro
-00011a30: 7574 655f 6164 6472 6573 732c 2061 6269  ute_address, abi
-00011a40: 3d5f 6162 6929 0a0a 2020 2020 2020 2020  =_abi)..        
-00011a50: 2320 7479 7065 3d5b 2762 7974 6573 272c  # type=['bytes',
-00011a60: 2761 6464 7265 7373 272c 2775 696e 7432  'address','uint2
-00011a70: 3536 272c 2775 696e 7432 3536 272c 2775  56','uint256','u
-00011a80: 696e 7432 3536 275d 0a20 2020 2020 2020  int256'].       
-00011a90: 2023 2064 6174 613d 5b5f 7061 7468 2c5f   # data=[_path,_
-00011aa0: 7265 6369 7069 656e 742c 5f64 6561 646c  recipient,_deadl
-00011ab0: 696e 652c 5f61 6d6f 756e 7449 6e2c 5f61  ine,_amountIn,_a
-00011ac0: 6d6f 756e 744f 7574 4d69 6e5d 0a20 2020  mountOutMin].   
-00011ad0: 2020 2020 2023 2066 756e 6374 696f 6e5f       # function_
-00011ae0: 7061 7261 6d73 3d65 6e63 6f64 655f 6162  params=encode_ab
-00011af0: 6928 7479 7065 2c64 6174 6129 0a20 2020  i(type,data).   
-00011b00: 2020 2020 2066 756e 6374 696f 6e5f 7061       function_pa
-00011b10: 7261 6d73 3d7b 0a20 2020 2020 2020 2020  rams={.         
-00011b20: 2020 2027 7061 7468 273a 5f70 6174 682c     'path':_path,
-00011b30: 0a20 2020 2020 2020 2020 2020 2027 7265  .            're
-00011b40: 6369 7069 656e 7427 3a5f 7265 6369 7069  cipient':_recipi
-00011b50: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
-00011b60: 2027 6465 6164 6c69 6e65 273a 5f64 6561   'deadline':_dea
-00011b70: 646c 696e 652c 0a20 2020 2020 2020 2020  dline,.         
-00011b80: 2020 2027 616d 6f75 6e74 496e 273a 5f61     'amountIn':_a
-00011b90: 6d6f 756e 7449 6e2c 0a20 2020 2020 2020  mountIn,.       
-00011ba0: 2020 2020 2027 616d 6f75 6e74 4f75 744d       'amountOutM
-00011bb0: 696e 696d 756d 273a 5f61 6d6f 756e 744f  inimum':_amountO
-00011bc0: 7574 4d69 6e0a 2020 2020 2020 2020 7d0a  utMin.        }.
-00011bd0: 2020 2020 2020 2020 2320 6675 6e63 7469          # functi
-00011be0: 6f6e 5f70 6172 616d 733d 285f 7061 7468  on_params=(_path
-00011bf0: 2c5f 7265 6369 7069 656e 742c 5f64 6561  ,_recipient,_dea
-00011c00: 646c 696e 652c 5f61 6d6f 756e 7449 6e2c  dline,_amountIn,
-00011c10: 5f61 6d6f 756e 744f 7574 4d69 6e29 0a20  _amountOutMin). 
-00011c20: 2020 2020 2020 2073 7761 705f 6675 6e63         swap_func
-00011c30: 7469 6f6e 3d72 6f75 7465 5f63 6f6e 7472  tion=route_contr
-00011c40: 6163 742e 6675 6e63 7469 6f6e 732e 6578  act.functions.ex
-00011c50: 6163 7449 6e70 7574 2866 756e 6374 696f  actInput(functio
-00011c60: 6e5f 7061 7261 6d73 290a 2020 2020 2020  n_params).      
-00011c70: 2020 7478 5f70 6172 616d 733d 7b0a 2020    tx_params={.  
-00011c80: 2020 2020 2020 2020 2020 2766 726f 6d27            'from'
-00011c90: 3a20 5f70 7562 6c69 635f 6b65 792c 0a20  : _public_key,. 
-00011ca0: 2020 2020 2020 2020 2020 2027 7661 6c75             'valu
-00011cb0: 6527 3a20 302c 0a20 2020 2020 2020 2020  e': 0,.         
-00011cc0: 2020 2027 6e6f 6e63 6527 3a20 5f6e 6f6e     'nonce': _non
-00011cd0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
-00011ce0: 2774 7970 6527 3a20 2730 7832 272c 0a20  'type': '0x2',. 
-00011cf0: 2020 2020 2020 2020 2020 2023 2027 6761             # 'ga
-00011d00: 7327 3a5f 6761 730a 2020 2020 2020 2020  s':_gas.        
-00011d10: 7d0a 2020 2020 2020 2020 7472 616e 7361  }.        transa
-00011d20: 6374 696f 6e3d 7377 6170 5f66 756e 6374  ction=swap_funct
-00011d30: 696f 6e2e 6275 696c 6454 7261 6e73 6163  ion.buildTransac
-00011d40: 7469 6f6e 2874 785f 7061 7261 6d73 290a  tion(tx_params).
-00011d50: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
-00011d60: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
-00011d70: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
-00011d80: 6e5f 7472 616e 7361 6374 696f 6e28 7472  n_transaction(tr
-00011d90: 616e 7361 6374 696f 6e2c 2070 7269 7661  ansaction, priva
-00011da0: 7465 5f6b 6579 3d5f 7072 6976 6174 655f  te_key=_private_
-00011db0: 6b65 7929 0a20 2020 2020 2020 2072 6574  key).        ret
-00011dc0: 7572 6e20 5f77 6562 332e 746f 4865 7828  urn _web3.toHex(
-00011dd0: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
-00011de0: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
-00011df0: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
-00011e00: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
-00011e10: 2929 0a0a 2020 2020 2320 7374 7275 6374  ))..    # struct
-00011e20: 2045 7861 6374 4f75 7470 7574 5369 6e67   ExactOutputSing
-00011e30: 6c65 5061 7261 6d73 207b 0a20 2020 2023  leParams {.    #
-00011e40: 2020 2020 2061 6464 7265 7373 2074 6f6b       address tok
-00011e50: 656e 496e 3b0a 2020 2020 2320 2020 2020  enIn;.    #     
-00011e60: 6164 6472 6573 7320 746f 6b65 6e4f 7574  address tokenOut
-00011e70: 3b0a 2020 2020 2320 2020 2020 7569 6e74  ;.    #     uint
-00011e80: 3234 2066 6565 3b0a 2020 2020 2320 2020  24 fee;.    #   
-00011e90: 2020 6164 6472 6573 7320 7265 6369 7069    address recipi
-00011ea0: 656e 743b 0a20 2020 2023 2020 2020 2075  ent;.    #     u
-00011eb0: 696e 7432 3536 2064 6561 646c 696e 653b  int256 deadline;
-00011ec0: 0a20 2020 2023 2020 2020 2075 696e 7432  .    #     uint2
-00011ed0: 3536 2061 6d6f 756e 744f 7574 3b0a 2020  56 amountOut;.  
-00011ee0: 2020 2320 2020 2020 7569 6e74 3235 3620    #     uint256 
-00011ef0: 616d 6f75 6e74 496e 4d61 7869 6d75 6d3b  amountInMaximum;
-00011f00: 0a20 2020 2023 2020 2020 2075 696e 7431  .    #     uint1
-00011f10: 3630 2073 7172 7450 7269 6365 4c69 6d69  60 sqrtPriceLimi
-00011f20: 7458 3936 3b0a 2020 2020 2320 7d0a 2020  tX96;.    # }.  
-00011f30: 2020 6465 6620 6578 6163 744f 7574 7075    def exactOutpu
-00011f40: 7453 696e 676c 6528 5f77 6562 333a 5765  tSingle(_web3:We
-00011f50: 6233 2c5f 726f 7574 655f 6164 6472 6573  b3,_route_addres
-00011f60: 732c 5f61 6269 2c5f 6e6f 6e63 652c 5f70  s,_abi,_nonce,_p
-00011f70: 7562 6c69 635f 6b65 792c 5f70 7269 7661  ublic_key,_priva
-00011f80: 7465 5f6b 6579 2c0a 2020 2020 2020 2020  te_key,.        
-00011f90: 5f74 6f6b 656e 5f69 6e2c 5f74 6f6b 656e  _token_in,_token
-00011fa0: 5f6f 7574 2c5f 6665 652c 5f72 6563 6970  _out,_fee,_recip
-00011fb0: 6965 6e74 2c5f 6465 6164 6c69 6e65 2c5f  ient,_deadline,_
-00011fc0: 616d 6f75 6e74 5f6f 7574 2c5f 616d 6f75  amount_out,_amou
-00011fd0: 6e74 5f69 6e5f 6d61 782c 5f73 7172 745f  nt_in_max,_sqrt_
-00011fe0: 7072 6963 655f 6c69 6d69 7429 3a0a 2020  price_limit):.  
-00011ff0: 2020 2020 2020 726f 7574 655f 636f 6e74        route_cont
-00012000: 7261 6374 3d5f 7765 6233 2e65 7468 2e63  ract=_web3.eth.c
-00012010: 6f6e 7472 6163 7428 6164 6472 6573 733d  ontract(address=
-00012020: 5f72 6f75 7465 5f61 6464 7265 7373 2c20  _route_address, 
-00012030: 6162 693d 5f61 6269 290a 2020 2020 2020  abi=_abi).      
-00012040: 2020 6675 6e63 7469 6f6e 5f70 6172 616d    function_param
-00012050: 3d7b 0a20 2020 2020 2020 2020 2020 2027  ={.            '
-00012060: 746f 6b65 6e49 6e27 3a5f 746f 6b65 6e5f  tokenIn':_token_
-00012070: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
-00012080: 2774 6f6b 656e 4f75 7427 3a5f 746f 6b65  'tokenOut':_toke
-00012090: 6e5f 6f75 742c 0a20 2020 2020 2020 2020  n_out,.         
-000120a0: 2020 2027 6665 6527 3a5f 6665 652c 0a20     'fee':_fee,. 
-000120b0: 2020 2020 2020 2020 2020 2027 7265 6369             'reci
-000120c0: 7069 656e 7427 3a5f 7265 6369 7069 656e  pient':_recipien
-000120d0: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
-000120e0: 6465 6164 6c69 6e65 273a 5f64 6561 646c  deadline':_deadl
-000120f0: 696e 652c 0a20 2020 2020 2020 2020 2020  ine,.           
-00012100: 2027 616d 6f75 6e74 4f75 7427 3a5f 616d   'amountOut':_am
-00012110: 6f75 6e74 5f6f 7574 2c0a 2020 2020 2020  ount_out,.      
-00012120: 2020 2020 2020 2761 6d6f 756e 7449 6e4d        'amountInM
-00012130: 6178 696d 756d 273a 5f61 6d6f 756e 745f  aximum':_amount_
-00012140: 696e 5f6d 6178 2c0a 2020 2020 2020 2020  in_max,.        
-00012150: 2020 2020 2773 7172 7450 7269 6365 4c69      'sqrtPriceLi
-00012160: 6d69 7458 3936 273a 5f73 7172 745f 7072  mitX96':_sqrt_pr
-00012170: 6963 655f 6c69 6d69 740a 2020 2020 2020  ice_limit.      
-00012180: 2020 7d0a 2020 2020 2020 2020 7377 6170    }.        swap
-00012190: 5f66 756e 6374 696f 6e3d 726f 7574 655f  _function=route_
-000121a0: 636f 6e74 7261 6374 2e66 756e 6374 696f  contract.functio
-000121b0: 6e73 2e65 7861 6374 4f75 7470 7574 5369  ns.exactOutputSi
-000121c0: 6e67 6c65 2866 756e 6374 696f 6e5f 7061  ngle(function_pa
-000121d0: 7261 6d29 0a20 2020 2020 2020 2074 785f  ram).        tx_
-000121e0: 7061 7261 6d73 3d7b 0a20 2020 2020 2020  params={.       
-000121f0: 2020 2020 2027 6672 6f6d 273a 205f 7075       'from': _pu
-00012200: 626c 6963 5f6b 6579 2c0a 2020 2020 2020  blic_key,.      
-00012210: 2020 2020 2020 2776 616c 7565 273a 2030        'value': 0
-00012220: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
-00012230: 6f6e 6365 273a 205f 6e6f 6e63 652c 0a20  once': _nonce,. 
-00012240: 2020 2020 2020 2020 2020 2027 7479 7065             'type
-00012250: 273a 2027 3078 3227 0a20 2020 2020 2020  ': '0x2'.       
-00012260: 207d 0a20 2020 2020 2020 2074 7261 6e73   }.        trans
-00012270: 6163 7469 6f6e 3d73 7761 705f 6675 6e63  action=swap_func
-00012280: 7469 6f6e 2e62 7569 6c64 5472 616e 7361  tion.buildTransa
-00012290: 6374 696f 6e28 7478 5f70 6172 616d 7329  ction(tx_params)
-000122a0: 0a20 2020 2020 2020 2073 6967 6e65 645f  .        signed_
-000122b0: 7472 616e 7361 6374 696f 6e3d 5f77 6562  transaction=_web
-000122c0: 332e 6574 682e 6163 636f 756e 742e 7369  3.eth.account.si
-000122d0: 676e 5f74 7261 6e73 6163 7469 6f6e 2874  gn_transaction(t
-000122e0: 7261 6e73 6163 7469 6f6e 2c20 7072 6976  ransaction, priv
-000122f0: 6174 655f 6b65 793d 5f70 7269 7661 7465  ate_key=_private
-00012300: 5f6b 6579 290a 2020 2020 2020 2020 7265  _key).        re
-00012310: 7475 726e 205f 7765 6233 2e74 6f48 6578  turn _web3.toHex
-00012320: 285f 7765 6233 2e65 7468 2e73 656e 645f  (_web3.eth.send_
-00012330: 7261 775f 7472 616e 7361 6374 696f 6e28  raw_transaction(
-00012340: 7369 676e 6564 5f74 7261 6e73 6163 7469  signed_transacti
-00012350: 6f6e 2e72 6177 5472 616e 7361 6374 696f  on.rawTransactio
-00012360: 6e29 290a 0a0a 2020 2020 2320 7374 7275  n))...    # stru
-00012370: 6374 2045 7861 6374 4f75 7470 7574 5061  ct ExactOutputPa
-00012380: 7261 6d73 207b 0a20 2020 2023 2020 2020  rams {.    #    
-00012390: 2062 7974 6573 2070 6174 683b 0a20 2020   bytes path;.   
-000123a0: 2023 2020 2020 2061 6464 7265 7373 2072   #     address r
-000123b0: 6563 6970 6965 6e74 3b0a 2020 2020 2320  ecipient;.    # 
-000123c0: 2020 2020 7569 6e74 3235 3620 6465 6164      uint256 dead
-000123d0: 6c69 6e65 3b0a 2020 2020 2320 2020 2020  line;.    #     
-000123e0: 7569 6e74 3235 3620 616d 6f75 6e74 4f75  uint256 amountOu
-000123f0: 743b 0a20 2020 2023 2020 2020 2075 696e  t;.    #     uin
-00012400: 7432 3536 2061 6d6f 756e 7449 6e4d 6178  t256 amountInMax
-00012410: 696d 756d 3b0a 2020 2020 2320 7d0a 2020  imum;.    # }.  
-00012420: 2020 6465 6620 6578 6163 744f 7574 7075    def exactOutpu
-00012430: 7428 5f77 6562 333a 5765 6233 2c5f 726f  t(_web3:Web3,_ro
-00012440: 7574 655f 6164 6472 6573 732c 5f61 6269  ute_address,_abi
-00012450: 2c5f 6e6f 6e63 652c 5f70 7562 6c69 635f  ,_nonce,_public_
-00012460: 6b65 792c 5f70 7269 7661 7465 5f6b 6579  key,_private_key
-00012470: 2c0a 2020 2020 2020 2020 5f70 6174 682c  ,.        _path,
-00012480: 5f72 6563 6970 6965 6e74 2c5f 6465 6164  _recipient,_dead
-00012490: 6c69 6e65 2c5f 616d 6f75 6e74 5f6f 7574  line,_amount_out
-000124a0: 2c5f 616d 6f75 6e74 5f69 6e5f 6d61 7829  ,_amount_in_max)
-000124b0: 3a0a 2020 2020 2020 2020 726f 7574 655f  :.        route_
-000124c0: 636f 6e74 7261 6374 3d5f 7765 6233 2e65  contract=_web3.e
-000124d0: 7468 2e63 6f6e 7472 6163 7428 6164 6472  th.contract(addr
-000124e0: 6573 733d 5f72 6f75 7465 5f61 6464 7265  ess=_route_addre
-000124f0: 7373 2c20 6162 693d 5f61 6269 290a 2020  ss, abi=_abi).  
-00012500: 2020 2020 2020 6675 6e63 7469 6f6e 5f70        function_p
-00012510: 6172 616d 3d7b 0a20 2020 2020 2020 2020  aram={.         
-00012520: 2020 2027 7061 7468 273a 5f70 6174 682c     'path':_path,
-00012530: 0a20 2020 2020 2020 2020 2020 2027 7265  .            're
-00012540: 6369 7069 656e 7427 3a5f 7265 6369 7069  cipient':_recipi
-00012550: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
-00012560: 2027 6465 6164 6c69 6e65 273a 5f64 6561   'deadline':_dea
-00012570: 646c 696e 652c 0a20 2020 2020 2020 2020  dline,.         
-00012580: 2020 2027 616d 6f75 6e74 4f75 7427 3a5f     'amountOut':_
-00012590: 616d 6f75 6e74 5f6f 7574 2c0a 2020 2020  amount_out,.    
-000125a0: 2020 2020 2020 2020 2761 6d6f 756e 7449          'amountI
-000125b0: 6e4d 6178 696d 756d 273a 5f61 6d6f 756e  nMaximum':_amoun
-000125c0: 745f 696e 5f6d 6178 0a20 2020 2020 2020  t_in_max.       
-000125d0: 207d 0a20 2020 2020 2020 2073 7761 705f   }.        swap_
-000125e0: 6675 6e63 7469 6f6e 3d72 6f75 7465 5f63  function=route_c
-000125f0: 6f6e 7472 6163 742e 6675 6e63 7469 6f6e  ontract.function
-00012600: 732e 6578 6163 744f 7574 7075 7428 6675  s.exactOutput(fu
-00012610: 6e63 7469 6f6e 5f70 6172 616d 290a 2020  nction_param).  
-00012620: 2020 2020 2020 7478 5f70 6172 616d 733d        tx_params=
-00012630: 7b0a 2020 2020 2020 2020 2020 2020 2766  {.            'f
-00012640: 726f 6d27 3a20 5f70 7562 6c69 635f 6b65  rom': _public_ke
-00012650: 792c 0a20 2020 2020 2020 2020 2020 2027  y,.            '
-00012660: 7661 6c75 6527 3a20 302c 0a20 2020 2020  value': 0,.     
-00012670: 2020 2020 2020 2027 6e6f 6e63 6527 3a20         'nonce': 
-00012680: 5f6e 6f6e 6365 2c0a 2020 2020 2020 2020  _nonce,.        
-00012690: 2020 2020 2774 7970 6527 3a20 2730 7832      'type': '0x2
-000126a0: 270a 2020 2020 2020 2020 7d0a 2020 2020  '.        }.    
-000126b0: 2020 2020 7472 616e 7361 6374 696f 6e3d      transaction=
-000126c0: 7377 6170 5f66 756e 6374 696f 6e2e 6275  swap_function.bu
-000126d0: 696c 6454 7261 6e73 6163 7469 6f6e 2874  ildTransaction(t
-000126e0: 785f 7061 7261 6d73 290a 2020 2020 2020  x_params).      
-000126f0: 2020 7369 676e 6564 5f74 7261 6e73 6163    signed_transac
-00012700: 7469 6f6e 3d5f 7765 6233 2e65 7468 2e61  tion=_web3.eth.a
-00012710: 6363 6f75 6e74 2e73 6967 6e5f 7472 616e  ccount.sign_tran
-00012720: 7361 6374 696f 6e28 7472 616e 7361 6374  saction(transact
-00012730: 696f 6e2c 2070 7269 7661 7465 5f6b 6579  ion, private_key
-00012740: 3d5f 7072 6976 6174 655f 6b65 7929 0a20  =_private_key). 
-00012750: 2020 2020 2020 2072 6574 7572 6e20 5f77         return _w
-00012760: 6562 332e 746f 4865 7828 5f77 6562 332e  eb3.toHex(_web3.
-00012770: 6574 682e 7365 6e64 5f72 6177 5f74 7261  eth.send_raw_tra
-00012780: 6e73 6163 7469 6f6e 2873 6967 6e65 645f  nsaction(signed_
-00012790: 7472 616e 7361 6374 696f 6e2e 7261 7754  transaction.rawT
-000127a0: 7261 6e73 6163 7469 6f6e 2929 0a63 6c61  ransaction)).cla
-000127b0: 7373 204a 6f65 5632 4661 6374 6f72 793a  ss JoeV2Factory:
-000127c0: 0a20 2020 206a 6f65 5f66 6163 746f 7279  .    joe_factory
-000127d0: 5f76 325f 6162 693d 6a73 6f6e 2e6c 6f61  _v2_abi=json.loa
-000127e0: 6473 2827 5b7b 2269 6e70 7574 7322 3a5b  ds('[{"inputs":[
-000127f0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00012800: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-00012810: 3a22 5f66 6565 5265 6369 7069 656e 7422  :"_feeRecipient"
-00012820: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00012830: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00012840: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00012850: 6d65 223a 225f 666c 6173 684c 6f61 6e46  me":"_flashLoanF
-00012860: 6565 222c 2274 7970 6522 3a22 7569 6e74  ee","type":"uint
-00012870: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
-00012880: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
-00012890: 6162 6c65 222c 2274 7970 6522 3a22 636f  able","type":"co
-000128a0: 6e73 7472 7563 746f 7222 7d2c 7b22 696e  nstructor"},{"in
-000128b0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-000128c0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-000128d0: 2c22 6e61 6d65 223a 2262 7022 2c22 7479  ,"name":"bp","ty
-000128e0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-000128f0: 226e 616d 6522 3a22 4269 6e48 656c 7065  "name":"BinHelpe
-00012900: 725f 5f42 696e 5374 6570 4f76 6572 666c  r__BinStepOverfl
-00012910: 6f77 7322 2c22 7479 7065 223a 2265 7272  ows","type":"err
-00012920: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-00012930: 5d2c 226e 616d 6522 3a22 4269 6e48 656c  ],"name":"BinHel
-00012940: 7065 725f 5f49 644f 7665 7266 6c6f 7773  per__IdOverflows
-00012950: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-00012960: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-00012970: 6e61 6d65 223a 224c 4246 6163 746f 7279  name":"LBFactory
-00012980: 5f5f 4164 6472 6573 735a 6572 6f22 2c22  __AddressZero","
-00012990: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-000129a0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-000129b0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-000129c0: 3536 222c 226e 616d 6522 3a22 6269 6e53  56","name":"binS
-000129d0: 7465 7022 2c22 7479 7065 223a 2275 696e  tep","type":"uin
-000129e0: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-000129f0: 4c42 4661 6374 6f72 795f 5f42 696e 5374  LBFactory__BinSt
-00012a00: 6570 4861 734e 6f50 7265 7365 7422 2c22  epHasNoPreset","
-00012a10: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-00012a20: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-00012a30: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00012a40: 3536 222c 226e 616d 6522 3a22 6c6f 7765  56","name":"lowe
-00012a50: 7242 6f75 6e64 222c 2274 7970 6522 3a22  rBound","type":"
-00012a60: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-00012a70: 726e 616c 5479 7065 223a 2275 696e 7431  rnalType":"uint1
-00012a80: 3622 2c22 6e61 6d65 223a 2262 696e 5374  6","name":"binSt
-00012a90: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
-00012aa0: 3136 227d 2c7b 2269 6e74 6572 6e61 6c54  16"},{"internalT
-00012ab0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00012ac0: 6e61 6d65 223a 2268 6967 6865 7242 6f75  name":"higherBou
-00012ad0: 6e64 222c 2274 7970 6522 3a22 7569 6e74  nd","type":"uint
-00012ae0: 3235 3622 7d5d 2c22 6e61 6d65 223a 224c  256"}],"name":"L
-00012af0: 4246 6163 746f 7279 5f5f 4269 6e53 7465  BFactory__BinSte
-00012b00: 7052 6571 7569 7265 6d65 6e74 7342 7265  pRequirementsBre
-00012b10: 6163 6865 6422 2c22 7479 7065 223a 2265  ached","type":"e
-00012b20: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-00012b30: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00012b40: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-00012b50: 223a 2266 696c 7465 7250 6572 696f 6422  ":"filterPeriod"
-00012b60: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
-00012b70: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00012b80: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-00012b90: 223a 2264 6563 6179 5065 7269 6f64 222c  ":"decayPeriod",
-00012ba0: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
-00012bb0: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
-00012bc0: 6f72 795f 5f44 6563 7265 6173 696e 6750  ory__DecreasingP
-00012bd0: 6572 696f 6473 222c 2274 7970 6522 3a22  eriods","type":"
-00012be0: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00012bf0: 223a 5b5d 2c22 6e61 6d65 223a 224c 4246  ":[],"name":"LBF
-00012c00: 6163 746f 7279 5f5f 4661 6374 6f72 794c  actory__FactoryL
-00012c10: 6f63 6b49 7341 6c72 6561 6479 496e 5468  ockIsAlreadyInTh
-00012c20: 6553 616d 6553 7461 7465 222c 2274 7970  eSameState","typ
-00012c30: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-00012c40: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00012c50: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00012c60: 2c22 6e61 6d65 223a 2266 6565 7322 2c22  ,"name":"fees","
-00012c70: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00012c80: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00012c90: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00012ca0: 223a 226d 6178 4665 6573 222c 2274 7970  ":"maxFees","typ
-00012cb0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-00012cc0: 6e61 6d65 223a 224c 4246 6163 746f 7279  name":"LBFactory
-00012cd0: 5f5f 4665 6573 4162 6f76 654d 6178 222c  __FeesAboveMax",
-00012ce0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-00012cf0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-00012d00: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00012d10: 3235 3622 2c22 6e61 6d65 223a 2266 6565  256","name":"fee
-00012d20: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
-00012d30: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-00012d40: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00012d50: 6e61 6d65 223a 226d 6178 4665 6573 222c  name":"maxFees",
-00012d60: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00012d70: 7d5d 2c22 6e61 6d65 223a 224c 4246 6163  }],"name":"LBFac
-00012d80: 746f 7279 5f5f 466c 6173 684c 6f61 6e46  tory__FlashLoanF
-00012d90: 6565 4162 6f76 654d 6178 222c 2274 7970  eeAboveMax","typ
-00012da0: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-00012db0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00012dc0: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-00012dd0: 2c22 6e61 6d65 223a 2275 7365 7222 2c22  ,"name":"user","
-00012de0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-00012df0: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
-00012e00: 6f72 795f 5f46 756e 6374 696f 6e49 734c  ory__FunctionIsL
-00012e10: 6f63 6b65 6446 6f72 5573 6572 7322 2c22  ockedForUsers","
-00012e20: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-00012e30: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-00012e40: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-00012e50: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
-00012e60: 6522 3a22 746f 6b65 6e22 2c22 7479 7065  e":"token","type
-00012e70: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
-00012e80: 616d 6522 3a22 4c42 4661 6374 6f72 795f  ame":"LBFactory_
-00012e90: 5f49 6465 6e74 6963 616c 4164 6472 6573  _IdenticalAddres
-00012ea0: 7365 7322 2c22 7479 7065 223a 2265 7272  ses","type":"err
-00012eb0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-00012ec0: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
-00012ed0: 6f72 795f 5f49 6d70 6c65 6d65 6e74 6174  ory__Implementat
-00012ee0: 696f 6e4e 6f74 5365 7422 2c22 7479 7065  ionNotSet","type
-00012ef0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-00012f00: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00012f10: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-00012f20: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-00012f30: 746f 6b65 6e58 222c 2274 7970 6522 3a22  tokenX","type":"
-00012f40: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+00010960: 7072 696e 7428 2263 6f6e 7472 6163 7420  print("contract 
+00010970: 636f 6e6e 6563 7469 6f6e 2069 7320 222b  connection is "+
+00010980: 7374 7228 7365 6c66 2e77 6562 332e 6973  str(self.web3.is
+00010990: 436f 6e6e 6563 7465 6428 2929 290a 2020  Connected())).  
+000109a0: 2020 2020 2020 6966 2073 656c 662e 7765        if self.we
+000109b0: 6233 2e69 7343 6f6e 6e65 6374 6564 2829  b3.isConnected()
+000109c0: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+000109d0: 6c66 2e6e 6f6e 6365 3d73 656c 662e 7765  lf.nonce=self.we
+000109e0: 6233 2e65 7468 2e67 6574 5f74 7261 6e73  b3.eth.get_trans
+000109f0: 6163 7469 6f6e 5f63 6f75 6e74 2873 656c  action_count(sel
+00010a00: 662e 6d79 5f70 7562 6c69 635f 6b65 7929  f.my_public_key)
+00010a10: 0a20 2020 2020 2020 2020 2020 2070 7269  .            pri
+00010a20: 6e74 2822 6e6f 6e63 6520 3d20 222c 7365  nt("nonce = ",se
+00010a30: 6c66 2e6e 6f6e 6365 290a 2020 2020 2020  lf.nonce).      
+00010a40: 2020 7072 696e 7428 2723 2323 2323 2323    print('#######
+00010a50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010a60: 2323 2323 2327 290a 2020 2020 2020 2020  #####').        
+00010a70: 2320 756e 6973 7761 705f 4661 6374 6f72  # uniswap_Factor
+00010a80: 790a 2020 2020 2020 2020 7365 6c66 2e66  y.        self.f
+00010a90: 6163 746f 7279 5f61 6269 203d 206a 736f  actory_abi = jso
+00010aa0: 6e2e 6c6f 6164 7328 7365 6c66 2e75 6e69  n.loads(self.uni
+00010ab0: 7377 6170 5f76 335f 6661 6374 6f72 795f  swap_v3_factory_
+00010ac0: 6162 6929 0a20 2020 2020 2020 2073 656c  abi).        sel
+00010ad0: 662e 7061 6972 5f61 6269 3d6a 736f 6e2e  f.pair_abi=json.
+00010ae0: 6c6f 6164 7328 7365 6c66 2e75 6e69 7377  loads(self.unisw
+00010af0: 6170 5f76 335f 7061 6972 5f61 6269 290a  ap_v3_pair_abi).
+00010b00: 2020 2020 2020 2020 7365 6c66 2e65 7263          self.erc
+00010b10: 3230 5f61 6269 3d6a 736f 6e2e 6c6f 6164  20_abi=json.load
+00010b20: 7328 7365 6c66 2e75 6e69 7377 6170 5f76  s(self.uniswap_v
+00010b30: 335f 6572 6332 305f 6162 6929 0a20 2020  3_erc20_abi).   
+00010b40: 2020 2020 2073 656c 662e 726f 7574 655f       self.route_
+00010b50: 6162 693d 6a73 6f6e 2e6c 6f61 6473 2873  abi=json.loads(s
+00010b60: 656c 662e 756e 6973 7761 705f 7633 5f72  elf.uniswap_v3_r
+00010b70: 6f75 7465 5f61 6269 290a 0a20 2020 2020  oute_abi)..     
+00010b80: 2020 2073 656c 662e 6661 6374 6f72 795f     self.factory_
+00010b90: 636f 6e74 7261 6374 203d 2073 656c 662e  contract = self.
+00010ba0: 7765 6233 2e65 7468 2e63 6f6e 7472 6163  web3.eth.contrac
+00010bb0: 7428 6164 6472 6573 733d 7365 6c66 2e66  t(address=self.f
+00010bc0: 6163 746f 7279 5f61 6464 7265 7373 2c20  actory_address, 
+00010bd0: 6162 693d 7365 6c66 2e66 6163 746f 7279  abi=self.factory
+00010be0: 5f61 6269 290a 2020 2020 2020 2020 7365  _abi).        se
+00010bf0: 6c66 2e72 6f75 7465 5f63 6f6e 7472 6163  lf.route_contrac
+00010c00: 743d 7365 6c66 2e77 6562 332e 6574 682e  t=self.web3.eth.
+00010c10: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
+00010c20: 3d73 656c 662e 726f 7574 655f 6164 6472  =self.route_addr
+00010c30: 6573 732c 6162 693d 7365 6c66 2e72 6f75  ess,abi=self.rou
+00010c40: 7465 5f61 6269 290a 636c 6173 7320 556e  te_abi).class Un
+00010c50: 6973 7761 7056 3346 6163 746f 7279 3a0a  iswapV3Factory:.
+00010c60: 0a20 2020 2023 6661 6374 6f72 790a 2020  .    #factory.  
+00010c70: 2020 2372 6574 7572 6e20 6164 6472 6573    #return addres
+00010c80: 7320 6f66 2070 6f6f 6c20 666f 7220 746f  s of pool for to
+00010c90: 6b65 6e41 2061 6e64 2074 6f6b 656e 4220  kenA and tokenB 
+00010ca0: 7769 7468 2073 7065 6369 6669 6320 6665  with specific fe
+00010cb0: 650a 2020 2020 2331 3030 3030 2066 6f72  e.    #10000 for
+00010cc0: 2031 2520 6665 652c 2033 3030 3020 666f   1% fee, 3000 fo
+00010cd0: 7220 302e 3325 2c20 616e 6420 3530 3020  r 0.3%, and 500 
+00010ce0: 666f 7220 302e 3035 250a 2020 2020 6465  for 0.05%.    de
+00010cf0: 6620 6765 7450 6f6f 6c28 5f77 6562 333a  f getPool(_web3:
+00010d00: 5765 6233 2c5f 6661 6374 6f72 795f 6164  Web3,_factory_ad
+00010d10: 6472 6573 732c 5f61 6269 2c5f 746f 6b65  dress,_abi,_toke
+00010d20: 6e41 3a73 7472 2c5f 746f 6b65 6e42 3a73  nA:str,_tokenB:s
+00010d30: 7472 2c5f 6665 653a 696e 7429 3a0a 2020  tr,_fee:int):.  
+00010d40: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
+00010d50: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
+00010d60: 6164 6472 6573 733d 5f66 6163 746f 7279  address=_factory
+00010d70: 5f61 6464 7265 7373 2c20 6162 693d 5f61  _address, abi=_a
+00010d80: 6269 292e 6675 6e63 7469 6f6e 732e 6765  bi).functions.ge
+00010d90: 7450 6f6f 6c28 5f74 6f6b 656e 412c 5f74  tPool(_tokenA,_t
+00010da0: 6f6b 656e 422c 5f66 6565 292e 6361 6c6c  okenB,_fee).call
+00010db0: 2829 0a20 2020 200a 636c 6173 7320 556e  ().    .class Un
+00010dc0: 6973 7761 7056 3351 756f 7465 723a 0a20  iswapV3Quoter:. 
+00010dd0: 2020 2023 7265 7475 726e 2061 6464 7265     #return addre
+00010de0: 7373 206f 6620 706f 6f6c 2066 6f72 2074  ss of pool for t
+00010df0: 6f6b 656e 4120 616e 6420 746f 6b65 6e42  okenA and tokenB
+00010e00: 2077 6974 6820 7370 6563 6966 6963 2066   with specific f
+00010e10: 6565 0a20 2020 2023 3130 3030 3020 666f  ee.    #10000 fo
+00010e20: 7220 3125 2066 6565 2c20 3330 3030 2066  r 1% fee, 3000 f
+00010e30: 6f72 2030 2e33 252c 2061 6e64 2035 3030  or 0.3%, and 500
+00010e40: 2066 6f72 2030 2e30 3525 0a20 2020 2064   for 0.05%.    d
+00010e50: 6566 2067 6574 506f 6f6c 285f 7765 6233  ef getPool(_web3
+00010e60: 3a57 6562 332c 5f71 756f 7465 725f 6164  :Web3,_quoter_ad
+00010e70: 6472 6573 732c 5f61 6269 2c5f 746f 6b65  dress,_abi,_toke
+00010e80: 6e41 3a73 7472 2c5f 746f 6b65 6e42 3a73  nA:str,_tokenB:s
+00010e90: 7472 2c5f 6665 653a 696e 7429 3a0a 2020  tr,_fee:int):.  
+00010ea0: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
+00010eb0: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
+00010ec0: 6164 6472 6573 733d 5f71 756f 7465 725f  address=_quoter_
+00010ed0: 6164 6472 6573 732c 2061 6269 3d5f 6162  address, abi=_ab
+00010ee0: 6929 2e66 756e 6374 696f 6e73 2e67 6574  i).functions.get
+00010ef0: 506f 6f6c 285f 746f 6b65 6e41 2c5f 746f  Pool(_tokenA,_to
+00010f00: 6b65 6e42 2c5f 6665 6529 2e63 616c 6c28  kenB,_fee).call(
+00010f10: 290a 2020 2020 0a20 2020 2023 2073 7472  ).    .    # str
+00010f20: 7563 7420 5175 6f74 6545 7861 6374 496e  uct QuoteExactIn
+00010f30: 7075 7453 696e 676c 6550 6172 616d 7320  putSingleParams 
+00010f40: 7b0a 2020 2020 2320 2020 2020 6164 6472  {.    #     addr
+00010f50: 6573 7320 746f 6b65 6e49 6e3b 0a20 2020  ess tokenIn;.   
+00010f60: 2023 2020 2020 2061 6464 7265 7373 2074   #     address t
+00010f70: 6f6b 656e 4f75 743b 0a20 2020 2023 2020  okenOut;.    #  
+00010f80: 2020 2075 696e 7432 3536 2061 6d6f 756e     uint256 amoun
+00010f90: 7449 6e3b 0a20 2020 2023 2020 2020 2075  tIn;.    #     u
+00010fa0: 696e 7432 3420 6665 653b 0a20 2020 2023  int24 fee;.    #
+00010fb0: 2020 2020 2075 696e 7431 3630 2073 7172       uint160 sqr
+00010fc0: 7450 7269 6365 4c69 6d69 7458 3936 3b0a  tPriceLimitX96;.
+00010fd0: 2020 2020 2320 7d0a 2020 2020 6465 6620      # }.    def 
+00010fe0: 7175 6f74 6545 7861 6374 496e 7075 7453  quoteExactInputS
+00010ff0: 696e 676c 6528 5f77 6562 333a 5765 6233  ingle(_web3:Web3
+00011000: 2c5f 7175 6f74 6572 5f61 6464 7265 7373  ,_quoter_address
+00011010: 2c5f 6162 692c 5f70 6172 616d 293a 0a20  ,_abi,_param):. 
+00011020: 2020 2020 2020 2072 6574 7572 6e20 5f77         return _w
+00011030: 6562 332e 6574 682e 636f 6e74 7261 6374  eb3.eth.contract
+00011040: 2861 6464 7265 7373 3d5f 7175 6f74 6572  (address=_quoter
+00011050: 5f61 6464 7265 7373 2c20 6162 693d 5f61  _address, abi=_a
+00011060: 6269 292e 6675 6e63 7469 6f6e 732e 7175  bi).functions.qu
+00011070: 6f74 6545 7861 6374 496e 7075 7453 696e  oteExactInputSin
+00011080: 676c 6528 5f70 6172 616d 292e 6361 6c6c  gle(_param).call
+00011090: 2829 0a0a 2020 2020 2370 6174 6820 7374  ()..    #path st
+000110a0: 6172 7477 6974 6820 696e 7075 7420 746f  artwith input to
+000110b0: 6b65 6e0a 2020 2020 6465 6620 7175 6f74  ken.    def quot
+000110c0: 6545 7861 6374 496e 7075 7428 5f77 6562  eExactInput(_web
+000110d0: 333a 5765 6233 2c5f 7175 6f74 6572 5f61  3:Web3,_quoter_a
+000110e0: 6464 7265 7373 2c5f 6162 692c 7061 7468  ddress,_abi,path
+000110f0: 2c5f 616d 6f75 6e74 5f69 6e29 3a0a 2020  ,_amount_in):.  
+00011100: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
+00011110: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
+00011120: 6164 6472 6573 733d 5f71 756f 7465 725f  address=_quoter_
+00011130: 6164 6472 6573 732c 2061 6269 3d5f 6162  address, abi=_ab
+00011140: 6929 2e66 756e 6374 696f 6e73 2e71 756f  i).functions.quo
+00011150: 7465 4578 6163 7449 6e70 7574 2870 6174  teExactInput(pat
+00011160: 682c 5f61 6d6f 756e 745f 696e 292e 6361  h,_amount_in).ca
+00011170: 6c6c 2829 0a20 2020 200a 2020 2020 2320  ll().    .    # 
+00011180: 7374 7275 6374 2051 756f 7465 4578 6163  struct QuoteExac
+00011190: 744f 7574 7075 7453 696e 676c 6550 6172  tOutputSinglePar
+000111a0: 616d 7320 7b0a 2020 2020 2320 2020 2020  ams {.    #     
+000111b0: 6164 6472 6573 7320 746f 6b65 6e49 6e3b  address tokenIn;
+000111c0: 0a20 2020 2023 2020 2020 2061 6464 7265  .    #     addre
+000111d0: 7373 2074 6f6b 656e 4f75 743b 0a20 2020  ss tokenOut;.   
+000111e0: 2023 2020 2020 2075 696e 7432 3536 2061   #     uint256 a
+000111f0: 6d6f 756e 743b 0a20 2020 2023 2020 2020  mount;.    #    
+00011200: 2075 696e 7432 3420 6665 653b 0a20 2020   uint24 fee;.   
+00011210: 2023 2020 2020 2075 696e 7431 3630 2073   #     uint160 s
+00011220: 7172 7450 7269 6365 4c69 6d69 7458 3936  qrtPriceLimitX96
+00011230: 3b0a 2020 2020 2320 7d0a 2020 2020 6465  ;.    # }.    de
+00011240: 6620 7175 6f74 6545 7861 6374 4f75 7470  f quoteExactOutp
+00011250: 7574 5369 6e67 6c65 285f 7765 6233 3a57  utSingle(_web3:W
+00011260: 6562 332c 5f71 756f 7465 725f 6164 6472  eb3,_quoter_addr
+00011270: 6573 732c 5f61 6269 2c5f 7061 7261 6d29  ess,_abi,_param)
+00011280: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00011290: 205f 7765 6233 2e65 7468 2e63 6f6e 7472   _web3.eth.contr
+000112a0: 6163 7428 6164 6472 6573 733d 5f71 756f  act(address=_quo
+000112b0: 7465 725f 6164 6472 6573 732c 2061 6269  ter_address, abi
+000112c0: 3d5f 6162 6929 2e66 756e 6374 696f 6e73  =_abi).functions
+000112d0: 2e71 756f 7465 4578 6163 744f 7574 7075  .quoteExactOutpu
+000112e0: 7453 696e 676c 6528 5f70 6172 616d 292e  tSingle(_param).
+000112f0: 6361 6c6c 2829 0a20 2020 200a 2020 2020  call().    .    
+00011300: 2370 6174 6820 7374 6172 7420 7769 7468  #path start with
+00011310: 206f 7574 7075 7420 746f 6b65 6e0a 2020   output token.  
+00011320: 2020 6465 6620 7175 6f74 6545 7861 6374    def quoteExact
+00011330: 4f75 7470 7574 285f 7765 6233 3a57 6562  Output(_web3:Web
+00011340: 332c 5f71 756f 7465 725f 6164 6472 6573  3,_quoter_addres
+00011350: 732c 5f61 6269 2c70 6174 682c 5f61 6d6f  s,_abi,path,_amo
+00011360: 756e 745f 6f75 7429 3a0a 2020 2020 2020  unt_out):.      
+00011370: 2020 7265 7475 726e 205f 7765 6233 2e65    return _web3.e
+00011380: 7468 2e63 6f6e 7472 6163 7428 6164 6472  th.contract(addr
+00011390: 6573 733d 5f71 756f 7465 725f 6164 6472  ess=_quoter_addr
+000113a0: 6573 732c 2061 6269 3d5f 6162 6929 2e66  ess, abi=_abi).f
+000113b0: 756e 6374 696f 6e73 2e71 756f 7465 4578  unctions.quoteEx
+000113c0: 6163 744f 7574 7075 7428 7061 7468 2c5f  actOutput(path,_
+000113d0: 616d 6f75 6e74 5f6f 7574 292e 6361 6c6c  amount_out).call
+000113e0: 2829 0a0a 636c 6173 7320 556e 6973 7761  ()..class Uniswa
+000113f0: 7056 3352 6f75 7465 723a 0a0a 2020 2020  pV3Router:..    
+00011400: 2320 7374 7275 6374 2045 7861 6374 496e  # struct ExactIn
+00011410: 7075 7453 696e 676c 6550 6172 616d 7320  putSingleParams 
+00011420: 7b0a 2020 2020 2320 2020 2020 6164 6472  {.    #     addr
+00011430: 6573 7320 746f 6b65 6e49 6e3b 0a20 2020  ess tokenIn;.   
+00011440: 2023 2020 2020 2061 6464 7265 7373 2074   #     address t
+00011450: 6f6b 656e 4f75 743b 0a20 2020 2023 2020  okenOut;.    #  
+00011460: 2020 2075 696e 7432 3420 6665 653b 0a20     uint24 fee;. 
+00011470: 2020 2023 2020 2020 2061 6464 7265 7373     #     address
+00011480: 2072 6563 6970 6965 6e74 3b0a 2020 2020   recipient;.    
+00011490: 2320 2020 2020 7569 6e74 3235 3620 6465  #     uint256 de
+000114a0: 6164 6c69 6e65 3b0a 2020 2020 2320 2020  adline;.    #   
+000114b0: 2020 7569 6e74 3235 3620 616d 6f75 6e74    uint256 amount
+000114c0: 496e 3b0a 2020 2020 2320 2020 2020 7569  In;.    #     ui
+000114d0: 6e74 3235 3620 616d 6f75 6e74 4f75 744d  nt256 amountOutM
+000114e0: 696e 696d 756d 3b0a 2020 2020 2320 2020  inimum;.    #   
+000114f0: 2020 7569 6e74 3136 3020 7371 7274 5072    uint160 sqrtPr
+00011500: 6963 654c 696d 6974 5839 363b 0a20 2020  iceLimitX96;.   
+00011510: 2023 207d 0a20 2020 2064 6566 2065 7861   # }.    def exa
+00011520: 6374 496e 7075 7453 696e 676c 6528 5f77  ctInputSingle(_w
+00011530: 6562 333a 5765 6233 2c5f 726f 7574 655f  eb3:Web3,_route_
+00011540: 6164 6472 6573 732c 5f61 6269 2c5f 6e6f  address,_abi,_no
+00011550: 6e63 652c 5f70 7562 6c69 635f 6b65 792c  nce,_public_key,
+00011560: 5f70 7269 7661 7465 5f6b 6579 2c0a 2020  _private_key,.  
+00011570: 2020 2020 2020 5f74 6f6b 656e 5f69 6e2c        _token_in,
+00011580: 5f74 6f6b 656e 5f6f 7574 2c5f 6665 652c  _token_out,_fee,
+00011590: 5f72 6563 6970 6965 6e74 2c5f 6465 6164  _recipient,_dead
+000115a0: 6c69 6e65 2c5f 616d 6f75 6e74 5f69 6e2c  line,_amount_in,
+000115b0: 5f61 6d6f 756e 745f 6f75 745f 6d69 6e2c  _amount_out_min,
+000115c0: 5f73 7172 745f 7072 6963 655f 6c69 6d69  _sqrt_price_limi
+000115d0: 7429 3a0a 2020 2020 2020 2020 726f 7574  t):.        rout
+000115e0: 655f 636f 6e74 7261 6374 3d5f 7765 6233  e_contract=_web3
+000115f0: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
+00011600: 6472 6573 733d 5f72 6f75 7465 5f61 6464  dress=_route_add
+00011610: 7265 7373 2c20 6162 693d 5f61 6269 290a  ress, abi=_abi).
+00011620: 2020 2020 2020 2020 6675 6e63 7469 6f6e          function
+00011630: 5f70 6172 616d 733d 7b0a 2020 2020 2020  _params={.      
+00011640: 2020 2020 2020 2774 6f6b 656e 496e 273a        'tokenIn':
+00011650: 5f74 6f6b 656e 5f69 6e2c 0a20 2020 2020  _token_in,.     
+00011660: 2020 2020 2020 2027 746f 6b65 6e4f 7574         'tokenOut
+00011670: 273a 5f74 6f6b 656e 5f6f 7574 2c0a 2020  ':_token_out,.  
+00011680: 2020 2020 2020 2020 2020 2766 6565 273a            'fee':
+00011690: 5f66 6565 2c0a 2020 2020 2020 2020 2020  _fee,.          
+000116a0: 2020 2772 6563 6970 6965 6e74 273a 5f72    'recipient':_r
+000116b0: 6563 6970 6965 6e74 2c0a 2020 2020 2020  ecipient,.      
+000116c0: 2020 2020 2020 2764 6561 646c 696e 6527        'deadline'
+000116d0: 3a5f 6465 6164 6c69 6e65 2c0a 2020 2020  :_deadline,.    
+000116e0: 2020 2020 2020 2020 2761 6d6f 756e 7449          'amountI
+000116f0: 6e27 3a5f 616d 6f75 6e74 5f69 6e2c 0a20  n':_amount_in,. 
+00011700: 2020 2020 2020 2020 2020 2027 616d 6f75             'amou
+00011710: 6e74 4f75 744d 696e 696d 756d 273a 5f61  ntOutMinimum':_a
+00011720: 6d6f 756e 745f 6f75 745f 6d69 6e2c 0a20  mount_out_min,. 
+00011730: 2020 2020 2020 2020 2020 2027 7371 7274             'sqrt
+00011740: 5072 6963 654c 696d 6974 5839 3627 3a5f  PriceLimitX96':_
+00011750: 7371 7274 5f70 7269 6365 5f6c 696d 6974  sqrt_price_limit
+00011760: 0a20 2020 2020 2020 207d 0a20 2020 2020  .        }.     
+00011770: 2020 2023 2066 756e 6374 696f 6e5f 7061     # function_pa
+00011780: 7261 6d73 3d28 5f74 6f6b 656e 5f69 6e2c  rams=(_token_in,
+00011790: 5f74 6f6b 656e 5f6f 7574 2c5f 6665 652c  _token_out,_fee,
+000117a0: 5f72 6563 6970 6965 6e74 2c5f 6465 6164  _recipient,_dead
+000117b0: 6c69 6e65 2c5f 616d 6f75 6e74 5f69 6e2c  line,_amount_in,
+000117c0: 5f61 6d6f 756e 745f 6f75 745f 6d69 6e2c  _amount_out_min,
+000117d0: 5f73 7172 745f 7072 6963 655f 6c69 6d69  _sqrt_price_limi
+000117e0: 7429 0a20 2020 2020 2020 2073 7761 705f  t).        swap_
+000117f0: 6675 6e63 7469 6f6e 3d72 6f75 7465 5f63  function=route_c
+00011800: 6f6e 7472 6163 742e 6675 6e63 7469 6f6e  ontract.function
+00011810: 732e 6578 6163 7449 6e70 7574 5369 6e67  s.exactInputSing
+00011820: 6c65 2866 756e 6374 696f 6e5f 7061 7261  le(function_para
+00011830: 6d73 290a 2020 2020 2020 2020 7478 5f70  ms).        tx_p
+00011840: 6172 616d 733d 7b0a 2020 2020 2020 2020  arams={.        
+00011850: 2020 2020 2766 726f 6d27 3a20 5f70 7562      'from': _pub
+00011860: 6c69 635f 6b65 792c 0a20 2020 2020 2020  lic_key,.       
+00011870: 2020 2020 2027 7661 6c75 6527 3a20 302c       'value': 0,
+00011880: 0a20 2020 2020 2020 2020 2020 2027 6e6f  .            'no
+00011890: 6e63 6527 3a20 5f6e 6f6e 6365 2c0a 2020  nce': _nonce,.  
+000118a0: 2020 2020 2020 2020 2020 2774 7970 6527            'type'
+000118b0: 3a20 2730 7832 270a 2020 2020 2020 2020  : '0x2'.        
+000118c0: 7d0a 2020 2020 2020 2020 7472 616e 7361  }.        transa
+000118d0: 6374 696f 6e3d 7377 6170 5f66 756e 6374  ction=swap_funct
+000118e0: 696f 6e2e 6275 696c 6454 7261 6e73 6163  ion.buildTransac
+000118f0: 7469 6f6e 2874 785f 7061 7261 6d73 290a  tion(tx_params).
+00011900: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
+00011910: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
+00011920: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
+00011930: 6e5f 7472 616e 7361 6374 696f 6e28 7472  n_transaction(tr
+00011940: 616e 7361 6374 696f 6e2c 2070 7269 7661  ansaction, priva
+00011950: 7465 5f6b 6579 3d5f 7072 6976 6174 655f  te_key=_private_
+00011960: 6b65 7929 0a20 2020 2020 2020 2072 6574  key).        ret
+00011970: 7572 6e20 5f77 6562 332e 746f 4865 7828  urn _web3.toHex(
+00011980: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
+00011990: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
+000119a0: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
+000119b0: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
+000119c0: 2929 0a0a 2020 2020 2320 7374 7275 6374  ))..    # struct
+000119d0: 2045 7861 6374 496e 7075 7450 6172 616d   ExactInputParam
+000119e0: 7320 7b0a 2020 2020 2320 2020 2020 6279  s {.    #     by
+000119f0: 7465 7320 7061 7468 3b0a 2020 2020 2320  tes path;.    # 
+00011a00: 2020 2020 6164 6472 6573 7320 7265 6369      address reci
+00011a10: 7069 656e 743b 0a20 2020 2023 2020 2020  pient;.    #    
+00011a20: 2075 696e 7432 3536 2064 6561 646c 696e   uint256 deadlin
+00011a30: 653b 0a20 2020 2023 2020 2020 2075 696e  e;.    #     uin
+00011a40: 7432 3536 2061 6d6f 756e 7449 6e3b 0a20  t256 amountIn;. 
+00011a50: 2020 2023 2020 2020 2075 696e 7432 3536     #     uint256
+00011a60: 2061 6d6f 756e 744f 7574 4d69 6e69 6d75   amountOutMinimu
+00011a70: 6d3b 0a20 2020 2023 207d 0a20 2020 2064  m;.    # }.    d
+00011a80: 6566 2065 7861 6374 496e 7075 7428 5f77  ef exactInput(_w
+00011a90: 6562 333a 5765 6233 2c5f 726f 7574 655f  eb3:Web3,_route_
+00011aa0: 6164 6472 6573 732c 5f61 6269 2c5f 6e6f  address,_abi,_no
+00011ab0: 6e63 652c 5f70 7562 6c69 635f 6b65 792c  nce,_public_key,
+00011ac0: 5f70 7269 7661 7465 5f6b 6579 2c0a 2020  _private_key,.  
+00011ad0: 2020 2020 2020 5f70 6174 682c 5f72 6563        _path,_rec
+00011ae0: 6970 6965 6e74 2c5f 6465 6164 6c69 6e65  ipient,_deadline
+00011af0: 2c5f 616d 6f75 6e74 496e 2c5f 616d 6f75  ,_amountIn,_amou
+00011b00: 6e74 4f75 744d 696e 293a 0a20 2020 2020  ntOutMin):.     
+00011b10: 2020 2072 6f75 7465 5f63 6f6e 7472 6163     route_contrac
+00011b20: 743d 5f77 6562 332e 6574 682e 636f 6e74  t=_web3.eth.cont
+00011b30: 7261 6374 2861 6464 7265 7373 3d5f 726f  ract(address=_ro
+00011b40: 7574 655f 6164 6472 6573 732c 2061 6269  ute_address, abi
+00011b50: 3d5f 6162 6929 0a0a 2020 2020 2020 2020  =_abi)..        
+00011b60: 2320 7479 7065 3d5b 2762 7974 6573 272c  # type=['bytes',
+00011b70: 2761 6464 7265 7373 272c 2775 696e 7432  'address','uint2
+00011b80: 3536 272c 2775 696e 7432 3536 272c 2775  56','uint256','u
+00011b90: 696e 7432 3536 275d 0a20 2020 2020 2020  int256'].       
+00011ba0: 2023 2064 6174 613d 5b5f 7061 7468 2c5f   # data=[_path,_
+00011bb0: 7265 6369 7069 656e 742c 5f64 6561 646c  recipient,_deadl
+00011bc0: 696e 652c 5f61 6d6f 756e 7449 6e2c 5f61  ine,_amountIn,_a
+00011bd0: 6d6f 756e 744f 7574 4d69 6e5d 0a20 2020  mountOutMin].   
+00011be0: 2020 2020 2023 2066 756e 6374 696f 6e5f       # function_
+00011bf0: 7061 7261 6d73 3d65 6e63 6f64 655f 6162  params=encode_ab
+00011c00: 6928 7479 7065 2c64 6174 6129 0a20 2020  i(type,data).   
+00011c10: 2020 2020 2066 756e 6374 696f 6e5f 7061       function_pa
+00011c20: 7261 6d73 3d7b 0a20 2020 2020 2020 2020  rams={.         
+00011c30: 2020 2027 7061 7468 273a 5f70 6174 682c     'path':_path,
+00011c40: 0a20 2020 2020 2020 2020 2020 2027 7265  .            're
+00011c50: 6369 7069 656e 7427 3a5f 7265 6369 7069  cipient':_recipi
+00011c60: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
+00011c70: 2027 6465 6164 6c69 6e65 273a 5f64 6561   'deadline':_dea
+00011c80: 646c 696e 652c 0a20 2020 2020 2020 2020  dline,.         
+00011c90: 2020 2027 616d 6f75 6e74 496e 273a 5f61     'amountIn':_a
+00011ca0: 6d6f 756e 7449 6e2c 0a20 2020 2020 2020  mountIn,.       
+00011cb0: 2020 2020 2027 616d 6f75 6e74 4f75 744d       'amountOutM
+00011cc0: 696e 696d 756d 273a 5f61 6d6f 756e 744f  inimum':_amountO
+00011cd0: 7574 4d69 6e0a 2020 2020 2020 2020 7d0a  utMin.        }.
+00011ce0: 2020 2020 2020 2020 2320 6675 6e63 7469          # functi
+00011cf0: 6f6e 5f70 6172 616d 733d 285f 7061 7468  on_params=(_path
+00011d00: 2c5f 7265 6369 7069 656e 742c 5f64 6561  ,_recipient,_dea
+00011d10: 646c 696e 652c 5f61 6d6f 756e 7449 6e2c  dline,_amountIn,
+00011d20: 5f61 6d6f 756e 744f 7574 4d69 6e29 0a20  _amountOutMin). 
+00011d30: 2020 2020 2020 2073 7761 705f 6675 6e63         swap_func
+00011d40: 7469 6f6e 3d72 6f75 7465 5f63 6f6e 7472  tion=route_contr
+00011d50: 6163 742e 6675 6e63 7469 6f6e 732e 6578  act.functions.ex
+00011d60: 6163 7449 6e70 7574 2866 756e 6374 696f  actInput(functio
+00011d70: 6e5f 7061 7261 6d73 290a 2020 2020 2020  n_params).      
+00011d80: 2020 7478 5f70 6172 616d 733d 7b0a 2020    tx_params={.  
+00011d90: 2020 2020 2020 2020 2020 2766 726f 6d27            'from'
+00011da0: 3a20 5f70 7562 6c69 635f 6b65 792c 0a20  : _public_key,. 
+00011db0: 2020 2020 2020 2020 2020 2027 7661 6c75             'valu
+00011dc0: 6527 3a20 302c 0a20 2020 2020 2020 2020  e': 0,.         
+00011dd0: 2020 2027 6e6f 6e63 6527 3a20 5f6e 6f6e     'nonce': _non
+00011de0: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+00011df0: 2774 7970 6527 3a20 2730 7832 272c 0a20  'type': '0x2',. 
+00011e00: 2020 2020 2020 2020 2020 2023 2027 6761             # 'ga
+00011e10: 7327 3a5f 6761 730a 2020 2020 2020 2020  s':_gas.        
+00011e20: 7d0a 2020 2020 2020 2020 7472 616e 7361  }.        transa
+00011e30: 6374 696f 6e3d 7377 6170 5f66 756e 6374  ction=swap_funct
+00011e40: 696f 6e2e 6275 696c 6454 7261 6e73 6163  ion.buildTransac
+00011e50: 7469 6f6e 2874 785f 7061 7261 6d73 290a  tion(tx_params).
+00011e60: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
+00011e70: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
+00011e80: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
+00011e90: 6e5f 7472 616e 7361 6374 696f 6e28 7472  n_transaction(tr
+00011ea0: 616e 7361 6374 696f 6e2c 2070 7269 7661  ansaction, priva
+00011eb0: 7465 5f6b 6579 3d5f 7072 6976 6174 655f  te_key=_private_
+00011ec0: 6b65 7929 0a20 2020 2020 2020 2072 6574  key).        ret
+00011ed0: 7572 6e20 5f77 6562 332e 746f 4865 7828  urn _web3.toHex(
+00011ee0: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
+00011ef0: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
+00011f00: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
+00011f10: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
+00011f20: 2929 0a0a 2020 2020 2320 7374 7275 6374  ))..    # struct
+00011f30: 2045 7861 6374 4f75 7470 7574 5369 6e67   ExactOutputSing
+00011f40: 6c65 5061 7261 6d73 207b 0a20 2020 2023  leParams {.    #
+00011f50: 2020 2020 2061 6464 7265 7373 2074 6f6b       address tok
+00011f60: 656e 496e 3b0a 2020 2020 2320 2020 2020  enIn;.    #     
+00011f70: 6164 6472 6573 7320 746f 6b65 6e4f 7574  address tokenOut
+00011f80: 3b0a 2020 2020 2320 2020 2020 7569 6e74  ;.    #     uint
+00011f90: 3234 2066 6565 3b0a 2020 2020 2320 2020  24 fee;.    #   
+00011fa0: 2020 6164 6472 6573 7320 7265 6369 7069    address recipi
+00011fb0: 656e 743b 0a20 2020 2023 2020 2020 2075  ent;.    #     u
+00011fc0: 696e 7432 3536 2064 6561 646c 696e 653b  int256 deadline;
+00011fd0: 0a20 2020 2023 2020 2020 2075 696e 7432  .    #     uint2
+00011fe0: 3536 2061 6d6f 756e 744f 7574 3b0a 2020  56 amountOut;.  
+00011ff0: 2020 2320 2020 2020 7569 6e74 3235 3620    #     uint256 
+00012000: 616d 6f75 6e74 496e 4d61 7869 6d75 6d3b  amountInMaximum;
+00012010: 0a20 2020 2023 2020 2020 2075 696e 7431  .    #     uint1
+00012020: 3630 2073 7172 7450 7269 6365 4c69 6d69  60 sqrtPriceLimi
+00012030: 7458 3936 3b0a 2020 2020 2320 7d0a 2020  tX96;.    # }.  
+00012040: 2020 6465 6620 6578 6163 744f 7574 7075    def exactOutpu
+00012050: 7453 696e 676c 6528 5f77 6562 333a 5765  tSingle(_web3:We
+00012060: 6233 2c5f 726f 7574 655f 6164 6472 6573  b3,_route_addres
+00012070: 732c 5f61 6269 2c5f 6e6f 6e63 652c 5f70  s,_abi,_nonce,_p
+00012080: 7562 6c69 635f 6b65 792c 5f70 7269 7661  ublic_key,_priva
+00012090: 7465 5f6b 6579 2c0a 2020 2020 2020 2020  te_key,.        
+000120a0: 5f74 6f6b 656e 5f69 6e2c 5f74 6f6b 656e  _token_in,_token
+000120b0: 5f6f 7574 2c5f 6665 652c 5f72 6563 6970  _out,_fee,_recip
+000120c0: 6965 6e74 2c5f 6465 6164 6c69 6e65 2c5f  ient,_deadline,_
+000120d0: 616d 6f75 6e74 5f6f 7574 2c5f 616d 6f75  amount_out,_amou
+000120e0: 6e74 5f69 6e5f 6d61 782c 5f73 7172 745f  nt_in_max,_sqrt_
+000120f0: 7072 6963 655f 6c69 6d69 7429 3a0a 2020  price_limit):.  
+00012100: 2020 2020 2020 726f 7574 655f 636f 6e74        route_cont
+00012110: 7261 6374 3d5f 7765 6233 2e65 7468 2e63  ract=_web3.eth.c
+00012120: 6f6e 7472 6163 7428 6164 6472 6573 733d  ontract(address=
+00012130: 5f72 6f75 7465 5f61 6464 7265 7373 2c20  _route_address, 
+00012140: 6162 693d 5f61 6269 290a 2020 2020 2020  abi=_abi).      
+00012150: 2020 6675 6e63 7469 6f6e 5f70 6172 616d    function_param
+00012160: 3d7b 0a20 2020 2020 2020 2020 2020 2027  ={.            '
+00012170: 746f 6b65 6e49 6e27 3a5f 746f 6b65 6e5f  tokenIn':_token_
+00012180: 696e 2c0a 2020 2020 2020 2020 2020 2020  in,.            
+00012190: 2774 6f6b 656e 4f75 7427 3a5f 746f 6b65  'tokenOut':_toke
+000121a0: 6e5f 6f75 742c 0a20 2020 2020 2020 2020  n_out,.         
+000121b0: 2020 2027 6665 6527 3a5f 6665 652c 0a20     'fee':_fee,. 
+000121c0: 2020 2020 2020 2020 2020 2027 7265 6369             'reci
+000121d0: 7069 656e 7427 3a5f 7265 6369 7069 656e  pient':_recipien
+000121e0: 742c 0a20 2020 2020 2020 2020 2020 2027  t,.            '
+000121f0: 6465 6164 6c69 6e65 273a 5f64 6561 646c  deadline':_deadl
+00012200: 696e 652c 0a20 2020 2020 2020 2020 2020  ine,.           
+00012210: 2027 616d 6f75 6e74 4f75 7427 3a5f 616d   'amountOut':_am
+00012220: 6f75 6e74 5f6f 7574 2c0a 2020 2020 2020  ount_out,.      
+00012230: 2020 2020 2020 2761 6d6f 756e 7449 6e4d        'amountInM
+00012240: 6178 696d 756d 273a 5f61 6d6f 756e 745f  aximum':_amount_
+00012250: 696e 5f6d 6178 2c0a 2020 2020 2020 2020  in_max,.        
+00012260: 2020 2020 2773 7172 7450 7269 6365 4c69      'sqrtPriceLi
+00012270: 6d69 7458 3936 273a 5f73 7172 745f 7072  mitX96':_sqrt_pr
+00012280: 6963 655f 6c69 6d69 740a 2020 2020 2020  ice_limit.      
+00012290: 2020 7d0a 2020 2020 2020 2020 7377 6170    }.        swap
+000122a0: 5f66 756e 6374 696f 6e3d 726f 7574 655f  _function=route_
+000122b0: 636f 6e74 7261 6374 2e66 756e 6374 696f  contract.functio
+000122c0: 6e73 2e65 7861 6374 4f75 7470 7574 5369  ns.exactOutputSi
+000122d0: 6e67 6c65 2866 756e 6374 696f 6e5f 7061  ngle(function_pa
+000122e0: 7261 6d29 0a20 2020 2020 2020 2074 785f  ram).        tx_
+000122f0: 7061 7261 6d73 3d7b 0a20 2020 2020 2020  params={.       
+00012300: 2020 2020 2027 6672 6f6d 273a 205f 7075       'from': _pu
+00012310: 626c 6963 5f6b 6579 2c0a 2020 2020 2020  blic_key,.      
+00012320: 2020 2020 2020 2776 616c 7565 273a 2030        'value': 0
+00012330: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
+00012340: 6f6e 6365 273a 205f 6e6f 6e63 652c 0a20  once': _nonce,. 
+00012350: 2020 2020 2020 2020 2020 2027 7479 7065             'type
+00012360: 273a 2027 3078 3227 0a20 2020 2020 2020  ': '0x2'.       
+00012370: 207d 0a20 2020 2020 2020 2074 7261 6e73   }.        trans
+00012380: 6163 7469 6f6e 3d73 7761 705f 6675 6e63  action=swap_func
+00012390: 7469 6f6e 2e62 7569 6c64 5472 616e 7361  tion.buildTransa
+000123a0: 6374 696f 6e28 7478 5f70 6172 616d 7329  ction(tx_params)
+000123b0: 0a20 2020 2020 2020 2073 6967 6e65 645f  .        signed_
+000123c0: 7472 616e 7361 6374 696f 6e3d 5f77 6562  transaction=_web
+000123d0: 332e 6574 682e 6163 636f 756e 742e 7369  3.eth.account.si
+000123e0: 676e 5f74 7261 6e73 6163 7469 6f6e 2874  gn_transaction(t
+000123f0: 7261 6e73 6163 7469 6f6e 2c20 7072 6976  ransaction, priv
+00012400: 6174 655f 6b65 793d 5f70 7269 7661 7465  ate_key=_private
+00012410: 5f6b 6579 290a 2020 2020 2020 2020 7265  _key).        re
+00012420: 7475 726e 205f 7765 6233 2e74 6f48 6578  turn _web3.toHex
+00012430: 285f 7765 6233 2e65 7468 2e73 656e 645f  (_web3.eth.send_
+00012440: 7261 775f 7472 616e 7361 6374 696f 6e28  raw_transaction(
+00012450: 7369 676e 6564 5f74 7261 6e73 6163 7469  signed_transacti
+00012460: 6f6e 2e72 6177 5472 616e 7361 6374 696f  on.rawTransactio
+00012470: 6e29 290a 0a0a 2020 2020 2320 7374 7275  n))...    # stru
+00012480: 6374 2045 7861 6374 4f75 7470 7574 5061  ct ExactOutputPa
+00012490: 7261 6d73 207b 0a20 2020 2023 2020 2020  rams {.    #    
+000124a0: 2062 7974 6573 2070 6174 683b 0a20 2020   bytes path;.   
+000124b0: 2023 2020 2020 2061 6464 7265 7373 2072   #     address r
+000124c0: 6563 6970 6965 6e74 3b0a 2020 2020 2320  ecipient;.    # 
+000124d0: 2020 2020 7569 6e74 3235 3620 6465 6164      uint256 dead
+000124e0: 6c69 6e65 3b0a 2020 2020 2320 2020 2020  line;.    #     
+000124f0: 7569 6e74 3235 3620 616d 6f75 6e74 4f75  uint256 amountOu
+00012500: 743b 0a20 2020 2023 2020 2020 2075 696e  t;.    #     uin
+00012510: 7432 3536 2061 6d6f 756e 7449 6e4d 6178  t256 amountInMax
+00012520: 696d 756d 3b0a 2020 2020 2320 7d0a 2020  imum;.    # }.  
+00012530: 2020 6465 6620 6578 6163 744f 7574 7075    def exactOutpu
+00012540: 7428 5f77 6562 333a 5765 6233 2c5f 726f  t(_web3:Web3,_ro
+00012550: 7574 655f 6164 6472 6573 732c 5f61 6269  ute_address,_abi
+00012560: 2c5f 6e6f 6e63 652c 5f70 7562 6c69 635f  ,_nonce,_public_
+00012570: 6b65 792c 5f70 7269 7661 7465 5f6b 6579  key,_private_key
+00012580: 2c0a 2020 2020 2020 2020 5f70 6174 682c  ,.        _path,
+00012590: 5f72 6563 6970 6965 6e74 2c5f 6465 6164  _recipient,_dead
+000125a0: 6c69 6e65 2c5f 616d 6f75 6e74 5f6f 7574  line,_amount_out
+000125b0: 2c5f 616d 6f75 6e74 5f69 6e5f 6d61 7829  ,_amount_in_max)
+000125c0: 3a0a 2020 2020 2020 2020 726f 7574 655f  :.        route_
+000125d0: 636f 6e74 7261 6374 3d5f 7765 6233 2e65  contract=_web3.e
+000125e0: 7468 2e63 6f6e 7472 6163 7428 6164 6472  th.contract(addr
+000125f0: 6573 733d 5f72 6f75 7465 5f61 6464 7265  ess=_route_addre
+00012600: 7373 2c20 6162 693d 5f61 6269 290a 2020  ss, abi=_abi).  
+00012610: 2020 2020 2020 6675 6e63 7469 6f6e 5f70        function_p
+00012620: 6172 616d 3d7b 0a20 2020 2020 2020 2020  aram={.         
+00012630: 2020 2027 7061 7468 273a 5f70 6174 682c     'path':_path,
+00012640: 0a20 2020 2020 2020 2020 2020 2027 7265  .            're
+00012650: 6369 7069 656e 7427 3a5f 7265 6369 7069  cipient':_recipi
+00012660: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
+00012670: 2027 6465 6164 6c69 6e65 273a 5f64 6561   'deadline':_dea
+00012680: 646c 696e 652c 0a20 2020 2020 2020 2020  dline,.         
+00012690: 2020 2027 616d 6f75 6e74 4f75 7427 3a5f     'amountOut':_
+000126a0: 616d 6f75 6e74 5f6f 7574 2c0a 2020 2020  amount_out,.    
+000126b0: 2020 2020 2020 2020 2761 6d6f 756e 7449          'amountI
+000126c0: 6e4d 6178 696d 756d 273a 5f61 6d6f 756e  nMaximum':_amoun
+000126d0: 745f 696e 5f6d 6178 0a20 2020 2020 2020  t_in_max.       
+000126e0: 207d 0a20 2020 2020 2020 2073 7761 705f   }.        swap_
+000126f0: 6675 6e63 7469 6f6e 3d72 6f75 7465 5f63  function=route_c
+00012700: 6f6e 7472 6163 742e 6675 6e63 7469 6f6e  ontract.function
+00012710: 732e 6578 6163 744f 7574 7075 7428 6675  s.exactOutput(fu
+00012720: 6e63 7469 6f6e 5f70 6172 616d 290a 2020  nction_param).  
+00012730: 2020 2020 2020 7478 5f70 6172 616d 733d        tx_params=
+00012740: 7b0a 2020 2020 2020 2020 2020 2020 2766  {.            'f
+00012750: 726f 6d27 3a20 5f70 7562 6c69 635f 6b65  rom': _public_ke
+00012760: 792c 0a20 2020 2020 2020 2020 2020 2027  y,.            '
+00012770: 7661 6c75 6527 3a20 302c 0a20 2020 2020  value': 0,.     
+00012780: 2020 2020 2020 2027 6e6f 6e63 6527 3a20         'nonce': 
+00012790: 5f6e 6f6e 6365 2c0a 2020 2020 2020 2020  _nonce,.        
+000127a0: 2020 2020 2774 7970 6527 3a20 2730 7832      'type': '0x2
+000127b0: 270a 2020 2020 2020 2020 7d0a 2020 2020  '.        }.    
+000127c0: 2020 2020 7472 616e 7361 6374 696f 6e3d      transaction=
+000127d0: 7377 6170 5f66 756e 6374 696f 6e2e 6275  swap_function.bu
+000127e0: 696c 6454 7261 6e73 6163 7469 6f6e 2874  ildTransaction(t
+000127f0: 785f 7061 7261 6d73 290a 2020 2020 2020  x_params).      
+00012800: 2020 7369 676e 6564 5f74 7261 6e73 6163    signed_transac
+00012810: 7469 6f6e 3d5f 7765 6233 2e65 7468 2e61  tion=_web3.eth.a
+00012820: 6363 6f75 6e74 2e73 6967 6e5f 7472 616e  ccount.sign_tran
+00012830: 7361 6374 696f 6e28 7472 616e 7361 6374  saction(transact
+00012840: 696f 6e2c 2070 7269 7661 7465 5f6b 6579  ion, private_key
+00012850: 3d5f 7072 6976 6174 655f 6b65 7929 0a20  =_private_key). 
+00012860: 2020 2020 2020 2072 6574 7572 6e20 5f77         return _w
+00012870: 6562 332e 746f 4865 7828 5f77 6562 332e  eb3.toHex(_web3.
+00012880: 6574 682e 7365 6e64 5f72 6177 5f74 7261  eth.send_raw_tra
+00012890: 6e73 6163 7469 6f6e 2873 6967 6e65 645f  nsaction(signed_
+000128a0: 7472 616e 7361 6374 696f 6e2e 7261 7754  transaction.rawT
+000128b0: 7261 6e73 6163 7469 6f6e 2929 0a63 6c61  ransaction)).cla
+000128c0: 7373 204a 6f65 5632 4661 6374 6f72 793a  ss JoeV2Factory:
+000128d0: 0a20 2020 206a 6f65 5f66 6163 746f 7279  .    joe_factory
+000128e0: 5f76 325f 6162 693d 6a73 6f6e 2e6c 6f61  _v2_abi=json.loa
+000128f0: 6473 2827 5b7b 2269 6e70 7574 7322 3a5b  ds('[{"inputs":[
+00012900: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00012910: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00012920: 3a22 5f66 6565 5265 6369 7069 656e 7422  :"_feeRecipient"
+00012930: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+00012940: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00012950: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00012960: 6d65 223a 225f 666c 6173 684c 6f61 6e46  me":"_flashLoanF
+00012970: 6565 222c 2274 7970 6522 3a22 7569 6e74  ee","type":"uint
+00012980: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
+00012990: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
+000129a0: 6162 6c65 222c 2274 7970 6522 3a22 636f  able","type":"co
+000129b0: 6e73 7472 7563 746f 7222 7d2c 7b22 696e  nstructor"},{"in
+000129c0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+000129d0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+000129e0: 2c22 6e61 6d65 223a 2262 7022 2c22 7479  ,"name":"bp","ty
+000129f0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00012a00: 226e 616d 6522 3a22 4269 6e48 656c 7065  "name":"BinHelpe
+00012a10: 725f 5f42 696e 5374 6570 4f76 6572 666c  r__BinStepOverfl
+00012a20: 6f77 7322 2c22 7479 7065 223a 2265 7272  ows","type":"err
+00012a30: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00012a40: 5d2c 226e 616d 6522 3a22 4269 6e48 656c  ],"name":"BinHel
+00012a50: 7065 725f 5f49 644f 7665 7266 6c6f 7773  per__IdOverflows
+00012a60: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+00012a70: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+00012a80: 6e61 6d65 223a 224c 4246 6163 746f 7279  name":"LBFactory
+00012a90: 5f5f 4164 6472 6573 735a 6572 6f22 2c22  __AddressZero","
+00012aa0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00012ab0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00012ac0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00012ad0: 3536 222c 226e 616d 6522 3a22 6269 6e53  56","name":"binS
+00012ae0: 7465 7022 2c22 7479 7065 223a 2275 696e  tep","type":"uin
+00012af0: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+00012b00: 4c42 4661 6374 6f72 795f 5f42 696e 5374  LBFactory__BinSt
+00012b10: 6570 4861 734e 6f50 7265 7365 7422 2c22  epHasNoPreset","
+00012b20: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00012b30: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00012b40: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00012b50: 3536 222c 226e 616d 6522 3a22 6c6f 7765  56","name":"lowe
+00012b60: 7242 6f75 6e64 222c 2274 7970 6522 3a22  rBound","type":"
+00012b70: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+00012b80: 726e 616c 5479 7065 223a 2275 696e 7431  rnalType":"uint1
+00012b90: 3622 2c22 6e61 6d65 223a 2262 696e 5374  6","name":"binSt
+00012ba0: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
+00012bb0: 3136 227d 2c7b 2269 6e74 6572 6e61 6c54  16"},{"internalT
+00012bc0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00012bd0: 6e61 6d65 223a 2268 6967 6865 7242 6f75  name":"higherBou
+00012be0: 6e64 222c 2274 7970 6522 3a22 7569 6e74  nd","type":"uint
+00012bf0: 3235 3622 7d5d 2c22 6e61 6d65 223a 224c  256"}],"name":"L
+00012c00: 4246 6163 746f 7279 5f5f 4269 6e53 7465  BFactory__BinSte
+00012c10: 7052 6571 7569 7265 6d65 6e74 7342 7265  pRequirementsBre
+00012c20: 6163 6865 6422 2c22 7479 7065 223a 2265  ached","type":"e
+00012c30: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+00012c40: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00012c50: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
+00012c60: 223a 2266 696c 7465 7250 6572 696f 6422  ":"filterPeriod"
+00012c70: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
+00012c80: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00012c90: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
+00012ca0: 223a 2264 6563 6179 5065 7269 6f64 222c  ":"decayPeriod",
+00012cb0: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
+00012cc0: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
+00012cd0: 6f72 795f 5f44 6563 7265 6173 696e 6750  ory__DecreasingP
+00012ce0: 6572 696f 6473 222c 2274 7970 6522 3a22  eriods","type":"
+00012cf0: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00012d00: 223a 5b5d 2c22 6e61 6d65 223a 224c 4246  ":[],"name":"LBF
+00012d10: 6163 746f 7279 5f5f 4661 6374 6f72 794c  actory__FactoryL
+00012d20: 6f63 6b49 7341 6c72 6561 6479 496e 5468  ockIsAlreadyInTh
+00012d30: 6553 616d 6553 7461 7465 222c 2274 7970  eSameState","typ
+00012d40: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+00012d50: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00012d60: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00012d70: 2c22 6e61 6d65 223a 2266 6565 7322 2c22  ,"name":"fees","
+00012d80: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00012d90: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00012da0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00012db0: 223a 226d 6178 4665 6573 222c 2274 7970  ":"maxFees","typ
+00012dc0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+00012dd0: 6e61 6d65 223a 224c 4246 6163 746f 7279  name":"LBFactory
+00012de0: 5f5f 4665 6573 4162 6f76 654d 6178 222c  __FeesAboveMax",
+00012df0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00012e00: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00012e10: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00012e20: 3235 3622 2c22 6e61 6d65 223a 2266 6565  256","name":"fee
+00012e30: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
+00012e40: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+00012e50: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00012e60: 6e61 6d65 223a 226d 6178 4665 6573 222c  name":"maxFees",
+00012e70: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00012e80: 7d5d 2c22 6e61 6d65 223a 224c 4246 6163  }],"name":"LBFac
+00012e90: 746f 7279 5f5f 466c 6173 684c 6f61 6e46  tory__FlashLoanF
+00012ea0: 6565 4162 6f76 654d 6178 222c 2274 7970  eeAboveMax","typ
+00012eb0: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+00012ec0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00012ed0: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+00012ee0: 2c22 6e61 6d65 223a 2275 7365 7222 2c22  ,"name":"user","
+00012ef0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+00012f00: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
+00012f10: 6f72 795f 5f46 756e 6374 696f 6e49 734c  ory__FunctionIsL
+00012f20: 6f63 6b65 6446 6f72 5573 6572 7322 2c22  ockedForUsers","
+00012f30: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00012f40: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
 00012f50: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
 00012f60: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
-00012f70: 6522 3a22 746f 6b65 6e59 222c 2274 7970  e":"tokenY","typ
-00012f80: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-00012f90: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00012fa0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00012fb0: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
-00012fc0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-00012fd0: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
-00012fe0: 4c42 5061 6972 416c 7265 6164 7945 7869  LBPairAlreadyExi
-00012ff0: 7374 7322 2c22 7479 7065 223a 2265 7272  sts","type":"err
-00013000: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-00013010: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
-00013020: 6f72 795f 5f4c 4250 6169 7249 676e 6f72  ory__LBPairIgnor
-00013030: 6564 4973 416c 7265 6164 7949 6e54 6865  edIsAlreadyInThe
-00013040: 5361 6d65 5374 6174 6522 2c22 7479 7065  SameState","type
-00013050: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-00013060: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00013070: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-00013080: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-00013090: 746f 6b65 6e58 222c 2274 7970 6522 3a22  tokenX","type":"
-000130a0: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-000130b0: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-000130c0: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
-000130d0: 6522 3a22 746f 6b65 6e59 222c 2274 7970  e":"tokenY","typ
-000130e0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-000130f0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00013100: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00013110: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
-00013120: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-00013130: 6522 3a22 4c42 4661 6374 6f72 795f 5f4c  e":"LBFactory__L
-00013140: 4250 6169 724e 6f74 4372 6561 7465 6422  BPairNotCreated"
-00013150: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-00013160: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-00013170: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-00013180: 7265 7373 222c 226e 616d 6522 3a22 4c42  ress","name":"LB
-00013190: 5061 6972 496d 706c 656d 656e 7461 7469  PairImplementati
-000131a0: 6f6e 222c 2274 7970 6522 3a22 6164 6472  on","type":"addr
-000131b0: 6573 7322 7d5d 2c22 6e61 6d65 223a 224c  ess"}],"name":"L
-000131c0: 4246 6163 746f 7279 5f5f 4c42 5061 6972  BFactory__LBPair
-000131d0: 5361 6665 7479 4368 6563 6b46 6169 6c65  SafetyCheckFaile
-000131e0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
-000131f0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00012f70: 6522 3a22 746f 6b65 6e22 2c22 7479 7065  e":"token","type
+00012f80: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
+00012f90: 616d 6522 3a22 4c42 4661 6374 6f72 795f  ame":"LBFactory_
+00012fa0: 5f49 6465 6e74 6963 616c 4164 6472 6573  _IdenticalAddres
+00012fb0: 7365 7322 2c22 7479 7065 223a 2265 7272  ses","type":"err
+00012fc0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00012fd0: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
+00012fe0: 6f72 795f 5f49 6d70 6c65 6d65 6e74 6174  ory__Implementat
+00012ff0: 696f 6e4e 6f74 5365 7422 2c22 7479 7065  ionNotSet","type
+00013000: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+00013010: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00013020: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+00013030: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
+00013040: 746f 6b65 6e58 222c 2274 7970 6522 3a22  tokenX","type":"
+00013050: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+00013060: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
+00013070: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
+00013080: 6522 3a22 746f 6b65 6e59 222c 2274 7970  e":"tokenY","typ
+00013090: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+000130a0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000130b0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000130c0: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
+000130d0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+000130e0: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
+000130f0: 4c42 5061 6972 416c 7265 6164 7945 7869  LBPairAlreadyExi
+00013100: 7374 7322 2c22 7479 7065 223a 2265 7272  sts","type":"err
+00013110: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00013120: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
+00013130: 6f72 795f 5f4c 4250 6169 7249 676e 6f72  ory__LBPairIgnor
+00013140: 6564 4973 416c 7265 6164 7949 6e54 6865  edIsAlreadyInThe
+00013150: 5361 6d65 5374 6174 6522 2c22 7479 7065  SameState","type
+00013160: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+00013170: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00013180: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+00013190: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
+000131a0: 746f 6b65 6e58 222c 2274 7970 6522 3a22  tokenX","type":"
+000131b0: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+000131c0: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
+000131d0: 6163 7420 4945 5243 3230 222c 226e 616d  act IERC20","nam
+000131e0: 6522 3a22 746f 6b65 6e59 222c 2274 7970  e":"tokenY","typ
+000131f0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
 00013200: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00013210: 696e 7431 3622 2c22 6e61 6d65 223a 2270  int16","name":"p
-00013220: 726f 746f 636f 6c53 6861 7265 222c 2274  rotocolShare","t
-00013230: 7970 6522 3a22 7569 6e74 3136 227d 2c7b  ype":"uint16"},{
-00013240: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00013250: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00013260: 226d 6178 222c 2274 7970 6522 3a22 7569  "max","type":"ui
-00013270: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-00013280: 224c 4246 6163 746f 7279 5f5f 5072 6f74  "LBFactory__Prot
-00013290: 6f63 6f6c 5368 6172 654f 7665 7266 6c6f  ocolShareOverflo
-000132a0: 7773 222c 2274 7970 6522 3a22 6572 726f  ws","type":"erro
-000132b0: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
-000132c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000132d0: 636f 6e74 7261 6374 2049 4552 4332 3022  contract IERC20"
-000132e0: 2c22 6e61 6d65 223a 2271 756f 7465 4173  ,"name":"quoteAs
-000132f0: 7365 7422 2c22 7479 7065 223a 2261 6464  set","type":"add
-00013300: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
-00013310: 4c42 4661 6374 6f72 795f 5f51 756f 7465  LBFactory__Quote
-00013320: 4173 7365 7441 6c72 6561 6479 5768 6974  AssetAlreadyWhit
-00013330: 656c 6973 7465 6422 2c22 7479 7065 223a  elisted","type":
-00013340: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00013350: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00013360: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
-00013370: 5243 3230 222c 226e 616d 6522 3a22 7175  RC20","name":"qu
-00013380: 6f74 6541 7373 6574 222c 2274 7970 6522  oteAsset","type"
-00013390: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
-000133a0: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
-000133b0: 5175 6f74 6541 7373 6574 4e6f 7457 6869  QuoteAssetNotWhi
-000133c0: 7465 6c69 7374 6564 222c 2274 7970 6522  telisted","type"
-000133d0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-000133e0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-000133f0: 7970 6522 3a22 7569 6e74 3136 222c 226e  ype":"uint16","n
-00013400: 616d 6522 3a22 7265 6475 6374 696f 6e46  ame":"reductionF
-00013410: 6163 746f 7222 2c22 7479 7065 223a 2275  actor","type":"u
-00013420: 696e 7431 3622 7d2c 7b22 696e 7465 726e  int16"},{"intern
-00013430: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00013440: 222c 226e 616d 6522 3a22 6d61 7822 2c22  ","name":"max","
-00013450: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00013460: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
-00013470: 6f72 795f 5f52 6564 7563 7469 6f6e 4661  ory__ReductionFa
-00013480: 6374 6f72 4f76 6572 666c 6f77 7322 2c22  ctorOverflows","
-00013490: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-000134a0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-000134b0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-000134c0: 7373 222c 226e 616d 6522 3a22 6665 6552  ss","name":"feeR
-000134d0: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
-000134e0: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
-000134f0: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
-00013500: 5361 6d65 4665 6552 6563 6970 6965 6e74  SameFeeRecipient
-00013510: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-00013520: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-00013530: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00013540: 6e74 3235 3622 2c22 6e61 6d65 223a 2266  nt256","name":"f
-00013550: 6c61 7368 4c6f 616e 4665 6522 2c22 7479  lashLoanFee","ty
-00013560: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-00013570: 226e 616d 6522 3a22 4c42 4661 6374 6f72  "name":"LBFactor
-00013580: 795f 5f53 616d 6546 6c61 7368 4c6f 616e  y__SameFlashLoan
-00013590: 4665 6522 2c22 7479 7065 223a 2265 7272  Fee","type":"err
-000135a0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-000135b0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-000135c0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-000135d0: 3a22 4c42 5061 6972 496d 706c 656d 656e  :"LBPairImplemen
-000135e0: 7461 7469 6f6e 222c 2274 7970 6522 3a22  tation","type":"
-000135f0: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
-00013600: 223a 224c 4246 6163 746f 7279 5f5f 5361  ":"LBFactory__Sa
-00013610: 6d65 496d 706c 656d 656e 7461 7469 6f6e  meImplementation
+00013210: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00013220: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
+00013230: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+00013240: 6522 3a22 4c42 4661 6374 6f72 795f 5f4c  e":"LBFactory__L
+00013250: 4250 6169 724e 6f74 4372 6561 7465 6422  BPairNotCreated"
+00013260: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+00013270: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00013280: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+00013290: 7265 7373 222c 226e 616d 6522 3a22 4c42  ress","name":"LB
+000132a0: 5061 6972 496d 706c 656d 656e 7461 7469  PairImplementati
+000132b0: 6f6e 222c 2274 7970 6522 3a22 6164 6472  on","type":"addr
+000132c0: 6573 7322 7d5d 2c22 6e61 6d65 223a 224c  ess"}],"name":"L
+000132d0: 4246 6163 746f 7279 5f5f 4c42 5061 6972  BFactory__LBPair
+000132e0: 5361 6665 7479 4368 6563 6b46 6169 6c65  SafetyCheckFaile
+000132f0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
+00013300: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00013310: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00013320: 696e 7431 3622 2c22 6e61 6d65 223a 2270  int16","name":"p
+00013330: 726f 746f 636f 6c53 6861 7265 222c 2274  rotocolShare","t
+00013340: 7970 6522 3a22 7569 6e74 3136 227d 2c7b  ype":"uint16"},{
+00013350: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00013360: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00013370: 226d 6178 222c 2274 7970 6522 3a22 7569  "max","type":"ui
+00013380: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+00013390: 224c 4246 6163 746f 7279 5f5f 5072 6f74  "LBFactory__Prot
+000133a0: 6f63 6f6c 5368 6172 654f 7665 7266 6c6f  ocolShareOverflo
+000133b0: 7773 222c 2274 7970 6522 3a22 6572 726f  ws","type":"erro
+000133c0: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
+000133d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000133e0: 636f 6e74 7261 6374 2049 4552 4332 3022  contract IERC20"
+000133f0: 2c22 6e61 6d65 223a 2271 756f 7465 4173  ,"name":"quoteAs
+00013400: 7365 7422 2c22 7479 7065 223a 2261 6464  set","type":"add
+00013410: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
+00013420: 4c42 4661 6374 6f72 795f 5f51 756f 7465  LBFactory__Quote
+00013430: 4173 7365 7441 6c72 6561 6479 5768 6974  AssetAlreadyWhit
+00013440: 656c 6973 7465 6422 2c22 7479 7065 223a  elisted","type":
+00013450: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00013460: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00013470: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
+00013480: 5243 3230 222c 226e 616d 6522 3a22 7175  RC20","name":"qu
+00013490: 6f74 6541 7373 6574 222c 2274 7970 6522  oteAsset","type"
+000134a0: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
+000134b0: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
+000134c0: 5175 6f74 6541 7373 6574 4e6f 7457 6869  QuoteAssetNotWhi
+000134d0: 7465 6c69 7374 6564 222c 2274 7970 6522  telisted","type"
+000134e0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+000134f0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00013500: 7970 6522 3a22 7569 6e74 3136 222c 226e  ype":"uint16","n
+00013510: 616d 6522 3a22 7265 6475 6374 696f 6e46  ame":"reductionF
+00013520: 6163 746f 7222 2c22 7479 7065 223a 2275  actor","type":"u
+00013530: 696e 7431 3622 7d2c 7b22 696e 7465 726e  int16"},{"intern
+00013540: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00013550: 222c 226e 616d 6522 3a22 6d61 7822 2c22  ","name":"max","
+00013560: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00013570: 5d2c 226e 616d 6522 3a22 4c42 4661 6374  ],"name":"LBFact
+00013580: 6f72 795f 5f52 6564 7563 7469 6f6e 4661  ory__ReductionFa
+00013590: 6374 6f72 4f76 6572 666c 6f77 7322 2c22  ctorOverflows","
+000135a0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+000135b0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+000135c0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+000135d0: 7373 222c 226e 616d 6522 3a22 6665 6552  ss","name":"feeR
+000135e0: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
+000135f0: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
+00013600: 6d65 223a 224c 4246 6163 746f 7279 5f5f  me":"LBFactory__
+00013610: 5361 6d65 4665 6552 6563 6970 6965 6e74  SameFeeRecipient
 00013620: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
 00013630: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
 00013640: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00013650: 6e74 3235 3622 2c22 6e61 6d65 223a 2278  nt256","name":"x
-00013660: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00013670: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00013680: 7065 223a 2269 6e74 3235 3622 2c22 6e61  pe":"int256","na
-00013690: 6d65 223a 2279 222c 2274 7970 6522 3a22  me":"y","type":"
-000136a0: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-000136b0: 3a22 4d61 7468 3132 3878 3132 385f 5f50  :"Math128x128__P
-000136c0: 6f77 6572 556e 6465 7266 6c6f 7722 2c22  owerUnderflow","
-000136d0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-000136e0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-000136f0: 6522 3a22 5065 6e64 696e 674f 776e 6162  e":"PendingOwnab
-00013700: 6c65 5f5f 4164 6472 6573 735a 6572 6f22  le__AddressZero"
-00013710: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-00013720: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-00013730: 616d 6522 3a22 5065 6e64 696e 674f 776e  ame":"PendingOwn
-00013740: 6162 6c65 5f5f 4e6f 5065 6e64 696e 674f  able__NoPendingO
-00013750: 776e 6572 222c 2274 7970 6522 3a22 6572  wner","type":"er
-00013760: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
-00013770: 5b5d 2c22 6e61 6d65 223a 2250 656e 6469  [],"name":"Pendi
-00013780: 6e67 4f77 6e61 626c 655f 5f4e 6f74 4f77  ngOwnable__NotOw
-00013790: 6e65 7222 2c22 7479 7065 223a 2265 7272  ner","type":"err
-000137a0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-000137b0: 5d2c 226e 616d 6522 3a22 5065 6e64 696e  ],"name":"Pendin
-000137c0: 674f 776e 6162 6c65 5f5f 4e6f 7450 656e  gOwnable__NotPen
-000137d0: 6469 6e67 4f77 6e65 7222 2c22 7479 7065  dingOwner","type
-000137e0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-000137f0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-00013800: 5065 6e64 696e 674f 776e 6162 6c65 5f5f  PendingOwnable__
-00013810: 5065 6e64 696e 674f 776e 6572 416c 7265  PendingOwnerAlre
-00013820: 6164 7953 6574 222c 2274 7970 6522 3a22  adySet","type":"
-00013830: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00013840: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00013850: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00013860: 6d65 223a 2278 222c 2274 7970 6522 3a22  me":"x","type":"
-00013870: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
-00013880: 223a 2253 6166 6543 6173 745f 5f45 7863  ":"SafeCast__Exc
-00013890: 6565 6473 3136 4269 7473 222c 2274 7970  eeds16Bits","typ
-000138a0: 6522 3a22 6572 726f 7222 7d2c 7b22 616e  e":"error"},{"an
-000138b0: 6f6e 796d 6f75 7322 3a66 616c 7365 2c22  onymous":false,"
-000138c0: 696e 7075 7473 223a 5b7b 2269 6e64 6578  inputs":[{"index
-000138d0: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
-000138e0: 6e61 6c54 7970 6522 3a22 626f 6f6c 222c  nalType":"bool",
-000138f0: 226e 616d 6522 3a22 756e 6c6f 636b 6564  "name":"unlocked
-00013900: 222c 2274 7970 6522 3a22 626f 6f6c 227d  ","type":"bool"}
-00013910: 5d2c 226e 616d 6522 3a22 4661 6374 6f72  ],"name":"Factor
-00013920: 794c 6f63 6b65 6453 7461 7475 7355 7064  yLockedStatusUpd
-00013930: 6174 6564 222c 2274 7970 6522 3a22 6576  ated","type":"ev
-00013940: 656e 7422 7d2c 7b22 616e 6f6e 796d 6f75  ent"},{"anonymou
-00013950: 7322 3a66 616c 7365 2c22 696e 7075 7473  s":false,"inputs
-00013960: 223a 5b7b 2269 6e64 6578 6564 223a 7472  ":[{"indexed":tr
-00013970: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
-00013980: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-00013990: 6522 3a22 7365 6e64 6572 222c 2274 7970  e":"sender","typ
-000139a0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-000139b0: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
-000139c0: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
-000139d0: 6e74 7261 6374 2049 4c42 5061 6972 222c  ntract ILBPair",
-000139e0: 226e 616d 6522 3a22 4c42 5061 6972 222c  "name":"LBPair",
-000139f0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-00013a00: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-00013a10: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-00013a20: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00013a30: 6522 3a22 6269 6e53 7465 7022 2c22 7479  e":"binStep","ty
-00013a40: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-00013a50: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
-00013a60: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00013a70: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00013a80: 2262 6173 6546 6163 746f 7222 2c22 7479  "baseFactor","ty
-00013a90: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-00013aa0: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
-00013ab0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00013ac0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00013ad0: 2266 696c 7465 7250 6572 696f 6422 2c22  "filterPeriod","
-00013ae0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00013af0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-00013b00: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-00013b10: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00013b20: 223a 2264 6563 6179 5065 7269 6f64 222c  ":"decayPeriod",
-00013b30: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00013b40: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-00013b50: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-00013b60: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00013b70: 6522 3a22 7265 6475 6374 696f 6e46 6163  e":"reductionFac
-00013b80: 746f 7222 2c22 7479 7065 223a 2275 696e  tor","type":"uin
-00013b90: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
-00013ba0: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
-00013bb0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00013bc0: 2c22 6e61 6d65 223a 2276 6172 6961 626c  ,"name":"variabl
-00013bd0: 6546 6565 436f 6e74 726f 6c22 2c22 7479  eFeeControl","ty
-00013be0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-00013bf0: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
-00013c00: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00013c10: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00013c20: 2270 726f 746f 636f 6c53 6861 7265 222c  "protocolShare",
-00013c30: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00013c40: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-00013c50: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-00013c60: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00013c70: 6522 3a22 6d61 7856 6f6c 6174 696c 6974  e":"maxVolatilit
-00013c80: 7941 6363 756d 756c 6174 6564 222c 2274  yAccumulated","t
-00013c90: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-00013ca0: 2c22 6e61 6d65 223a 2246 6565 5061 7261  ,"name":"FeePara
-00013cb0: 6d65 7465 7273 5365 7422 2c22 7479 7065  metersSet","type
-00013cc0: 223a 2265 7665 6e74 227d 2c7b 2261 6e6f  ":"event"},{"ano
-00013cd0: 6e79 6d6f 7573 223a 6661 6c73 652c 2269  nymous":false,"i
-00013ce0: 6e70 7574 7322 3a5b 7b22 696e 6465 7865  nputs":[{"indexe
-00013cf0: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
-00013d00: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-00013d10: 222c 226e 616d 6522 3a22 6f6c 6452 6563  ","name":"oldRec
-00013d20: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
-00013d30: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
-00013d40: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-00013d50: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-00013d60: 7373 222c 226e 616d 6522 3a22 6e65 7752  ss","name":"newR
-00013d70: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
-00013d80: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
-00013d90: 6d65 223a 2246 6565 5265 6369 7069 656e  me":"FeeRecipien
-00013da0: 7453 6574 222c 2274 7970 6522 3a22 6576  tSet","type":"ev
-00013db0: 656e 7422 7d2c 7b22 616e 6f6e 796d 6f75  ent"},{"anonymou
-00013dc0: 7322 3a66 616c 7365 2c22 696e 7075 7473  s":false,"inputs
-00013dd0: 223a 5b7b 2269 6e64 6578 6564 223a 6661  ":[{"indexed":fa
-00013de0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
-00013df0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00013e00: 6d65 223a 226f 6c64 466c 6173 684c 6f61  me":"oldFlashLoa
-00013e10: 6e46 6565 222c 2274 7970 6522 3a22 7569  nFee","type":"ui
-00013e20: 6e74 3235 3622 7d2c 7b22 696e 6465 7865  nt256"},{"indexe
-00013e30: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
-00013e40: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00013e50: 222c 226e 616d 6522 3a22 6e65 7746 6c61  ","name":"newFla
-00013e60: 7368 4c6f 616e 4665 6522 2c22 7479 7065  shLoanFee","type
-00013e70: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-00013e80: 616d 6522 3a22 466c 6173 684c 6f61 6e46  ame":"FlashLoanF
-00013e90: 6565 5365 7422 2c22 7479 7065 223a 2265  eeSet","type":"e
-00013ea0: 7665 6e74 227d 2c7b 2261 6e6f 6e79 6d6f  vent"},{"anonymo
-00013eb0: 7573 223a 6661 6c73 652c 2269 6e70 7574  us":false,"input
-00013ec0: 7322 3a5b 7b22 696e 6465 7865 6422 3a74  s":[{"indexed":t
-00013ed0: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
-00013ee0: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-00013ef0: 4332 3022 2c22 6e61 6d65 223a 2274 6f6b  C20","name":"tok
-00013f00: 656e 5822 2c22 7479 7065 223a 2261 6464  enX","type":"add
-00013f10: 7265 7373 227d 2c7b 2269 6e64 6578 6564  ress"},{"indexed
-00013f20: 223a 7472 7565 2c22 696e 7465 726e 616c  ":true,"internal
-00013f30: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-00013f40: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-00013f50: 746f 6b65 6e59 222c 2274 7970 6522 3a22  tokenY","type":"
-00013f60: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
-00013f70: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
-00013f80: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00013f90: 3622 2c22 6e61 6d65 223a 2262 696e 5374  6","name":"binSt
-00013fa0: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
-00013fb0: 3235 3622 7d2c 7b22 696e 6465 7865 6422  256"},{"indexed"
-00013fc0: 3a66 616c 7365 2c22 696e 7465 726e 616c  :false,"internal
-00013fd0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-00013fe0: 494c 4250 6169 7222 2c22 6e61 6d65 223a  ILBPair","name":
-00013ff0: 224c 4250 6169 7222 2c22 7479 7065 223a  "LBPair","type":
-00014000: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
-00014010: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-00014020: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00014030: 3235 3622 2c22 6e61 6d65 223a 2270 6964  256","name":"pid
-00014040: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00014050: 3622 7d5d 2c22 6e61 6d65 223a 224c 4250  6"}],"name":"LBP
-00014060: 6169 7243 7265 6174 6564 222c 2274 7970  airCreated","typ
-00014070: 6522 3a22 6576 656e 7422 7d2c 7b22 616e  e":"event"},{"an
-00014080: 6f6e 796d 6f75 7322 3a66 616c 7365 2c22  onymous":false,"
-00014090: 696e 7075 7473 223a 5b7b 2269 6e64 6578  inputs":[{"index
-000140a0: 6564 223a 7472 7565 2c22 696e 7465 726e  ed":true,"intern
-000140b0: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-000140c0: 7420 494c 4250 6169 7222 2c22 6e61 6d65  t ILBPair","name
-000140d0: 223a 224c 4250 6169 7222 2c22 7479 7065  ":"LBPair","type
-000140e0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-000140f0: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
-00014100: 6e74 6572 6e61 6c54 7970 6522 3a22 626f  nternalType":"bo
-00014110: 6f6c 222c 226e 616d 6522 3a22 6967 6e6f  ol","name":"igno
-00014120: 7265 6422 2c22 7479 7065 223a 2262 6f6f  red","type":"boo
-00014130: 6c22 7d5d 2c22 6e61 6d65 223a 224c 4250  l"}],"name":"LBP
-00014140: 6169 7249 676e 6f72 6564 5374 6174 6543  airIgnoredStateC
-00014150: 6861 6e67 6564 222c 2274 7970 6522 3a22  hanged","type":"
-00014160: 6576 656e 7422 7d2c 7b22 616e 6f6e 796d  event"},{"anonym
-00014170: 6f75 7322 3a66 616c 7365 2c22 696e 7075  ous":false,"inpu
-00014180: 7473 223a 5b7b 2269 6e64 6578 6564 223a  ts":[{"indexed":
-00014190: 6661 6c73 652c 2269 6e74 6572 6e61 6c54  false,"internalT
-000141a0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-000141b0: 6e61 6d65 223a 226f 6c64 4c42 5061 6972  name":"oldLBPair
-000141c0: 496d 706c 656d 656e 7461 7469 6f6e 222c  Implementation",
-000141d0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-000141e0: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-000141f0: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-00014200: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-00014210: 6522 3a22 4c42 5061 6972 496d 706c 656d  e":"LBPairImplem
-00014220: 656e 7461 7469 6f6e 222c 2274 7970 6522  entation","type"
-00014230: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
-00014240: 6d65 223a 224c 4250 6169 7249 6d70 6c65  me":"LBPairImple
-00014250: 6d65 6e74 6174 696f 6e53 6574 222c 2274  mentationSet","t
-00014260: 7970 6522 3a22 6576 656e 7422 7d2c 7b22  ype":"event"},{"
-00014270: 616e 6f6e 796d 6f75 7322 3a66 616c 7365  anonymous":false
-00014280: 2c22 696e 7075 7473 223a 5b7b 2269 6e64  ,"inputs":[{"ind
-00014290: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
-000142a0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-000142b0: 7373 222c 226e 616d 6522 3a22 7072 6576  ss","name":"prev
-000142c0: 696f 7573 4f77 6e65 7222 2c22 7479 7065  iousOwner","type
-000142d0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-000142e0: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
-000142f0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-00014300: 7265 7373 222c 226e 616d 6522 3a22 6e65  ress","name":"ne
-00014310: 774f 776e 6572 222c 2274 7970 6522 3a22  wOwner","type":"
-00014320: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
-00014330: 223a 224f 776e 6572 7368 6970 5472 616e  ":"OwnershipTran
-00014340: 7366 6572 7265 6422 2c22 7479 7065 223a  sferred","type":
-00014350: 2265 7665 6e74 227d 2c7b 2261 6e6f 6e79  "event"},{"anony
-00014360: 6d6f 7573 223a 6661 6c73 652c 2269 6e70  mous":false,"inp
-00014370: 7574 7322 3a5b 7b22 696e 6465 7865 6422  uts":[{"indexed"
-00014380: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
-00014390: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-000143a0: 6e61 6d65 223a 2270 656e 6469 6e67 4f77  name":"pendingOw
-000143b0: 6e65 7222 2c22 7479 7065 223a 2261 6464  ner","type":"add
-000143c0: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
-000143d0: 5065 6e64 696e 674f 776e 6572 5365 7422  PendingOwnerSet"
-000143e0: 2c22 7479 7065 223a 2265 7665 6e74 227d  ,"type":"event"}
-000143f0: 2c7b 2261 6e6f 6e79 6d6f 7573 223a 6661  ,{"anonymous":fa
-00014400: 6c73 652c 2269 6e70 7574 7322 3a5b 7b22  lse,"inputs":[{"
-00014410: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
-00014420: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00014430: 6e74 3235 3622 2c22 6e61 6d65 223a 2262  nt256","name":"b
-00014440: 696e 5374 6570 222c 2274 7970 6522 3a22  inStep","type":"
-00014450: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
-00014460: 223a 2250 7265 7365 7452 656d 6f76 6564  ":"PresetRemoved
-00014470: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
-00014480: 7d2c 7b22 616e 6f6e 796d 6f75 7322 3a66  },{"anonymous":f
-00014490: 616c 7365 2c22 696e 7075 7473 223a 5b7b  alse,"inputs":[{
-000144a0: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
-000144b0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-000144c0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-000144d0: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
-000144e0: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
-000144f0: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-00014500: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00014510: 3235 3622 2c22 6e61 6d65 223a 2262 6173  256","name":"bas
-00014520: 6546 6163 746f 7222 2c22 7479 7065 223a  eFactor","type":
-00014530: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
-00014540: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-00014550: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00014560: 3235 3622 2c22 6e61 6d65 223a 2266 696c  256","name":"fil
-00014570: 7465 7250 6572 696f 6422 2c22 7479 7065  terPeriod","type
-00014580: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-00014590: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
-000145a0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-000145b0: 6e74 3235 3622 2c22 6e61 6d65 223a 2264  nt256","name":"d
-000145c0: 6563 6179 5065 7269 6f64 222c 2274 7970  ecayPeriod","typ
-000145d0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-000145e0: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
-000145f0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00014600: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00014610: 7265 6475 6374 696f 6e46 6163 746f 7222  reductionFactor"
-00014620: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00014630: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
-00014640: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
-00014650: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00014660: 6d65 223a 2276 6172 6961 626c 6546 6565  me":"variableFee
-00014670: 436f 6e74 726f 6c22 2c22 7479 7065 223a  Control","type":
-00014680: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
-00014690: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-000146a0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-000146b0: 3235 3622 2c22 6e61 6d65 223a 2270 726f  256","name":"pro
-000146c0: 746f 636f 6c53 6861 7265 222c 2274 7970  tocolShare","typ
-000146d0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-000146e0: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
-000146f0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00014700: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00014710: 6d61 7856 6f6c 6174 696c 6974 7941 6363  maxVolatilityAcc
-00014720: 756d 756c 6174 6564 222c 2274 7970 6522  umulated","type"
-00014730: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-00014740: 6465 7865 6422 3a66 616c 7365 2c22 696e  dexed":false,"in
-00014750: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00014760: 7432 3536 222c 226e 616d 6522 3a22 7361  t256","name":"sa
-00014770: 6d70 6c65 4c69 6665 7469 6d65 222c 2274  mpleLifetime","t
-00014780: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-00014790: 2c22 6e61 6d65 223a 2250 7265 7365 7453  ,"name":"PresetS
-000147a0: 6574 222c 2274 7970 6522 3a22 6576 656e  et","type":"even
-000147b0: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
-000147c0: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
-000147d0: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
-000147e0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-000147f0: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
-00014800: 222c 226e 616d 6522 3a22 7175 6f74 6541  ","name":"quoteA
-00014810: 7373 6574 222c 2274 7970 6522 3a22 6164  sset","type":"ad
-00014820: 6472 6573 7322 7d5d 2c22 6e61 6d65 223a  dress"}],"name":
-00014830: 2251 756f 7465 4173 7365 7441 6464 6564  "QuoteAssetAdded
-00014840: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
-00014850: 7d2c 7b22 616e 6f6e 796d 6f75 7322 3a66  },{"anonymous":f
-00014860: 616c 7365 2c22 696e 7075 7473 223a 5b7b  alse,"inputs":[{
-00014870: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
-00014880: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-00014890: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
-000148a0: 226e 616d 6522 3a22 7175 6f74 6541 7373  "name":"quoteAss
-000148b0: 6574 222c 2274 7970 6522 3a22 6164 6472  et","type":"addr
-000148c0: 6573 7322 7d5d 2c22 6e61 6d65 223a 2251  ess"}],"name":"Q
-000148d0: 756f 7465 4173 7365 7452 656d 6f76 6564  uoteAssetRemoved
-000148e0: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
-000148f0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-00014900: 6e61 6d65 223a 224c 4250 6169 7249 6d70  name":"LBPairImp
-00014910: 6c65 6d65 6e74 6174 696f 6e22 2c22 6f75  lementation","ou
-00014920: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-00014930: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-00014940: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-00014950: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-00014960: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00014970: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-00014980: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00014990: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-000149a0: 4d41 585f 4249 4e5f 5354 4550 222c 226f  MAX_BIN_STEP","o
-000149b0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-000149c0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-000149d0: 3622 2c22 6e61 6d65 223a 2222 2c22 7479  6","name":"","ty
-000149e0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-000149f0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00014a00: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-00014a10: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00014a20: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-00014a30: 224d 4158 5f46 4545 222c 226f 7574 7075  "MAX_FEE","outpu
-00014a40: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00014a50: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00014a60: 6e61 6d65 223a 2222 2c22 7479 7065 223a  name":"","type":
-00014a70: 2275 696e 7432 3536 227d 5d2c 2273 7461  "uint256"}],"sta
-00014a80: 7465 4d75 7461 6269 6c69 7479 223a 2276  teMutability":"v
-00014a90: 6965 7722 2c22 7479 7065 223a 2266 756e  iew","type":"fun
-00014aa0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-00014ab0: 223a 5b5d 2c22 6e61 6d65 223a 224d 4158  ":[],"name":"MAX
-00014ac0: 5f50 524f 544f 434f 4c5f 5348 4152 4522  _PROTOCOL_SHARE"
-00014ad0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-00014ae0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00014af0: 7432 3536 222c 226e 616d 6522 3a22 222c  t256","name":"",
-00014b00: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00014b10: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
-00014b20: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
-00014b30: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00014b40: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00014b50: 6522 3a22 4d49 4e5f 4249 4e5f 5354 4550  e":"MIN_BIN_STEP
-00014b60: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
-00014b70: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00014b80: 6e74 3235 3622 2c22 6e61 6d65 223a 2222  nt256","name":""
-00014b90: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00014ba0: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
-00014bb0: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
-00014bc0: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-00014bd0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-00014be0: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-00014bf0: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
-00014c00: 6d65 223a 225f 7175 6f74 6541 7373 6574  me":"_quoteAsset
-00014c10: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00014c20: 7322 7d5d 2c22 6e61 6d65 223a 2261 6464  s"}],"name":"add
-00014c30: 5175 6f74 6541 7373 6574 222c 226f 7574  QuoteAsset","out
-00014c40: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
-00014c50: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-00014c60: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-00014c70: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00014c80: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00014c90: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00014ca0: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
-00014cb0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-00014cc0: 6d65 223a 2261 6c6c 4c42 5061 6972 7322  me":"allLBPairs"
-00014cd0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-00014ce0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
-00014cf0: 7472 6163 7420 494c 4250 6169 7222 2c22  tract ILBPair","
-00014d00: 6e61 6d65 223a 2222 2c22 7479 7065 223a  name":"","type":
-00014d10: 2261 6464 7265 7373 227d 5d2c 2273 7461  "address"}],"sta
-00014d20: 7465 4d75 7461 6269 6c69 7479 223a 2276  teMutability":"v
-00014d30: 6965 7722 2c22 7479 7065 223a 2266 756e  iew","type":"fun
-00014d40: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-00014d50: 223a 5b5d 2c22 6e61 6d65 223a 2262 6563  ":[],"name":"bec
-00014d60: 6f6d 654f 776e 6572 222c 226f 7574 7075  omeOwner","outpu
-00014d70: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
-00014d80: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
-00014d90: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
-00014da0: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-00014db0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00014dc0: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
-00014dd0: 5243 3230 222c 226e 616d 6522 3a22 5f74  RC20","name":"_t
-00014de0: 6f6b 656e 5822 2c22 7479 7065 223a 2261  okenX","type":"a
-00014df0: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-00014e00: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
-00014e10: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
-00014e20: 223a 225f 746f 6b65 6e59 222c 2274 7970  ":"_tokenY","typ
-00014e30: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-00014e40: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00014e50: 696e 7432 3422 2c22 6e61 6d65 223a 225f  int24","name":"_
-00014e60: 6163 7469 7665 4964 222c 2274 7970 6522  activeId","type"
-00014e70: 3a22 7569 6e74 3234 227d 2c7b 2269 6e74  :"uint24"},{"int
-00014e80: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00014e90: 3136 222c 226e 616d 6522 3a22 5f62 696e  16","name":"_bin
-00014ea0: 5374 6570 222c 2274 7970 6522 3a22 7569  Step","type":"ui
-00014eb0: 6e74 3136 227d 5d2c 226e 616d 6522 3a22  nt16"}],"name":"
-00014ec0: 6372 6561 7465 4c42 5061 6972 222c 226f  createLBPair","o
-00014ed0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-00014ee0: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
-00014ef0: 6374 2049 4c42 5061 6972 222c 226e 616d  ct ILBPair","nam
-00014f00: 6522 3a22 5f4c 4250 6169 7222 2c22 7479  e":"_LBPair","ty
-00014f10: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
-00014f20: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00014f30: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
-00014f40: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00014f50: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-00014f60: 6e61 6d65 223a 2263 7265 6174 696f 6e55  name":"creationU
-00014f70: 6e6c 6f63 6b65 6422 2c22 6f75 7470 7574  nlocked","output
-00014f80: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00014f90: 7065 223a 2262 6f6f 6c22 2c22 6e61 6d65  pe":"bool","name
-00014fa0: 223a 2222 2c22 7479 7065 223a 2262 6f6f  ":"","type":"boo
-00014fb0: 6c22 7d5d 2c22 7374 6174 654d 7574 6162  l"}],"stateMutab
-00014fc0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
-00014fd0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00014fe0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-00014ff0: 616d 6522 3a22 6665 6552 6563 6970 6965  ame":"feeRecipie
-00015000: 6e74 222c 226f 7574 7075 7473 223a 5b7b  nt","outputs":[{
-00015010: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00015020: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-00015030: 2222 2c22 7479 7065 223a 2261 6464 7265  "","type":"addre
-00015040: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
-00015050: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
-00015060: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00015070: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-00015080: 6e61 6d65 223a 2266 6c61 7368 4c6f 616e  name":"flashLoan
-00015090: 4665 6522 2c22 6f75 7470 7574 7322 3a5b  Fee","outputs":[
-000150a0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-000150b0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-000150c0: 3a22 222c 2274 7970 6522 3a22 7569 6e74  :"","type":"uint
-000150d0: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
-000150e0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-000150f0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-00015100: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-00015110: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-00015120: 6f6e 7472 6163 7420 494c 4250 6169 7222  ontract ILBPair"
-00015130: 2c22 6e61 6d65 223a 225f 4c42 5061 6972  ,"name":"_LBPair
-00015140: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00015150: 7322 7d5d 2c22 6e61 6d65 223a 2266 6f72  s"}],"name":"for
-00015160: 6365 4465 6361 7922 2c22 6f75 7470 7574  ceDecay","output
-00015170: 7322 3a5b 5d2c 2273 7461 7465 4d75 7461  s":[],"stateMuta
-00015180: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
-00015190: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
-000151a0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
-000151b0: 223a 5b5d 2c22 6e61 6d65 223a 2267 6574  ":[],"name":"get
-000151c0: 416c 6c42 696e 5374 6570 7322 2c22 6f75  AllBinSteps","ou
-000151d0: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-000151e0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-000151f0: 5b5d 222c 226e 616d 6522 3a22 7072 6573  []","name":"pres
-00015200: 6574 7342 696e 5374 6570 222c 2274 7970  etsBinStep","typ
-00015210: 6522 3a22 7569 6e74 3235 365b 5d22 7d5d  e":"uint256[]"}]
-00015220: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00015230: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
-00015240: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00015250: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00015260: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-00015270: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
-00015280: 3a22 5f74 6f6b 656e 5822 2c22 7479 7065  :"_tokenX","type
-00015290: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-000152a0: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
-000152b0: 6e74 7261 6374 2049 4552 4332 3022 2c22  ntract IERC20","
-000152c0: 6e61 6d65 223a 225f 746f 6b65 6e59 222c  name":"_tokenY",
-000152d0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-000152e0: 7d5d 2c22 6e61 6d65 223a 2267 6574 416c  }],"name":"getAl
-000152f0: 6c4c 4250 6169 7273 222c 226f 7574 7075  lLBPairs","outpu
-00015300: 7473 223a 5b7b 2263 6f6d 706f 6e65 6e74  ts":[{"component
-00015310: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00015320: 7065 223a 2275 696e 7431 3622 2c22 6e61  pe":"uint16","na
-00015330: 6d65 223a 2262 696e 5374 6570 222c 2274  me":"binStep","t
-00015340: 7970 6522 3a22 7569 6e74 3136 227d 2c7b  ype":"uint16"},{
-00015350: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00015360: 636f 6e74 7261 6374 2049 4c42 5061 6972  contract ILBPair
-00015370: 222c 226e 616d 6522 3a22 4c42 5061 6972  ","name":"LBPair
-00015380: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00015390: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-000153a0: 7065 223a 2262 6f6f 6c22 2c22 6e61 6d65  pe":"bool","name
-000153b0: 223a 2263 7265 6174 6564 4279 4f77 6e65  ":"createdByOwne
-000153c0: 7222 2c22 7479 7065 223a 2262 6f6f 6c22  r","type":"bool"
-000153d0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-000153e0: 223a 2262 6f6f 6c22 2c22 6e61 6d65 223a  ":"bool","name":
-000153f0: 2269 676e 6f72 6564 466f 7252 6f75 7469  "ignoredForRouti
-00015400: 6e67 222c 2274 7970 6522 3a22 626f 6f6c  ng","type":"bool
-00015410: 227d 5d2c 2269 6e74 6572 6e61 6c54 7970  "}],"internalTyp
-00015420: 6522 3a22 7374 7275 6374 2049 4c42 4661  e":"struct ILBFa
-00015430: 6374 6f72 792e 4c42 5061 6972 496e 666f  ctory.LBPairInfo
-00015440: 726d 6174 696f 6e5b 5d22 2c22 6e61 6d65  rmation[]","name
-00015450: 223a 224c 4250 6169 7273 4176 6169 6c61  ":"LBPairsAvaila
-00015460: 626c 6522 2c22 7479 7065 223a 2274 7570  ble","type":"tup
-00015470: 6c65 5b5d 227d 5d2c 2273 7461 7465 4d75  le[]"}],"stateMu
-00015480: 7461 6269 6c69 7479 223a 2276 6965 7722  tability":"view"
-00015490: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-000154a0: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
-000154b0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000154c0: 636f 6e74 7261 6374 2049 4552 4332 3022  contract IERC20"
-000154d0: 2c22 6e61 6d65 223a 225f 746f 6b65 6e41  ,"name":"_tokenA
-000154e0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-000154f0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-00015500: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
-00015510: 5243 3230 222c 226e 616d 6522 3a22 5f74  RC20","name":"_t
-00015520: 6f6b 656e 4222 2c22 7479 7065 223a 2261  okenB","type":"a
-00015530: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-00015540: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00015550: 3622 2c22 6e61 6d65 223a 225f 6269 6e53  6","name":"_binS
-00015560: 7465 7022 2c22 7479 7065 223a 2275 696e  tep","type":"uin
-00015570: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-00015580: 6765 744c 4250 6169 7249 6e66 6f72 6d61  getLBPairInforma
-00015590: 7469 6f6e 222c 226f 7574 7075 7473 223a  tion","outputs":
-000155a0: 5b7b 2263 6f6d 706f 6e65 6e74 7322 3a5b  [{"components":[
-000155b0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-000155c0: 2275 696e 7431 3622 2c22 6e61 6d65 223a  "uint16","name":
-000155d0: 2262 696e 5374 6570 222c 2274 7970 6522  "binStep","type"
-000155e0: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
-000155f0: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-00015600: 7261 6374 2049 4c42 5061 6972 222c 226e  ract ILBPair","n
-00015610: 616d 6522 3a22 4c42 5061 6972 222c 2274  ame":"LBPair","t
-00015620: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-00015630: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00015640: 2262 6f6f 6c22 2c22 6e61 6d65 223a 2263  "bool","name":"c
-00015650: 7265 6174 6564 4279 4f77 6e65 7222 2c22  reatedByOwner","
-00015660: 7479 7065 223a 2262 6f6f 6c22 7d2c 7b22  type":"bool"},{"
-00015670: 696e 7465 726e 616c 5479 7065 223a 2262  internalType":"b
-00015680: 6f6f 6c22 2c22 6e61 6d65 223a 2269 676e  ool","name":"ign
-00015690: 6f72 6564 466f 7252 6f75 7469 6e67 222c  oredForRouting",
-000156a0: 2274 7970 6522 3a22 626f 6f6c 227d 5d2c  "type":"bool"}],
-000156b0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000156c0: 7374 7275 6374 2049 4c42 4661 6374 6f72  struct ILBFactor
-000156d0: 792e 4c42 5061 6972 496e 666f 726d 6174  y.LBPairInformat
-000156e0: 696f 6e22 2c22 6e61 6d65 223a 2222 2c22  ion","name":"","
-000156f0: 7479 7065 223a 2274 7570 6c65 227d 5d2c  type":"tuple"}],
-00015700: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00015710: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-00015720: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00015730: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-00015740: 2267 6574 4e75 6d62 6572 4f66 4c42 5061  "getNumberOfLBPa
-00015750: 6972 7322 2c22 6f75 7470 7574 7322 3a5b  irs","outputs":[
-00015760: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00015770: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00015780: 3a22 222c 2274 7970 6522 3a22 7569 6e74  :"","type":"uint
-00015790: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
-000157a0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-000157b0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-000157c0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-000157d0: 226e 616d 6522 3a22 6765 744e 756d 6265  "name":"getNumbe
-000157e0: 724f 6651 756f 7465 4173 7365 7473 222c  rOfQuoteAssets",
-000157f0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-00015800: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00015810: 3235 3622 2c22 6e61 6d65 223a 2222 2c22  256","name":"","
-00015820: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00015830: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-00015840: 7479 223a 2276 6965 7722 2c22 7479 7065  ty":"view","type
-00015850: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00015860: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00015870: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
-00015880: 222c 226e 616d 6522 3a22 5f62 696e 5374  ","name":"_binSt
-00015890: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
-000158a0: 3136 227d 5d2c 226e 616d 6522 3a22 6765  16"}],"name":"ge
-000158b0: 7450 7265 7365 7422 2c22 6f75 7470 7574  tPreset","output
-000158c0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-000158d0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-000158e0: 616d 6522 3a22 6261 7365 4661 6374 6f72  ame":"baseFactor
-000158f0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00015900: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00015910: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00015920: 616d 6522 3a22 6669 6c74 6572 5065 7269  ame":"filterPeri
-00015930: 6f64 222c 2274 7970 6522 3a22 7569 6e74  od","type":"uint
-00015940: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-00015950: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00015960: 226e 616d 6522 3a22 6465 6361 7950 6572  "name":"decayPer
-00015970: 696f 6422 2c22 7479 7065 223a 2275 696e  iod","type":"uin
-00015980: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-00015990: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-000159a0: 2c22 6e61 6d65 223a 2272 6564 7563 7469  ,"name":"reducti
-000159b0: 6f6e 4661 6374 6f72 222c 2274 7970 6522  onFactor","type"
-000159c0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-000159d0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-000159e0: 7432 3536 222c 226e 616d 6522 3a22 7661  t256","name":"va
-000159f0: 7269 6162 6c65 4665 6543 6f6e 7472 6f6c  riableFeeControl
+00013650: 6e74 3235 3622 2c22 6e61 6d65 223a 2266  nt256","name":"f
+00013660: 6c61 7368 4c6f 616e 4665 6522 2c22 7479  lashLoanFee","ty
+00013670: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00013680: 226e 616d 6522 3a22 4c42 4661 6374 6f72  "name":"LBFactor
+00013690: 795f 5f53 616d 6546 6c61 7368 4c6f 616e  y__SameFlashLoan
+000136a0: 4665 6522 2c22 7479 7065 223a 2265 7272  Fee","type":"err
+000136b0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+000136c0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000136d0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+000136e0: 3a22 4c42 5061 6972 496d 706c 656d 656e  :"LBPairImplemen
+000136f0: 7461 7469 6f6e 222c 2274 7970 6522 3a22  tation","type":"
+00013700: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+00013710: 223a 224c 4246 6163 746f 7279 5f5f 5361  ":"LBFactory__Sa
+00013720: 6d65 496d 706c 656d 656e 7461 7469 6f6e  meImplementation
+00013730: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+00013740: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00013750: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00013760: 6e74 3235 3622 2c22 6e61 6d65 223a 2278  nt256","name":"x
+00013770: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00013780: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+00013790: 7065 223a 2269 6e74 3235 3622 2c22 6e61  pe":"int256","na
+000137a0: 6d65 223a 2279 222c 2274 7970 6522 3a22  me":"y","type":"
+000137b0: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+000137c0: 3a22 4d61 7468 3132 3878 3132 385f 5f50  :"Math128x128__P
+000137d0: 6f77 6572 556e 6465 7266 6c6f 7722 2c22  owerUnderflow","
+000137e0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+000137f0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+00013800: 6522 3a22 5065 6e64 696e 674f 776e 6162  e":"PendingOwnab
+00013810: 6c65 5f5f 4164 6472 6573 735a 6572 6f22  le__AddressZero"
+00013820: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+00013830: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+00013840: 616d 6522 3a22 5065 6e64 696e 674f 776e  ame":"PendingOwn
+00013850: 6162 6c65 5f5f 4e6f 5065 6e64 696e 674f  able__NoPendingO
+00013860: 776e 6572 222c 2274 7970 6522 3a22 6572  wner","type":"er
+00013870: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+00013880: 5b5d 2c22 6e61 6d65 223a 2250 656e 6469  [],"name":"Pendi
+00013890: 6e67 4f77 6e61 626c 655f 5f4e 6f74 4f77  ngOwnable__NotOw
+000138a0: 6e65 7222 2c22 7479 7065 223a 2265 7272  ner","type":"err
+000138b0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+000138c0: 5d2c 226e 616d 6522 3a22 5065 6e64 696e  ],"name":"Pendin
+000138d0: 674f 776e 6162 6c65 5f5f 4e6f 7450 656e  gOwnable__NotPen
+000138e0: 6469 6e67 4f77 6e65 7222 2c22 7479 7065  dingOwner","type
+000138f0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+00013900: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+00013910: 5065 6e64 696e 674f 776e 6162 6c65 5f5f  PendingOwnable__
+00013920: 5065 6e64 696e 674f 776e 6572 416c 7265  PendingOwnerAlre
+00013930: 6164 7953 6574 222c 2274 7970 6522 3a22  adySet","type":"
+00013940: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00013950: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00013960: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00013970: 6d65 223a 2278 222c 2274 7970 6522 3a22  me":"x","type":"
+00013980: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+00013990: 223a 2253 6166 6543 6173 745f 5f45 7863  ":"SafeCast__Exc
+000139a0: 6565 6473 3136 4269 7473 222c 2274 7970  eeds16Bits","typ
+000139b0: 6522 3a22 6572 726f 7222 7d2c 7b22 616e  e":"error"},{"an
+000139c0: 6f6e 796d 6f75 7322 3a66 616c 7365 2c22  onymous":false,"
+000139d0: 696e 7075 7473 223a 5b7b 2269 6e64 6578  inputs":[{"index
+000139e0: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
+000139f0: 6e61 6c54 7970 6522 3a22 626f 6f6c 222c  nalType":"bool",
+00013a00: 226e 616d 6522 3a22 756e 6c6f 636b 6564  "name":"unlocked
+00013a10: 222c 2274 7970 6522 3a22 626f 6f6c 227d  ","type":"bool"}
+00013a20: 5d2c 226e 616d 6522 3a22 4661 6374 6f72  ],"name":"Factor
+00013a30: 794c 6f63 6b65 6453 7461 7475 7355 7064  yLockedStatusUpd
+00013a40: 6174 6564 222c 2274 7970 6522 3a22 6576  ated","type":"ev
+00013a50: 656e 7422 7d2c 7b22 616e 6f6e 796d 6f75  ent"},{"anonymou
+00013a60: 7322 3a66 616c 7365 2c22 696e 7075 7473  s":false,"inputs
+00013a70: 223a 5b7b 2269 6e64 6578 6564 223a 7472  ":[{"indexed":tr
+00013a80: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
+00013a90: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+00013aa0: 6522 3a22 7365 6e64 6572 222c 2274 7970  e":"sender","typ
+00013ab0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+00013ac0: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
+00013ad0: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
+00013ae0: 6e74 7261 6374 2049 4c42 5061 6972 222c  ntract ILBPair",
+00013af0: 226e 616d 6522 3a22 4c42 5061 6972 222c  "name":"LBPair",
+00013b00: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+00013b10: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
+00013b20: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
+00013b30: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00013b40: 6522 3a22 6269 6e53 7465 7022 2c22 7479  e":"binStep","ty
+00013b50: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+00013b60: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
+00013b70: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00013b80: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00013b90: 2262 6173 6546 6163 746f 7222 2c22 7479  "baseFactor","ty
+00013ba0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+00013bb0: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
+00013bc0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00013bd0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00013be0: 2266 696c 7465 7250 6572 696f 6422 2c22  "filterPeriod","
+00013bf0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00013c00: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+00013c10: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+00013c20: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00013c30: 223a 2264 6563 6179 5065 7269 6f64 222c  ":"decayPeriod",
+00013c40: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00013c50: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
+00013c60: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
+00013c70: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00013c80: 6522 3a22 7265 6475 6374 696f 6e46 6163  e":"reductionFac
+00013c90: 746f 7222 2c22 7479 7065 223a 2275 696e  tor","type":"uin
+00013ca0: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
+00013cb0: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
+00013cc0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00013cd0: 2c22 6e61 6d65 223a 2276 6172 6961 626c  ,"name":"variabl
+00013ce0: 6546 6565 436f 6e74 726f 6c22 2c22 7479  eFeeControl","ty
+00013cf0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+00013d00: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
+00013d10: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00013d20: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00013d30: 2270 726f 746f 636f 6c53 6861 7265 222c  "protocolShare",
+00013d40: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00013d50: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
+00013d60: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
+00013d70: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00013d80: 6522 3a22 6d61 7856 6f6c 6174 696c 6974  e":"maxVolatilit
+00013d90: 7941 6363 756d 756c 6174 6564 222c 2274  yAccumulated","t
+00013da0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+00013db0: 2c22 6e61 6d65 223a 2246 6565 5061 7261  ,"name":"FeePara
+00013dc0: 6d65 7465 7273 5365 7422 2c22 7479 7065  metersSet","type
+00013dd0: 223a 2265 7665 6e74 227d 2c7b 2261 6e6f  ":"event"},{"ano
+00013de0: 6e79 6d6f 7573 223a 6661 6c73 652c 2269  nymous":false,"i
+00013df0: 6e70 7574 7322 3a5b 7b22 696e 6465 7865  nputs":[{"indexe
+00013e00: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+00013e10: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+00013e20: 222c 226e 616d 6522 3a22 6f6c 6452 6563  ","name":"oldRec
+00013e30: 6970 6965 6e74 222c 2274 7970 6522 3a22  ipient","type":"
+00013e40: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
+00013e50: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
+00013e60: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+00013e70: 7373 222c 226e 616d 6522 3a22 6e65 7752  ss","name":"newR
+00013e80: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
+00013e90: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
+00013ea0: 6d65 223a 2246 6565 5265 6369 7069 656e  me":"FeeRecipien
+00013eb0: 7453 6574 222c 2274 7970 6522 3a22 6576  tSet","type":"ev
+00013ec0: 656e 7422 7d2c 7b22 616e 6f6e 796d 6f75  ent"},{"anonymou
+00013ed0: 7322 3a66 616c 7365 2c22 696e 7075 7473  s":false,"inputs
+00013ee0: 223a 5b7b 2269 6e64 6578 6564 223a 6661  ":[{"indexed":fa
+00013ef0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
+00013f00: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00013f10: 6d65 223a 226f 6c64 466c 6173 684c 6f61  me":"oldFlashLoa
+00013f20: 6e46 6565 222c 2274 7970 6522 3a22 7569  nFee","type":"ui
+00013f30: 6e74 3235 3622 7d2c 7b22 696e 6465 7865  nt256"},{"indexe
+00013f40: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+00013f50: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00013f60: 222c 226e 616d 6522 3a22 6e65 7746 6c61  ","name":"newFla
+00013f70: 7368 4c6f 616e 4665 6522 2c22 7479 7065  shLoanFee","type
+00013f80: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+00013f90: 616d 6522 3a22 466c 6173 684c 6f61 6e46  ame":"FlashLoanF
+00013fa0: 6565 5365 7422 2c22 7479 7065 223a 2265  eeSet","type":"e
+00013fb0: 7665 6e74 227d 2c7b 2261 6e6f 6e79 6d6f  vent"},{"anonymo
+00013fc0: 7573 223a 6661 6c73 652c 2269 6e70 7574  us":false,"input
+00013fd0: 7322 3a5b 7b22 696e 6465 7865 6422 3a74  s":[{"indexed":t
+00013fe0: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
+00013ff0: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
+00014000: 4332 3022 2c22 6e61 6d65 223a 2274 6f6b  C20","name":"tok
+00014010: 656e 5822 2c22 7479 7065 223a 2261 6464  enX","type":"add
+00014020: 7265 7373 227d 2c7b 2269 6e64 6578 6564  ress"},{"indexed
+00014030: 223a 7472 7565 2c22 696e 7465 726e 616c  ":true,"internal
+00014040: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+00014050: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
+00014060: 746f 6b65 6e59 222c 2274 7970 6522 3a22  tokenY","type":"
+00014070: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
+00014080: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
+00014090: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+000140a0: 3622 2c22 6e61 6d65 223a 2262 696e 5374  6","name":"binSt
+000140b0: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
+000140c0: 3235 3622 7d2c 7b22 696e 6465 7865 6422  256"},{"indexed"
+000140d0: 3a66 616c 7365 2c22 696e 7465 726e 616c  :false,"internal
+000140e0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+000140f0: 494c 4250 6169 7222 2c22 6e61 6d65 223a  ILBPair","name":
+00014100: 224c 4250 6169 7222 2c22 7479 7065 223a  "LBPair","type":
+00014110: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
+00014120: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+00014130: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00014140: 3235 3622 2c22 6e61 6d65 223a 2270 6964  256","name":"pid
+00014150: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00014160: 3622 7d5d 2c22 6e61 6d65 223a 224c 4250  6"}],"name":"LBP
+00014170: 6169 7243 7265 6174 6564 222c 2274 7970  airCreated","typ
+00014180: 6522 3a22 6576 656e 7422 7d2c 7b22 616e  e":"event"},{"an
+00014190: 6f6e 796d 6f75 7322 3a66 616c 7365 2c22  onymous":false,"
+000141a0: 696e 7075 7473 223a 5b7b 2269 6e64 6578  inputs":[{"index
+000141b0: 6564 223a 7472 7565 2c22 696e 7465 726e  ed":true,"intern
+000141c0: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+000141d0: 7420 494c 4250 6169 7222 2c22 6e61 6d65  t ILBPair","name
+000141e0: 223a 224c 4250 6169 7222 2c22 7479 7065  ":"LBPair","type
+000141f0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+00014200: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
+00014210: 6e74 6572 6e61 6c54 7970 6522 3a22 626f  nternalType":"bo
+00014220: 6f6c 222c 226e 616d 6522 3a22 6967 6e6f  ol","name":"igno
+00014230: 7265 6422 2c22 7479 7065 223a 2262 6f6f  red","type":"boo
+00014240: 6c22 7d5d 2c22 6e61 6d65 223a 224c 4250  l"}],"name":"LBP
+00014250: 6169 7249 676e 6f72 6564 5374 6174 6543  airIgnoredStateC
+00014260: 6861 6e67 6564 222c 2274 7970 6522 3a22  hanged","type":"
+00014270: 6576 656e 7422 7d2c 7b22 616e 6f6e 796d  event"},{"anonym
+00014280: 6f75 7322 3a66 616c 7365 2c22 696e 7075  ous":false,"inpu
+00014290: 7473 223a 5b7b 2269 6e64 6578 6564 223a  ts":[{"indexed":
+000142a0: 6661 6c73 652c 2269 6e74 6572 6e61 6c54  false,"internalT
+000142b0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+000142c0: 6e61 6d65 223a 226f 6c64 4c42 5061 6972  name":"oldLBPair
+000142d0: 496d 706c 656d 656e 7461 7469 6f6e 222c  Implementation",
+000142e0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+000142f0: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
+00014300: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
+00014310: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+00014320: 6522 3a22 4c42 5061 6972 496d 706c 656d  e":"LBPairImplem
+00014330: 656e 7461 7469 6f6e 222c 2274 7970 6522  entation","type"
+00014340: 3a22 6164 6472 6573 7322 7d5d 2c22 6e61  :"address"}],"na
+00014350: 6d65 223a 224c 4250 6169 7249 6d70 6c65  me":"LBPairImple
+00014360: 6d65 6e74 6174 696f 6e53 6574 222c 2274  mentationSet","t
+00014370: 7970 6522 3a22 6576 656e 7422 7d2c 7b22  ype":"event"},{"
+00014380: 616e 6f6e 796d 6f75 7322 3a66 616c 7365  anonymous":false
+00014390: 2c22 696e 7075 7473 223a 5b7b 2269 6e64  ,"inputs":[{"ind
+000143a0: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
+000143b0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+000143c0: 7373 222c 226e 616d 6522 3a22 7072 6576  ss","name":"prev
+000143d0: 696f 7573 4f77 6e65 7222 2c22 7479 7065  iousOwner","type
+000143e0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+000143f0: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
+00014400: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+00014410: 7265 7373 222c 226e 616d 6522 3a22 6e65  ress","name":"ne
+00014420: 774f 776e 6572 222c 2274 7970 6522 3a22  wOwner","type":"
+00014430: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+00014440: 223a 224f 776e 6572 7368 6970 5472 616e  ":"OwnershipTran
+00014450: 7366 6572 7265 6422 2c22 7479 7065 223a  sferred","type":
+00014460: 2265 7665 6e74 227d 2c7b 2261 6e6f 6e79  "event"},{"anony
+00014470: 6d6f 7573 223a 6661 6c73 652c 2269 6e70  mous":false,"inp
+00014480: 7574 7322 3a5b 7b22 696e 6465 7865 6422  uts":[{"indexed"
+00014490: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
+000144a0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+000144b0: 6e61 6d65 223a 2270 656e 6469 6e67 4f77  name":"pendingOw
+000144c0: 6e65 7222 2c22 7479 7065 223a 2261 6464  ner","type":"add
+000144d0: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
+000144e0: 5065 6e64 696e 674f 776e 6572 5365 7422  PendingOwnerSet"
+000144f0: 2c22 7479 7065 223a 2265 7665 6e74 227d  ,"type":"event"}
+00014500: 2c7b 2261 6e6f 6e79 6d6f 7573 223a 6661  ,{"anonymous":fa
+00014510: 6c73 652c 2269 6e70 7574 7322 3a5b 7b22  lse,"inputs":[{"
+00014520: 696e 6465 7865 6422 3a74 7275 652c 2269  indexed":true,"i
+00014530: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00014540: 6e74 3235 3622 2c22 6e61 6d65 223a 2262  nt256","name":"b
+00014550: 696e 5374 6570 222c 2274 7970 6522 3a22  inStep","type":"
+00014560: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+00014570: 223a 2250 7265 7365 7452 656d 6f76 6564  ":"PresetRemoved
+00014580: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
+00014590: 7d2c 7b22 616e 6f6e 796d 6f75 7322 3a66  },{"anonymous":f
+000145a0: 616c 7365 2c22 696e 7075 7473 223a 5b7b  alse,"inputs":[{
+000145b0: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
+000145c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000145d0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000145e0: 6269 6e53 7465 7022 2c22 7479 7065 223a  binStep","type":
+000145f0: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
+00014600: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+00014610: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00014620: 3235 3622 2c22 6e61 6d65 223a 2262 6173  256","name":"bas
+00014630: 6546 6163 746f 7222 2c22 7479 7065 223a  eFactor","type":
+00014640: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
+00014650: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+00014660: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00014670: 3235 3622 2c22 6e61 6d65 223a 2266 696c  256","name":"fil
+00014680: 7465 7250 6572 696f 6422 2c22 7479 7065  terPeriod","type
+00014690: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+000146a0: 6e64 6578 6564 223a 6661 6c73 652c 2269  ndexed":false,"i
+000146b0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+000146c0: 6e74 3235 3622 2c22 6e61 6d65 223a 2264  nt256","name":"d
+000146d0: 6563 6179 5065 7269 6f64 222c 2274 7970  ecayPeriod","typ
+000146e0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+000146f0: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
+00014700: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00014710: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00014720: 7265 6475 6374 696f 6e46 6163 746f 7222  reductionFactor"
+00014730: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00014740: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
+00014750: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
+00014760: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00014770: 6d65 223a 2276 6172 6961 626c 6546 6565  me":"variableFee
+00014780: 436f 6e74 726f 6c22 2c22 7479 7065 223a  Control","type":
+00014790: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
+000147a0: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+000147b0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+000147c0: 3235 3622 2c22 6e61 6d65 223a 2270 726f  256","name":"pro
+000147d0: 746f 636f 6c53 6861 7265 222c 2274 7970  tocolShare","typ
+000147e0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+000147f0: 696e 6465 7865 6422 3a66 616c 7365 2c22  indexed":false,"
+00014800: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00014810: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00014820: 6d61 7856 6f6c 6174 696c 6974 7941 6363  maxVolatilityAcc
+00014830: 756d 756c 6174 6564 222c 2274 7970 6522  umulated","type"
+00014840: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+00014850: 6465 7865 6422 3a66 616c 7365 2c22 696e  dexed":false,"in
+00014860: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00014870: 7432 3536 222c 226e 616d 6522 3a22 7361  t256","name":"sa
+00014880: 6d70 6c65 4c69 6665 7469 6d65 222c 2274  mpleLifetime","t
+00014890: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+000148a0: 2c22 6e61 6d65 223a 2250 7265 7365 7453  ,"name":"PresetS
+000148b0: 6574 222c 2274 7970 6522 3a22 6576 656e  et","type":"even
+000148c0: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
+000148d0: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
+000148e0: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
+000148f0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+00014900: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
+00014910: 222c 226e 616d 6522 3a22 7175 6f74 6541  ","name":"quoteA
+00014920: 7373 6574 222c 2274 7970 6522 3a22 6164  sset","type":"ad
+00014930: 6472 6573 7322 7d5d 2c22 6e61 6d65 223a  dress"}],"name":
+00014940: 2251 756f 7465 4173 7365 7441 6464 6564  "QuoteAssetAdded
+00014950: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
+00014960: 7d2c 7b22 616e 6f6e 796d 6f75 7322 3a66  },{"anonymous":f
+00014970: 616c 7365 2c22 696e 7075 7473 223a 5b7b  alse,"inputs":[{
+00014980: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
+00014990: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+000149a0: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
+000149b0: 226e 616d 6522 3a22 7175 6f74 6541 7373  "name":"quoteAss
+000149c0: 6574 222c 2274 7970 6522 3a22 6164 6472  et","type":"addr
+000149d0: 6573 7322 7d5d 2c22 6e61 6d65 223a 2251  ess"}],"name":"Q
+000149e0: 756f 7465 4173 7365 7452 656d 6f76 6564  uoteAssetRemoved
+000149f0: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
+00014a00: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+00014a10: 6e61 6d65 223a 224c 4250 6169 7249 6d70  name":"LBPairImp
+00014a20: 6c65 6d65 6e74 6174 696f 6e22 2c22 6f75  lementation","ou
+00014a30: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
+00014a40: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+00014a50: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
+00014a60: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+00014a70: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00014a80: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
+00014a90: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00014aa0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+00014ab0: 4d41 585f 4249 4e5f 5354 4550 222c 226f  MAX_BIN_STEP","o
+00014ac0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+00014ad0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00014ae0: 3622 2c22 6e61 6d65 223a 2222 2c22 7479  6","name":"","ty
+00014af0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00014b00: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00014b10: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
+00014b20: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00014b30: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+00014b40: 224d 4158 5f46 4545 222c 226f 7574 7075  "MAX_FEE","outpu
+00014b50: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00014b60: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00014b70: 6e61 6d65 223a 2222 2c22 7479 7065 223a  name":"","type":
+00014b80: 2275 696e 7432 3536 227d 5d2c 2273 7461  "uint256"}],"sta
+00014b90: 7465 4d75 7461 6269 6c69 7479 223a 2276  teMutability":"v
+00014ba0: 6965 7722 2c22 7479 7065 223a 2266 756e  iew","type":"fun
+00014bb0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+00014bc0: 223a 5b5d 2c22 6e61 6d65 223a 224d 4158  ":[],"name":"MAX
+00014bd0: 5f50 524f 544f 434f 4c5f 5348 4152 4522  _PROTOCOL_SHARE"
+00014be0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+00014bf0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00014c00: 7432 3536 222c 226e 616d 6522 3a22 222c  t256","name":"",
+00014c10: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00014c20: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
+00014c30: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
+00014c40: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00014c50: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+00014c60: 6522 3a22 4d49 4e5f 4249 4e5f 5354 4550  e":"MIN_BIN_STEP
+00014c70: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
+00014c80: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00014c90: 6e74 3235 3622 2c22 6e61 6d65 223a 2222  nt256","name":""
+00014ca0: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00014cb0: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
+00014cc0: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
+00014cd0: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+00014ce0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+00014cf0: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+00014d00: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
+00014d10: 6d65 223a 225f 7175 6f74 6541 7373 6574  me":"_quoteAsset
+00014d20: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00014d30: 7322 7d5d 2c22 6e61 6d65 223a 2261 6464  s"}],"name":"add
+00014d40: 5175 6f74 6541 7373 6574 222c 226f 7574  QuoteAsset","out
+00014d50: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
+00014d60: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
+00014d70: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
+00014d80: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00014d90: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00014da0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+00014db0: 226e 616d 6522 3a22 222c 2274 7970 6522  "name":"","type"
+00014dc0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+00014dd0: 6d65 223a 2261 6c6c 4c42 5061 6972 7322  me":"allLBPairs"
+00014de0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+00014df0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+00014e00: 7472 6163 7420 494c 4250 6169 7222 2c22  tract ILBPair","
+00014e10: 6e61 6d65 223a 2222 2c22 7479 7065 223a  name":"","type":
+00014e20: 2261 6464 7265 7373 227d 5d2c 2273 7461  "address"}],"sta
+00014e30: 7465 4d75 7461 6269 6c69 7479 223a 2276  teMutability":"v
+00014e40: 6965 7722 2c22 7479 7065 223a 2266 756e  iew","type":"fun
+00014e50: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+00014e60: 223a 5b5d 2c22 6e61 6d65 223a 2262 6563  ":[],"name":"bec
+00014e70: 6f6d 654f 776e 6572 222c 226f 7574 7075  omeOwner","outpu
+00014e80: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
+00014e90: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
+00014ea0: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
+00014eb0: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+00014ec0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00014ed0: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
+00014ee0: 5243 3230 222c 226e 616d 6522 3a22 5f74  RC20","name":"_t
+00014ef0: 6f6b 656e 5822 2c22 7479 7065 223a 2261  okenX","type":"a
+00014f00: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+00014f10: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+00014f20: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
+00014f30: 223a 225f 746f 6b65 6e59 222c 2274 7970  ":"_tokenY","typ
+00014f40: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+00014f50: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00014f60: 696e 7432 3422 2c22 6e61 6d65 223a 225f  int24","name":"_
+00014f70: 6163 7469 7665 4964 222c 2274 7970 6522  activeId","type"
+00014f80: 3a22 7569 6e74 3234 227d 2c7b 2269 6e74  :"uint24"},{"int
+00014f90: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00014fa0: 3136 222c 226e 616d 6522 3a22 5f62 696e  16","name":"_bin
+00014fb0: 5374 6570 222c 2274 7970 6522 3a22 7569  Step","type":"ui
+00014fc0: 6e74 3136 227d 5d2c 226e 616d 6522 3a22  nt16"}],"name":"
+00014fd0: 6372 6561 7465 4c42 5061 6972 222c 226f  createLBPair","o
+00014fe0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+00014ff0: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+00015000: 6374 2049 4c42 5061 6972 222c 226e 616d  ct ILBPair","nam
+00015010: 6522 3a22 5f4c 4250 6169 7222 2c22 7479  e":"_LBPair","ty
+00015020: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
+00015030: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00015040: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+00015050: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00015060: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+00015070: 6e61 6d65 223a 2263 7265 6174 696f 6e55  name":"creationU
+00015080: 6e6c 6f63 6b65 6422 2c22 6f75 7470 7574  nlocked","output
+00015090: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+000150a0: 7065 223a 2262 6f6f 6c22 2c22 6e61 6d65  pe":"bool","name
+000150b0: 223a 2222 2c22 7479 7065 223a 2262 6f6f  ":"","type":"boo
+000150c0: 6c22 7d5d 2c22 7374 6174 654d 7574 6162  l"}],"stateMutab
+000150d0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+000150e0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+000150f0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+00015100: 616d 6522 3a22 6665 6552 6563 6970 6965  ame":"feeRecipie
+00015110: 6e74 222c 226f 7574 7075 7473 223a 5b7b  nt","outputs":[{
+00015120: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00015130: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+00015140: 2222 2c22 7479 7065 223a 2261 6464 7265  "","type":"addre
+00015150: 7373 227d 5d2c 2273 7461 7465 4d75 7461  ss"}],"stateMuta
+00015160: 6269 6c69 7479 223a 2276 6965 7722 2c22  bility":"view","
+00015170: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00015180: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+00015190: 6e61 6d65 223a 2266 6c61 7368 4c6f 616e  name":"flashLoan
+000151a0: 4665 6522 2c22 6f75 7470 7574 7322 3a5b  Fee","outputs":[
+000151b0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000151c0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+000151d0: 3a22 222c 2274 7970 6522 3a22 7569 6e74  :"","type":"uint
+000151e0: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
+000151f0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+00015200: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00015210: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00015220: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+00015230: 6f6e 7472 6163 7420 494c 4250 6169 7222  ontract ILBPair"
+00015240: 2c22 6e61 6d65 223a 225f 4c42 5061 6972  ,"name":"_LBPair
+00015250: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00015260: 7322 7d5d 2c22 6e61 6d65 223a 2266 6f72  s"}],"name":"for
+00015270: 6365 4465 6361 7922 2c22 6f75 7470 7574  ceDecay","output
+00015280: 7322 3a5b 5d2c 2273 7461 7465 4d75 7461  s":[],"stateMuta
+00015290: 6269 6c69 7479 223a 226e 6f6e 7061 7961  bility":"nonpaya
+000152a0: 626c 6522 2c22 7479 7065 223a 2266 756e  ble","type":"fun
+000152b0: 6374 696f 6e22 7d2c 7b22 696e 7075 7473  ction"},{"inputs
+000152c0: 223a 5b5d 2c22 6e61 6d65 223a 2267 6574  ":[],"name":"get
+000152d0: 416c 6c42 696e 5374 6570 7322 2c22 6f75  AllBinSteps","ou
+000152e0: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
+000152f0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00015300: 5b5d 222c 226e 616d 6522 3a22 7072 6573  []","name":"pres
+00015310: 6574 7342 696e 5374 6570 222c 2274 7970  etsBinStep","typ
+00015320: 6522 3a22 7569 6e74 3235 365b 5d22 7d5d  e":"uint256[]"}]
+00015330: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+00015340: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+00015350: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+00015360: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00015370: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+00015380: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
+00015390: 3a22 5f74 6f6b 656e 5822 2c22 7479 7065  :"_tokenX","type
+000153a0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+000153b0: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
+000153c0: 6e74 7261 6374 2049 4552 4332 3022 2c22  ntract IERC20","
+000153d0: 6e61 6d65 223a 225f 746f 6b65 6e59 222c  name":"_tokenY",
+000153e0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+000153f0: 7d5d 2c22 6e61 6d65 223a 2267 6574 416c  }],"name":"getAl
+00015400: 6c4c 4250 6169 7273 222c 226f 7574 7075  lLBPairs","outpu
+00015410: 7473 223a 5b7b 2263 6f6d 706f 6e65 6e74  ts":[{"component
+00015420: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00015430: 7065 223a 2275 696e 7431 3622 2c22 6e61  pe":"uint16","na
+00015440: 6d65 223a 2262 696e 5374 6570 222c 2274  me":"binStep","t
+00015450: 7970 6522 3a22 7569 6e74 3136 227d 2c7b  ype":"uint16"},{
+00015460: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00015470: 636f 6e74 7261 6374 2049 4c42 5061 6972  contract ILBPair
+00015480: 222c 226e 616d 6522 3a22 4c42 5061 6972  ","name":"LBPair
+00015490: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000154a0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+000154b0: 7065 223a 2262 6f6f 6c22 2c22 6e61 6d65  pe":"bool","name
+000154c0: 223a 2263 7265 6174 6564 4279 4f77 6e65  ":"createdByOwne
+000154d0: 7222 2c22 7479 7065 223a 2262 6f6f 6c22  r","type":"bool"
+000154e0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000154f0: 223a 2262 6f6f 6c22 2c22 6e61 6d65 223a  ":"bool","name":
+00015500: 2269 676e 6f72 6564 466f 7252 6f75 7469  "ignoredForRouti
+00015510: 6e67 222c 2274 7970 6522 3a22 626f 6f6c  ng","type":"bool
+00015520: 227d 5d2c 2269 6e74 6572 6e61 6c54 7970  "}],"internalTyp
+00015530: 6522 3a22 7374 7275 6374 2049 4c42 4661  e":"struct ILBFa
+00015540: 6374 6f72 792e 4c42 5061 6972 496e 666f  ctory.LBPairInfo
+00015550: 726d 6174 696f 6e5b 5d22 2c22 6e61 6d65  rmation[]","name
+00015560: 223a 224c 4250 6169 7273 4176 6169 6c61  ":"LBPairsAvaila
+00015570: 626c 6522 2c22 7479 7065 223a 2274 7570  ble","type":"tup
+00015580: 6c65 5b5d 227d 5d2c 2273 7461 7465 4d75  le[]"}],"stateMu
+00015590: 7461 6269 6c69 7479 223a 2276 6965 7722  tability":"view"
+000155a0: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+000155b0: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
+000155c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000155d0: 636f 6e74 7261 6374 2049 4552 4332 3022  contract IERC20"
+000155e0: 2c22 6e61 6d65 223a 225f 746f 6b65 6e41  ,"name":"_tokenA
+000155f0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00015600: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+00015610: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
+00015620: 5243 3230 222c 226e 616d 6522 3a22 5f74  RC20","name":"_t
+00015630: 6f6b 656e 4222 2c22 7479 7065 223a 2261  okenB","type":"a
+00015640: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+00015650: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00015660: 3622 2c22 6e61 6d65 223a 225f 6269 6e53  6","name":"_binS
+00015670: 7465 7022 2c22 7479 7065 223a 2275 696e  tep","type":"uin
+00015680: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+00015690: 6765 744c 4250 6169 7249 6e66 6f72 6d61  getLBPairInforma
+000156a0: 7469 6f6e 222c 226f 7574 7075 7473 223a  tion","outputs":
+000156b0: 5b7b 2263 6f6d 706f 6e65 6e74 7322 3a5b  [{"components":[
+000156c0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000156d0: 2275 696e 7431 3622 2c22 6e61 6d65 223a  "uint16","name":
+000156e0: 2262 696e 5374 6570 222c 2274 7970 6522  "binStep","type"
+000156f0: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
+00015700: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+00015710: 7261 6374 2049 4c42 5061 6972 222c 226e  ract ILBPair","n
+00015720: 616d 6522 3a22 4c42 5061 6972 222c 2274  ame":"LBPair","t
+00015730: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+00015740: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00015750: 2262 6f6f 6c22 2c22 6e61 6d65 223a 2263  "bool","name":"c
+00015760: 7265 6174 6564 4279 4f77 6e65 7222 2c22  reatedByOwner","
+00015770: 7479 7065 223a 2262 6f6f 6c22 7d2c 7b22  type":"bool"},{"
+00015780: 696e 7465 726e 616c 5479 7065 223a 2262  internalType":"b
+00015790: 6f6f 6c22 2c22 6e61 6d65 223a 2269 676e  ool","name":"ign
+000157a0: 6f72 6564 466f 7252 6f75 7469 6e67 222c  oredForRouting",
+000157b0: 2274 7970 6522 3a22 626f 6f6c 227d 5d2c  "type":"bool"}],
+000157c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000157d0: 7374 7275 6374 2049 4c42 4661 6374 6f72  struct ILBFactor
+000157e0: 792e 4c42 5061 6972 496e 666f 726d 6174  y.LBPairInformat
+000157f0: 696f 6e22 2c22 6e61 6d65 223a 2222 2c22  ion","name":"","
+00015800: 7479 7065 223a 2274 7570 6c65 227d 5d2c  type":"tuple"}],
+00015810: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00015820: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
+00015830: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00015840: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+00015850: 2267 6574 4e75 6d62 6572 4f66 4c42 5061  "getNumberOfLBPa
+00015860: 6972 7322 2c22 6f75 7470 7574 7322 3a5b  irs","outputs":[
+00015870: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00015880: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00015890: 3a22 222c 2274 7970 6522 3a22 7569 6e74  :"","type":"uint
+000158a0: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
+000158b0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+000158c0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+000158d0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+000158e0: 226e 616d 6522 3a22 6765 744e 756d 6265  "name":"getNumbe
+000158f0: 724f 6651 756f 7465 4173 7365 7473 222c  rOfQuoteAssets",
+00015900: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
+00015910: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00015920: 3235 3622 2c22 6e61 6d65 223a 2222 2c22  256","name":"","
+00015930: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00015940: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+00015950: 7479 223a 2276 6965 7722 2c22 7479 7065  ty":"view","type
+00015960: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
+00015970: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00015980: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
+00015990: 222c 226e 616d 6522 3a22 5f62 696e 5374  ","name":"_binSt
+000159a0: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
+000159b0: 3136 227d 5d2c 226e 616d 6522 3a22 6765  16"}],"name":"ge
+000159c0: 7450 7265 7365 7422 2c22 6f75 7470 7574  tPreset","output
+000159d0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+000159e0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000159f0: 616d 6522 3a22 6261 7365 4661 6374 6f72  ame":"baseFactor
 00015a00: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
 00015a10: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
 00015a20: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00015a30: 616d 6522 3a22 7072 6f74 6f63 6f6c 5368  ame":"protocolSh
-00015a40: 6172 6522 2c22 7479 7065 223a 2275 696e  are","type":"uin
-00015a50: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-00015a60: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00015a70: 2c22 6e61 6d65 223a 226d 6178 566f 6c61  ,"name":"maxVola
-00015a80: 7469 6c69 7479 4163 6375 6d75 6c61 7465  tilityAccumulate
-00015a90: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-00015aa0: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-00015ab0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00015ac0: 6e61 6d65 223a 2273 616d 706c 654c 6966  name":"sampleLif
-00015ad0: 6574 696d 6522 2c22 7479 7065 223a 2275  etime","type":"u
-00015ae0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-00015af0: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
-00015b00: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
-00015b10: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-00015b20: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00015b30: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00015b40: 223a 225f 696e 6465 7822 2c22 7479 7065  ":"_index","type
-00015b50: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-00015b60: 616d 6522 3a22 6765 7451 756f 7465 4173  ame":"getQuoteAs
-00015b70: 7365 7422 2c22 6f75 7470 7574 7322 3a5b  set","outputs":[
-00015b80: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00015b90: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
-00015ba0: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-00015bb0: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-00015bc0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00015bd0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-00015be0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00015bf0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00015c00: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-00015c10: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-00015c20: 5f74 6f6b 656e 222c 2274 7970 6522 3a22  _token","type":"
-00015c30: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
-00015c40: 223a 2269 7351 756f 7465 4173 7365 7422  ":"isQuoteAsset"
-00015c50: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-00015c60: 7465 726e 616c 5479 7065 223a 2262 6f6f  ternalType":"boo
-00015c70: 6c22 2c22 6e61 6d65 223a 2222 2c22 7479  l","name":"","ty
-00015c80: 7065 223a 2262 6f6f 6c22 7d5d 2c22 7374  pe":"bool"}],"st
-00015c90: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-00015ca0: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
-00015cb0: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-00015cc0: 7322 3a5b 5d2c 226e 616d 6522 3a22 6f77  s":[],"name":"ow
-00015cd0: 6e65 7222 2c22 6f75 7470 7574 7322 3a5b  ner","outputs":[
-00015ce0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00015cf0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-00015d00: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
-00015d10: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
-00015d20: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-00015d30: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-00015d40: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-00015d50: 226e 616d 6522 3a22 7065 6e64 696e 674f  "name":"pendingO
-00015d60: 776e 6572 222c 226f 7574 7075 7473 223a  wner","outputs":
-00015d70: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00015d80: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-00015d90: 223a 2222 2c22 7479 7065 223a 2261 6464  ":"","type":"add
-00015da0: 7265 7373 227d 5d2c 2273 7461 7465 4d75  ress"}],"stateMu
-00015db0: 7461 6269 6c69 7479 223a 2276 6965 7722  tability":"view"
-00015dc0: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-00015dd0: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
-00015de0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00015df0: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
-00015e00: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
-00015e10: 3a22 7569 6e74 3136 227d 5d2c 226e 616d  :"uint16"}],"nam
-00015e20: 6522 3a22 7265 6d6f 7665 5072 6573 6574  e":"removePreset
-00015e30: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
-00015e40: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00015e50: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-00015e60: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00015e70: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-00015e80: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
-00015e90: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
-00015ea0: 616d 6522 3a22 5f71 756f 7465 4173 7365  ame":"_quoteAsse
-00015eb0: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
-00015ec0: 7373 227d 5d2c 226e 616d 6522 3a22 7265  ss"}],"name":"re
-00015ed0: 6d6f 7665 5175 6f74 6541 7373 6574 222c  moveQuoteAsset",
-00015ee0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
-00015ef0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-00015f00: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
-00015f10: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00015f20: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00015f30: 6522 3a22 7265 6e6f 756e 6365 4f77 6e65  e":"renounceOwne
-00015f40: 7273 6869 7022 2c22 6f75 7470 7574 7322  rship","outputs"
-00015f50: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
-00015f60: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
-00015f70: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
-00015f80: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-00015f90: 5b5d 2c22 6e61 6d65 223a 2272 6576 6f6b  [],"name":"revok
-00015fa0: 6550 656e 6469 6e67 4f77 6e65 7222 2c22  ePendingOwner","
-00015fb0: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-00015fc0: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-00015fd0: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-00015fe0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00015ff0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00016000: 6e61 6c54 7970 6522 3a22 626f 6f6c 222c  nalType":"bool",
-00016010: 226e 616d 6522 3a22 5f6c 6f63 6b65 6422  "name":"_locked"
-00016020: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
-00016030: 2c22 6e61 6d65 223a 2273 6574 4661 6374  ,"name":"setFact
-00016040: 6f72 794c 6f63 6b65 6453 7461 7465 222c  oryLockedState",
-00016050: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
-00016060: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-00016070: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
-00016080: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00016090: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-000160a0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-000160b0: 7373 222c 226e 616d 6522 3a22 5f66 6565  ss","name":"_fee
-000160c0: 5265 6369 7069 656e 7422 2c22 7479 7065  Recipient","type
-000160d0: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
-000160e0: 616d 6522 3a22 7365 7446 6565 5265 6369  ame":"setFeeReci
-000160f0: 7069 656e 7422 2c22 6f75 7470 7574 7322  pient","outputs"
-00016100: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
-00016110: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
-00016120: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
-00016130: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-00016140: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00016150: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
-00016160: 3022 2c22 6e61 6d65 223a 225f 746f 6b65  0","name":"_toke
-00016170: 6e58 222c 2274 7970 6522 3a22 6164 6472  nX","type":"addr
-00016180: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-00016190: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-000161a0: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-000161b0: 5f74 6f6b 656e 5922 2c22 7479 7065 223a  _tokenY","type":
-000161c0: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-000161d0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-000161e0: 3136 222c 226e 616d 6522 3a22 5f62 696e  16","name":"_bin
-000161f0: 5374 6570 222c 2274 7970 6522 3a22 7569  Step","type":"ui
-00016200: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
-00016210: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
-00016220: 226e 616d 6522 3a22 5f62 6173 6546 6163  "name":"_baseFac
-00016230: 746f 7222 2c22 7479 7065 223a 2275 696e  tor","type":"uin
-00016240: 7431 3622 7d2c 7b22 696e 7465 726e 616c  t16"},{"internal
-00016250: 5479 7065 223a 2275 696e 7431 3622 2c22  Type":"uint16","
-00016260: 6e61 6d65 223a 225f 6669 6c74 6572 5065  name":"_filterPe
-00016270: 7269 6f64 222c 2274 7970 6522 3a22 7569  riod","type":"ui
-00016280: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
-00016290: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
-000162a0: 226e 616d 6522 3a22 5f64 6563 6179 5065  "name":"_decayPe
-000162b0: 7269 6f64 222c 2274 7970 6522 3a22 7569  riod","type":"ui
-000162c0: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
-000162d0: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
-000162e0: 226e 616d 6522 3a22 5f72 6564 7563 7469  "name":"_reducti
-000162f0: 6f6e 4661 6374 6f72 222c 2274 7970 6522  onFactor","type"
-00016300: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
-00016310: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00016320: 3234 222c 226e 616d 6522 3a22 5f76 6172  24","name":"_var
-00016330: 6961 626c 6546 6565 436f 6e74 726f 6c22  iableFeeControl"
-00016340: 2c22 7479 7065 223a 2275 696e 7432 3422  ,"type":"uint24"
-00016350: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00016360: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-00016370: 223a 225f 7072 6f74 6f63 6f6c 5368 6172  ":"_protocolShar
-00016380: 6522 2c22 7479 7065 223a 2275 696e 7431  e","type":"uint1
-00016390: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-000163a0: 7065 223a 2275 696e 7432 3422 2c22 6e61  pe":"uint24","na
-000163b0: 6d65 223a 225f 6d61 7856 6f6c 6174 696c  me":"_maxVolatil
-000163c0: 6974 7941 6363 756d 756c 6174 6564 222c  ityAccumulated",
-000163d0: 2274 7970 6522 3a22 7569 6e74 3234 227d  "type":"uint24"}
-000163e0: 5d2c 226e 616d 6522 3a22 7365 7446 6565  ],"name":"setFee
-000163f0: 7350 6172 616d 6574 6572 734f 6e50 6169  sParametersOnPai
-00016400: 7222 2c22 6f75 7470 7574 7322 3a5b 5d2c  r","outputs":[],
-00016410: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00016420: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
-00016430: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-00016440: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-00016450: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00016460: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
-00016470: 666c 6173 684c 6f61 6e46 6565 222c 2274  flashLoanFee","t
-00016480: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-00016490: 2c22 6e61 6d65 223a 2273 6574 466c 6173  ,"name":"setFlas
-000164a0: 684c 6f61 6e46 6565 222c 226f 7574 7075  hLoanFee","outpu
-000164b0: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
-000164c0: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
-000164d0: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
-000164e0: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-000164f0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00016500: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
-00016510: 5243 3230 222c 226e 616d 6522 3a22 5f74  RC20","name":"_t
-00016520: 6f6b 656e 5822 2c22 7479 7065 223a 2261  okenX","type":"a
-00016530: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
-00016540: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
-00016550: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
-00016560: 223a 225f 746f 6b65 6e59 222c 2274 7970  ":"_tokenY","typ
-00016570: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-00016580: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00016590: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-000165a0: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
-000165b0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-000165c0: 7465 726e 616c 5479 7065 223a 2262 6f6f  ternalType":"boo
-000165d0: 6c22 2c22 6e61 6d65 223a 225f 6967 6e6f  l","name":"_igno
-000165e0: 7265 6422 2c22 7479 7065 223a 2262 6f6f  red","type":"boo
-000165f0: 6c22 7d5d 2c22 6e61 6d65 223a 2273 6574  l"}],"name":"set
-00016600: 4c42 5061 6972 4967 6e6f 7265 6422 2c22  LBPairIgnored","
-00016610: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-00016620: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-00016630: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-00016640: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00016650: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00016660: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00016670: 7322 2c22 6e61 6d65 223a 225f 4c42 5061  s","name":"_LBPa
-00016680: 6972 496d 706c 656d 656e 7461 7469 6f6e  irImplementation
-00016690: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-000166a0: 7322 7d5d 2c22 6e61 6d65 223a 2273 6574  s"}],"name":"set
-000166b0: 4c42 5061 6972 496d 706c 656d 656e 7461  LBPairImplementa
-000166c0: 7469 6f6e 222c 226f 7574 7075 7473 223a  tion","outputs":
-000166d0: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
-000166e0: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
-000166f0: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-00016700: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-00016710: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00016720: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-00016730: 3a22 7065 6e64 696e 674f 776e 6572 5f22  :"pendingOwner_"
-00016740: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00016750: 227d 5d2c 226e 616d 6522 3a22 7365 7450  "}],"name":"setP
-00016760: 656e 6469 6e67 4f77 6e65 7222 2c22 6f75  endingOwner","ou
-00016770: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
-00016780: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-00016790: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-000167a0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-000167b0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-000167c0: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
-000167d0: 226e 616d 6522 3a22 5f62 696e 5374 6570  "name":"_binStep
-000167e0: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
-000167f0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00016800: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
-00016810: 6522 3a22 5f62 6173 6546 6163 746f 7222  e":"_baseFactor"
-00016820: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
-00016830: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00016840: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-00016850: 223a 225f 6669 6c74 6572 5065 7269 6f64  ":"_filterPeriod
-00016860: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
-00016870: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00016880: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
-00016890: 6522 3a22 5f64 6563 6179 5065 7269 6f64  e":"_decayPeriod
-000168a0: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
-000168b0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-000168c0: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
-000168d0: 6522 3a22 5f72 6564 7563 7469 6f6e 4661  e":"_reductionFa
-000168e0: 6374 6f72 222c 2274 7970 6522 3a22 7569  ctor","type":"ui
-000168f0: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
-00016900: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
-00016910: 226e 616d 6522 3a22 5f76 6172 6961 626c  "name":"_variabl
-00016920: 6546 6565 436f 6e74 726f 6c22 2c22 7479  eFeeControl","ty
-00016930: 7065 223a 2275 696e 7432 3422 7d2c 7b22  pe":"uint24"},{"
-00016940: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00016950: 696e 7431 3622 2c22 6e61 6d65 223a 225f  int16","name":"_
-00016960: 7072 6f74 6f63 6f6c 5368 6172 6522 2c22  protocolShare","
-00016970: 7479 7065 223a 2275 696e 7431 3622 7d2c  type":"uint16"},
-00016980: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00016990: 2275 696e 7432 3422 2c22 6e61 6d65 223a  "uint24","name":
-000169a0: 225f 6d61 7856 6f6c 6174 696c 6974 7941  "_maxVolatilityA
-000169b0: 6363 756d 756c 6174 6564 222c 2274 7970  ccumulated","typ
-000169c0: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
-000169d0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-000169e0: 6e74 3136 222c 226e 616d 6522 3a22 5f73  nt16","name":"_s
-000169f0: 616d 706c 654c 6966 6574 696d 6522 2c22  ampleLifetime","
-00016a00: 7479 7065 223a 2275 696e 7431 3622 7d5d  type":"uint16"}]
-00016a10: 2c22 6e61 6d65 223a 2273 6574 5072 6573  ,"name":"setPres
-00016a20: 6574 222c 226f 7574 7075 7473 223a 5b5d  et","outputs":[]
-00016a30: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00016a40: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
-00016a50: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-00016a60: 227d 5d27 290a 0a20 2020 2023 6a6f 6520  "}]')..    #joe 
-00016a70: 6661 636f 7472 790a 2020 2020 6465 6620  facotry.    def 
-00016a80: 6765 745f 6e75 6d62 6572 5f6f 665f 6c62  get_number_of_lb
-00016a90: 5f70 6169 7273 285f 7765 6233 3a57 6562  _pairs(_web3:Web
-00016aa0: 332c 5f66 6163 746f 7279 5f61 6464 7265  3,_factory_addre
-00016ab0: 7373 293a 0a20 2020 2020 2020 2072 6574  ss):.        ret
-00016ac0: 7572 6e20 5f77 6562 332e 6574 682e 636f  urn _web3.eth.co
-00016ad0: 6e74 7261 6374 2861 6464 7265 7373 3d5f  ntract(address=_
-00016ae0: 6661 6374 6f72 795f 6164 6472 6573 732c  factory_address,
-00016af0: 2061 6269 3d4a 6f65 5632 4661 6374 6f72   abi=JoeV2Factor
-00016b00: 792e 6a6f 655f 6661 6374 6f72 795f 7632  y.joe_factory_v2
-00016b10: 5f61 6269 292e 6675 6e63 7469 6f6e 732e  _abi).functions.
-00016b20: 6765 744e 756d 6265 724f 664c 4250 6169  getNumberOfLBPai
-00016b30: 7273 2829 2e63 616c 6c28 290a 0a20 2020  rs().call()..   
-00016b40: 2064 6566 2067 6574 5f6e 756d 6265 725f   def get_number_
-00016b50: 6f66 5f71 756f 7465 5f61 7373 6574 7328  of_quote_assets(
-00016b60: 5f77 6562 333a 5765 6233 2c5f 6661 6374  _web3:Web3,_fact
-00016b70: 6f72 795f 6164 6472 6573 7329 3a0a 2020  ory_address):.  
-00016b80: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
-00016b90: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
-00016ba0: 6164 6472 6573 733d 5f66 6163 746f 7279  address=_factory
-00016bb0: 5f61 6464 7265 7373 2c20 6162 693d 4a6f  _address, abi=Jo
-00016bc0: 6556 3246 6163 746f 7279 2e6a 6f65 5f66  eV2Factory.joe_f
-00016bd0: 6163 746f 7279 5f76 325f 6162 6929 2e66  actory_v2_abi).f
-00016be0: 756e 6374 696f 6e73 2e67 6574 4e75 6d62  unctions.getNumb
-00016bf0: 6572 4f66 5175 6f74 6541 7373 6574 7328  erOfQuoteAssets(
-00016c00: 292e 6361 6c6c 2829 0a0a 2020 2020 6465  ).call()..    de
-00016c10: 6620 6765 745f 7175 6f74 655f 6173 7365  f get_quote_asse
-00016c20: 7428 5f77 6562 333a 5765 6233 2c5f 6661  t(_web3:Web3,_fa
-00016c30: 6374 6f72 795f 6164 6472 6573 732c 5f69  ctory_address,_i
-00016c40: 6e64 6578 293a 0a20 2020 2020 2020 2072  ndex):.        r
-00016c50: 6574 7572 6e20 5f77 6562 332e 6574 682e  eturn _web3.eth.
-00016c60: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
-00016c70: 3d5f 6661 6374 6f72 795f 6164 6472 6573  =_factory_addres
-00016c80: 732c 2061 6269 3d4a 6f65 5632 4661 6374  s, abi=JoeV2Fact
-00016c90: 6f72 792e 6a6f 655f 6661 6374 6f72 795f  ory.joe_factory_
-00016ca0: 7632 5f61 6269 292e 6675 6e63 7469 6f6e  v2_abi).function
-00016cb0: 732e 6765 7451 756f 7465 4173 7365 7428  s.getQuoteAsset(
-00016cc0: 5f69 6e64 6578 292e 6361 6c6c 2829 0a0a  _index).call()..
-00016cd0: 2020 2020 6465 6620 6973 5f71 756f 7465      def is_quote
-00016ce0: 5f61 7373 6574 285f 7765 6233 3a57 6562  _asset(_web3:Web
-00016cf0: 332c 5f66 6163 746f 7279 5f61 6464 7265  3,_factory_addre
-00016d00: 7373 2c5f 6164 6472 6573 733a 7374 7229  ss,_address:str)
-00016d10: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00016d20: 205f 7765 6233 2e65 7468 2e63 6f6e 7472   _web3.eth.contr
-00016d30: 6163 7428 6164 6472 6573 733d 5f66 6163  act(address=_fac
-00016d40: 746f 7279 5f61 6464 7265 7373 2c20 6162  tory_address, ab
-00016d50: 693d 4a6f 6556 3246 6163 746f 7279 2e6a  i=JoeV2Factory.j
-00016d60: 6f65 5f66 6163 746f 7279 5f76 325f 6162  oe_factory_v2_ab
-00016d70: 6929 2e66 756e 6374 696f 6e73 2e69 7351  i).functions.isQ
-00016d80: 756f 7465 4173 7365 7428 5f61 6464 7265  uoteAsset(_addre
-00016d90: 7373 292e 6361 6c6c 2829 0a0a 2020 2020  ss).call()..    
-00016da0: 6465 6620 6765 745f 7061 6972 5f69 6e66  def get_pair_inf
-00016db0: 6f72 6d61 7469 6f6e 285f 7765 6233 3a57  ormation(_web3:W
-00016dc0: 6562 332c 5f66 6163 746f 7279 5f61 6464  eb3,_factory_add
-00016dd0: 7265 7373 2c5f 746f 6b65 6e5f 613a 7374  ress,_token_a:st
-00016de0: 722c 5f74 6f6b 656e 5f62 3a73 7472 2c5f  r,_token_b:str,_
-00016df0: 6269 6e5f 7374 6570 293a 0a20 2020 2020  bin_step):.     
-00016e00: 2020 2072 6574 7572 6e20 5f77 6562 332e     return _web3.
-00016e10: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
-00016e20: 7265 7373 3d5f 6661 6374 6f72 795f 6164  ress=_factory_ad
-00016e30: 6472 6573 732c 2061 6269 3d4a 6f65 5632  dress, abi=JoeV2
-00016e40: 4661 6374 6f72 792e 6a6f 655f 6661 6374  Factory.joe_fact
-00016e50: 6f72 795f 7632 5f61 6269 292e 6675 6e63  ory_v2_abi).func
-00016e60: 7469 6f6e 732e 6765 744c 4250 6169 7249  tions.getLBPairI
-00016e70: 6e66 6f72 6d61 7469 6f6e 285f 746f 6b65  nformation(_toke
-00016e80: 6e5f 612c 5f74 6f6b 656e 5f62 2c5f 6269  n_a,_token_b,_bi
-00016e90: 6e5f 7374 6570 292e 6361 6c6c 2829 0a0a  n_step).call()..
-00016ea0: 2020 2020 6465 6620 6765 745f 616c 6c5f      def get_all_
-00016eb0: 6c62 5f70 6169 7273 285f 7765 6233 3a57  lb_pairs(_web3:W
-00016ec0: 6562 332c 5f66 6163 746f 7279 5f61 6464  eb3,_factory_add
-00016ed0: 7265 7373 2c5f 746f 6b65 6e5f 613a 7374  ress,_token_a:st
-00016ee0: 722c 5f74 6f6b 656e 5f62 3a73 7472 293a  r,_token_b:str):
-00016ef0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00016f00: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
-00016f10: 6374 2861 6464 7265 7373 3d5f 6661 6374  ct(address=_fact
-00016f20: 6f72 795f 6164 6472 6573 732c 2061 6269  ory_address, abi
-00016f30: 3d4a 6f65 5632 4661 6374 6f72 792e 6a6f  =JoeV2Factory.jo
-00016f40: 655f 6661 6374 6f72 795f 7632 5f61 6269  e_factory_v2_abi
-00016f50: 292e 6675 6e63 7469 6f6e 732e 6765 7441  ).functions.getA
-00016f60: 6c6c 4c42 5061 6972 7328 5f74 6f6b 656e  llLBPairs(_token
-00016f70: 5f61 2c5f 746f 6b65 6e5f 6229 2e63 616c  _a,_token_b).cal
-00016f80: 6c28 290a 0a20 2020 2064 6566 2067 6574  l()..    def get
-00016f90: 5f61 6c6c 5f62 696e 5f73 7465 7073 285f  _all_bin_steps(_
-00016fa0: 7765 6233 3a57 6562 332c 5f66 6163 746f  web3:Web3,_facto
-00016fb0: 7279 5f61 6464 7265 7373 293a 0a20 2020  ry_address):.   
-00016fc0: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
-00016fd0: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
-00016fe0: 6464 7265 7373 3d5f 6661 6374 6f72 795f  ddress=_factory_
-00016ff0: 6164 6472 6573 732c 2061 6269 3d4a 6f65  address, abi=Joe
-00017000: 5632 4661 6374 6f72 792e 6a6f 655f 6661  V2Factory.joe_fa
-00017010: 6374 6f72 795f 7632 5f61 6269 292e 6675  ctory_v2_abi).fu
-00017020: 6e63 7469 6f6e 732e 6765 7441 6c6c 4269  nctions.getAllBi
-00017030: 6e53 7465 7073 2829 2e63 616c 6c28 290a  nSteps().call().
-00017040: 0a63 6c61 7373 204a 6f65 5632 5175 6f74  .class JoeV2Quot
-00017050: 653a 0a20 2020 206a 6f65 5f71 756f 7465  e:.    joe_quote
-00017060: 5f76 325f 6162 693d 275b 7b22 696e 7075  _v2_abi='[{"inpu
-00017070: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00017080: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-00017090: 6e61 6d65 223a 225f 726f 7574 6572 5632  name":"_routerV2
-000170a0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-000170b0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-000170c0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-000170d0: 616d 6522 3a22 5f66 6163 746f 7279 5631  ame":"_factoryV1
-000170e0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-000170f0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-00017100: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-00017110: 616d 6522 3a22 5f66 6163 746f 7279 5632  ame":"_factoryV2
-00017120: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00017130: 7322 7d5d 2c22 7374 6174 654d 7574 6162  s"}],"stateMutab
-00017140: 696c 6974 7922 3a22 6e6f 6e70 6179 6162  ility":"nonpayab
-00017150: 6c65 222c 2274 7970 6522 3a22 636f 6e73  le","type":"cons
-00017160: 7472 7563 746f 7222 7d2c 7b22 696e 7075  tructor"},{"inpu
-00017170: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00017180: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00017190: 6e61 6d65 223a 2262 7022 2c22 7479 7065  name":"bp","type
-000171a0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-000171b0: 616d 6522 3a22 4269 6e48 656c 7065 725f  ame":"BinHelper_
-000171c0: 5f42 696e 5374 6570 4f76 6572 666c 6f77  _BinStepOverflow
-000171d0: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
-000171e0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-000171f0: 226e 616d 6522 3a22 4269 6e48 656c 7065  "name":"BinHelpe
-00017200: 725f 5f49 644f 7665 7266 6c6f 7773 222c  r__IdOverflows",
-00017210: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-00017220: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-00017230: 6d65 223a 224a 6f65 4c69 6272 6172 795f  me":"JoeLibrary_
-00017240: 5f41 6464 7265 7373 5a65 726f 222c 2274  _AddressZero","t
-00017250: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-00017260: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
-00017270: 223a 224a 6f65 4c69 6272 6172 795f 5f49  ":"JoeLibrary__I
-00017280: 6465 6e74 6963 616c 4164 6472 6573 7365  denticalAddresse
-00017290: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
-000172a0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-000172b0: 226e 616d 6522 3a22 4a6f 654c 6962 7261  "name":"JoeLibra
-000172c0: 7279 5f5f 496e 7375 6666 6963 6965 6e74  ry__Insufficient
-000172d0: 416d 6f75 6e74 222c 2274 7970 6522 3a22  Amount","type":"
-000172e0: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-000172f0: 223a 5b5d 2c22 6e61 6d65 223a 224a 6f65  ":[],"name":"Joe
-00017300: 4c69 6272 6172 795f 5f49 6e73 7566 6669  Library__Insuffi
-00017310: 6369 656e 744c 6971 7569 6469 7479 222c  cientLiquidity",
+00015a30: 616d 6522 3a22 6669 6c74 6572 5065 7269  ame":"filterPeri
+00015a40: 6f64 222c 2274 7970 6522 3a22 7569 6e74  od","type":"uint
+00015a50: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+00015a60: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+00015a70: 226e 616d 6522 3a22 6465 6361 7950 6572  "name":"decayPer
+00015a80: 696f 6422 2c22 7479 7065 223a 2275 696e  iod","type":"uin
+00015a90: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00015aa0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00015ab0: 2c22 6e61 6d65 223a 2272 6564 7563 7469  ,"name":"reducti
+00015ac0: 6f6e 4661 6374 6f72 222c 2274 7970 6522  onFactor","type"
+00015ad0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+00015ae0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00015af0: 7432 3536 222c 226e 616d 6522 3a22 7661  t256","name":"va
+00015b00: 7269 6162 6c65 4665 6543 6f6e 7472 6f6c  riableFeeControl
+00015b10: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00015b20: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+00015b30: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00015b40: 616d 6522 3a22 7072 6f74 6f63 6f6c 5368  ame":"protocolSh
+00015b50: 6172 6522 2c22 7479 7065 223a 2275 696e  are","type":"uin
+00015b60: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00015b70: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00015b80: 2c22 6e61 6d65 223a 226d 6178 566f 6c61  ,"name":"maxVola
+00015b90: 7469 6c69 7479 4163 6375 6d75 6c61 7465  tilityAccumulate
+00015ba0: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
+00015bb0: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+00015bc0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00015bd0: 6e61 6d65 223a 2273 616d 706c 654c 6966  name":"sampleLif
+00015be0: 6574 696d 6522 2c22 7479 7065 223a 2275  etime","type":"u
+00015bf0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
+00015c00: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
+00015c10: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
+00015c20: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+00015c30: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+00015c40: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00015c50: 223a 225f 696e 6465 7822 2c22 7479 7065  ":"_index","type
+00015c60: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+00015c70: 616d 6522 3a22 6765 7451 756f 7465 4173  ame":"getQuoteAs
+00015c80: 7365 7422 2c22 6f75 7470 7574 7322 3a5b  set","outputs":[
+00015c90: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00015ca0: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
+00015cb0: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
+00015cc0: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+00015cd0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00015ce0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
+00015cf0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00015d00: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00015d10: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+00015d20: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
+00015d30: 5f74 6f6b 656e 222c 2274 7970 6522 3a22  _token","type":"
+00015d40: 6164 6472 6573 7322 7d5d 2c22 6e61 6d65  address"}],"name
+00015d50: 223a 2269 7351 756f 7465 4173 7365 7422  ":"isQuoteAsset"
+00015d60: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+00015d70: 7465 726e 616c 5479 7065 223a 2262 6f6f  ternalType":"boo
+00015d80: 6c22 2c22 6e61 6d65 223a 2222 2c22 7479  l","name":"","ty
+00015d90: 7065 223a 2262 6f6f 6c22 7d5d 2c22 7374  pe":"bool"}],"st
+00015da0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00015db0: 7669 6577 222c 2274 7970 6522 3a22 6675  view","type":"fu
+00015dc0: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+00015dd0: 7322 3a5b 5d2c 226e 616d 6522 3a22 6f77  s":[],"name":"ow
+00015de0: 6e65 7222 2c22 6f75 7470 7574 7322 3a5b  ner","outputs":[
+00015df0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00015e00: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00015e10: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
+00015e20: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
+00015e30: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+00015e40: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00015e50: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+00015e60: 226e 616d 6522 3a22 7065 6e64 696e 674f  "name":"pendingO
+00015e70: 776e 6572 222c 226f 7574 7075 7473 223a  wner","outputs":
+00015e80: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+00015e90: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+00015ea0: 223a 2222 2c22 7479 7065 223a 2261 6464  ":"","type":"add
+00015eb0: 7265 7373 227d 5d2c 2273 7461 7465 4d75  ress"}],"stateMu
+00015ec0: 7461 6269 6c69 7479 223a 2276 6965 7722  tability":"view"
+00015ed0: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+00015ee0: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
+00015ef0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00015f00: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
+00015f10: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
+00015f20: 3a22 7569 6e74 3136 227d 5d2c 226e 616d  :"uint16"}],"nam
+00015f30: 6522 3a22 7265 6d6f 7665 5072 6573 6574  e":"removePreset
+00015f40: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
+00015f50: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00015f60: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+00015f70: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00015f80: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00015f90: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+00015fa0: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
+00015fb0: 616d 6522 3a22 5f71 756f 7465 4173 7365  ame":"_quoteAsse
+00015fc0: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
+00015fd0: 7373 227d 5d2c 226e 616d 6522 3a22 7265  ss"}],"name":"re
+00015fe0: 6d6f 7665 5175 6f74 6541 7373 6574 222c  moveQuoteAsset",
+00015ff0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+00016000: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00016010: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+00016020: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00016030: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+00016040: 6522 3a22 7265 6e6f 756e 6365 4f77 6e65  e":"renounceOwne
+00016050: 7273 6869 7022 2c22 6f75 7470 7574 7322  rship","outputs"
+00016060: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
+00016070: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
+00016080: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
+00016090: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+000160a0: 5b5d 2c22 6e61 6d65 223a 2272 6576 6f6b  [],"name":"revok
+000160b0: 6550 656e 6469 6e67 4f77 6e65 7222 2c22  ePendingOwner","
+000160c0: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
+000160d0: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
+000160e0: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
+000160f0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
+00016100: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00016110: 6e61 6c54 7970 6522 3a22 626f 6f6c 222c  nalType":"bool",
+00016120: 226e 616d 6522 3a22 5f6c 6f63 6b65 6422  "name":"_locked"
+00016130: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
+00016140: 2c22 6e61 6d65 223a 2273 6574 4661 6374  ,"name":"setFact
+00016150: 6f72 794c 6f63 6b65 6453 7461 7465 222c  oryLockedState",
+00016160: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+00016170: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00016180: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+00016190: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+000161a0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+000161b0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+000161c0: 7373 222c 226e 616d 6522 3a22 5f66 6565  ss","name":"_fee
+000161d0: 5265 6369 7069 656e 7422 2c22 7479 7065  Recipient","type
+000161e0: 223a 2261 6464 7265 7373 227d 5d2c 226e  ":"address"}],"n
+000161f0: 616d 6522 3a22 7365 7446 6565 5265 6369  ame":"setFeeReci
+00016200: 7069 656e 7422 2c22 6f75 7470 7574 7322  pient","outputs"
+00016210: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
+00016220: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
+00016230: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
+00016240: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+00016250: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+00016260: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
+00016270: 3022 2c22 6e61 6d65 223a 225f 746f 6b65  0","name":"_toke
+00016280: 6e58 222c 2274 7970 6522 3a22 6164 6472  nX","type":"addr
+00016290: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+000162a0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+000162b0: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
+000162c0: 5f74 6f6b 656e 5922 2c22 7479 7065 223a  _tokenY","type":
+000162d0: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+000162e0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+000162f0: 3136 222c 226e 616d 6522 3a22 5f62 696e  16","name":"_bin
+00016300: 5374 6570 222c 2274 7970 6522 3a22 7569  Step","type":"ui
+00016310: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
+00016320: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
+00016330: 226e 616d 6522 3a22 5f62 6173 6546 6163  "name":"_baseFac
+00016340: 746f 7222 2c22 7479 7065 223a 2275 696e  tor","type":"uin
+00016350: 7431 3622 7d2c 7b22 696e 7465 726e 616c  t16"},{"internal
+00016360: 5479 7065 223a 2275 696e 7431 3622 2c22  Type":"uint16","
+00016370: 6e61 6d65 223a 225f 6669 6c74 6572 5065  name":"_filterPe
+00016380: 7269 6f64 222c 2274 7970 6522 3a22 7569  riod","type":"ui
+00016390: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
+000163a0: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
+000163b0: 226e 616d 6522 3a22 5f64 6563 6179 5065  "name":"_decayPe
+000163c0: 7269 6f64 222c 2274 7970 6522 3a22 7569  riod","type":"ui
+000163d0: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
+000163e0: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
+000163f0: 226e 616d 6522 3a22 5f72 6564 7563 7469  "name":"_reducti
+00016400: 6f6e 4661 6374 6f72 222c 2274 7970 6522  onFactor","type"
+00016410: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
+00016420: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00016430: 3234 222c 226e 616d 6522 3a22 5f76 6172  24","name":"_var
+00016440: 6961 626c 6546 6565 436f 6e74 726f 6c22  iableFeeControl"
+00016450: 2c22 7479 7065 223a 2275 696e 7432 3422  ,"type":"uint24"
+00016460: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00016470: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
+00016480: 223a 225f 7072 6f74 6f63 6f6c 5368 6172  ":"_protocolShar
+00016490: 6522 2c22 7479 7065 223a 2275 696e 7431  e","type":"uint1
+000164a0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+000164b0: 7065 223a 2275 696e 7432 3422 2c22 6e61  pe":"uint24","na
+000164c0: 6d65 223a 225f 6d61 7856 6f6c 6174 696c  me":"_maxVolatil
+000164d0: 6974 7941 6363 756d 756c 6174 6564 222c  ityAccumulated",
+000164e0: 2274 7970 6522 3a22 7569 6e74 3234 227d  "type":"uint24"}
+000164f0: 5d2c 226e 616d 6522 3a22 7365 7446 6565  ],"name":"setFee
+00016500: 7350 6172 616d 6574 6572 734f 6e50 6169  sParametersOnPai
+00016510: 7222 2c22 6f75 7470 7574 7322 3a5b 5d2c  r","outputs":[],
+00016520: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00016530: 223a 226e 6f6e 7061 7961 626c 6522 2c22  ":"nonpayable","
+00016540: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00016550: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00016560: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00016570: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
+00016580: 666c 6173 684c 6f61 6e46 6565 222c 2274  flashLoanFee","t
+00016590: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+000165a0: 2c22 6e61 6d65 223a 2273 6574 466c 6173  ,"name":"setFlas
+000165b0: 684c 6f61 6e46 6565 222c 226f 7574 7075  hLoanFee","outpu
+000165c0: 7473 223a 5b5d 2c22 7374 6174 654d 7574  ts":[],"stateMut
+000165d0: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
+000165e0: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
+000165f0: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+00016600: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00016610: 7065 223a 2263 6f6e 7472 6163 7420 4945  pe":"contract IE
+00016620: 5243 3230 222c 226e 616d 6522 3a22 5f74  RC20","name":"_t
+00016630: 6f6b 656e 5822 2c22 7479 7065 223a 2261  okenX","type":"a
+00016640: 6464 7265 7373 227d 2c7b 2269 6e74 6572  ddress"},{"inter
+00016650: 6e61 6c54 7970 6522 3a22 636f 6e74 7261  nalType":"contra
+00016660: 6374 2049 4552 4332 3022 2c22 6e61 6d65  ct IERC20","name
+00016670: 223a 225f 746f 6b65 6e59 222c 2274 7970  ":"_tokenY","typ
+00016680: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+00016690: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000166a0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000166b0: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
+000166c0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+000166d0: 7465 726e 616c 5479 7065 223a 2262 6f6f  ternalType":"boo
+000166e0: 6c22 2c22 6e61 6d65 223a 225f 6967 6e6f  l","name":"_igno
+000166f0: 7265 6422 2c22 7479 7065 223a 2262 6f6f  red","type":"boo
+00016700: 6c22 7d5d 2c22 6e61 6d65 223a 2273 6574  l"}],"name":"set
+00016710: 4c42 5061 6972 4967 6e6f 7265 6422 2c22  LBPairIgnored","
+00016720: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
+00016730: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
+00016740: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
+00016750: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
+00016760: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00016770: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+00016780: 7322 2c22 6e61 6d65 223a 225f 4c42 5061  s","name":"_LBPa
+00016790: 6972 496d 706c 656d 656e 7461 7469 6f6e  irImplementation
+000167a0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000167b0: 7322 7d5d 2c22 6e61 6d65 223a 2273 6574  s"}],"name":"set
+000167c0: 4c42 5061 6972 496d 706c 656d 656e 7461  LBPairImplementa
+000167d0: 7469 6f6e 222c 226f 7574 7075 7473 223a  tion","outputs":
+000167e0: 5b5d 2c22 7374 6174 654d 7574 6162 696c  [],"stateMutabil
+000167f0: 6974 7922 3a22 6e6f 6e70 6179 6162 6c65  ity":"nonpayable
+00016800: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+00016810: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+00016820: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00016830: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00016840: 3a22 7065 6e64 696e 674f 776e 6572 5f22  :"pendingOwner_"
+00016850: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+00016860: 227d 5d2c 226e 616d 6522 3a22 7365 7450  "}],"name":"setP
+00016870: 656e 6469 6e67 4f77 6e65 7222 2c22 6f75  endingOwner","ou
+00016880: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
+00016890: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+000168a0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+000168b0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+000168c0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+000168d0: 6c54 7970 6522 3a22 7569 6e74 3136 222c  lType":"uint16",
+000168e0: 226e 616d 6522 3a22 5f62 696e 5374 6570  "name":"_binStep
+000168f0: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
+00016900: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00016910: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
+00016920: 6522 3a22 5f62 6173 6546 6163 746f 7222  e":"_baseFactor"
+00016930: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
+00016940: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00016950: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
+00016960: 223a 225f 6669 6c74 6572 5065 7269 6f64  ":"_filterPeriod
+00016970: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
+00016980: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00016990: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
+000169a0: 6522 3a22 5f64 6563 6179 5065 7269 6f64  e":"_decayPeriod
+000169b0: 222c 2274 7970 6522 3a22 7569 6e74 3136  ","type":"uint16
+000169c0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+000169d0: 6522 3a22 7569 6e74 3136 222c 226e 616d  e":"uint16","nam
+000169e0: 6522 3a22 5f72 6564 7563 7469 6f6e 4661  e":"_reductionFa
+000169f0: 6374 6f72 222c 2274 7970 6522 3a22 7569  ctor","type":"ui
+00016a00: 6e74 3136 227d 2c7b 2269 6e74 6572 6e61  nt16"},{"interna
+00016a10: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
+00016a20: 226e 616d 6522 3a22 5f76 6172 6961 626c  "name":"_variabl
+00016a30: 6546 6565 436f 6e74 726f 6c22 2c22 7479  eFeeControl","ty
+00016a40: 7065 223a 2275 696e 7432 3422 7d2c 7b22  pe":"uint24"},{"
+00016a50: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00016a60: 696e 7431 3622 2c22 6e61 6d65 223a 225f  int16","name":"_
+00016a70: 7072 6f74 6f63 6f6c 5368 6172 6522 2c22  protocolShare","
+00016a80: 7479 7065 223a 2275 696e 7431 3622 7d2c  type":"uint16"},
+00016a90: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00016aa0: 2275 696e 7432 3422 2c22 6e61 6d65 223a  "uint24","name":
+00016ab0: 225f 6d61 7856 6f6c 6174 696c 6974 7941  "_maxVolatilityA
+00016ac0: 6363 756d 756c 6174 6564 222c 2274 7970  ccumulated","typ
+00016ad0: 6522 3a22 7569 6e74 3234 227d 2c7b 2269  e":"uint24"},{"i
+00016ae0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00016af0: 6e74 3136 222c 226e 616d 6522 3a22 5f73  nt16","name":"_s
+00016b00: 616d 706c 654c 6966 6574 696d 6522 2c22  ampleLifetime","
+00016b10: 7479 7065 223a 2275 696e 7431 3622 7d5d  type":"uint16"}]
+00016b20: 2c22 6e61 6d65 223a 2273 6574 5072 6573  ,"name":"setPres
+00016b30: 6574 222c 226f 7574 7075 7473 223a 5b5d  et","outputs":[]
+00016b40: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+00016b50: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
+00016b60: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00016b70: 227d 5d27 290a 0a20 2020 2023 6a6f 6520  "}]')..    #joe 
+00016b80: 6661 636f 7472 790a 2020 2020 6465 6620  facotry.    def 
+00016b90: 6765 745f 6e75 6d62 6572 5f6f 665f 6c62  get_number_of_lb
+00016ba0: 5f70 6169 7273 285f 7765 6233 3a57 6562  _pairs(_web3:Web
+00016bb0: 332c 5f66 6163 746f 7279 5f61 6464 7265  3,_factory_addre
+00016bc0: 7373 293a 0a20 2020 2020 2020 2072 6574  ss):.        ret
+00016bd0: 7572 6e20 5f77 6562 332e 6574 682e 636f  urn _web3.eth.co
+00016be0: 6e74 7261 6374 2861 6464 7265 7373 3d5f  ntract(address=_
+00016bf0: 6661 6374 6f72 795f 6164 6472 6573 732c  factory_address,
+00016c00: 2061 6269 3d4a 6f65 5632 4661 6374 6f72   abi=JoeV2Factor
+00016c10: 792e 6a6f 655f 6661 6374 6f72 795f 7632  y.joe_factory_v2
+00016c20: 5f61 6269 292e 6675 6e63 7469 6f6e 732e  _abi).functions.
+00016c30: 6765 744e 756d 6265 724f 664c 4250 6169  getNumberOfLBPai
+00016c40: 7273 2829 2e63 616c 6c28 290a 0a20 2020  rs().call()..   
+00016c50: 2064 6566 2067 6574 5f6e 756d 6265 725f   def get_number_
+00016c60: 6f66 5f71 756f 7465 5f61 7373 6574 7328  of_quote_assets(
+00016c70: 5f77 6562 333a 5765 6233 2c5f 6661 6374  _web3:Web3,_fact
+00016c80: 6f72 795f 6164 6472 6573 7329 3a0a 2020  ory_address):.  
+00016c90: 2020 2020 2020 7265 7475 726e 205f 7765        return _we
+00016ca0: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
+00016cb0: 6164 6472 6573 733d 5f66 6163 746f 7279  address=_factory
+00016cc0: 5f61 6464 7265 7373 2c20 6162 693d 4a6f  _address, abi=Jo
+00016cd0: 6556 3246 6163 746f 7279 2e6a 6f65 5f66  eV2Factory.joe_f
+00016ce0: 6163 746f 7279 5f76 325f 6162 6929 2e66  actory_v2_abi).f
+00016cf0: 756e 6374 696f 6e73 2e67 6574 4e75 6d62  unctions.getNumb
+00016d00: 6572 4f66 5175 6f74 6541 7373 6574 7328  erOfQuoteAssets(
+00016d10: 292e 6361 6c6c 2829 0a0a 2020 2020 6465  ).call()..    de
+00016d20: 6620 6765 745f 7175 6f74 655f 6173 7365  f get_quote_asse
+00016d30: 7428 5f77 6562 333a 5765 6233 2c5f 6661  t(_web3:Web3,_fa
+00016d40: 6374 6f72 795f 6164 6472 6573 732c 5f69  ctory_address,_i
+00016d50: 6e64 6578 293a 0a20 2020 2020 2020 2072  ndex):.        r
+00016d60: 6574 7572 6e20 5f77 6562 332e 6574 682e  eturn _web3.eth.
+00016d70: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
+00016d80: 3d5f 6661 6374 6f72 795f 6164 6472 6573  =_factory_addres
+00016d90: 732c 2061 6269 3d4a 6f65 5632 4661 6374  s, abi=JoeV2Fact
+00016da0: 6f72 792e 6a6f 655f 6661 6374 6f72 795f  ory.joe_factory_
+00016db0: 7632 5f61 6269 292e 6675 6e63 7469 6f6e  v2_abi).function
+00016dc0: 732e 6765 7451 756f 7465 4173 7365 7428  s.getQuoteAsset(
+00016dd0: 5f69 6e64 6578 292e 6361 6c6c 2829 0a0a  _index).call()..
+00016de0: 2020 2020 6465 6620 6973 5f71 756f 7465      def is_quote
+00016df0: 5f61 7373 6574 285f 7765 6233 3a57 6562  _asset(_web3:Web
+00016e00: 332c 5f66 6163 746f 7279 5f61 6464 7265  3,_factory_addre
+00016e10: 7373 2c5f 6164 6472 6573 733a 7374 7229  ss,_address:str)
+00016e20: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+00016e30: 205f 7765 6233 2e65 7468 2e63 6f6e 7472   _web3.eth.contr
+00016e40: 6163 7428 6164 6472 6573 733d 5f66 6163  act(address=_fac
+00016e50: 746f 7279 5f61 6464 7265 7373 2c20 6162  tory_address, ab
+00016e60: 693d 4a6f 6556 3246 6163 746f 7279 2e6a  i=JoeV2Factory.j
+00016e70: 6f65 5f66 6163 746f 7279 5f76 325f 6162  oe_factory_v2_ab
+00016e80: 6929 2e66 756e 6374 696f 6e73 2e69 7351  i).functions.isQ
+00016e90: 756f 7465 4173 7365 7428 5f61 6464 7265  uoteAsset(_addre
+00016ea0: 7373 292e 6361 6c6c 2829 0a0a 2020 2020  ss).call()..    
+00016eb0: 6465 6620 6765 745f 7061 6972 5f69 6e66  def get_pair_inf
+00016ec0: 6f72 6d61 7469 6f6e 285f 7765 6233 3a57  ormation(_web3:W
+00016ed0: 6562 332c 5f66 6163 746f 7279 5f61 6464  eb3,_factory_add
+00016ee0: 7265 7373 2c5f 746f 6b65 6e5f 613a 7374  ress,_token_a:st
+00016ef0: 722c 5f74 6f6b 656e 5f62 3a73 7472 2c5f  r,_token_b:str,_
+00016f00: 6269 6e5f 7374 6570 293a 0a20 2020 2020  bin_step):.     
+00016f10: 2020 2072 6574 7572 6e20 5f77 6562 332e     return _web3.
+00016f20: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
+00016f30: 7265 7373 3d5f 6661 6374 6f72 795f 6164  ress=_factory_ad
+00016f40: 6472 6573 732c 2061 6269 3d4a 6f65 5632  dress, abi=JoeV2
+00016f50: 4661 6374 6f72 792e 6a6f 655f 6661 6374  Factory.joe_fact
+00016f60: 6f72 795f 7632 5f61 6269 292e 6675 6e63  ory_v2_abi).func
+00016f70: 7469 6f6e 732e 6765 744c 4250 6169 7249  tions.getLBPairI
+00016f80: 6e66 6f72 6d61 7469 6f6e 285f 746f 6b65  nformation(_toke
+00016f90: 6e5f 612c 5f74 6f6b 656e 5f62 2c5f 6269  n_a,_token_b,_bi
+00016fa0: 6e5f 7374 6570 292e 6361 6c6c 2829 0a0a  n_step).call()..
+00016fb0: 2020 2020 6465 6620 6765 745f 616c 6c5f      def get_all_
+00016fc0: 6c62 5f70 6169 7273 285f 7765 6233 3a57  lb_pairs(_web3:W
+00016fd0: 6562 332c 5f66 6163 746f 7279 5f61 6464  eb3,_factory_add
+00016fe0: 7265 7373 2c5f 746f 6b65 6e5f 613a 7374  ress,_token_a:st
+00016ff0: 722c 5f74 6f6b 656e 5f62 3a73 7472 293a  r,_token_b:str):
+00017000: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00017010: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
+00017020: 6374 2861 6464 7265 7373 3d5f 6661 6374  ct(address=_fact
+00017030: 6f72 795f 6164 6472 6573 732c 2061 6269  ory_address, abi
+00017040: 3d4a 6f65 5632 4661 6374 6f72 792e 6a6f  =JoeV2Factory.jo
+00017050: 655f 6661 6374 6f72 795f 7632 5f61 6269  e_factory_v2_abi
+00017060: 292e 6675 6e63 7469 6f6e 732e 6765 7441  ).functions.getA
+00017070: 6c6c 4c42 5061 6972 7328 5f74 6f6b 656e  llLBPairs(_token
+00017080: 5f61 2c5f 746f 6b65 6e5f 6229 2e63 616c  _a,_token_b).cal
+00017090: 6c28 290a 0a20 2020 2064 6566 2067 6574  l()..    def get
+000170a0: 5f61 6c6c 5f62 696e 5f73 7465 7073 285f  _all_bin_steps(_
+000170b0: 7765 6233 3a57 6562 332c 5f66 6163 746f  web3:Web3,_facto
+000170c0: 7279 5f61 6464 7265 7373 293a 0a20 2020  ry_address):.   
+000170d0: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
+000170e0: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
+000170f0: 6464 7265 7373 3d5f 6661 6374 6f72 795f  ddress=_factory_
+00017100: 6164 6472 6573 732c 2061 6269 3d4a 6f65  address, abi=Joe
+00017110: 5632 4661 6374 6f72 792e 6a6f 655f 6661  V2Factory.joe_fa
+00017120: 6374 6f72 795f 7632 5f61 6269 292e 6675  ctory_v2_abi).fu
+00017130: 6e63 7469 6f6e 732e 6765 7441 6c6c 4269  nctions.getAllBi
+00017140: 6e53 7465 7073 2829 2e63 616c 6c28 290a  nSteps().call().
+00017150: 0a63 6c61 7373 204a 6f65 5632 5175 6f74  .class JoeV2Quot
+00017160: 653a 0a20 2020 206a 6f65 5f71 756f 7465  e:.    joe_quote
+00017170: 5f76 325f 6162 693d 275b 7b22 696e 7075  _v2_abi='[{"inpu
+00017180: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00017190: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+000171a0: 6e61 6d65 223a 225f 726f 7574 6572 5632  name":"_routerV2
+000171b0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000171c0: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+000171d0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+000171e0: 616d 6522 3a22 5f66 6163 746f 7279 5631  ame":"_factoryV1
+000171f0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00017200: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+00017210: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+00017220: 616d 6522 3a22 5f66 6163 746f 7279 5632  ame":"_factoryV2
+00017230: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00017240: 7322 7d5d 2c22 7374 6174 654d 7574 6162  s"}],"stateMutab
+00017250: 696c 6974 7922 3a22 6e6f 6e70 6179 6162  ility":"nonpayab
+00017260: 6c65 222c 2274 7970 6522 3a22 636f 6e73  le","type":"cons
+00017270: 7472 7563 746f 7222 7d2c 7b22 696e 7075  tructor"},{"inpu
+00017280: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00017290: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+000172a0: 6e61 6d65 223a 2262 7022 2c22 7479 7065  name":"bp","type
+000172b0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+000172c0: 616d 6522 3a22 4269 6e48 656c 7065 725f  ame":"BinHelper_
+000172d0: 5f42 696e 5374 6570 4f76 6572 666c 6f77  _BinStepOverflow
+000172e0: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
+000172f0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+00017300: 226e 616d 6522 3a22 4269 6e48 656c 7065  "name":"BinHelpe
+00017310: 725f 5f49 644f 7665 7266 6c6f 7773 222c  r__IdOverflows",
 00017320: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
 00017330: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-00017340: 6d65 223a 224c 4251 756f 7465 725f 496e  me":"LBQuoter_In
-00017350: 7661 6c69 644c 656e 6774 6822 2c22 7479  validLength","ty
-00017360: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-00017370: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00017380: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00017390: 222c 226e 616d 6522 3a22 7822 2c22 7479  ","name":"x","ty
-000173a0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-000173b0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000173c0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-000173d0: 7922 2c22 7479 7065 223a 2269 6e74 3235  y","type":"int25
-000173e0: 3622 7d5d 2c22 6e61 6d65 223a 224d 6174  6"}],"name":"Mat
-000173f0: 6831 3238 7831 3238 5f5f 506f 7765 7255  h128x128__PowerU
-00017400: 6e64 6572 666c 6f77 222c 2274 7970 6522  nderflow","type"
-00017410: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00017420: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00017430: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00017440: 6e61 6d65 223a 2270 726f 6431 222c 2274  name":"prod1","t
-00017450: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-00017460: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00017470: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-00017480: 3a22 6465 6e6f 6d69 6e61 746f 7222 2c22  :"denominator","
-00017490: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-000174a0: 5d2c 226e 616d 6522 3a22 4d61 7468 3531  ],"name":"Math51
-000174b0: 3242 6974 735f 5f4d 756c 4469 764f 7665  2Bits__MulDivOve
-000174c0: 7266 6c6f 7722 2c22 7479 7065 223a 2265  rflow","type":"e
-000174d0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-000174e0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-000174f0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00017500: 6522 3a22 7072 6f64 3122 2c22 7479 7065  e":"prod1","type
-00017510: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-00017520: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00017530: 6e74 3235 3622 2c22 6e61 6d65 223a 226f  nt256","name":"o
-00017540: 6666 7365 7422 2c22 7479 7065 223a 2275  ffset","type":"u
-00017550: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-00017560: 3a22 4d61 7468 3531 3242 6974 735f 5f4d  :"Math512Bits__M
-00017570: 756c 5368 6966 744f 7665 7266 6c6f 7722  ulShiftOverflow"
-00017580: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-00017590: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-000175a0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-000175b0: 7432 3536 222c 226e 616d 6522 3a22 6f66  t256","name":"of
-000175c0: 6673 6574 222c 2274 7970 6522 3a22 7569  fset","type":"ui
-000175d0: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-000175e0: 224d 6174 6835 3132 4269 7473 5f5f 4f66  "Math512Bits__Of
-000175f0: 6673 6574 4f76 6572 666c 6f77 7322 2c22  fsetOverflows","
-00017600: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-00017610: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00017620: 6522 3a22 6661 6374 6f72 7956 3122 2c22  e":"factoryV1","
-00017630: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-00017640: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-00017650: 7373 222c 226e 616d 6522 3a22 222c 2274  ss","name":"","t
-00017660: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
-00017670: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00017680: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
-00017690: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-000176a0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-000176b0: 3a22 6661 6374 6f72 7956 3222 2c22 6f75  :"factoryV2","ou
-000176c0: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-000176d0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-000176e0: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-000176f0: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-00017700: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00017710: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-00017720: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00017730: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00017740: 5479 7065 223a 2261 6464 7265 7373 5b5d  Type":"address[]
-00017750: 222c 226e 616d 6522 3a22 5f72 6f75 7465  ","name":"_route
-00017760: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00017770: 735b 5d22 7d2c 7b22 696e 7465 726e 616c  s[]"},{"internal
-00017780: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-00017790: 226e 616d 6522 3a22 5f61 6d6f 756e 7449  "name":"_amountI
-000177a0: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-000177b0: 3536 227d 5d2c 226e 616d 6522 3a22 6669  56"}],"name":"fi
-000177c0: 6e64 4265 7374 5061 7468 4672 6f6d 416d  ndBestPathFromAm
-000177d0: 6f75 6e74 496e 222c 226f 7574 7075 7473  ountIn","outputs
-000177e0: 223a 5b7b 2263 6f6d 706f 6e65 6e74 7322  ":[{"components"
-000177f0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00017800: 223a 2261 6464 7265 7373 5b5d 222c 226e  ":"address[]","n
-00017810: 616d 6522 3a22 726f 7574 6522 2c22 7479  ame":"route","ty
-00017820: 7065 223a 2261 6464 7265 7373 5b5d 227d  pe":"address[]"}
-00017830: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00017840: 3a22 6164 6472 6573 735b 5d22 2c22 6e61  :"address[]","na
-00017850: 6d65 223a 2270 6169 7273 222c 2274 7970  me":"pairs","typ
-00017860: 6522 3a22 6164 6472 6573 735b 5d22 7d2c  e":"address[]"},
-00017870: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00017880: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
-00017890: 6522 3a22 6269 6e53 7465 7073 222c 2274  e":"binSteps","t
-000178a0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-000178b0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-000178c0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
-000178d0: 616d 6522 3a22 616d 6f75 6e74 7322 2c22  ame":"amounts","
-000178e0: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
-000178f0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00017900: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
-00017910: 6e61 6d65 223a 2276 6972 7475 616c 416d  name":"virtualAm
-00017920: 6f75 6e74 7357 6974 686f 7574 536c 6970  ountsWithoutSlip
-00017930: 7061 6765 222c 2274 7970 6522 3a22 7569  page","type":"ui
-00017940: 6e74 3235 365b 5d22 7d2c 7b22 696e 7465  nt256[]"},{"inte
-00017950: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00017960: 3536 5b5d 222c 226e 616d 6522 3a22 6665  56[]","name":"fe
-00017970: 6573 222c 2274 7970 6522 3a22 7569 6e74  es","type":"uint
-00017980: 3235 365b 5d22 7d5d 2c22 696e 7465 726e  256[]"}],"intern
-00017990: 616c 5479 7065 223a 2273 7472 7563 7420  alType":"struct 
-000179a0: 4c42 5175 6f74 6572 2e51 756f 7465 222c  LBQuoter.Quote",
-000179b0: 226e 616d 6522 3a22 7175 6f74 6522 2c22  "name":"quote","
-000179c0: 7479 7065 223a 2274 7570 6c65 227d 5d2c  type":"tuple"}],
-000179d0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-000179e0: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-000179f0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00017a00: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00017a10: 6c54 7970 6522 3a22 6164 6472 6573 735b  lType":"address[
-00017a20: 5d22 2c22 6e61 6d65 223a 225f 726f 7574  ]","name":"_rout
-00017a30: 6522 2c22 7479 7065 223a 2261 6464 7265  e","type":"addre
-00017a40: 7373 5b5d 227d 2c7b 2269 6e74 6572 6e61  ss[]"},{"interna
-00017a50: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00017a60: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
-00017a70: 4f75 7422 2c22 7479 7065 223a 2275 696e  Out","type":"uin
-00017a80: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-00017a90: 6669 6e64 4265 7374 5061 7468 4672 6f6d  findBestPathFrom
-00017aa0: 416d 6f75 6e74 4f75 7422 2c22 6f75 7470  AmountOut","outp
-00017ab0: 7574 7322 3a5b 7b22 636f 6d70 6f6e 656e  uts":[{"componen
-00017ac0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00017ad0: 7970 6522 3a22 6164 6472 6573 735b 5d22  ype":"address[]"
-00017ae0: 2c22 6e61 6d65 223a 2272 6f75 7465 222c  ,"name":"route",
-00017af0: 2274 7970 6522 3a22 6164 6472 6573 735b  "type":"address[
-00017b00: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
-00017b10: 7065 223a 2261 6464 7265 7373 5b5d 222c  pe":"address[]",
-00017b20: 226e 616d 6522 3a22 7061 6972 7322 2c22  "name":"pairs","
-00017b30: 7479 7065 223a 2261 6464 7265 7373 5b5d  type":"address[]
-00017b40: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00017b50: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
-00017b60: 6e61 6d65 223a 2262 696e 5374 6570 7322  name":"binSteps"
-00017b70: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00017b80: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
-00017b90: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-00017ba0: 2c22 6e61 6d65 223a 2261 6d6f 756e 7473  ,"name":"amounts
-00017bb0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00017bc0: 365b 5d22 7d2c 7b22 696e 7465 726e 616c  6[]"},{"internal
-00017bd0: 5479 7065 223a 2275 696e 7432 3536 5b5d  Type":"uint256[]
-00017be0: 222c 226e 616d 6522 3a22 7669 7274 7561  ","name":"virtua
-00017bf0: 6c41 6d6f 756e 7473 5769 7468 6f75 7453  lAmountsWithoutS
-00017c00: 6c69 7070 6167 6522 2c22 7479 7065 223a  lippage","type":
-00017c10: 2275 696e 7432 3536 5b5d 227d 2c7b 2269  "uint256[]"},{"i
-00017c20: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00017c30: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
-00017c40: 2266 6565 7322 2c22 7479 7065 223a 2275  "fees","type":"u
-00017c50: 696e 7432 3536 5b5d 227d 5d2c 2269 6e74  int256[]"}],"int
-00017c60: 6572 6e61 6c54 7970 6522 3a22 7374 7275  ernalType":"stru
-00017c70: 6374 204c 4251 756f 7465 722e 5175 6f74  ct LBQuoter.Quot
-00017c80: 6522 2c22 6e61 6d65 223a 2271 756f 7465  e","name":"quote
-00017c90: 222c 2274 7970 6522 3a22 7475 706c 6522  ","type":"tuple"
-00017ca0: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
-00017cb0: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
-00017cc0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00017cd0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00017ce0: 6522 3a22 726f 7574 6572 5632 222c 226f  e":"routerV2","o
-00017cf0: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-00017d00: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00017d10: 7322 2c22 6e61 6d65 223a 2222 2c22 7479  s","name":"","ty
-00017d20: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
-00017d30: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00017d40: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-00017d50: 2266 756e 6374 696f 6e22 7d5d 270a 0a20  "function"}]'.. 
-00017d60: 2020 2023 7265 7475 726e 2071 756f 7465     #return quote
-00017d70: 0a20 2020 2023 2020 2020 7374 7275 6374  .    #    struct
-00017d80: 2051 756f 7465 207b 0a20 2020 2023 2020   Quote {.    #  
-00017d90: 2020 2061 6464 7265 7373 5b5d 2072 6f75     address[] rou
-00017da0: 7465 3b20 696e 2074 6f6b 656e 20e5 9ca8  te; in token ...
-00017db0: e589 8d0a 2020 2020 2320 2020 2020 6164  ....    #     ad
-00017dc0: 6472 6573 735b 5d20 7061 6972 733b 0a20  dress[] pairs;. 
-00017dd0: 2020 2023 2020 2020 2075 696e 7432 3536     #     uint256
-00017de0: 5b5d 2062 696e 5374 6570 733b 0a20 2020  [] binSteps;.   
-00017df0: 2023 2020 2020 2075 696e 7432 3536 5b5d   #     uint256[]
-00017e00: 2061 6d6f 756e 7473 3b20 e695 b0e7 bb84   amounts; ......
-00017e10: 2ce9 a1ba e5ba 8fe4 b88e e8b7 afe5 be84  ,...............
-00017e20: e4b8 80e8 87b4 0a20 2020 2023 2020 2020  .......    #    
-00017e30: 2075 696e 7432 3536 5b5d 2076 6972 7475   uint256[] virtu
-00017e40: 616c 416d 6f75 6e74 7357 6974 686f 7574  alAmountsWithout
-00017e50: 536c 6970 7061 6765 3b0a 2020 2020 2320  Slippage;.    # 
-00017e60: 2020 2020 7569 6e74 3235 365b 5d20 6665      uint256[] fe
-00017e70: 6573 3b0a 2020 2020 2320 7d0a 2020 2020  es;.    # }.    
-00017e80: 6465 6620 6669 6e64 5f62 6573 745f 7061  def find_best_pa
-00017e90: 7468 5f66 6f72 5f61 6d6f 756e 745f 696e  th_for_amount_in
-00017ea0: 285f 7765 6233 3a57 6562 332c 5f71 756f  (_web3:Web3,_quo
-00017eb0: 7465 5f61 6464 7265 7373 2c5f 7175 6f74  te_address,_quot
-00017ec0: 655f 6162 692c 5f70 6174 682c 5f61 6d6f  e_abi,_path,_amo
-00017ed0: 756e 745f 696e 293a 0a20 2020 2020 2020  unt_in):.       
-00017ee0: 2072 6574 7572 6e20 5f77 6562 332e 6574   return _web3.et
-00017ef0: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
-00017f00: 7373 3d5f 7175 6f74 655f 6164 6472 6573  ss=_quote_addres
-00017f10: 732c 6162 693d 5f71 756f 7465 5f61 6269  s,abi=_quote_abi
-00017f20: 292e 6675 6e63 7469 6f6e 732e 6669 6e64  ).functions.find
-00017f30: 4265 7374 5061 7468 4672 6f6d 416d 6f75  BestPathFromAmou
-00017f40: 6e74 496e 285f 7061 7468 2c5f 616d 6f75  ntIn(_path,_amou
-00017f50: 6e74 5f69 6e29 2e63 616c 6c28 290a 2020  nt_in).call().  
-00017f60: 2020 2372 6574 7572 6e20 7175 6f74 650a    #return quote.
-00017f70: 2020 2020 2320 2020 2073 7472 7563 7420      #    struct 
-00017f80: 5175 6f74 6520 7b0a 2020 2020 2320 2020  Quote {.    #   
-00017f90: 2020 6164 6472 6573 735b 5d20 726f 7574    address[] rout
-00017fa0: 653b 206f 7574 2074 6f6b 656e e59c a8e5  e; out token....
-00017fb0: 898d 0a20 2020 2023 2020 2020 2061 6464  ...    #     add
-00017fc0: 7265 7373 5b5d 2070 6169 7273 3b0a 2020  ress[] pairs;.  
-00017fd0: 2020 2320 2020 2020 7569 6e74 3235 365b    #     uint256[
-00017fe0: 5d20 6269 6e53 7465 7073 3b0a 2020 2020  ] binSteps;.    
-00017ff0: 2320 2020 2020 7569 6e74 3235 365b 5d20  #     uint256[] 
-00018000: 616d 6f75 6e74 733b 0a20 2020 2023 2020  amounts;.    #  
-00018010: 2020 2075 696e 7432 3536 5b5d 2076 6972     uint256[] vir
-00018020: 7475 616c 416d 6f75 6e74 7357 6974 686f  tualAmountsWitho
-00018030: 7574 536c 6970 7061 6765 3b0a 2020 2020  utSlippage;.    
-00018040: 2320 2020 2020 7569 6e74 3235 365b 5d20  #     uint256[] 
-00018050: 6665 6573 3b0a 2020 2020 2320 7d0a 2020  fees;.    # }.  
-00018060: 2020 6465 6620 6669 6e64 5f62 6573 745f    def find_best_
-00018070: 7061 7468 5f66 6f72 5f61 6d6f 756e 745f  path_for_amount_
-00018080: 6f75 7428 5f77 6562 333a 5765 6233 2c5f  out(_web3:Web3,_
-00018090: 7175 6f74 655f 6164 6472 6573 732c 5f71  quote_address,_q
-000180a0: 756f 7465 5f61 6269 2c5f 7061 7468 2c5f  uote_abi,_path,_
-000180b0: 616d 6f75 6e74 5f6f 7574 293a 0a20 2020  amount_out):.   
-000180c0: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
-000180d0: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
-000180e0: 6464 7265 7373 3d5f 7175 6f74 655f 6164  ddress=_quote_ad
-000180f0: 6472 6573 732c 6162 693d 5f71 756f 7465  dress,abi=_quote
-00018100: 5f61 6269 292e 6675 6e63 7469 6f6e 732e  _abi).functions.
-00018110: 6669 6e64 4265 7374 5061 7468 4672 6f6d  findBestPathFrom
-00018120: 416d 6f75 6e74 496e 285f 7061 7468 2c5f  AmountIn(_path,_
-00018130: 616d 6f75 6e74 5f6f 7574 292e 6361 6c6c  amount_out).call
-00018140: 2829 0a0a 0a63 6c61 7373 204a 6f65 5632  ()...class JoeV2
-00018150: 4572 6332 303a 0a20 2020 206a 6f65 5f65  Erc20:.    joe_e
-00018160: 7263 3230 5f61 6269 3d27 5b20 7b20 2261  rc20_abi='[ { "a
-00018170: 6e6f 6e79 6d6f 7573 223a 2066 616c 7365  nonymous": false
-00018180: 2c20 2269 6e70 7574 7322 3a20 5b20 7b20  , "inputs": [ { 
-00018190: 2269 6e64 6578 6564 223a 2074 7275 652c  "indexed": true,
-000181a0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-000181b0: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
-000181c0: 6522 3a20 226f 776e 6572 222c 2022 7479  e": "owner", "ty
-000181d0: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
-000181e0: 2c20 7b20 2269 6e64 6578 6564 223a 2074  , { "indexed": t
-000181f0: 7275 652c 2022 696e 7465 726e 616c 5479  rue, "internalTy
-00018200: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
-00018210: 226e 616d 6522 3a20 2273 7065 6e64 6572  "name": "spender
-00018220: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
-00018230: 6573 7322 207d 2c20 7b20 2269 6e64 6578  ess" }, { "index
-00018240: 6564 223a 2066 616c 7365 2c20 2269 6e74  ed": false, "int
-00018250: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
-00018260: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
-00018270: 7661 6c75 6522 2c20 2274 7970 6522 3a20  value", "type": 
-00018280: 2275 696e 7432 3536 2220 7d20 5d2c 2022  "uint256" } ], "
-00018290: 6e61 6d65 223a 2022 4170 7072 6f76 616c  name": "Approval
-000182a0: 222c 2022 7479 7065 223a 2022 6576 656e  ", "type": "even
-000182b0: 7422 207d 2c20 7b20 2261 6e6f 6e79 6d6f  t" }, { "anonymo
-000182c0: 7573 223a 2066 616c 7365 2c20 2269 6e70  us": false, "inp
-000182d0: 7574 7322 3a20 5b20 7b20 2269 6e64 6578  uts": [ { "index
-000182e0: 6564 223a 2074 7275 652c 2022 696e 7465  ed": true, "inte
-000182f0: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
-00018300: 6573 7322 2c20 226e 616d 6522 3a20 2266  ess", "name": "f
-00018310: 726f 6d22 2c20 2274 7970 6522 3a20 2261  rom", "type": "a
-00018320: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
-00018330: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
-00018340: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
-00018350: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
-00018360: 2022 746f 222c 2022 7479 7065 223a 2022   "to", "type": "
-00018370: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
-00018380: 6e64 6578 6564 223a 2066 616c 7365 2c20  ndexed": false, 
-00018390: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
-000183a0: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
-000183b0: 223a 2022 7661 6c75 6522 2c20 2274 7970  ": "value", "typ
-000183c0: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
-000183d0: 5d2c 2022 6e61 6d65 223a 2022 5472 616e  ], "name": "Tran
-000183e0: 7366 6572 222c 2022 7479 7065 223a 2022  sfer", "type": "
-000183f0: 6576 656e 7422 207d 2c20 7b20 2269 6e70  event" }, { "inp
-00018400: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
-00018410: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
-00018420: 7373 222c 2022 6e61 6d65 223a 2022 6f77  ss", "name": "ow
-00018430: 6e65 7222 2c20 2274 7970 6522 3a20 2261  ner", "type": "a
-00018440: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
-00018450: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
-00018460: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
-00018470: 2273 7065 6e64 6572 222c 2022 7479 7065  "spender", "type
-00018480: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
-00018490: 2c20 226e 616d 6522 3a20 2261 6c6c 6f77  , "name": "allow
-000184a0: 616e 6365 222c 2022 6f75 7470 7574 7322  ance", "outputs"
-000184b0: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-000184c0: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
-000184d0: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
-000184e0: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
-000184f0: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
-00018500: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
-00018510: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
-00018520: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
-00018530: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-00018540: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
-00018550: 226e 616d 6522 3a20 2273 7065 6e64 6572  "name": "spender
-00018560: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
-00018570: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
-00018580: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
-00018590: 3536 222c 2022 6e61 6d65 223a 2022 7661  56", "name": "va
-000185a0: 6c75 6522 2c20 2274 7970 6522 3a20 2275  lue", "type": "u
-000185b0: 696e 7432 3536 2220 7d20 5d2c 2022 6e61  int256" } ], "na
-000185c0: 6d65 223a 2022 6170 7072 6f76 6522 2c20  me": "approve", 
-000185d0: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
-000185e0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-000185f0: 626f 6f6c 222c 2022 6e61 6d65 223a 2022  bool", "name": "
-00018600: 222c 2022 7479 7065 223a 2022 626f 6f6c  ", "type": "bool
-00018610: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
-00018620: 6162 696c 6974 7922 3a20 226e 6f6e 7061  ability": "nonpa
-00018630: 7961 626c 6522 2c20 2274 7970 6522 3a20  yable", "type": 
-00018640: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
-00018650: 2269 6e70 7574 7322 3a20 5b20 7b20 2269  "inputs": [ { "i
-00018660: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
-00018670: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
-00018680: 2022 6f77 6e65 7222 2c20 2274 7970 6522   "owner", "type"
-00018690: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
-000186a0: 2022 6e61 6d65 223a 2022 6261 6c61 6e63   "name": "balanc
-000186b0: 654f 6622 2c20 226f 7574 7075 7473 223a  eOf", "outputs":
-000186c0: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
-000186d0: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
-000186e0: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-000186f0: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
-00018700: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
-00018710: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
-00018720: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
-00018730: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
-00018740: 5b5d 2c20 226e 616d 6522 3a20 2264 6563  [], "name": "dec
-00018750: 696d 616c 7322 2c20 226f 7574 7075 7473  imals", "outputs
-00018760: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-00018770: 5479 7065 223a 2022 7569 6e74 3822 2c20  Type": "uint8", 
-00018780: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
-00018790: 6522 3a20 2275 696e 7438 2220 7d20 5d2c  e": "uint8" } ],
-000187a0: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
-000187b0: 7922 3a20 2276 6965 7722 2c20 2274 7970  y": "view", "typ
-000187c0: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
-000187d0: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
-000187e0: 2c20 226e 616d 6522 3a20 226e 616d 6522  , "name": "name"
-000187f0: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
-00018800: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-00018810: 2022 7374 7269 6e67 222c 2022 6e61 6d65   "string", "name
-00018820: 223a 2022 222c 2022 7479 7065 223a 2022  ": "", "type": "
-00018830: 7374 7269 6e67 2220 7d20 5d2c 2022 7374  string" } ], "st
-00018840: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
-00018850: 2276 6965 7722 2c20 2274 7970 6522 3a20  "view", "type": 
-00018860: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
-00018870: 2269 6e70 7574 7322 3a20 5b5d 2c20 226e  "inputs": [], "n
-00018880: 616d 6522 3a20 2273 796d 626f 6c22 2c20  ame": "symbol", 
-00018890: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
-000188a0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
-000188b0: 7374 7269 6e67 222c 2022 6e61 6d65 223a  string", "name":
-000188c0: 2022 222c 2022 7479 7065 223a 2022 7374   "", "type": "st
-000188d0: 7269 6e67 2220 7d20 5d2c 2022 7374 6174  ring" } ], "stat
-000188e0: 654d 7574 6162 696c 6974 7922 3a20 2276  eMutability": "v
-000188f0: 6965 7722 2c20 2274 7970 6522 3a20 2266  iew", "type": "f
-00018900: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
-00018910: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
-00018920: 6522 3a20 2274 6f74 616c 5375 7070 6c79  e": "totalSupply
-00018930: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
-00018940: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-00018950: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
-00018960: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
-00018970: 2022 7569 6e74 3235 3622 207d 205d 2c20   "uint256" } ], 
-00018980: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00018990: 223a 2022 7669 6577 222c 2022 7479 7065  ": "view", "type
-000189a0: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
-000189b0: 207b 2022 696e 7075 7473 223a 205b 207b   { "inputs": [ {
-000189c0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-000189d0: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
-000189e0: 6522 3a20 2274 6f22 2c20 2274 7970 6522  e": "to", "type"
-000189f0: 3a20 2261 6464 7265 7373 2220 7d2c 207b  : "address" }, {
-00018a00: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
-00018a10: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
-00018a20: 6522 3a20 2276 616c 7565 222c 2022 7479  e": "value", "ty
-00018a30: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
-00018a40: 205d 2c20 226e 616d 6522 3a20 2274 7261   ], "name": "tra
-00018a50: 6e73 6665 7222 2c20 226f 7574 7075 7473  nsfer", "outputs
-00018a60: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
-00018a70: 5479 7065 223a 2022 626f 6f6c 222c 2022  Type": "bool", "
-00018a80: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
-00018a90: 223a 2022 626f 6f6c 2220 7d20 5d2c 2022  ": "bool" } ], "
-00018aa0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00018ab0: 3a20 226e 6f6e 7061 7961 626c 6522 2c20  : "nonpayable", 
-00018ac0: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
-00018ad0: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
-00018ae0: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
-00018af0: 7970 6522 3a20 2261 6464 7265 7373 222c  ype": "address",
-00018b00: 2022 6e61 6d65 223a 2022 6672 6f6d 222c   "name": "from",
-00018b10: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
-00018b20: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
-00018b30: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
-00018b40: 222c 2022 6e61 6d65 223a 2022 746f 222c  ", "name": "to",
-00018b50: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
-00018b60: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
-00018b70: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
-00018b80: 222c 2022 6e61 6d65 223a 2022 7661 6c75  ", "name": "valu
-00018b90: 6522 2c20 2274 7970 6522 3a20 2275 696e  e", "type": "uin
-00018ba0: 7432 3536 2220 7d20 5d2c 2022 6e61 6d65  t256" } ], "name
-00018bb0: 223a 2022 7472 616e 7366 6572 4672 6f6d  ": "transferFrom
-00018bc0: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
-00018bd0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
-00018be0: 3a20 2262 6f6f 6c22 2c20 226e 616d 6522  : "bool", "name"
-00018bf0: 3a20 2222 2c20 2274 7970 6522 3a20 2262  : "", "type": "b
-00018c00: 6f6f 6c22 207d 205d 2c20 2273 7461 7465  ool" } ], "state
-00018c10: 4d75 7461 6269 6c69 7479 223a 2022 6e6f  Mutability": "no
-00018c20: 6e70 6179 6162 6c65 222c 2022 7479 7065  npayable", "type
-00018c30: 223a 2022 6675 6e63 7469 6f6e 2220 7d20  ": "function" } 
-00018c40: 5d27 2020 0a0a 636c 6173 7320 4a6f 6556  ]'  ..class JoeV
-00018c50: 3252 6f75 7465 3a0a 2020 2020 6a6f 655f  2Route:.    joe_
-00018c60: 726f 7574 655f 7632 5f61 6269 3d6a 736f  route_v2_abi=jso
-00018c70: 6e2e 6c6f 6164 7328 275b 7b22 696e 7075  n.loads('[{"inpu
-00018c80: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00018c90: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-00018ca0: 4c42 4661 6374 6f72 7922 2c22 6e61 6d65  LBFactory","name
-00018cb0: 223a 225f 6661 6374 6f72 7922 2c22 7479  ":"_factory","ty
-00018cc0: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-00018cd0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00018ce0: 636f 6e74 7261 6374 2049 4a6f 6546 6163  contract IJoeFac
-00018cf0: 746f 7279 222c 226e 616d 6522 3a22 5f6f  tory","name":"_o
-00018d00: 6c64 4661 6374 6f72 7922 2c22 7479 7065  ldFactory","type
-00018d10: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-00018d20: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
-00018d30: 6e74 7261 6374 2049 5741 5641 5822 2c22  ntract IWAVAX","
-00018d40: 6e61 6d65 223a 225f 7761 7661 7822 2c22  name":"_wavax","
-00018d50: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-00018d60: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-00018d70: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
-00018d80: 2c22 7479 7065 223a 2263 6f6e 7374 7275  ,"type":"constru
-00018d90: 6374 6f72 227d 2c7b 2269 6e70 7574 7322  ctor"},{"inputs"
-00018da0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00018db0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00018dc0: 6522 3a22 6270 222c 2274 7970 6522 3a22  e":"bp","type":"
-00018dd0: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
-00018de0: 223a 2242 696e 4865 6c70 6572 5f5f 4269  ":"BinHelper__Bi
-00018df0: 6e53 7465 704f 7665 7266 6c6f 7773 222c  nStepOverflows",
-00018e00: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-00018e10: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-00018e20: 6d65 223a 2242 696e 4865 6c70 6572 5f5f  me":"BinHelper__
-00018e30: 4964 4f76 6572 666c 6f77 7322 2c22 7479  IdOverflows","ty
-00018e40: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-00018e50: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-00018e60: 3a22 4a6f 654c 6962 7261 7279 5f5f 496e  :"JoeLibrary__In
-00018e70: 7375 6666 6963 6965 6e74 416d 6f75 6e74  sufficientAmount
-00018e80: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-00018e90: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-00018ea0: 6e61 6d65 223a 224a 6f65 4c69 6272 6172  name":"JoeLibrar
-00018eb0: 795f 5f49 6e73 7566 6669 6369 656e 744c  y__InsufficientL
-00018ec0: 6971 7569 6469 7479 222c 2274 7970 6522  iquidity","type"
-00018ed0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00018ee0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00018ef0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00018f00: 6e61 6d65 223a 2261 6d6f 756e 7458 4d69  name":"amountXMi
-00018f10: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-00018f20: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-00018f30: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00018f40: 6e61 6d65 223a 2261 6d6f 756e 7458 222c  name":"amountX",
-00018f50: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00018f60: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00018f70: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00018f80: 6522 3a22 616d 6f75 6e74 594d 696e 222c  e":"amountYMin",
-00018f90: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00018fa0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00018fb0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00018fc0: 6522 3a22 616d 6f75 6e74 5922 2c22 7479  e":"amountY","ty
-00018fd0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-00018fe0: 226e 616d 6522 3a22 4c42 526f 7574 6572  "name":"LBRouter
-00018ff0: 5f5f 416d 6f75 6e74 536c 6970 7061 6765  __AmountSlippage
-00019000: 4361 7567 6874 222c 2274 7970 6522 3a22  Caught","type":"
-00019010: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00019020: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00019030: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00019040: 6d65 223a 2269 6422 2c22 7479 7065 223a  me":"id","type":
-00019050: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-00019060: 6522 3a22 4c42 526f 7574 6572 5f5f 4269  e":"LBRouter__Bi
-00019070: 6e52 6573 6572 7665 4f76 6572 666c 6f77  nReserveOverflow
-00019080: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
-00019090: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-000190a0: 226e 616d 6522 3a22 4c42 526f 7574 6572  "name":"LBRouter
-000190b0: 5f5f 4272 6f6b 656e 5377 6170 5361 6665  __BrokenSwapSafe
-000190c0: 7479 4368 6563 6b22 2c22 7479 7065 223a  tyCheck","type":
-000190d0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-000190e0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-000190f0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00019100: 616d 6522 3a22 6465 6164 6c69 6e65 222c  ame":"deadline",
-00019110: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00019120: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00019130: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00019140: 6522 3a22 6375 7272 656e 7454 696d 6573  e":"currentTimes
-00019150: 7461 6d70 222c 2274 7970 6522 3a22 7569  tamp","type":"ui
-00019160: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-00019170: 224c 4252 6f75 7465 725f 5f44 6561 646c  "LBRouter__Deadl
-00019180: 696e 6545 7863 6565 6465 6422 2c22 7479  ineExceeded","ty
-00019190: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-000191a0: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-000191b0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-000191c0: 222c 226e 616d 6522 3a22 7265 6369 7069  ","name":"recipi
-000191d0: 656e 7422 2c22 7479 7065 223a 2261 6464  ent","type":"add
-000191e0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-000191f0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00019200: 2c22 6e61 6d65 223a 2261 6d6f 756e 7422  ,"name":"amount"
-00019210: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00019220: 227d 5d2c 226e 616d 6522 3a22 4c42 526f  "}],"name":"LBRo
-00019230: 7574 6572 5f5f 4661 696c 6564 546f 5365  uter__FailedToSe
-00019240: 6e64 4156 4158 222c 2274 7970 6522 3a22  ndAVAX","type":"
-00019250: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00019260: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00019270: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00019280: 6d65 223a 2269 6444 6573 6972 6564 222c  me":"idDesired",
-00019290: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-000192a0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-000192b0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-000192c0: 6522 3a22 6964 536c 6970 7061 6765 222c  e":"idSlippage",
-000192d0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-000192e0: 7d5d 2c22 6e61 6d65 223a 224c 4252 6f75  }],"name":"LBRou
-000192f0: 7465 725f 5f49 6444 6573 6972 6564 4f76  ter__IdDesiredOv
-00019300: 6572 666c 6f77 7322 2c22 7479 7065 223a  erflows","type":
-00019310: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00019320: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00019330: 7065 223a 2269 6e74 3235 3622 2c22 6e61  pe":"int256","na
-00019340: 6d65 223a 2269 6422 2c22 7479 7065 223a  me":"id","type":
-00019350: 2269 6e74 3235 3622 7d5d 2c22 6e61 6d65  "int256"}],"name
-00019360: 223a 224c 4252 6f75 7465 725f 5f49 644f  ":"LBRouter__IdO
-00019370: 7665 7266 6c6f 7773 222c 2274 7970 6522  verflows","type"
-00019380: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00019390: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-000193a0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-000193b0: 6e61 6d65 223a 2261 6374 6976 6549 6444  name":"activeIdD
-000193c0: 6573 6972 6564 222c 2274 7970 6522 3a22  esired","type":"
-000193d0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-000193e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-000193f0: 3536 222c 226e 616d 6522 3a22 6964 536c  56","name":"idSl
-00019400: 6970 7061 6765 222c 2274 7970 6522 3a22  ippage","type":"
-00019410: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-00019420: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00019430: 3536 222c 226e 616d 6522 3a22 6163 7469  56","name":"acti
-00019440: 7665 4964 222c 2274 7970 6522 3a22 7569  veId","type":"ui
-00019450: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-00019460: 224c 4252 6f75 7465 725f 5f49 6453 6c69  "LBRouter__IdSli
-00019470: 7070 6167 6543 6175 6768 7422 2c22 7479  ppageCaught","ty
-00019480: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-00019490: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-000194a0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-000194b0: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
-000194c0: 4f75 744d 696e 222c 2274 7970 6522 3a22  OutMin","type":"
-000194d0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-000194e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-000194f0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-00019500: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
-00019510: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-00019520: 3a22 4c42 526f 7574 6572 5f5f 496e 7375  :"LBRouter__Insu
-00019530: 6666 6963 6965 6e74 416d 6f75 6e74 4f75  fficientAmountOu
-00019540: 7422 2c22 7479 7065 223a 2265 7272 6f72  t","type":"error
-00019550: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-00019560: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-00019570: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-00019580: 7772 6f6e 6754 6f6b 656e 222c 2274 7970  wrongToken","typ
-00019590: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-000195a0: 6e61 6d65 223a 224c 4252 6f75 7465 725f  name":"LBRouter_
-000195b0: 5f49 6e76 616c 6964 546f 6b65 6e50 6174  _InvalidTokenPat
-000195c0: 6822 2c22 7479 7065 223a 2265 7272 6f72  h","type":"error
-000195d0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-000195e0: 226e 616d 6522 3a22 4c42 526f 7574 6572  "name":"LBRouter
-000195f0: 5f5f 4c65 6e67 7468 734d 6973 6d61 7463  __LengthsMismatc
-00019600: 6822 2c22 7479 7065 223a 2265 7272 6f72  h","type":"error
-00019610: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-00019620: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00019630: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00019640: 616d 6f75 6e74 496e 4d61 7822 2c22 7479  amountInMax","ty
-00019650: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-00019660: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00019670: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00019680: 2261 6d6f 756e 7449 6e22 2c22 7479 7065  "amountIn","type
-00019690: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-000196a0: 616d 6522 3a22 4c42 526f 7574 6572 5f5f  ame":"LBRouter__
-000196b0: 4d61 7841 6d6f 756e 7449 6e45 7863 6565  MaxAmountInExcee
-000196c0: 6465 6422 2c22 7479 7065 223a 2265 7272  ded","type":"err
-000196d0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-000196e0: 5d2c 226e 616d 6522 3a22 4c42 526f 7574  ],"name":"LBRout
-000196f0: 6572 5f5f 4e6f 7446 6163 746f 7279 4f77  er__NotFactoryOw
-00019700: 6e65 7222 2c22 7479 7065 223a 2265 7272  ner","type":"err
-00019710: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-00019720: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00019730: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-00019740: 3a22 746f 6b65 6e58 222c 2274 7970 6522  :"tokenX","type"
-00019750: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-00019760: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-00019770: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
-00019780: 6b65 6e59 222c 2274 7970 6522 3a22 6164  kenY","type":"ad
-00019790: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-000197a0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-000197b0: 222c 226e 616d 6522 3a22 6269 6e53 7465  ","name":"binSte
-000197c0: 7022 2c22 7479 7065 223a 2275 696e 7432  p","type":"uint2
-000197d0: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
-000197e0: 526f 7574 6572 5f5f 5061 6972 4e6f 7443  Router__PairNotC
-000197f0: 7265 6174 6564 222c 2274 7970 6522 3a22  reated","type":"
-00019800: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-00019810: 223a 5b5d 2c22 6e61 6d65 223a 224c 4252  ":[],"name":"LBR
-00019820: 6f75 7465 725f 5f53 656e 6465 7249 734e  outer__SenderIsN
-00019830: 6f74 5741 5641 5822 2c22 7479 7065 223a  otWAVAX","type":
-00019840: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00019850: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00019860: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00019870: 616d 6522 3a22 6964 222c 2274 7970 6522  ame":"id","type"
-00019880: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-00019890: 6d65 223a 224c 4252 6f75 7465 725f 5f53  me":"LBRouter__S
-000198a0: 7761 704f 7665 7266 6c6f 7773 222c 2274  wapOverflows","t
-000198b0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-000198c0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-000198d0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-000198e0: 3622 2c22 6e61 6d65 223a 2265 7863 6573  6","name":"exces
-000198f0: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
-00019900: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
-00019910: 526f 7574 6572 5f5f 546f 6f4d 7563 6854  Router__TooMuchT
-00019920: 6f6b 656e 7349 6e22 2c22 7479 7065 223a  okensIn","type":
-00019930: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-00019940: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00019950: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00019960: 616d 6522 3a22 616d 6f75 6e74 222c 2274  ame":"amount","t
-00019970: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-00019980: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00019990: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-000199a0: 3a22 7265 7365 7276 6522 2c22 7479 7065  :"reserve","type
-000199b0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-000199c0: 616d 6522 3a22 4c42 526f 7574 6572 5f5f  ame":"LBRouter__
-000199d0: 5772 6f6e 6741 6d6f 756e 7473 222c 2274  WrongAmounts","t
-000199e0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-000199f0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00019a00: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00019a10: 7322 2c22 6e61 6d65 223a 2274 6f6b 656e  s","name":"token
-00019a20: 5822 2c22 7479 7065 223a 2261 6464 7265  X","type":"addre
-00019a30: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-00019a40: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-00019a50: 6e61 6d65 223a 2274 6f6b 656e 5922 2c22  name":"tokenY","
-00019a60: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-00019a70: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00019a80: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00019a90: 223a 2261 6d6f 756e 7458 222c 2274 7970  ":"amountX","typ
-00019aa0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-00019ab0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00019ac0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00019ad0: 616d 6f75 6e74 5922 2c22 7479 7065 223a  amountY","type":
-00019ae0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-00019af0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00019b00: 3235 3622 2c22 6e61 6d65 223a 226d 7367  256","name":"msg
-00019b10: 5661 6c75 6522 2c22 7479 7065 223a 2275  Value","type":"u
-00019b20: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-00019b30: 3a22 4c42 526f 7574 6572 5f5f 5772 6f6e  :"LBRouter__Wron
-00019b40: 6741 7661 784c 6971 7569 6469 7479 5061  gAvaxLiquidityPa
-00019b50: 7261 6d65 7465 7273 222c 2274 7970 6522  rameters","type"
-00019b60: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00019b70: 7473 223a 5b5d 2c22 6e61 6d65 223a 224c  ts":[],"name":"L
-00019b80: 4252 6f75 7465 725f 5f57 726f 6e67 546f  BRouter__WrongTo
-00019b90: 6b65 6e4f 7264 6572 222c 2274 7970 6522  kenOrder","type"
-00019ba0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00019bb0: 7473 223a 5b5d 2c22 6e61 6d65 223a 224d  ts":[],"name":"M
-00019bc0: 6174 6831 3238 7831 3238 5f5f 4c6f 6755  ath128x128__LogU
-00019bd0: 6e64 6572 666c 6f77 222c 2274 7970 6522  nderflow","type"
-00019be0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-00019bf0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00019c00: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00019c10: 6e61 6d65 223a 2278 222c 2274 7970 6522  name":"x","type"
-00019c20: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-00019c30: 7465 726e 616c 5479 7065 223a 2269 6e74  ternalType":"int
-00019c40: 3235 3622 2c22 6e61 6d65 223a 2279 222c  256","name":"y",
-00019c50: 2274 7970 6522 3a22 696e 7432 3536 227d  "type":"int256"}
-00019c60: 5d2c 226e 616d 6522 3a22 4d61 7468 3132  ],"name":"Math12
-00019c70: 3878 3132 385f 5f50 6f77 6572 556e 6465  8x128__PowerUnde
-00019c80: 7266 6c6f 7722 2c22 7479 7065 223a 2265  rflow","type":"e
-00019c90: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-00019ca0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00019cb0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00019cc0: 6522 3a22 7072 6f64 3122 2c22 7479 7065  e":"prod1","type
-00019cd0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-00019ce0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00019cf0: 6e74 3235 3622 2c22 6e61 6d65 223a 2264  nt256","name":"d
-00019d00: 656e 6f6d 696e 6174 6f72 222c 2274 7970  enominator","typ
-00019d10: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-00019d20: 6e61 6d65 223a 224d 6174 6835 3132 4269  name":"Math512Bi
-00019d30: 7473 5f5f 4d75 6c44 6976 4f76 6572 666c  ts__MulDivOverfl
-00019d40: 6f77 222c 2274 7970 6522 3a22 6572 726f  ow","type":"erro
-00019d50: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
-00019d60: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00019d70: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00019d80: 2270 726f 6431 222c 2274 7970 6522 3a22  "prod1","type":"
-00019d90: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-00019da0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00019db0: 3536 222c 226e 616d 6522 3a22 6f66 6673  56","name":"offs
-00019dc0: 6574 222c 2274 7970 6522 3a22 7569 6e74  et","type":"uint
-00019dd0: 3235 3622 7d5d 2c22 6e61 6d65 223a 224d  256"}],"name":"M
-00019de0: 6174 6835 3132 4269 7473 5f5f 4d75 6c53  ath512Bits__MulS
-00019df0: 6869 6674 4f76 6572 666c 6f77 222c 2274  hiftOverflow","t
-00019e00: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
-00019e10: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00019e20: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00019e30: 3622 2c22 6e61 6d65 223a 226f 6666 7365  6","name":"offse
-00019e40: 7422 2c22 7479 7065 223a 2275 696e 7432  t","type":"uint2
-00019e50: 3536 227d 5d2c 226e 616d 6522 3a22 4d61  56"}],"name":"Ma
-00019e60: 7468 3531 3242 6974 735f 5f4f 6666 7365  th512Bits__Offse
-00019e70: 744f 7665 7266 6c6f 7773 222c 2274 7970  tOverflows","typ
-00019e80: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-00019e90: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00019ea0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00019eb0: 2c22 6e61 6d65 223a 2278 222c 2274 7970  ,"name":"x","typ
-00019ec0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-00019ed0: 6e61 6d65 223a 2253 6166 6543 6173 745f  name":"SafeCast_
-00019ee0: 5f45 7863 6565 6473 3132 3842 6974 7322  _Exceeds128Bits"
-00019ef0: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-00019f00: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-00019f10: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00019f20: 7432 3536 222c 226e 616d 6522 3a22 7822  t256","name":"x"
-00019f30: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-00019f40: 227d 5d2c 226e 616d 6522 3a22 5361 6665  "}],"name":"Safe
-00019f50: 4361 7374 5f5f 4578 6365 6564 7334 3042  Cast__Exceeds40B
-00019f60: 6974 7322 2c22 7479 7065 223a 2265 7272  its","type":"err
-00019f70: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-00019f80: 5d2c 226e 616d 6522 3a22 546f 6b65 6e48  ],"name":"TokenH
-00019f90: 656c 7065 725f 5f43 616c 6c46 6169 6c65  elper__CallFaile
-00019fa0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
-00019fb0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-00019fc0: 226e 616d 6522 3a22 546f 6b65 6e48 656c  "name":"TokenHel
-00019fd0: 7065 725f 5f4e 6f6e 436f 6e74 7261 6374  per__NonContract
-00019fe0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-00019ff0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-0001a000: 6e61 6d65 223a 2254 6f6b 656e 4865 6c70  name":"TokenHelp
-0001a010: 6572 5f5f 5472 616e 7366 6572 4661 696c  er__TransferFail
-0001a020: 6564 222c 2274 7970 6522 3a22 6572 726f  ed","type":"erro
-0001a030: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
-0001a040: 2263 6f6d 706f 6e65 6e74 7322 3a5b 7b22  "components":[{"
-0001a050: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-0001a060: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
-0001a070: 226e 616d 6522 3a22 746f 6b65 6e58 222c  "name":"tokenX",
-0001a080: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001a090: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001a0a0: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
-0001a0b0: 3230 222c 226e 616d 6522 3a22 746f 6b65  20","name":"toke
-0001a0c0: 6e59 222c 2274 7970 6522 3a22 6164 6472  nY","type":"addr
-0001a0d0: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0001a0e0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001a0f0: 226e 616d 6522 3a22 6269 6e53 7465 7022  "name":"binStep"
-0001a100: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001a110: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001a120: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001a130: 6d65 223a 2261 6d6f 756e 7458 222c 2274  me":"amountX","t
-0001a140: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0001a150: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001a160: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001a170: 3a22 616d 6f75 6e74 5922 2c22 7479 7065  :"amountY","type
-0001a180: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0001a190: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001a1a0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
-0001a1b0: 6d6f 756e 7458 4d69 6e22 2c22 7479 7065  mountXMin","type
-0001a1c0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0001a1d0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001a1e0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
-0001a1f0: 6d6f 756e 7459 4d69 6e22 2c22 7479 7065  mountYMin","type
-0001a200: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0001a210: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001a220: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
-0001a230: 6374 6976 6549 6444 6573 6972 6564 222c  ctiveIdDesired",
-0001a240: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001a250: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001a260: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001a270: 6522 3a22 6964 536c 6970 7061 6765 222c  e":"idSlippage",
-0001a280: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001a290: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001a2a0: 223a 2269 6e74 3235 365b 5d22 2c22 6e61  ":"int256[]","na
-0001a2b0: 6d65 223a 2264 656c 7461 4964 7322 2c22  me":"deltaIds","
-0001a2c0: 7479 7065 223a 2269 6e74 3235 365b 5d22  type":"int256[]"
-0001a2d0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001a2e0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
-0001a2f0: 616d 6522 3a22 6469 7374 7269 6275 7469  ame":"distributi
-0001a300: 6f6e 5822 2c22 7479 7065 223a 2275 696e  onX","type":"uin
-0001a310: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
-0001a320: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001a330: 365b 5d22 2c22 6e61 6d65 223a 2264 6973  6[]","name":"dis
-0001a340: 7472 6962 7574 696f 6e59 222c 2274 7970  tributionY","typ
-0001a350: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
-0001a360: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001a370: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0001a380: 3a22 746f 222c 2274 7970 6522 3a22 6164  :"to","type":"ad
-0001a390: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0001a3a0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001a3b0: 222c 226e 616d 6522 3a22 6465 6164 6c69  ","name":"deadli
-0001a3c0: 6e65 222c 2274 7970 6522 3a22 7569 6e74  ne","type":"uint
-0001a3d0: 3235 3622 7d5d 2c22 696e 7465 726e 616c  256"}],"internal
-0001a3e0: 5479 7065 223a 2273 7472 7563 7420 494c  Type":"struct IL
-0001a3f0: 4252 6f75 7465 722e 4c69 7175 6964 6974  BRouter.Liquidit
-0001a400: 7950 6172 616d 6574 6572 7322 2c22 6e61  yParameters","na
-0001a410: 6d65 223a 225f 6c69 7175 6964 6974 7950  me":"_liquidityP
-0001a420: 6172 616d 6574 6572 7322 2c22 7479 7065  arameters","type
-0001a430: 223a 2274 7570 6c65 227d 5d2c 226e 616d  ":"tuple"}],"nam
-0001a440: 6522 3a22 6164 644c 6971 7569 6469 7479  e":"addLiquidity
-0001a450: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
-0001a460: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001a470: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
-0001a480: 2264 6570 6f73 6974 4964 7322 2c22 7479  "depositIds","ty
-0001a490: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
-0001a4a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001a4b0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
-0001a4c0: 6d65 223a 226c 6971 7569 6469 7479 4d69  me":"liquidityMi
-0001a4d0: 6e74 6564 222c 2274 7970 6522 3a22 7569  nted","type":"ui
-0001a4e0: 6e74 3235 365b 5d22 7d5d 2c22 7374 6174  nt256[]"}],"stat
-0001a4f0: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
-0001a500: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
-0001a510: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-0001a520: 6e70 7574 7322 3a5b 7b22 636f 6d70 6f6e  nputs":[{"compon
-0001a530: 656e 7473 223a 5b7b 2269 6e74 6572 6e61  ents":[{"interna
-0001a540: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-0001a550: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
-0001a560: 2274 6f6b 656e 5822 2c22 7479 7065 223a  "tokenX","type":
-0001a570: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-0001a580: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-0001a590: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
-0001a5a0: 6d65 223a 2274 6f6b 656e 5922 2c22 7479  me":"tokenY","ty
-0001a5b0: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0001a5c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001a5d0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001a5e0: 2262 696e 5374 6570 222c 2274 7970 6522  "binStep","type"
-0001a5f0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0001a600: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001a610: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
-0001a620: 6f75 6e74 5822 2c22 7479 7065 223a 2275  ountX","type":"u
-0001a630: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0001a640: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001a650: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
-0001a660: 7459 222c 2274 7970 6522 3a22 7569 6e74  tY","type":"uint
-0001a670: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001a680: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001a690: 226e 616d 6522 3a22 616d 6f75 6e74 584d  "name":"amountXM
-0001a6a0: 696e 222c 2274 7970 6522 3a22 7569 6e74  in","type":"uint
-0001a6b0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001a6c0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001a6d0: 226e 616d 6522 3a22 616d 6f75 6e74 594d  "name":"amountYM
-0001a6e0: 696e 222c 2274 7970 6522 3a22 7569 6e74  in","type":"uint
-0001a6f0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001a700: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001a710: 226e 616d 6522 3a22 6163 7469 7665 4964  "name":"activeId
-0001a720: 4465 7369 7265 6422 2c22 7479 7065 223a  Desired","type":
-0001a730: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0001a740: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001a750: 3235 3622 2c22 6e61 6d65 223a 2269 6453  256","name":"idS
-0001a760: 6c69 7070 6167 6522 2c22 7479 7065 223a  lippage","type":
-0001a770: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0001a780: 6572 6e61 6c54 7970 6522 3a22 696e 7432  ernalType":"int2
-0001a790: 3536 5b5d 222c 226e 616d 6522 3a22 6465  56[]","name":"de
-0001a7a0: 6c74 6149 6473 222c 2274 7970 6522 3a22  ltaIds","type":"
-0001a7b0: 696e 7432 3536 5b5d 227d 2c7b 2269 6e74  int256[]"},{"int
-0001a7c0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001a7d0: 3235 365b 5d22 2c22 6e61 6d65 223a 2264  256[]","name":"d
-0001a7e0: 6973 7472 6962 7574 696f 6e58 222c 2274  istributionX","t
-0001a7f0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-0001a800: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001a810: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
-0001a820: 616d 6522 3a22 6469 7374 7269 6275 7469  ame":"distributi
-0001a830: 6f6e 5922 2c22 7479 7065 223a 2275 696e  onY","type":"uin
-0001a840: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
-0001a850: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0001a860: 7322 2c22 6e61 6d65 223a 2274 6f22 2c22  s","name":"to","
-0001a870: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0001a880: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001a890: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001a8a0: 223a 2264 6561 646c 696e 6522 2c22 7479  ":"deadline","ty
-0001a8b0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-0001a8c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001a8d0: 7374 7275 6374 2049 4c42 526f 7574 6572  struct ILBRouter
-0001a8e0: 2e4c 6971 7569 6469 7479 5061 7261 6d65  .LiquidityParame
-0001a8f0: 7465 7273 222c 226e 616d 6522 3a22 5f6c  ters","name":"_l
-0001a900: 6971 7569 6469 7479 5061 7261 6d65 7465  iquidityParamete
-0001a910: 7273 222c 2274 7970 6522 3a22 7475 706c  rs","type":"tupl
-0001a920: 6522 7d5d 2c22 6e61 6d65 223a 2261 6464  e"}],"name":"add
-0001a930: 4c69 7175 6964 6974 7941 5641 5822 2c22  LiquidityAVAX","
-0001a940: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-0001a950: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001a960: 3536 5b5d 222c 226e 616d 6522 3a22 6465  56[]","name":"de
-0001a970: 706f 7369 7449 6473 222c 2274 7970 6522  positIds","type"
-0001a980: 3a22 7569 6e74 3235 365b 5d22 7d2c 7b22  :"uint256[]"},{"
-0001a990: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001a9a0: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
-0001a9b0: 3a22 6c69 7175 6964 6974 794d 696e 7465  :"liquidityMinte
-0001a9c0: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-0001a9d0: 3536 5b5d 227d 5d2c 2273 7461 7465 4d75  56[]"}],"stateMu
-0001a9e0: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
-0001a9f0: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
-0001aa00: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-0001aa10: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0001aa20: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
-0001aa30: 3230 222c 226e 616d 6522 3a22 5f74 6f6b  20","name":"_tok
-0001aa40: 656e 5822 2c22 7479 7065 223a 2261 6464  enX","type":"add
-0001aa50: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0001aa60: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-0001aa70: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
-0001aa80: 225f 746f 6b65 6e59 222c 2274 7970 6522  "_tokenY","type"
-0001aa90: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001aaa0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001aab0: 7432 3422 2c22 6e61 6d65 223a 225f 6163  t24","name":"_ac
-0001aac0: 7469 7665 4964 222c 2274 7970 6522 3a22  tiveId","type":"
-0001aad0: 7569 6e74 3234 227d 2c7b 2269 6e74 6572  uint24"},{"inter
-0001aae0: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
-0001aaf0: 222c 226e 616d 6522 3a22 5f62 696e 5374  ","name":"_binSt
-0001ab00: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
-0001ab10: 3136 227d 5d2c 226e 616d 6522 3a22 6372  16"}],"name":"cr
-0001ab20: 6561 7465 4c42 5061 6972 222c 226f 7574  eateLBPair","out
-0001ab30: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001ab40: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-0001ab50: 2049 4c42 5061 6972 222c 226e 616d 6522   ILBPair","name"
-0001ab60: 3a22 7061 6972 222c 2274 7970 6522 3a22  :"pair","type":"
-0001ab70: 6164 6472 6573 7322 7d5d 2c22 7374 6174  address"}],"stat
-0001ab80: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
-0001ab90: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
-0001aba0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-0001abb0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-0001abc0: 3a22 6661 6374 6f72 7922 2c22 6f75 7470  :"factory","outp
-0001abd0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001abe0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-0001abf0: 494c 4246 6163 746f 7279 222c 226e 616d  ILBFactory","nam
-0001ac00: 6522 3a22 222c 2274 7970 6522 3a22 6164  e":"","type":"ad
-0001ac10: 6472 6573 7322 7d5d 2c22 7374 6174 654d  dress"}],"stateM
-0001ac20: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
-0001ac30: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-0001ac40: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-0001ac50: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001ac60: 2263 6f6e 7472 6163 7420 494c 4250 6169  "contract ILBPai
-0001ac70: 7222 2c22 6e61 6d65 223a 225f 4c42 5061  r","name":"_LBPa
-0001ac80: 6972 222c 2274 7970 6522 3a22 6164 6472  ir","type":"addr
-0001ac90: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0001aca0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001acb0: 226e 616d 6522 3a22 5f70 7269 6365 222c  "name":"_price",
-0001acc0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001acd0: 7d5d 2c22 6e61 6d65 223a 2267 6574 4964  }],"name":"getId
-0001ace0: 4672 6f6d 5072 6963 6522 2c22 6f75 7470  FromPrice","outp
-0001acf0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001ad00: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
-0001ad10: 6e61 6d65 223a 2222 2c22 7479 7065 223a  name":"","type":
-0001ad20: 2275 696e 7432 3422 7d5d 2c22 7374 6174  "uint24"}],"stat
-0001ad30: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
-0001ad40: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
-0001ad50: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-0001ad60: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0001ad70: 223a 2263 6f6e 7472 6163 7420 494c 4250  ":"contract ILBP
-0001ad80: 6169 7222 2c22 6e61 6d65 223a 225f 4c42  air","name":"_LB
-0001ad90: 5061 6972 222c 2274 7970 6522 3a22 6164  Pair","type":"ad
-0001ada0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0001adb0: 616c 5479 7065 223a 2275 696e 7432 3422  alType":"uint24"
-0001adc0: 2c22 6e61 6d65 223a 225f 6964 222c 2274  ,"name":"_id","t
-0001add0: 7970 6522 3a22 7569 6e74 3234 227d 5d2c  ype":"uint24"}],
-0001ade0: 226e 616d 6522 3a22 6765 7450 7269 6365  "name":"getPrice
-0001adf0: 4672 6f6d 4964 222c 226f 7574 7075 7473  FromId","outputs
-0001ae00: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0001ae10: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001ae20: 6d65 223a 2222 2c22 7479 7065 223a 2275  me":"","type":"u
-0001ae30: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-0001ae40: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
-0001ae50: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
-0001ae60: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0001ae70: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0001ae80: 3a22 636f 6e74 7261 6374 2049 4c42 5061  :"contract ILBPa
-0001ae90: 6972 222c 226e 616d 6522 3a22 5f4c 4250  ir","name":"_LBP
-0001aea0: 6169 7222 2c22 7479 7065 223a 2261 6464  air","type":"add
-0001aeb0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0001aec0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001aed0: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
-0001aee0: 4f75 7422 2c22 7479 7065 223a 2275 696e  Out","type":"uin
-0001aef0: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-0001af00: 6c54 7970 6522 3a22 626f 6f6c 222c 226e  lType":"bool","n
-0001af10: 616d 6522 3a22 5f73 7761 7046 6f72 5922  ame":"_swapForY"
-0001af20: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
-0001af30: 2c22 6e61 6d65 223a 2267 6574 5377 6170  ,"name":"getSwap
-0001af40: 496e 222c 226f 7574 7075 7473 223a 5b7b  In","outputs":[{
-0001af50: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001af60: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001af70: 2261 6d6f 756e 7449 6e22 2c22 7479 7065  "amountIn","type
-0001af80: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-0001af90: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001afa0: 6e74 3235 3622 2c22 6e61 6d65 223a 2266  nt256","name":"f
-0001afb0: 6565 7349 6e22 2c22 7479 7065 223a 2275  eesIn","type":"u
-0001afc0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-0001afd0: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
-0001afe0: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
-0001aff0: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0001b000: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0001b010: 3a22 636f 6e74 7261 6374 2049 4c42 5061  :"contract ILBPa
-0001b020: 6972 222c 226e 616d 6522 3a22 5f4c 4250  ir","name":"_LBP
-0001b030: 6169 7222 2c22 7479 7065 223a 2261 6464  air","type":"add
-0001b040: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-0001b050: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001b060: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
-0001b070: 496e 222c 2274 7970 6522 3a22 7569 6e74  In","type":"uint
-0001b080: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001b090: 5479 7065 223a 2262 6f6f 6c22 2c22 6e61  Type":"bool","na
-0001b0a0: 6d65 223a 225f 7377 6170 466f 7259 222c  me":"_swapForY",
-0001b0b0: 2274 7970 6522 3a22 626f 6f6c 227d 5d2c  "type":"bool"}],
-0001b0c0: 226e 616d 6522 3a22 6765 7453 7761 704f  "name":"getSwapO
-0001b0d0: 7574 222c 226f 7574 7075 7473 223a 5b7b  ut","outputs":[{
-0001b0e0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001b0f0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001b100: 2261 6d6f 756e 744f 7574 222c 2274 7970  "amountOut","typ
-0001b110: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0001b120: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001b130: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001b140: 6665 6573 496e 222c 2274 7970 6522 3a22  feesIn","type":"
-0001b150: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
-0001b160: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
-0001b170: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
-0001b180: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-0001b190: 3a5b 5d2c 226e 616d 6522 3a22 6f6c 6446  :[],"name":"oldF
-0001b1a0: 6163 746f 7279 222c 226f 7574 7075 7473  actory","outputs
-0001b1b0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0001b1c0: 6522 3a22 636f 6e74 7261 6374 2049 4a6f  e":"contract IJo
-0001b1d0: 6546 6163 746f 7279 222c 226e 616d 6522  eFactory","name"
-0001b1e0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
-0001b1f0: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
-0001b200: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-0001b210: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-0001b220: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-0001b230: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
-0001b240: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
-0001b250: 226e 616d 6522 3a22 5f74 6f6b 656e 5822  "name":"_tokenX"
-0001b260: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0001b270: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001b280: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-0001b290: 4332 3022 2c22 6e61 6d65 223a 225f 746f  C20","name":"_to
-0001b2a0: 6b65 6e59 222c 2274 7970 6522 3a22 6164  kenY","type":"ad
-0001b2b0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0001b2c0: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
-0001b2d0: 2c22 6e61 6d65 223a 225f 6269 6e53 7465  ,"name":"_binSte
-0001b2e0: 7022 2c22 7479 7065 223a 2275 696e 7431  p","type":"uint1
-0001b2f0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-0001b300: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001b310: 616d 6522 3a22 5f61 6d6f 756e 7458 4d69  ame":"_amountXMi
-0001b320: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-0001b330: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001b340: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001b350: 6e61 6d65 223a 225f 616d 6f75 6e74 594d  name":"_amountYM
-0001b360: 696e 222c 2274 7970 6522 3a22 7569 6e74  in","type":"uint
-0001b370: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001b380: 5479 7065 223a 2275 696e 7432 3536 5b5d  Type":"uint256[]
-0001b390: 222c 226e 616d 6522 3a22 5f69 6473 222c  ","name":"_ids",
-0001b3a0: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
-0001b3b0: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
-0001b3c0: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
-0001b3d0: 226e 616d 6522 3a22 5f61 6d6f 756e 7473  "name":"_amounts
-0001b3e0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001b3f0: 365b 5d22 7d2c 7b22 696e 7465 726e 616c  6[]"},{"internal
-0001b400: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-0001b410: 226e 616d 6522 3a22 5f74 6f22 2c22 7479  "name":"_to","ty
-0001b420: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0001b430: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001b440: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001b450: 225f 6465 6164 6c69 6e65 222c 2274 7970  "_deadline","typ
-0001b460: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001b470: 6e61 6d65 223a 2272 656d 6f76 654c 6971  name":"removeLiq
-0001b480: 7569 6469 7479 222c 226f 7574 7075 7473  uidity","outputs
-0001b490: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0001b4a0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001b4b0: 6d65 223a 2261 6d6f 756e 7458 222c 2274  me":"amountX","t
-0001b4c0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0001b4d0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001b4e0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001b4f0: 3a22 616d 6f75 6e74 5922 2c22 7479 7065  :"amountY","type
-0001b500: 223a 2275 696e 7432 3536 227d 5d2c 2273  ":"uint256"}],"s
-0001b510: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-0001b520: 226e 6f6e 7061 7961 626c 6522 2c22 7479  "nonpayable","ty
-0001b530: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-0001b540: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-0001b550: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-0001b560: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
-0001b570: 6d65 223a 225f 746f 6b65 6e22 2c22 7479  me":"_token","ty
-0001b580: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0001b590: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001b5a0: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
-0001b5b0: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
-0001b5c0: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
-0001b5d0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001b5e0: 3235 3622 2c22 6e61 6d65 223a 225f 616d  256","name":"_am
-0001b5f0: 6f75 6e74 546f 6b65 6e4d 696e 222c 2274  ountTokenMin","t
-0001b600: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0001b610: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001b620: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001b630: 3a22 5f61 6d6f 756e 7441 5641 584d 696e  :"_amountAVAXMin
-0001b640: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001b650: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-0001b660: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
-0001b670: 226e 616d 6522 3a22 5f69 6473 222c 2274  "name":"_ids","t
-0001b680: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-0001b690: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001b6a0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
-0001b6b0: 616d 6522 3a22 5f61 6d6f 756e 7473 222c  ame":"_amounts",
-0001b6c0: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
-0001b6d0: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
-0001b6e0: 7065 223a 2261 6464 7265 7373 2070 6179  pe":"address pay
-0001b6f0: 6162 6c65 222c 226e 616d 6522 3a22 5f74  able","name":"_t
-0001b700: 6f22 2c22 7479 7065 223a 2261 6464 7265  o","type":"addre
-0001b710: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-0001b720: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001b730: 6e61 6d65 223a 225f 6465 6164 6c69 6e65  name":"_deadline
-0001b740: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001b750: 3622 7d5d 2c22 6e61 6d65 223a 2272 656d  6"}],"name":"rem
-0001b760: 6f76 654c 6971 7569 6469 7479 4156 4158  oveLiquidityAVAX
-0001b770: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
-0001b780: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001b790: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
-0001b7a0: 6d6f 756e 7454 6f6b 656e 222c 2274 7970  mountToken","typ
-0001b7b0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0001b7c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001b7d0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001b7e0: 616d 6f75 6e74 4156 4158 222c 2274 7970  amountAVAX","typ
-0001b7f0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001b800: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-0001b810: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-0001b820: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-0001b830: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-0001b840: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001b850: 7432 3536 222c 226e 616d 6522 3a22 5f61  t256","name":"_a
-0001b860: 6d6f 756e 744f 7574 222c 2274 7970 6522  mountOut","type"
-0001b870: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0001b880: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001b890: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
-0001b8a0: 5f70 6169 7242 696e 5374 6570 7322 2c22  _pairBinSteps","
-0001b8b0: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
-0001b8c0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001b8d0: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-0001b8e0: 4332 305b 5d22 2c22 6e61 6d65 223a 225f  C20[]","name":"_
-0001b8f0: 746f 6b65 6e50 6174 6822 2c22 7479 7065  tokenPath","type
-0001b900: 223a 2261 6464 7265 7373 5b5d 227d 2c7b  ":"address[]"},{
-0001b910: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001b920: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0001b930: 225f 746f 222c 2274 7970 6522 3a22 6164  "_to","type":"ad
-0001b940: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0001b950: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001b960: 222c 226e 616d 6522 3a22 5f64 6561 646c  ","name":"_deadl
-0001b970: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
-0001b980: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-0001b990: 7377 6170 4156 4158 466f 7245 7861 6374  swapAVAXForExact
-0001b9a0: 546f 6b65 6e73 222c 226f 7574 7075 7473  Tokens","outputs
-0001b9b0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-0001b9c0: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
-0001b9d0: 6e61 6d65 223a 2261 6d6f 756e 7473 496e  name":"amountsIn
-0001b9e0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001b9f0: 365b 5d22 7d5d 2c22 7374 6174 654d 7574  6[]"}],"stateMut
-0001ba00: 6162 696c 6974 7922 3a22 7061 7961 626c  ability":"payabl
-0001ba10: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
-0001ba20: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-0001ba30: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0001ba40: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001ba50: 223a 225f 616d 6f75 6e74 4f75 744d 696e  ":"_amountOutMin
-0001ba60: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001ba70: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-0001ba80: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
-0001ba90: 226e 616d 6522 3a22 5f70 6169 7242 696e  "name":"_pairBin
-0001baa0: 5374 6570 7322 2c22 7479 7065 223a 2275  Steps","type":"u
-0001bab0: 696e 7432 3536 5b5d 227d 2c7b 2269 6e74  int256[]"},{"int
-0001bac0: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-0001bad0: 7261 6374 2049 4552 4332 305b 5d22 2c22  ract IERC20[]","
-0001bae0: 6e61 6d65 223a 225f 746f 6b65 6e50 6174  name":"_tokenPat
-0001baf0: 6822 2c22 7479 7065 223a 2261 6464 7265  h","type":"addre
-0001bb00: 7373 5b5d 227d 2c7b 2269 6e74 6572 6e61  ss[]"},{"interna
-0001bb10: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-0001bb20: 2c22 6e61 6d65 223a 225f 746f 222c 2274  ,"name":"_to","t
-0001bb30: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-0001bb40: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001bb50: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001bb60: 3a22 5f64 6561 646c 696e 6522 2c22 7479  :"_deadline","ty
-0001bb70: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-0001bb80: 226e 616d 6522 3a22 7377 6170 4578 6163  "name":"swapExac
-0001bb90: 7441 5641 5846 6f72 546f 6b65 6e73 222c  tAVAXForTokens",
-0001bba0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-0001bbb0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001bbc0: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0001bbd0: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
-0001bbe0: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
-0001bbf0: 654d 7574 6162 696c 6974 7922 3a22 7061  eMutability":"pa
-0001bc00: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
-0001bc10: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-0001bc20: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0001bc30: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001bc40: 6e61 6d65 223a 225f 616d 6f75 6e74 4f75  name":"_amountOu
-0001bc50: 744d 696e 222c 2274 7970 6522 3a22 7569  tMin","type":"ui
-0001bc60: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
-0001bc70: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001bc80: 5b5d 222c 226e 616d 6522 3a22 5f70 6169  []","name":"_pai
-0001bc90: 7242 696e 5374 6570 7322 2c22 7479 7065  rBinSteps","type
-0001bca0: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
-0001bcb0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001bcc0: 636f 6e74 7261 6374 2049 4552 4332 305b  contract IERC20[
-0001bcd0: 5d22 2c22 6e61 6d65 223a 225f 746f 6b65  ]","name":"_toke
-0001bce0: 6e50 6174 6822 2c22 7479 7065 223a 2261  nPath","type":"a
-0001bcf0: 6464 7265 7373 5b5d 227d 2c7b 2269 6e74  ddress[]"},{"int
-0001bd00: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0001bd10: 6573 7322 2c22 6e61 6d65 223a 225f 746f  ess","name":"_to
-0001bd20: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0001bd30: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
-0001bd40: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001bd50: 616d 6522 3a22 5f64 6561 646c 696e 6522  ame":"_deadline"
-0001bd60: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001bd70: 227d 5d2c 226e 616d 6522 3a22 7377 6170  "}],"name":"swap
-0001bd80: 4578 6163 7441 5641 5846 6f72 546f 6b65  ExactAVAXForToke
-0001bd90: 6e73 5375 7070 6f72 7469 6e67 4665 654f  nsSupportingFeeO
-0001bda0: 6e54 7261 6e73 6665 7254 6f6b 656e 7322  nTransferTokens"
-0001bdb0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-0001bdc0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001bdd0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
-0001bde0: 6f75 6e74 4f75 7422 2c22 7479 7065 223a  ountOut","type":
-0001bdf0: 2275 696e 7432 3536 227d 5d2c 2273 7461  "uint256"}],"sta
-0001be00: 7465 4d75 7461 6269 6c69 7479 223a 2270  teMutability":"p
-0001be10: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-0001be20: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-0001be30: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001be40: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001be50: 226e 616d 6522 3a22 5f61 6d6f 756e 7449  "name":"_amountI
-0001be60: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
-0001be70: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001be80: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001be90: 6e61 6d65 223a 225f 616d 6f75 6e74 4f75  name":"_amountOu
-0001bea0: 744d 696e 4156 4158 222c 2274 7970 6522  tMinAVAX","type"
-0001beb0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0001bec0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001bed0: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
-0001bee0: 5f70 6169 7242 696e 5374 6570 7322 2c22  _pairBinSteps","
-0001bef0: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
-0001bf00: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001bf10: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-0001bf20: 4332 305b 5d22 2c22 6e61 6d65 223a 225f  C20[]","name":"_
-0001bf30: 746f 6b65 6e50 6174 6822 2c22 7479 7065  tokenPath","type
-0001bf40: 223a 2261 6464 7265 7373 5b5d 227d 2c7b  ":"address[]"},{
-0001bf50: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001bf60: 6164 6472 6573 7320 7061 7961 626c 6522  address payable"
-0001bf70: 2c22 6e61 6d65 223a 225f 746f 222c 2274  ,"name":"_to","t
-0001bf80: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-0001bf90: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001bfa0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001bfb0: 3a22 5f64 6561 646c 696e 6522 2c22 7479  :"_deadline","ty
-0001bfc0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-0001bfd0: 226e 616d 6522 3a22 7377 6170 4578 6163  "name":"swapExac
-0001bfe0: 7454 6f6b 656e 7346 6f72 4156 4158 222c  tTokensForAVAX",
-0001bff0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
-0001c000: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001c010: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0001c020: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
-0001c030: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
-0001c040: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
-0001c050: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
-0001c060: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-0001c070: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-0001c080: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001c090: 222c 226e 616d 6522 3a22 5f61 6d6f 756e  ","name":"_amoun
-0001c0a0: 7449 6e22 2c22 7479 7065 223a 2275 696e  tIn","type":"uin
-0001c0b0: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-0001c0c0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001c0d0: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
-0001c0e0: 4f75 744d 696e 4156 4158 222c 2274 7970  OutMinAVAX","typ
-0001c0f0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0001c100: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001c110: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
-0001c120: 3a22 5f70 6169 7242 696e 5374 6570 7322  :"_pairBinSteps"
-0001c130: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001c140: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
-0001c150: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-0001c160: 4552 4332 305b 5d22 2c22 6e61 6d65 223a  ERC20[]","name":
-0001c170: 225f 746f 6b65 6e50 6174 6822 2c22 7479  "_tokenPath","ty
-0001c180: 7065 223a 2261 6464 7265 7373 5b5d 227d  pe":"address[]"}
-0001c190: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001c1a0: 3a22 6164 6472 6573 7320 7061 7961 626c  :"address payabl
-0001c1b0: 6522 2c22 6e61 6d65 223a 225f 746f 222c  e","name":"_to",
-0001c1c0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001c1d0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001c1e0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001c1f0: 6522 3a22 5f64 6561 646c 696e 6522 2c22  e":"_deadline","
-0001c200: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001c210: 5d2c 226e 616d 6522 3a22 7377 6170 4578  ],"name":"swapEx
-0001c220: 6163 7454 6f6b 656e 7346 6f72 4156 4158  actTokensForAVAX
-0001c230: 5375 7070 6f72 7469 6e67 4665 654f 6e54  SupportingFeeOnT
-0001c240: 7261 6e73 6665 7254 6f6b 656e 7322 2c22  ransferTokens","
-0001c250: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-0001c260: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001c270: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0001c280: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
-0001c290: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-0001c2a0: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-0001c2b0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-0001c2c0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-0001c2d0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001c2e0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001c2f0: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
-0001c300: 496e 222c 2274 7970 6522 3a22 7569 6e74  In","type":"uint
-0001c310: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001c320: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001c330: 226e 616d 6522 3a22 5f61 6d6f 756e 744f  "name":"_amountO
-0001c340: 7574 4d69 6e22 2c22 7479 7065 223a 2275  utMin","type":"u
-0001c350: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-0001c360: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001c370: 365b 5d22 2c22 6e61 6d65 223a 225f 7061  6[]","name":"_pa
-0001c380: 6972 4269 6e53 7465 7073 222c 2274 7970  irBinSteps","typ
-0001c390: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
-0001c3a0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-0001c3b0: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
-0001c3c0: 5b5d 222c 226e 616d 6522 3a22 5f74 6f6b  []","name":"_tok
-0001c3d0: 656e 5061 7468 222c 2274 7970 6522 3a22  enPath","type":"
-0001c3e0: 6164 6472 6573 735b 5d22 7d2c 7b22 696e  address[]"},{"in
-0001c3f0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0001c400: 7265 7373 222c 226e 616d 6522 3a22 5f74  ress","name":"_t
-0001c410: 6f22 2c22 7479 7065 223a 2261 6464 7265  o","type":"addre
-0001c420: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-0001c430: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001c440: 6e61 6d65 223a 225f 6465 6164 6c69 6e65  name":"_deadline
-0001c450: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001c460: 3622 7d5d 2c22 6e61 6d65 223a 2273 7761  6"}],"name":"swa
-0001c470: 7045 7861 6374 546f 6b65 6e73 466f 7254  pExactTokensForT
-0001c480: 6f6b 656e 7322 2c22 6f75 7470 7574 7322  okens","outputs"
-0001c490: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0001c4a0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001c4b0: 6522 3a22 616d 6f75 6e74 4f75 7422 2c22  e":"amountOut","
-0001c4c0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001c4d0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-0001c4e0: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
-0001c4f0: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-0001c500: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
-0001c510: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001c520: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001c530: 225f 616d 6f75 6e74 496e 222c 2274 7970  "_amountIn","typ
-0001c540: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-0001c550: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001c560: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001c570: 5f61 6d6f 756e 744f 7574 4d69 6e22 2c22  _amountOutMin","
-0001c580: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001c590: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001c5a0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
-0001c5b0: 6d65 223a 225f 7061 6972 4269 6e53 7465  me":"_pairBinSte
-0001c5c0: 7073 222c 2274 7970 6522 3a22 7569 6e74  ps","type":"uint
-0001c5d0: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
-0001c5e0: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-0001c5f0: 7420 4945 5243 3230 5b5d 222c 226e 616d  t IERC20[]","nam
-0001c600: 6522 3a22 5f74 6f6b 656e 5061 7468 222c  e":"_tokenPath",
-0001c610: 2274 7970 6522 3a22 6164 6472 6573 735b  "type":"address[
-0001c620: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
-0001c630: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0001c640: 616d 6522 3a22 5f74 6f22 2c22 7479 7065  ame":"_to","type
-0001c650: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0001c660: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001c670: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
-0001c680: 6465 6164 6c69 6e65 222c 2274 7970 6522  deadline","type"
-0001c690: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-0001c6a0: 6d65 223a 2273 7761 7045 7861 6374 546f  me":"swapExactTo
-0001c6b0: 6b65 6e73 466f 7254 6f6b 656e 7353 7570  kensForTokensSup
-0001c6c0: 706f 7274 696e 6746 6565 4f6e 5472 616e  portingFeeOnTran
-0001c6d0: 7366 6572 546f 6b65 6e73 222c 226f 7574  sferTokens","out
-0001c6e0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001c6f0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001c700: 2c22 6e61 6d65 223a 2261 6d6f 756e 744f  ,"name":"amountO
-0001c710: 7574 222c 2274 7970 6522 3a22 7569 6e74  ut","type":"uint
-0001c720: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
-0001c730: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
-0001c740: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
-0001c750: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
-0001c760: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0001c770: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001c780: 616d 6522 3a22 5f61 6d6f 756e 7441 5641  ame":"_amountAVA
-0001c790: 584f 7574 222c 2274 7970 6522 3a22 7569  XOut","type":"ui
-0001c7a0: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
-0001c7b0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001c7c0: 222c 226e 616d 6522 3a22 5f61 6d6f 756e  ","name":"_amoun
-0001c7d0: 7449 6e4d 6178 222c 2274 7970 6522 3a22  tInMax","type":"
-0001c7e0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0001c7f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001c800: 3536 5b5d 222c 226e 616d 6522 3a22 5f70  56[]","name":"_p
-0001c810: 6169 7242 696e 5374 6570 7322 2c22 7479  airBinSteps","ty
-0001c820: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
-0001c830: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-0001c840: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
-0001c850: 305b 5d22 2c22 6e61 6d65 223a 225f 746f  0[]","name":"_to
-0001c860: 6b65 6e50 6174 6822 2c22 7479 7065 223a  kenPath","type":
-0001c870: 2261 6464 7265 7373 5b5d 227d 2c7b 2269  "address[]"},{"i
-0001c880: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-0001c890: 6472 6573 7320 7061 7961 626c 6522 2c22  dress payable","
-0001c8a0: 6e61 6d65 223a 225f 746f 222c 2274 7970  name":"_to","typ
-0001c8b0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0001c8c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001c8d0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001c8e0: 5f64 6561 646c 696e 6522 2c22 7479 7065  _deadline","type
-0001c8f0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-0001c900: 616d 6522 3a22 7377 6170 546f 6b65 6e73  ame":"swapTokens
-0001c910: 466f 7245 7861 6374 4156 4158 222c 226f  ForExactAVAX","o
-0001c920: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
-0001c930: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001c940: 365b 5d22 2c22 6e61 6d65 223a 2261 6d6f  6[]","name":"amo
-0001c950: 756e 7473 496e 222c 2274 7970 6522 3a22  untsIn","type":"
-0001c960: 7569 6e74 3235 365b 5d22 7d5d 2c22 7374  uint256[]"}],"st
-0001c970: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-0001c980: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
-0001c990: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-0001c9a0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001c9b0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001c9c0: 3536 222c 226e 616d 6522 3a22 5f61 6d6f  56","name":"_amo
-0001c9d0: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
-0001c9e0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0001c9f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001ca00: 3536 222c 226e 616d 6522 3a22 5f61 6d6f  56","name":"_amo
-0001ca10: 756e 7449 6e4d 6178 222c 2274 7970 6522  untInMax","type"
-0001ca20: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-0001ca30: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001ca40: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
-0001ca50: 5f70 6169 7242 696e 5374 6570 7322 2c22  _pairBinSteps","
-0001ca60: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
-0001ca70: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001ca80: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
-0001ca90: 4332 305b 5d22 2c22 6e61 6d65 223a 225f  C20[]","name":"_
-0001caa0: 746f 6b65 6e50 6174 6822 2c22 7479 7065  tokenPath","type
-0001cab0: 223a 2261 6464 7265 7373 5b5d 227d 2c7b  ":"address[]"},{
-0001cac0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001cad0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
-0001cae0: 225f 746f 222c 2274 7970 6522 3a22 6164  "_to","type":"ad
-0001caf0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
-0001cb00: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001cb10: 222c 226e 616d 6522 3a22 5f64 6561 646c  ","name":"_deadl
-0001cb20: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
-0001cb30: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-0001cb40: 7377 6170 546f 6b65 6e73 466f 7245 7861  swapTokensForExa
-0001cb50: 6374 546f 6b65 6e73 222c 226f 7574 7075  ctTokens","outpu
-0001cb60: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0001cb70: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-0001cb80: 2c22 6e61 6d65 223a 2261 6d6f 756e 7473  ,"name":"amounts
-0001cb90: 496e 222c 2274 7970 6522 3a22 7569 6e74  In","type":"uint
-0001cba0: 3235 365b 5d22 7d5d 2c22 7374 6174 654d  256[]"}],"stateM
-0001cbb0: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-0001cbc0: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-0001cbd0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-0001cbe0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-0001cbf0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-0001cc00: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
-0001cc10: 5f74 6f6b 656e 222c 2274 7970 6522 3a22  _token","type":"
-0001cc20: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
-0001cc30: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0001cc40: 7373 222c 226e 616d 6522 3a22 5f74 6f22  ss","name":"_to"
-0001cc50: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0001cc60: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-0001cc70: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001cc80: 6d65 223a 225f 616d 6f75 6e74 222c 2274  me":"_amount","t
-0001cc90: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-0001cca0: 2c22 6e61 6d65 223a 2273 7765 6570 222c  ,"name":"sweep",
-0001ccb0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
-0001ccc0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-0001ccd0: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
-0001cce0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-0001ccf0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001cd00: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
-0001cd10: 6163 7420 494c 4254 6f6b 656e 222c 226e  act ILBToken","n
-0001cd20: 616d 6522 3a22 5f6c 6254 6f6b 656e 222c  ame":"_lbToken",
-0001cd30: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001cd40: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001cd50: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0001cd60: 6522 3a22 5f74 6f22 2c22 7479 7065 223a  e":"_to","type":
-0001cd70: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-0001cd80: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001cd90: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
-0001cda0: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
-0001cdb0: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
-0001cdc0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001cdd0: 365b 5d22 2c22 6e61 6d65 223a 225f 616d  6[]","name":"_am
-0001cde0: 6f75 6e74 7322 2c22 7479 7065 223a 2275  ounts","type":"u
-0001cdf0: 696e 7432 3536 5b5d 227d 5d2c 226e 616d  int256[]"}],"nam
-0001ce00: 6522 3a22 7377 6565 704c 4254 6f6b 656e  e":"sweepLBToken
-0001ce10: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
-0001ce20: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-0001ce30: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-0001ce40: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-0001ce50: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-0001ce60: 616d 6522 3a22 7761 7661 7822 2c22 6f75  ame":"wavax","ou
-0001ce70: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-0001ce80: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-0001ce90: 7420 4957 4156 4158 222c 226e 616d 6522  t IWAVAX","name"
-0001cea0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
-0001ceb0: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
-0001cec0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-0001ced0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-0001cee0: 227d 2c7b 2273 7461 7465 4d75 7461 6269  "},{"stateMutabi
-0001cef0: 6c69 7479 223a 2270 6179 6162 6c65 222c  lity":"payable",
-0001cf00: 2274 7970 6522 3a22 7265 6365 6976 6522  "type":"receive"
-0001cf10: 7d5d 2729 0a0a 2020 2020 6465 6620 6765  }]')..    def ge
-0001cf20: 745f 6964 5f66 726f 6d5f 7072 6963 6528  t_id_from_price(
-0001cf30: 5f77 6562 333a 5765 6233 2c5f 726f 7574  _web3:Web3,_rout
-0001cf40: 655f 6164 6472 6573 733a 7374 722c 5f72  e_address:str,_r
-0001cf50: 6f75 7465 5f61 6269 2c5f 6c62 5f70 6169  oute_abi,_lb_pai
-0001cf60: 722c 5f70 7269 6365 293a 0a20 2020 2020  r,_price):.     
-0001cf70: 2020 2072 6574 7572 6e20 5f77 6562 332e     return _web3.
-0001cf80: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
-0001cf90: 7265 7373 3d5f 726f 7574 655f 6164 6472  ress=_route_addr
-0001cfa0: 6573 732c 2061 6269 3d5f 726f 7574 655f  ess, abi=_route_
-0001cfb0: 6162 6929 2e66 756e 6374 696f 6e73 2e67  abi).functions.g
-0001cfc0: 6574 4964 4672 6f6d 5072 6963 6528 5f6c  etIdFromPrice(_l
-0001cfd0: 625f 7061 6972 2c5f 7072 6963 6529 2e63  b_pair,_price).c
-0001cfe0: 616c 6c28 290a 0a20 2020 2064 6566 2067  all()..    def g
-0001cff0: 6574 5f70 7269 6365 5f66 726f 6d5f 6964  et_price_from_id
-0001d000: 285f 7765 6233 3a57 6562 332c 5f72 6f75  (_web3:Web3,_rou
-0001d010: 7465 5f61 6464 7265 7373 3a73 7472 2c5f  te_address:str,_
-0001d020: 726f 7574 655f 6162 692c 5f6c 625f 7061  route_abi,_lb_pa
-0001d030: 6972 2c5f 6964 293a 0a20 2020 2020 2020  ir,_id):.       
-0001d040: 2072 6574 7572 6e20 5f77 6562 332e 6574   return _web3.et
-0001d050: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
-0001d060: 7373 3d5f 726f 7574 655f 6164 6472 6573  ss=_route_addres
-0001d070: 732c 2061 6269 3d5f 726f 7574 655f 6162  s, abi=_route_ab
-0001d080: 6929 2e66 756e 6374 696f 6e73 2e67 6574  i).functions.get
-0001d090: 5072 6963 6546 726f 6d49 6428 5f6c 625f  PriceFromId(_lb_
-0001d0a0: 7061 6972 2c5f 6964 292e 6361 6c6c 2829  pair,_id).call()
-0001d0b0: 0a0a 2020 2020 2372 6574 7572 6e20 5b61  ..    #return [a
-0001d0c0: 6d6f 756e 745f 696e 2c66 6565 5d0a 2020  mount_in,fee].  
-0001d0d0: 2020 6465 6620 6765 745f 7377 6170 5f69    def get_swap_i
-0001d0e0: 6e28 5f77 6562 333a 5765 6233 2c5f 726f  n(_web3:Web3,_ro
-0001d0f0: 7574 655f 6164 6472 6573 733a 7374 722c  ute_address:str,
-0001d100: 5f72 6f75 7465 5f61 6269 3a73 7472 2c5f  _route_abi:str,_
-0001d110: 6c62 5f70 6169 722c 5f61 6d6f 756e 745f  lb_pair,_amount_
-0001d120: 6f75 742c 5f73 7761 705f 666f 725f 793a  out,_swap_for_y:
-0001d130: 626f 6f6c 293a 0a20 2020 2020 2020 2072  bool):.        r
-0001d140: 6574 7572 6e20 5f77 6562 332e 6574 682e  eturn _web3.eth.
-0001d150: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
-0001d160: 3d5f 726f 7574 655f 6164 6472 6573 732c  =_route_address,
-0001d170: 2061 6269 3d5f 726f 7574 655f 6162 6929   abi=_route_abi)
-0001d180: 2e66 756e 6374 696f 6e73 2e67 6574 5377  .functions.getSw
-0001d190: 6170 496e 285f 6c62 5f70 6169 722c 5f61  apIn(_lb_pair,_a
-0001d1a0: 6d6f 756e 745f 6f75 742c 5f73 7761 705f  mount_out,_swap_
-0001d1b0: 666f 725f 7929 2e63 616c 6c28 290a 2020  for_y).call().  
-0001d1c0: 2020 0a20 2020 2023 7265 7475 726e 205b    .    #return [
-0001d1d0: 616d 6f75 6e74 5f6f 7574 2c66 6565 5d0a  amount_out,fee].
-0001d1e0: 2020 2020 6465 6620 6765 745f 7377 6170      def get_swap
-0001d1f0: 5f6f 7574 285f 7765 6233 3a57 6562 332c  _out(_web3:Web3,
-0001d200: 5f72 6f75 7465 5f61 6464 7265 7373 3a73  _route_address:s
-0001d210: 7472 2c5f 726f 7574 655f 6162 693a 7374  tr,_route_abi:st
-0001d220: 722c 5f6c 625f 7061 6972 2c5f 616d 6f75  r,_lb_pair,_amou
-0001d230: 6e74 5f69 6e2c 5f73 7761 705f 666f 725f  nt_in,_swap_for_
-0001d240: 793a 626f 6f6c 293a 0a20 2020 2020 2020  y:bool):.       
-0001d250: 2072 6574 7572 6e20 5f77 6562 332e 6574   return _web3.et
-0001d260: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
-0001d270: 7373 3d5f 726f 7574 655f 6164 6472 6573  ss=_route_addres
-0001d280: 732c 2061 6269 3d5f 726f 7574 655f 6162  s, abi=_route_ab
-0001d290: 6929 2e66 756e 6374 696f 6e73 2e67 6574  i).functions.get
-0001d2a0: 5377 6170 4f75 7428 5f6c 625f 7061 6972  SwapOut(_lb_pair
-0001d2b0: 2c5f 616d 6f75 6e74 5f69 6e2c 5f73 7761  ,_amount_in,_swa
-0001d2c0: 705f 666f 725f 7929 2e63 616c 6c28 290a  p_for_y).call().
-0001d2d0: 0a20 2020 2064 6566 2073 7761 705f 6578  .    def swap_ex
-0001d2e0: 6163 745f 746f 6b65 6e73 5f66 6f72 5f74  act_tokens_for_t
-0001d2f0: 6f6b 656e 7328 5f77 6562 333a 5765 6233  okens(_web3:Web3
-0001d300: 2c5f 726f 7574 655f 6164 6472 6573 733a  ,_route_address:
-0001d310: 7374 722c 5f72 6f75 7465 5f61 6269 2c0a  str,_route_abi,.
-0001d320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d340: 2020 2020 205f 616d 6f75 6e74 5f69 6e2c       _amount_in,
-0001d350: 5f61 6d6f 756e 745f 6f75 745f 6d69 6e2c  _amount_out_min,
-0001d360: 5f70 6169 725f 6269 6e5f 7374 6570 732c  _pair_bin_steps,
-0001d370: 5f74 6f6b 656e 5f70 6174 682c 5f74 6f2c  _token_path,_to,
-0001d380: 5f64 6561 646c 696e 652c 0a20 2020 2020  _deadline,.     
-0001d390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d3b0: 5f70 7562 6c69 635f 6b65 792c 5f70 7269  _public_key,_pri
-0001d3c0: 7661 7465 5f6b 6579 293a 0a20 2020 2020  vate_key):.     
-0001d3d0: 2020 206e 6f6e 6365 3d5f 7765 6233 2e65     nonce=_web3.e
-0001d3e0: 7468 2e67 6574 5f74 7261 6e73 6163 7469  th.get_transacti
-0001d3f0: 6f6e 5f63 6f75 6e74 285f 7075 626c 6963  on_count(_public
-0001d400: 5f6b 6579 290a 2020 2020 2020 2020 726f  _key).        ro
-0001d410: 7574 655f 636f 6e74 7261 6374 3d5f 7765  ute_contract=_we
-0001d420: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
-0001d430: 6164 6472 6573 733d 5f72 6f75 7465 5f61  address=_route_a
-0001d440: 6464 7265 7373 2c20 6162 693d 5f72 6f75  ddress, abi=_rou
-0001d450: 7465 5f61 6269 290a 2020 2020 2020 2020  te_abi).        
-0001d460: 7377 6170 5f66 756e 6374 696f 6e3d 726f  swap_function=ro
-0001d470: 7574 655f 636f 6e74 7261 6374 2e66 756e  ute_contract.fun
-0001d480: 6374 696f 6e73 2e73 7761 7045 7861 6374  ctions.swapExact
-0001d490: 546f 6b65 6e73 466f 7254 6f6b 656e 7328  TokensForTokens(
-0001d4a0: 5f61 6d6f 756e 745f 696e 2c5f 616d 6f75  _amount_in,_amou
-0001d4b0: 6e74 5f6f 7574 5f6d 696e 2c5f 7061 6972  nt_out_min,_pair
-0001d4c0: 5f62 696e 5f73 7465 7073 2c5f 746f 6b65  _bin_steps,_toke
-0001d4d0: 6e5f 7061 7468 2c5f 746f 2c5f 6465 6164  n_path,_to,_dead
-0001d4e0: 6c69 6e65 290a 2020 2020 2020 2020 7061  line).        pa
-0001d4f0: 7261 6d73 3d7b 0a20 2020 2020 2020 2020  rams={.         
-0001d500: 2020 2027 6672 6f6d 273a 205f 7075 626c     'from': _publ
-0001d510: 6963 5f6b 6579 2c0a 2020 2020 2020 2020  ic_key,.        
-0001d520: 2020 2020 2776 616c 7565 273a 2030 2c0a      'value': 0,.
-0001d530: 2020 2020 2020 2020 2020 2020 276e 6f6e              'non
-0001d540: 6365 273a 206e 6f6e 6365 2c0a 2020 2020  ce': nonce,.    
-0001d550: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
-0001d560: 2730 7832 270a 2020 2020 2020 2020 7d0a  '0x2'.        }.
-0001d570: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
-0001d580: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
-0001d590: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
-0001d5a0: 6e5f 7472 616e 7361 6374 696f 6e28 7377  n_transaction(sw
-0001d5b0: 6170 5f66 756e 6374 696f 6e2e 6275 696c  ap_function.buil
-0001d5c0: 6454 7261 6e73 6163 7469 6f6e 2870 6172  dTransaction(par
-0001d5d0: 616d 7329 2c70 7269 7661 7465 5f6b 6579  ams),private_key
-0001d5e0: 3d5f 7072 6976 6174 655f 6b65 7929 0a20  =_private_key). 
-0001d5f0: 2020 2020 2020 2072 6573 706f 6e73 653d         response=
-0001d600: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
-0001d610: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
-0001d620: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
-0001d630: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
-0001d640: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-0001d650: 2057 6562 332e 746f 4865 7828 7265 7370   Web3.toHex(resp
-0001d660: 6f6e 7365 290a 2020 2020 0a20 2020 2064  onse).    .    d
-0001d670: 6566 2073 7761 705f 746f 6b65 6e73 5f66  ef swap_tokens_f
-0001d680: 6f72 5f65 7861 6374 5f74 6f6b 656e 7328  or_exact_tokens(
-0001d690: 5f77 6562 333a 5765 6233 2c5f 726f 7574  _web3:Web3,_rout
-0001d6a0: 655f 6164 6472 6573 733a 7374 722c 5f72  e_address:str,_r
-0001d6b0: 6f75 7465 5f61 6269 2c0a 2020 2020 2020  oute_abi,.      
-0001d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d6d0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-0001d6e0: 616d 6f75 6e74 5f6f 7574 2c5f 616d 6f75  amount_out,_amou
-0001d6f0: 6e74 5f69 6e5f 6d61 782c 5f70 6169 725f  nt_in_max,_pair_
-0001d700: 6269 6e5f 7374 6570 732c 5f74 6f6b 656e  bin_steps,_token
-0001d710: 5f70 6174 682c 5f74 6f2c 5f64 6561 646c  _path,_to,_deadl
-0001d720: 696e 652c 0a20 2020 2020 2020 2020 2020  ine,.           
-0001d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d740: 2020 2020 2020 2020 2020 5f70 7562 6c69            _publi
-0001d750: 635f 6b65 792c 5f70 7269 7661 7465 5f6b  c_key,_private_k
-0001d760: 6579 293a 0a20 2020 2020 2020 206e 6f6e  ey):.        non
-0001d770: 6365 3d5f 7765 6233 2e65 7468 2e67 6574  ce=_web3.eth.get
-0001d780: 5f74 7261 6e73 6163 7469 6f6e 5f63 6f75  _transaction_cou
-0001d790: 6e74 285f 7075 626c 6963 5f6b 6579 290a  nt(_public_key).
-0001d7a0: 2020 2020 2020 2020 726f 7574 655f 636f          route_co
-0001d7b0: 6e74 7261 6374 3d5f 7765 6233 2e65 7468  ntract=_web3.eth
-0001d7c0: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
-0001d7d0: 733d 5f72 6f75 7465 5f61 6464 7265 7373  s=_route_address
-0001d7e0: 2c20 6162 693d 5f72 6f75 7465 5f61 6269  , abi=_route_abi
-0001d7f0: 290a 2020 2020 2020 2020 7377 6170 5f66  ).        swap_f
-0001d800: 756e 6374 696f 6e3d 726f 7574 655f 636f  unction=route_co
-0001d810: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
-0001d820: 2e73 7761 7054 6f6b 656e 7346 6f72 4578  .swapTokensForEx
-0001d830: 6163 7454 6f6b 656e 7328 5f61 6d6f 756e  actTokens(_amoun
-0001d840: 745f 6f75 742c 5f61 6d6f 756e 745f 696e  t_out,_amount_in
-0001d850: 5f6d 6178 2c5f 7061 6972 5f62 696e 5f73  _max,_pair_bin_s
-0001d860: 7465 7073 2c5f 746f 6b65 6e5f 7061 7468  teps,_token_path
-0001d870: 2c5f 746f 2c5f 6465 6164 6c69 6e65 290a  ,_to,_deadline).
-0001d880: 2020 2020 2020 2020 7061 7261 6d73 3d7b          params={
-0001d890: 0a20 2020 2020 2020 2020 2020 2027 6672  .            'fr
-0001d8a0: 6f6d 273a 205f 7075 626c 6963 5f6b 6579  om': _public_key
-0001d8b0: 2c0a 2020 2020 2020 2020 2020 2020 2776  ,.            'v
-0001d8c0: 616c 7565 273a 2030 2c0a 2020 2020 2020  alue': 0,.      
-0001d8d0: 2020 2020 2020 276e 6f6e 6365 273a 206e        'nonce': n
-0001d8e0: 6f6e 6365 2c0a 2020 2020 2020 2020 2020  once,.          
-0001d8f0: 2020 2774 7970 6527 3a20 2730 7832 270a    'type': '0x2'.
-0001d900: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-0001d910: 2020 7369 676e 6564 5f74 7261 6e73 6163    signed_transac
-0001d920: 7469 6f6e 3d5f 7765 6233 2e65 7468 2e61  tion=_web3.eth.a
-0001d930: 6363 6f75 6e74 2e73 6967 6e5f 7472 616e  ccount.sign_tran
-0001d940: 7361 6374 696f 6e28 7377 6170 5f66 756e  saction(swap_fun
-0001d950: 6374 696f 6e2e 6275 696c 6454 7261 6e73  ction.buildTrans
-0001d960: 6163 7469 6f6e 2870 6172 616d 7329 2c70  action(params),p
-0001d970: 7269 7661 7465 5f6b 6579 3d5f 7072 6976  rivate_key=_priv
-0001d980: 6174 655f 6b65 7929 0a20 2020 2020 2020  ate_key).       
-0001d990: 2072 6573 706f 6e73 653d 5f77 6562 332e   response=_web3.
-0001d9a0: 6574 682e 7365 6e64 5f72 6177 5f74 7261  eth.send_raw_tra
-0001d9b0: 6e73 6163 7469 6f6e 2873 6967 6e65 645f  nsaction(signed_
-0001d9c0: 7472 616e 7361 6374 696f 6e2e 7261 7754  transaction.rawT
-0001d9d0: 7261 6e73 6163 7469 6f6e 290a 2020 2020  ransaction).    
-0001d9e0: 2020 2020 7265 7475 726e 2057 6562 332e      return Web3.
-0001d9f0: 746f 4865 7828 7265 7370 6f6e 7365 290a  toHex(response).
-0001da00: 0a63 6c61 7373 204a 6f65 5632 5061 6972  .class JoeV2Pair
-0001da10: 3a0a 0a20 2020 206a 6f65 5f70 6169 725f  :..    joe_pair_
-0001da20: 7632 5f61 6269 3d6a 736f 6e2e 6c6f 6164  v2_abi=json.load
-0001da30: 7328 275b 7b22 696e 7075 7473 223a 5b7b  s('[{"inputs":[{
-0001da40: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001da50: 636f 6e74 7261 6374 2049 4c42 4661 6374  contract ILBFact
-0001da60: 6f72 7922 2c22 6e61 6d65 223a 225f 6661  ory","name":"_fa
-0001da70: 6374 6f72 7922 2c22 7479 7065 223a 2261  ctory","type":"a
-0001da80: 6464 7265 7373 227d 5d2c 2273 7461 7465  ddress"}],"state
-0001da90: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-0001daa0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-0001dab0: 2263 6f6e 7374 7275 6374 6f72 227d 2c7b  "constructor"},{
-0001dac0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001dad0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001dae0: 3536 222c 226e 616d 6522 3a22 6270 222c  56","name":"bp",
-0001daf0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001db00: 7d5d 2c22 6e61 6d65 223a 2242 696e 4865  }],"name":"BinHe
-0001db10: 6c70 6572 5f5f 4269 6e53 7465 704f 7665  lper__BinStepOve
-0001db20: 7266 6c6f 7773 222c 2274 7970 6522 3a22  rflows","type":"
-0001db30: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
-0001db40: 223a 5b5d 2c22 6e61 6d65 223a 2242 696e  ":[],"name":"Bin
-0001db50: 4865 6c70 6572 5f5f 4964 4f76 6572 666c  Helper__IdOverfl
-0001db60: 6f77 7322 2c22 7479 7065 223a 2265 7272  ows","type":"err
-0001db70: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-0001db80: 5d2c 226e 616d 6522 3a22 4c42 5061 6972  ],"name":"LBPair
-0001db90: 5f5f 4164 6472 6573 735a 6572 6f22 2c22  __AddressZero","
-0001dba0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-0001dbb0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-0001dbc0: 6522 3a22 4c42 5061 6972 5f5f 4164 6472  e":"LBPair__Addr
-0001dbd0: 6573 735a 6572 6f4f 7254 6869 7322 2c22  essZeroOrThis","
-0001dbe0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-0001dbf0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-0001dc00: 6522 3a22 4c42 5061 6972 5f5f 416c 7265  e":"LBPair__Alre
-0001dc10: 6164 7949 6e69 7469 616c 697a 6564 222c  adyInitialized",
-0001dc20: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-0001dc30: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-0001dc40: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001dc50: 3235 3622 2c22 6e61 6d65 223a 2269 6422  256","name":"id"
-0001dc60: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001dc70: 227d 5d2c 226e 616d 6522 3a22 4c42 5061  "}],"name":"LBPa
-0001dc80: 6972 5f5f 436f 6d70 6f73 6974 696f 6e46  ir__CompositionF
-0001dc90: 6163 746f 7246 6c61 7765 6422 2c22 7479  actorFlawed","ty
-0001dca0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-0001dcb0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-0001dcc0: 3a22 4c42 5061 6972 5f5f 4469 7374 7269  :"LBPair__Distri
-0001dcd0: 6275 7469 6f6e 734f 7665 7266 6c6f 7722  butionsOverflow"
-0001dce0: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001dcf0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-0001dd00: 616d 6522 3a22 4c42 5061 6972 5f5f 466c  ame":"LBPair__Fl
-0001dd10: 6173 684c 6f61 6e43 616c 6c62 6163 6b46  ashLoanCallbackF
-0001dd20: 6169 6c65 6422 2c22 7479 7065 223a 2265  ailed","type":"e
-0001dd30: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-0001dd40: 3a5b 5d2c 226e 616d 6522 3a22 4c42 5061  :[],"name":"LBPa
-0001dd50: 6972 5f5f 466c 6173 684c 6f61 6e49 6e76  ir__FlashLoanInv
-0001dd60: 616c 6964 4261 6c61 6e63 6522 2c22 7479  alidBalance","ty
-0001dd70: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-0001dd80: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-0001dd90: 3a22 4c42 5061 6972 5f5f 466c 6173 684c  :"LBPair__FlashL
-0001dda0: 6f61 6e49 6e76 616c 6964 546f 6b65 6e22  oanInvalidToken"
-0001ddb0: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001ddc0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-0001ddd0: 616d 6522 3a22 4c42 5061 6972 5f5f 496e  ame":"LBPair__In
-0001dde0: 7375 6666 6963 6965 6e74 416d 6f75 6e74  sufficientAmount
-0001ddf0: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
-0001de00: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-0001de10: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001de20: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001de30: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
-0001de40: 3235 3622 7d5d 2c22 6e61 6d65 223a 224c  256"}],"name":"L
-0001de50: 4250 6169 725f 5f49 6e73 7566 6669 6369  BPair__Insuffici
-0001de60: 656e 744c 6971 7569 6469 7479 4275 726e  entLiquidityBurn
-0001de70: 6564 222c 2274 7970 6522 3a22 6572 726f  ed","type":"erro
-0001de80: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
-0001de90: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001dea0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001deb0: 2269 6422 2c22 7479 7065 223a 2275 696e  "id","type":"uin
-0001dec0: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-0001ded0: 4c42 5061 6972 5f5f 496e 7375 6666 6963  LBPair__Insuffic
-0001dee0: 6965 6e74 4c69 7175 6964 6974 794d 696e  ientLiquidityMin
-0001def0: 7465 6422 2c22 7479 7065 223a 2265 7272  ted","type":"err
-0001df00: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
-0001df10: 5d2c 226e 616d 6522 3a22 4c42 5061 6972  ],"name":"LBPair
-0001df20: 5f5f 4f6e 6c79 4661 6374 6f72 7922 2c22  __OnlyFactory","
-0001df30: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-0001df40: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001df50: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0001df60: 7373 222c 226e 616d 6522 3a22 6665 6552  ss","name":"feeR
-0001df70: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
-0001df80: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001df90: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0001dfa0: 7265 7373 222c 226e 616d 6522 3a22 7365  ress","name":"se
-0001dfb0: 6e64 6572 222c 2274 7970 6522 3a22 6164  nder","type":"ad
-0001dfc0: 6472 6573 7322 7d5d 2c22 6e61 6d65 223a  dress"}],"name":
-0001dfd0: 224c 4250 6169 725f 5f4f 6e6c 7946 6565  "LBPair__OnlyFee
-0001dfe0: 5265 6369 7069 656e 7422 2c22 7479 7065  Recipient","type
-0001dff0: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
-0001e000: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-0001e010: 4c42 5061 6972 5f5f 4f6e 6c79 5374 7269  LBPair__OnlyStri
-0001e020: 6374 6c79 496e 6372 6561 7369 6e67 4964  ctlyIncreasingId
-0001e030: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001e040: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-0001e050: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001e060: 6e74 3235 3622 2c22 6e61 6d65 223a 226e  nt256","name":"n
-0001e070: 6577 5369 7a65 222c 2274 7970 6522 3a22  ewSize","type":"
-0001e080: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0001e090: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001e0a0: 3536 222c 226e 616d 6522 3a22 6f72 6163  56","name":"orac
-0001e0b0: 6c65 5369 7a65 222c 2274 7970 6522 3a22  leSize","type":"
-0001e0c0: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
-0001e0d0: 223a 224c 4250 6169 725f 5f4f 7261 636c  ":"LBPair__Oracl
-0001e0e0: 654e 6577 5369 7a65 546f 6f53 6d61 6c6c  eNewSizeTooSmall
-0001e0f0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001e100: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-0001e110: 6e61 6d65 223a 224c 4250 6169 725f 5f57  name":"LBPair__W
-0001e120: 726f 6e67 4c65 6e67 7468 7322 2c22 7479  rongLengths","ty
-0001e130: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-0001e140: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-0001e150: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-0001e160: 222c 226e 616d 6522 3a22 6672 6f6d 222c  ","name":"from",
-0001e170: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001e180: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001e190: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001e1a0: 6522 3a22 6964 222c 2274 7970 6522 3a22  e":"id","type":"
-0001e1b0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-0001e1c0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001e1d0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-0001e1e0: 6e74 222c 2274 7970 6522 3a22 7569 6e74  nt","type":"uint
-0001e1f0: 3235 3622 7d5d 2c22 6e61 6d65 223a 224c  256"}],"name":"L
-0001e200: 4254 6f6b 656e 5f5f 4275 726e 4578 6365  BToken__BurnExce
-0001e210: 6564 7342 616c 616e 6365 222c 2274 7970  edsBalance","typ
-0001e220: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001e230: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-0001e240: 224c 4254 6f6b 656e 5f5f 4275 726e 4672  "LBToken__BurnFr
-0001e250: 6f6d 4164 6472 6573 7330 222c 2274 7970  omAddress0","typ
-0001e260: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001e270: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001e280: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001e290: 2c22 6e61 6d65 223a 2261 6363 6f75 6e74  ,"name":"account
-0001e2a0: 734c 656e 6774 6822 2c22 7479 7065 223a  sLength","type":
-0001e2b0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-0001e2c0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001e2d0: 3235 3622 2c22 6e61 6d65 223a 2269 6473  256","name":"ids
-0001e2e0: 4c65 6e67 7468 222c 2274 7970 6522 3a22  Length","type":"
-0001e2f0: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
-0001e300: 223a 224c 4254 6f6b 656e 5f5f 4c65 6e67  ":"LBToken__Leng
-0001e310: 7468 4d69 736d 6174 6368 222c 2274 7970  thMismatch","typ
-0001e320: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001e330: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-0001e340: 224c 4254 6f6b 656e 5f5f 4d69 6e74 546f  "LBToken__MintTo
-0001e350: 4164 6472 6573 7330 222c 2274 7970 6522  Address0","type"
-0001e360: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
-0001e370: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-0001e380: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0001e390: 6e61 6d65 223a 226f 776e 6572 222c 2274  name":"owner","t
-0001e3a0: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
-0001e3b0: 2c22 6e61 6d65 223a 224c 4254 6f6b 656e  ,"name":"LBToken
-0001e3c0: 5f5f 5365 6c66 4170 7072 6f76 616c 222c  __SelfApproval",
-0001e3d0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-0001e3e0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-0001e3f0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0001e400: 6573 7322 2c22 6e61 6d65 223a 226f 776e  ess","name":"own
-0001e410: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
-0001e420: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-0001e430: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-0001e440: 226e 616d 6522 3a22 7370 656e 6465 7222  "name":"spender"
-0001e450: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0001e460: 227d 5d2c 226e 616d 6522 3a22 4c42 546f  "}],"name":"LBTo
-0001e470: 6b65 6e5f 5f53 7065 6e64 6572 4e6f 7441  ken__SpenderNotA
-0001e480: 7070 726f 7665 6422 2c22 7479 7065 223a  pproved","type":
-0001e490: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
-0001e4a0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0001e4b0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0001e4c0: 616d 6522 3a22 6672 6f6d 222c 2274 7970  ame":"from","typ
-0001e4d0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-0001e4e0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001e4f0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001e500: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
-0001e510: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
-0001e520: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001e530: 226e 616d 6522 3a22 616d 6f75 6e74 222c  "name":"amount",
-0001e540: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001e550: 7d5d 2c22 6e61 6d65 223a 224c 4254 6f6b  }],"name":"LBTok
-0001e560: 656e 5f5f 5472 616e 7366 6572 4578 6365  en__TransferExce
-0001e570: 6564 7342 616c 616e 6365 222c 2274 7970  edsBalance","typ
-0001e580: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001e590: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-0001e5a0: 224c 4254 6f6b 656e 5f5f 5472 616e 7366  "LBToken__Transf
-0001e5b0: 6572 4672 6f6d 4f72 546f 4164 6472 6573  erFromOrToAddres
-0001e5c0: 7330 222c 2274 7970 6522 3a22 6572 726f  s0","type":"erro
-0001e5d0: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-0001e5e0: 2c22 6e61 6d65 223a 224c 4254 6f6b 656e  ,"name":"LBToken
-0001e5f0: 5f5f 5472 616e 7366 6572 546f 5365 6c66  __TransferToSelf
-0001e600: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001e610: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-0001e620: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001e630: 6e74 3235 3622 2c22 6e61 6d65 223a 2278  nt256","name":"x
-0001e640: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001e650: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-0001e660: 7065 223a 2269 6e74 3235 3622 2c22 6e61  pe":"int256","na
-0001e670: 6d65 223a 2279 222c 2274 7970 6522 3a22  me":"y","type":"
-0001e680: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-0001e690: 3a22 4d61 7468 3132 3878 3132 385f 5f50  :"Math128x128__P
-0001e6a0: 6f77 6572 556e 6465 7266 6c6f 7722 2c22  owerUnderflow","
-0001e6b0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
-0001e6c0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-0001e6d0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001e6e0: 3536 222c 226e 616d 6522 3a22 7072 6f64  56","name":"prod
-0001e6f0: 3122 2c22 7479 7065 223a 2275 696e 7432  1","type":"uint2
-0001e700: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-0001e710: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-0001e720: 6e61 6d65 223a 2264 656e 6f6d 696e 6174  name":"denominat
-0001e730: 6f72 222c 2274 7970 6522 3a22 7569 6e74  or","type":"uint
-0001e740: 3235 3622 7d5d 2c22 6e61 6d65 223a 224d  256"}],"name":"M
-0001e750: 6174 6835 3132 4269 7473 5f5f 4d75 6c44  ath512Bits__MulD
-0001e760: 6976 4f76 6572 666c 6f77 222c 2274 7970  ivOverflow","typ
-0001e770: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001e780: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001e790: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001e7a0: 2c22 6e61 6d65 223a 2270 726f 6431 222c  ,"name":"prod1",
-0001e7b0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001e7c0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001e7d0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001e7e0: 6522 3a22 6f66 6673 6574 222c 2274 7970  e":"offset","typ
-0001e7f0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001e800: 6e61 6d65 223a 224d 6174 6835 3132 4269  name":"Math512Bi
-0001e810: 7473 5f5f 4d75 6c53 6869 6674 4f76 6572  ts__MulShiftOver
-0001e820: 666c 6f77 222c 2274 7970 6522 3a22 6572  flow","type":"er
-0001e830: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
-0001e840: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-0001e850: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001e860: 223a 226f 6666 7365 7422 2c22 7479 7065  ":"offset","type
-0001e870: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
-0001e880: 616d 6522 3a22 4d61 7468 3531 3242 6974  ame":"Math512Bit
-0001e890: 735f 5f4f 6666 7365 744f 7665 7266 6c6f  s__OffsetOverflo
-0001e8a0: 7773 222c 2274 7970 6522 3a22 6572 726f  ws","type":"erro
-0001e8b0: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
-0001e8c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001e8d0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001e8e0: 225f 6d69 6e54 696d 6573 7461 6d70 222c  "_minTimestamp",
-0001e8f0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001e900: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001e910: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001e920: 6522 3a22 5f6c 6f6f 6b55 7054 696d 6573  e":"_lookUpTimes
-0001e930: 7461 6d70 222c 2274 7970 6522 3a22 7569  tamp","type":"ui
-0001e940: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
-0001e950: 224f 7261 636c 655f 5f4c 6f6f 6b55 7054  "Oracle__LookUpT
-0001e960: 696d 6573 7461 6d70 546f 6f4f 6c64 222c  imestampTooOld",
-0001e970: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-0001e980: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-0001e990: 6d65 223a 224f 7261 636c 655f 5f4e 6f74  me":"Oracle__Not
-0001e9a0: 496e 6974 6961 6c69 7a65 6422 2c22 7479  Initialized","ty
-0001e9b0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
-0001e9c0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-0001e9d0: 3a22 5265 656e 7472 616e 6379 4775 6172  :"ReentrancyGuar
-0001e9e0: 6455 7067 7261 6465 6162 6c65 5f5f 416c  dUpgradeable__Al
-0001e9f0: 7265 6164 7949 6e69 7469 616c 697a 6564  readyInitialized
-0001ea00: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001ea10: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-0001ea20: 6e61 6d65 223a 2252 6565 6e74 7261 6e63  name":"Reentranc
-0001ea30: 7947 7561 7264 5570 6772 6164 6561 626c  yGuardUpgradeabl
-0001ea40: 655f 5f52 6565 6e74 7261 6e74 4361 6c6c  e__ReentrantCall
-0001ea50: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001ea60: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-0001ea70: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-0001ea80: 6e74 3235 3622 2c22 6e61 6d65 223a 2278  nt256","name":"x
-0001ea90: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001eaa0: 3622 7d5d 2c22 6e61 6d65 223a 2253 6166  6"}],"name":"Saf
-0001eab0: 6543 6173 745f 5f45 7863 6565 6473 3131  eCast__Exceeds11
-0001eac0: 3242 6974 7322 2c22 7479 7065 223a 2265  2Bits","type":"e
-0001ead0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
-0001eae0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-0001eaf0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001eb00: 6522 3a22 7822 2c22 7479 7065 223a 2275  e":"x","type":"u
-0001eb10: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
-0001eb20: 3a22 5361 6665 4361 7374 5f5f 4578 6365  :"SafeCast__Exce
-0001eb30: 6564 7331 3238 4269 7473 222c 2274 7970  eds128Bits","typ
-0001eb40: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
-0001eb50: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-0001eb60: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001eb70: 2c22 6e61 6d65 223a 2278 222c 2274 7970  ,"name":"x","typ
-0001eb80: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001eb90: 6e61 6d65 223a 2253 6166 6543 6173 745f  name":"SafeCast_
-0001eba0: 5f45 7863 6565 6473 3234 4269 7473 222c  _Exceeds24Bits",
-0001ebb0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
-0001ebc0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
-0001ebd0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001ebe0: 3235 3622 2c22 6e61 6d65 223a 2278 222c  256","name":"x",
-0001ebf0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001ec00: 7d5d 2c22 6e61 6d65 223a 2253 6166 6543  }],"name":"SafeC
-0001ec10: 6173 745f 5f45 7863 6565 6473 3430 4269  ast__Exceeds40Bi
-0001ec20: 7473 222c 2274 7970 6522 3a22 6572 726f  ts","type":"erro
-0001ec30: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
-0001ec40: 2c22 6e61 6d65 223a 2254 6f6b 656e 4865  ,"name":"TokenHe
-0001ec50: 6c70 6572 5f5f 4361 6c6c 4661 696c 6564  lper__CallFailed
-0001ec60: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
-0001ec70: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
-0001ec80: 6e61 6d65 223a 2254 6f6b 656e 4865 6c70  name":"TokenHelp
-0001ec90: 6572 5f5f 4e6f 6e43 6f6e 7472 6163 7422  er__NonContract"
-0001eca0: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
-0001ecb0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-0001ecc0: 616d 6522 3a22 546f 6b65 6e48 656c 7065  ame":"TokenHelpe
-0001ecd0: 725f 5f54 7261 6e73 6665 7246 6169 6c65  r__TransferFaile
-0001ece0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
-0001ecf0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-0001ed00: 226e 616d 6522 3a22 5472 6565 4d61 7468  "name":"TreeMath
-0001ed10: 5f5f 4572 726f 7244 6570 7468 5365 6172  __ErrorDepthSear
-0001ed20: 6368 222c 2274 7970 6522 3a22 6572 726f  ch","type":"erro
-0001ed30: 7222 7d2c 7b22 616e 6f6e 796d 6f75 7322  r"},{"anonymous"
-0001ed40: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
-0001ed50: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
-0001ed60: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001ed70: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0001ed80: 3a22 6163 636f 756e 7422 2c22 7479 7065  :"account","type
-0001ed90: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0001eda0: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
-0001edb0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0001edc0: 7265 7373 222c 226e 616d 6522 3a22 7365  ress","name":"se
-0001edd0: 6e64 6572 222c 2274 7970 6522 3a22 6164  nder","type":"ad
-0001ede0: 6472 6573 7322 7d2c 7b22 696e 6465 7865  dress"},{"indexe
-0001edf0: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
-0001ee00: 616c 5479 7065 223a 2262 6f6f 6c22 2c22  alType":"bool","
-0001ee10: 6e61 6d65 223a 2261 7070 726f 7665 6422  name":"approved"
-0001ee20: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
-0001ee30: 2c22 6e61 6d65 223a 2241 7070 726f 7661  ,"name":"Approva
-0001ee40: 6c46 6f72 416c 6c22 2c22 7479 7065 223a  lForAll","type":
-0001ee50: 2265 7665 6e74 227d 2c7b 2261 6e6f 6e79  "event"},{"anony
-0001ee60: 6d6f 7573 223a 6661 6c73 652c 2269 6e70  mous":false,"inp
-0001ee70: 7574 7322 3a5b 7b22 696e 6465 7865 6422  uts":[{"indexed"
-0001ee80: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
-0001ee90: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0001eea0: 6e61 6d65 223a 2273 656e 6465 7222 2c22  name":"sender","
-0001eeb0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-0001eec0: 2c7b 2269 6e64 6578 6564 223a 7472 7565  ,{"indexed":true
-0001eed0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001eee0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0001eef0: 3a22 7265 6369 7069 656e 7422 2c22 7479  :"recipient","ty
-0001ef00: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0001ef10: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
-0001ef20: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-0001ef30: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-0001ef40: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
-0001ef50: 3235 3622 7d2c 7b22 696e 6465 7865 6422  256"},{"indexed"
-0001ef60: 3a66 616c 7365 2c22 696e 7465 726e 616c  :false,"internal
-0001ef70: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
-0001ef80: 226e 616d 6522 3a22 6665 6573 5822 2c22  "name":"feesX","
-0001ef90: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001efa0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-0001efb0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001efc0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001efd0: 223a 2266 6565 7359 222c 2274 7970 6522  ":"feesY","type"
-0001efe0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-0001eff0: 6d65 223a 2243 6f6d 706f 7369 7469 6f6e  me":"Composition
-0001f000: 4665 6522 2c22 7479 7065 223a 2265 7665  Fee","type":"eve
-0001f010: 6e74 227d 2c7b 2261 6e6f 6e79 6d6f 7573  nt"},{"anonymous
-0001f020: 223a 6661 6c73 652c 2269 6e70 7574 7322  ":false,"inputs"
-0001f030: 3a5b 7b22 696e 6465 7865 6422 3a74 7275  :[{"indexed":tru
-0001f040: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001f050: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-0001f060: 223a 2273 656e 6465 7222 2c22 7479 7065  ":"sender","type
-0001f070: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0001f080: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
-0001f090: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0001f0a0: 7265 7373 222c 226e 616d 6522 3a22 7265  ress","name":"re
-0001f0b0: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
-0001f0c0: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
-0001f0d0: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
-0001f0e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001f0f0: 3536 222c 226e 616d 6522 3a22 6964 222c  56","name":"id",
-0001f100: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001f110: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-0001f120: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-0001f130: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001f140: 6522 3a22 616d 6f75 6e74 5822 2c22 7479  e":"amountX","ty
-0001f150: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-0001f160: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
-0001f170: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-0001f180: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-0001f190: 2261 6d6f 756e 7459 222c 2274 7970 6522  "amountY","type"
-0001f1a0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
-0001f1b0: 6d65 223a 2244 6570 6f73 6974 6564 546f  me":"DepositedTo
-0001f1c0: 4269 6e22 2c22 7479 7065 223a 2265 7665  Bin","type":"eve
-0001f1d0: 6e74 227d 2c7b 2261 6e6f 6e79 6d6f 7573  nt"},{"anonymous
-0001f1e0: 223a 6661 6c73 652c 2269 6e70 7574 7322  ":false,"inputs"
-0001f1f0: 3a5b 7b22 696e 6465 7865 6422 3a74 7275  :[{"indexed":tru
-0001f200: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001f210: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
-0001f220: 223a 2273 656e 6465 7222 2c22 7479 7065  ":"sender","type
-0001f230: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0001f240: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
-0001f250: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-0001f260: 7265 7373 222c 226e 616d 6522 3a22 7265  ress","name":"re
-0001f270: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
-0001f280: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
-0001f290: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-0001f2a0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001f2b0: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0001f2c0: 756e 7458 222c 2274 7970 6522 3a22 7569  untX","type":"ui
-0001f2d0: 6e74 3235 3622 7d2c 7b22 696e 6465 7865  nt256"},{"indexe
-0001f2e0: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
-0001f2f0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-0001f300: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
-0001f310: 5922 2c22 7479 7065 223a 2275 696e 7432  Y","type":"uint2
-0001f320: 3536 227d 5d2c 226e 616d 6522 3a22 4665  56"}],"name":"Fe
-0001f330: 6573 436f 6c6c 6563 7465 6422 2c22 7479  esCollected","ty
-0001f340: 7065 223a 2265 7665 6e74 227d 2c7b 2261  pe":"event"},{"a
-0001f350: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
-0001f360: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
-0001f370: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
-0001f380: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0001f390: 7322 2c22 6e61 6d65 223a 2273 656e 6465  s","name":"sende
-0001f3a0: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
-0001f3b0: 7373 227d 2c7b 2269 6e64 6578 6564 223a  ss"},{"indexed":
-0001f3c0: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
-0001f3d0: 7065 223a 2263 6f6e 7472 6163 7420 494c  pe":"contract IL
-0001f3e0: 4246 6c61 7368 4c6f 616e 4361 6c6c 6261  BFlashLoanCallba
-0001f3f0: 636b 222c 226e 616d 6522 3a22 7265 6365  ck","name":"rece
-0001f400: 6976 6572 222c 2274 7970 6522 3a22 6164  iver","type":"ad
-0001f410: 6472 6573 7322 7d2c 7b22 696e 6465 7865  dress"},{"indexe
-0001f420: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
-0001f430: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-0001f440: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
-0001f450: 3a22 746f 6b65 6e22 2c22 7479 7065 223a  :"token","type":
-0001f460: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
-0001f470: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-0001f480: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001f490: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
-0001f4a0: 756e 7422 2c22 7479 7065 223a 2275 696e  unt","type":"uin
-0001f4b0: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
-0001f4c0: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
-0001f4d0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-0001f4e0: 2c22 6e61 6d65 223a 2266 6565 222c 2274  ,"name":"fee","t
-0001f4f0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-0001f500: 2c22 6e61 6d65 223a 2246 6c61 7368 4c6f  ,"name":"FlashLo
-0001f510: 616e 222c 2274 7970 6522 3a22 6576 656e  an","type":"even
-0001f520: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
-0001f530: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
-0001f540: 5b7b 2269 6e64 6578 6564 223a 6661 6c73  [{"indexed":fals
-0001f550: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001f560: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001f570: 223a 2270 7265 7669 6f75 7353 697a 6522  ":"previousSize"
-0001f580: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
-0001f590: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
-0001f5a0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
-0001f5b0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001f5c0: 6d65 223a 226e 6577 5369 7a65 222c 2274  me":"newSize","t
-0001f5d0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-0001f5e0: 2c22 6e61 6d65 223a 224f 7261 636c 6553  ,"name":"OracleS
-0001f5f0: 697a 6549 6e63 7265 6173 6564 222c 2274  izeIncreased","t
-0001f600: 7970 6522 3a22 6576 656e 7422 7d2c 7b22  ype":"event"},{"
-0001f610: 616e 6f6e 796d 6f75 7322 3a66 616c 7365  anonymous":false
-0001f620: 2c22 696e 7075 7473 223a 5b7b 2269 6e64  ,"inputs":[{"ind
-0001f630: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
-0001f640: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0001f650: 7373 222c 226e 616d 6522 3a22 7365 6e64  ss","name":"send
-0001f660: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
-0001f670: 6573 7322 7d2c 7b22 696e 6465 7865 6422  ess"},{"indexed"
-0001f680: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
-0001f690: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0001f6a0: 6e61 6d65 223a 2272 6563 6970 6965 6e74  name":"recipient
-0001f6b0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0001f6c0: 7322 7d2c 7b22 696e 6465 7865 6422 3a66  s"},{"indexed":f
-0001f6d0: 616c 7365 2c22 696e 7465 726e 616c 5479  alse,"internalTy
-0001f6e0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001f6f0: 616d 6522 3a22 616d 6f75 6e74 5822 2c22  ame":"amountX","
-0001f700: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001f710: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-0001f720: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001f730: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001f740: 223a 2261 6d6f 756e 7459 222c 2274 7970  ":"amountY","typ
-0001f750: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001f760: 6e61 6d65 223a 2250 726f 746f 636f 6c46  name":"ProtocolF
-0001f770: 6565 7343 6f6c 6c65 6374 6564 222c 2274  eesCollected","t
-0001f780: 7970 6522 3a22 6576 656e 7422 7d2c 7b22  ype":"event"},{"
-0001f790: 616e 6f6e 796d 6f75 7322 3a66 616c 7365  anonymous":false
-0001f7a0: 2c22 696e 7075 7473 223a 5b7b 2269 6e64  ,"inputs":[{"ind
-0001f7b0: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
-0001f7c0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-0001f7d0: 7373 222c 226e 616d 6522 3a22 7365 6e64  ss","name":"send
-0001f7e0: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
-0001f7f0: 6573 7322 7d2c 7b22 696e 6465 7865 6422  ess"},{"indexed"
-0001f800: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
-0001f810: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-0001f820: 6e61 6d65 223a 2272 6563 6970 6965 6e74  name":"recipient
-0001f830: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-0001f840: 7322 7d2c 7b22 696e 6465 7865 6422 3a74  s"},{"indexed":t
-0001f850: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
-0001f860: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001f870: 6d65 223a 2269 6422 2c22 7479 7065 223a  me":"id","type":
-0001f880: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
-0001f890: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-0001f8a0: 6572 6e61 6c54 7970 6522 3a22 626f 6f6c  ernalType":"bool
-0001f8b0: 222c 226e 616d 6522 3a22 7377 6170 466f  ","name":"swapFo
-0001f8c0: 7259 222c 2274 7970 6522 3a22 626f 6f6c  rY","type":"bool
-0001f8d0: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
-0001f8e0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
-0001f8f0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-0001f900: 6d65 223a 2261 6d6f 756e 7449 6e22 2c22  me":"amountIn","
-0001f910: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001f920: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-0001f930: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001f940: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001f950: 223a 2261 6d6f 756e 744f 7574 222c 2274  ":"amountOut","t
-0001f960: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-0001f970: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
-0001f980: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001f990: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-0001f9a0: 3a22 766f 6c61 7469 6c69 7479 4163 6375  :"volatilityAccu
-0001f9b0: 6d75 6c61 7465 6422 2c22 7479 7065 223a  mulated","type":
-0001f9c0: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
-0001f9d0: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
-0001f9e0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-0001f9f0: 3235 3622 2c22 6e61 6d65 223a 2266 6565  256","name":"fee
-0001fa00: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
-0001fa10: 3536 227d 5d2c 226e 616d 6522 3a22 5377  56"}],"name":"Sw
-0001fa20: 6170 222c 2274 7970 6522 3a22 6576 656e  ap","type":"even
-0001fa30: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
-0001fa40: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
-0001fa50: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
-0001fa60: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
-0001fa70: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-0001fa80: 3a22 7365 6e64 6572 222c 2274 7970 6522  :"sender","type"
-0001fa90: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001faa0: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
-0001fab0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
-0001fac0: 6573 7322 2c22 6e61 6d65 223a 2266 726f  ess","name":"fro
-0001fad0: 6d22 2c22 7479 7065 223a 2261 6464 7265  m","type":"addre
-0001fae0: 7373 227d 2c7b 2269 6e64 6578 6564 223a  ss"},{"indexed":
-0001faf0: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
-0001fb00: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0001fb10: 616d 6522 3a22 746f 222c 2274 7970 6522  ame":"to","type"
-0001fb20: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-0001fb30: 6465 7865 6422 3a66 616c 7365 2c22 696e  dexed":false,"in
-0001fb40: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001fb50: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
-0001fb60: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
-0001fb70: 7432 3536 5b5d 227d 2c7b 2269 6e64 6578  t256[]"},{"index
-0001fb80: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
-0001fb90: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-0001fba0: 365b 5d22 2c22 6e61 6d65 223a 2261 6d6f  6[]","name":"amo
-0001fbb0: 756e 7473 222c 2274 7970 6522 3a22 7569  unts","type":"ui
-0001fbc0: 6e74 3235 365b 5d22 7d5d 2c22 6e61 6d65  nt256[]"}],"name
-0001fbd0: 223a 2254 7261 6e73 6665 7242 6174 6368  ":"TransferBatch
-0001fbe0: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
-0001fbf0: 7d2c 7b22 616e 6f6e 796d 6f75 7322 3a66  },{"anonymous":f
-0001fc00: 616c 7365 2c22 696e 7075 7473 223a 5b7b  alse,"inputs":[{
-0001fc10: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
-0001fc20: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-0001fc30: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-0001fc40: 7365 6e64 6572 222c 2274 7970 6522 3a22  sender","type":"
-0001fc50: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
-0001fc60: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
-0001fc70: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-0001fc80: 7322 2c22 6e61 6d65 223a 2266 726f 6d22  s","name":"from"
-0001fc90: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-0001fca0: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
-0001fcb0: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
-0001fcc0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
-0001fcd0: 6522 3a22 746f 222c 2274 7970 6522 3a22  e":"to","type":"
-0001fce0: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
-0001fcf0: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
-0001fd00: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-0001fd10: 3536 222c 226e 616d 6522 3a22 6964 222c  56","name":"id",
-0001fd20: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-0001fd30: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
-0001fd40: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
-0001fd50: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001fd60: 6522 3a22 616d 6f75 6e74 222c 2274 7970  e":"amount","typ
-0001fd70: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001fd80: 6e61 6d65 223a 2254 7261 6e73 6665 7253  name":"TransferS
-0001fd90: 696e 676c 6522 2c22 7479 7065 223a 2265  ingle","type":"e
-0001fda0: 7665 6e74 227d 2c7b 2261 6e6f 6e79 6d6f  vent"},{"anonymo
-0001fdb0: 7573 223a 6661 6c73 652c 2269 6e70 7574  us":false,"input
-0001fdc0: 7322 3a5b 7b22 696e 6465 7865 6422 3a74  s":[{"indexed":t
-0001fdd0: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
-0001fde0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
-0001fdf0: 6d65 223a 2273 656e 6465 7222 2c22 7479  me":"sender","ty
-0001fe00: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-0001fe10: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
-0001fe20: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-0001fe30: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-0001fe40: 7265 6369 7069 656e 7422 2c22 7479 7065  recipient","type
-0001fe50: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
-0001fe60: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
-0001fe70: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-0001fe80: 7432 3536 222c 226e 616d 6522 3a22 6964  t256","name":"id
-0001fe90: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-0001fea0: 3622 7d2c 7b22 696e 6465 7865 6422 3a66  6"},{"indexed":f
-0001feb0: 616c 7365 2c22 696e 7465 726e 616c 5479  alse,"internalTy
-0001fec0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-0001fed0: 616d 6522 3a22 616d 6f75 6e74 5822 2c22  ame":"amountX","
-0001fee0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-0001fef0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
-0001ff00: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
-0001ff10: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-0001ff20: 223a 2261 6d6f 756e 7459 222c 2274 7970  ":"amountY","typ
-0001ff30: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-0001ff40: 6e61 6d65 223a 2257 6974 6864 7261 776e  name":"Withdrawn
-0001ff50: 4672 6f6d 4269 6e22 2c22 7479 7065 223a  FromBin","type":
-0001ff60: 2265 7665 6e74 227d 2c7b 2269 6e70 7574  "event"},{"input
-0001ff70: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-0001ff80: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
-0001ff90: 616d 6522 3a22 5f61 6363 6f75 6e74 222c  ame":"_account",
-0001ffa0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
-0001ffb0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-0001ffc0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-0001ffd0: 6522 3a22 5f69 6422 2c22 7479 7065 223a  e":"_id","type":
-0001ffe0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
-0001fff0: 6522 3a22 6261 6c61 6e63 654f 6622 2c22  e":"balanceOf","
-00020000: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-00020010: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00020020: 3536 222c 226e 616d 6522 3a22 222c 2274  56","name":"","t
-00020030: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-00020040: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00020050: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
-00020060: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00020070: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
-00020080: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
-00020090: 5b5d 222c 226e 616d 6522 3a22 5f61 6363  []","name":"_acc
-000200a0: 6f75 6e74 7322 2c22 7479 7065 223a 2261  ounts","type":"a
-000200b0: 6464 7265 7373 5b5d 227d 2c7b 2269 6e74  ddress[]"},{"int
-000200c0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-000200d0: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
-000200e0: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
-000200f0: 7432 3536 5b5d 227d 5d2c 226e 616d 6522  t256[]"}],"name"
-00020100: 3a22 6261 6c61 6e63 654f 6642 6174 6368  :"balanceOfBatch
-00020110: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
-00020120: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00020130: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
-00020140: 2262 6174 6368 4261 6c61 6e63 6573 222c  "batchBalances",
-00020150: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
-00020160: 5d22 7d5d 2c22 7374 6174 654d 7574 6162  ]"}],"stateMutab
-00020170: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
-00020180: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00020190: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-000201a0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-000201b0: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
-000201c0: 5f69 6473 222c 2274 7970 6522 3a22 7569  _ids","type":"ui
-000201d0: 6e74 3235 365b 5d22 7d2c 7b22 696e 7465  nt256[]"},{"inte
-000201e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-000201f0: 3536 5b5d 222c 226e 616d 6522 3a22 5f61  56[]","name":"_a
-00020200: 6d6f 756e 7473 222c 2274 7970 6522 3a22  mounts","type":"
-00020210: 7569 6e74 3235 365b 5d22 7d2c 7b22 696e  uint256[]"},{"in
-00020220: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-00020230: 7265 7373 222c 226e 616d 6522 3a22 5f74  ress","name":"_t
-00020240: 6f22 2c22 7479 7065 223a 2261 6464 7265  o","type":"addre
-00020250: 7373 227d 5d2c 226e 616d 6522 3a22 6275  ss"}],"name":"bu
-00020260: 726e 222c 226f 7574 7075 7473 223a 5b7b  rn","outputs":[{
-00020270: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00020280: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00020290: 2261 6d6f 756e 7458 222c 2274 7970 6522  "amountX","type"
-000202a0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+00017340: 6d65 223a 224a 6f65 4c69 6272 6172 795f  me":"JoeLibrary_
+00017350: 5f41 6464 7265 7373 5a65 726f 222c 2274  _AddressZero","t
+00017360: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00017370: 696e 7075 7473 223a 5b5d 2c22 6e61 6d65  inputs":[],"name
+00017380: 223a 224a 6f65 4c69 6272 6172 795f 5f49  ":"JoeLibrary__I
+00017390: 6465 6e74 6963 616c 4164 6472 6573 7365  denticalAddresse
+000173a0: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
+000173b0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+000173c0: 226e 616d 6522 3a22 4a6f 654c 6962 7261  "name":"JoeLibra
+000173d0: 7279 5f5f 496e 7375 6666 6963 6965 6e74  ry__Insufficient
+000173e0: 416d 6f75 6e74 222c 2274 7970 6522 3a22  Amount","type":"
+000173f0: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00017400: 223a 5b5d 2c22 6e61 6d65 223a 224a 6f65  ":[],"name":"Joe
+00017410: 4c69 6272 6172 795f 5f49 6e73 7566 6669  Library__Insuffi
+00017420: 6369 656e 744c 6971 7569 6469 7479 222c  cientLiquidity",
+00017430: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00017440: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
+00017450: 6d65 223a 224c 4251 756f 7465 725f 496e  me":"LBQuoter_In
+00017460: 7661 6c69 644c 656e 6774 6822 2c22 7479  validLength","ty
+00017470: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+00017480: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00017490: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000174a0: 222c 226e 616d 6522 3a22 7822 2c22 7479  ","name":"x","ty
+000174b0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+000174c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000174d0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000174e0: 7922 2c22 7479 7065 223a 2269 6e74 3235  y","type":"int25
+000174f0: 3622 7d5d 2c22 6e61 6d65 223a 224d 6174  6"}],"name":"Mat
+00017500: 6831 3238 7831 3238 5f5f 506f 7765 7255  h128x128__PowerU
+00017510: 6e64 6572 666c 6f77 222c 2274 7970 6522  nderflow","type"
+00017520: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+00017530: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00017540: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00017550: 6e61 6d65 223a 2270 726f 6431 222c 2274  name":"prod1","t
+00017560: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00017570: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00017580: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00017590: 3a22 6465 6e6f 6d69 6e61 746f 7222 2c22  :"denominator","
+000175a0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+000175b0: 5d2c 226e 616d 6522 3a22 4d61 7468 3531  ],"name":"Math51
+000175c0: 3242 6974 735f 5f4d 756c 4469 764f 7665  2Bits__MulDivOve
+000175d0: 7266 6c6f 7722 2c22 7479 7065 223a 2265  rflow","type":"e
+000175e0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+000175f0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00017600: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00017610: 6522 3a22 7072 6f64 3122 2c22 7479 7065  e":"prod1","type
+00017620: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00017630: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00017640: 6e74 3235 3622 2c22 6e61 6d65 223a 226f  nt256","name":"o
+00017650: 6666 7365 7422 2c22 7479 7065 223a 2275  ffset","type":"u
+00017660: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+00017670: 3a22 4d61 7468 3531 3242 6974 735f 5f4d  :"Math512Bits__M
+00017680: 756c 5368 6966 744f 7665 7266 6c6f 7722  ulShiftOverflow"
+00017690: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+000176a0: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+000176b0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+000176c0: 7432 3536 222c 226e 616d 6522 3a22 6f66  t256","name":"of
+000176d0: 6673 6574 222c 2274 7970 6522 3a22 7569  fset","type":"ui
+000176e0: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+000176f0: 224d 6174 6835 3132 4269 7473 5f5f 4f66  "Math512Bits__Of
+00017700: 6673 6574 4f76 6572 666c 6f77 7322 2c22  fsetOverflows","
+00017710: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+00017720: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+00017730: 6522 3a22 6661 6374 6f72 7956 3122 2c22  e":"factoryV1","
+00017740: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+00017750: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+00017760: 7373 222c 226e 616d 6522 3a22 222c 2274  ss","name":"","t
+00017770: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+00017780: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+00017790: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+000177a0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+000177b0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+000177c0: 3a22 6661 6374 6f72 7956 3222 2c22 6f75  :"factoryV2","ou
+000177d0: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
+000177e0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+000177f0: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
+00017800: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+00017810: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00017820: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
+00017830: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00017840: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00017850: 5479 7065 223a 2261 6464 7265 7373 5b5d  Type":"address[]
+00017860: 222c 226e 616d 6522 3a22 5f72 6f75 7465  ","name":"_route
+00017870: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+00017880: 735b 5d22 7d2c 7b22 696e 7465 726e 616c  s[]"},{"internal
+00017890: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+000178a0: 226e 616d 6522 3a22 5f61 6d6f 756e 7449  "name":"_amountI
+000178b0: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
+000178c0: 3536 227d 5d2c 226e 616d 6522 3a22 6669  56"}],"name":"fi
+000178d0: 6e64 4265 7374 5061 7468 4672 6f6d 416d  ndBestPathFromAm
+000178e0: 6f75 6e74 496e 222c 226f 7574 7075 7473  ountIn","outputs
+000178f0: 223a 5b7b 2263 6f6d 706f 6e65 6e74 7322  ":[{"components"
+00017900: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00017910: 223a 2261 6464 7265 7373 5b5d 222c 226e  ":"address[]","n
+00017920: 616d 6522 3a22 726f 7574 6522 2c22 7479  ame":"route","ty
+00017930: 7065 223a 2261 6464 7265 7373 5b5d 227d  pe":"address[]"}
+00017940: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00017950: 3a22 6164 6472 6573 735b 5d22 2c22 6e61  :"address[]","na
+00017960: 6d65 223a 2270 6169 7273 222c 2274 7970  me":"pairs","typ
+00017970: 6522 3a22 6164 6472 6573 735b 5d22 7d2c  e":"address[]"},
+00017980: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00017990: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
+000179a0: 6522 3a22 6269 6e53 7465 7073 222c 2274  e":"binSteps","t
+000179b0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+000179c0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000179d0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+000179e0: 616d 6522 3a22 616d 6f75 6e74 7322 2c22  ame":"amounts","
+000179f0: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
+00017a00: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00017a10: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
+00017a20: 6e61 6d65 223a 2276 6972 7475 616c 416d  name":"virtualAm
+00017a30: 6f75 6e74 7357 6974 686f 7574 536c 6970  ountsWithoutSlip
+00017a40: 7061 6765 222c 2274 7970 6522 3a22 7569  page","type":"ui
+00017a50: 6e74 3235 365b 5d22 7d2c 7b22 696e 7465  nt256[]"},{"inte
+00017a60: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00017a70: 3536 5b5d 222c 226e 616d 6522 3a22 6665  56[]","name":"fe
+00017a80: 6573 222c 2274 7970 6522 3a22 7569 6e74  es","type":"uint
+00017a90: 3235 365b 5d22 7d5d 2c22 696e 7465 726e  256[]"}],"intern
+00017aa0: 616c 5479 7065 223a 2273 7472 7563 7420  alType":"struct 
+00017ab0: 4c42 5175 6f74 6572 2e51 756f 7465 222c  LBQuoter.Quote",
+00017ac0: 226e 616d 6522 3a22 7175 6f74 6522 2c22  "name":"quote","
+00017ad0: 7479 7065 223a 2274 7570 6c65 227d 5d2c  type":"tuple"}],
+00017ae0: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00017af0: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
+00017b00: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00017b10: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00017b20: 6c54 7970 6522 3a22 6164 6472 6573 735b  lType":"address[
+00017b30: 5d22 2c22 6e61 6d65 223a 225f 726f 7574  ]","name":"_rout
+00017b40: 6522 2c22 7479 7065 223a 2261 6464 7265  e","type":"addre
+00017b50: 7373 5b5d 227d 2c7b 2269 6e74 6572 6e61  ss[]"},{"interna
+00017b60: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00017b70: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
+00017b80: 4f75 7422 2c22 7479 7065 223a 2275 696e  Out","type":"uin
+00017b90: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+00017ba0: 6669 6e64 4265 7374 5061 7468 4672 6f6d  findBestPathFrom
+00017bb0: 416d 6f75 6e74 4f75 7422 2c22 6f75 7470  AmountOut","outp
+00017bc0: 7574 7322 3a5b 7b22 636f 6d70 6f6e 656e  uts":[{"componen
+00017bd0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00017be0: 7970 6522 3a22 6164 6472 6573 735b 5d22  ype":"address[]"
+00017bf0: 2c22 6e61 6d65 223a 2272 6f75 7465 222c  ,"name":"route",
+00017c00: 2274 7970 6522 3a22 6164 6472 6573 735b  "type":"address[
+00017c10: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
+00017c20: 7065 223a 2261 6464 7265 7373 5b5d 222c  pe":"address[]",
+00017c30: 226e 616d 6522 3a22 7061 6972 7322 2c22  "name":"pairs","
+00017c40: 7479 7065 223a 2261 6464 7265 7373 5b5d  type":"address[]
+00017c50: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00017c60: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
+00017c70: 6e61 6d65 223a 2262 696e 5374 6570 7322  name":"binSteps"
+00017c80: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00017c90: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
+00017ca0: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+00017cb0: 2c22 6e61 6d65 223a 2261 6d6f 756e 7473  ,"name":"amounts
+00017cc0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00017cd0: 365b 5d22 7d2c 7b22 696e 7465 726e 616c  6[]"},{"internal
+00017ce0: 5479 7065 223a 2275 696e 7432 3536 5b5d  Type":"uint256[]
+00017cf0: 222c 226e 616d 6522 3a22 7669 7274 7561  ","name":"virtua
+00017d00: 6c41 6d6f 756e 7473 5769 7468 6f75 7453  lAmountsWithoutS
+00017d10: 6c69 7070 6167 6522 2c22 7479 7065 223a  lippage","type":
+00017d20: 2275 696e 7432 3536 5b5d 227d 2c7b 2269  "uint256[]"},{"i
+00017d30: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00017d40: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
+00017d50: 2266 6565 7322 2c22 7479 7065 223a 2275  "fees","type":"u
+00017d60: 696e 7432 3536 5b5d 227d 5d2c 2269 6e74  int256[]"}],"int
+00017d70: 6572 6e61 6c54 7970 6522 3a22 7374 7275  ernalType":"stru
+00017d80: 6374 204c 4251 756f 7465 722e 5175 6f74  ct LBQuoter.Quot
+00017d90: 6522 2c22 6e61 6d65 223a 2271 756f 7465  e","name":"quote
+00017da0: 222c 2274 7970 6522 3a22 7475 706c 6522  ","type":"tuple"
+00017db0: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
+00017dc0: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
+00017dd0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00017de0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+00017df0: 6522 3a22 726f 7574 6572 5632 222c 226f  e":"routerV2","o
+00017e00: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+00017e10: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+00017e20: 7322 2c22 6e61 6d65 223a 2222 2c22 7479  s","name":"","ty
+00017e30: 7065 223a 2261 6464 7265 7373 227d 5d2c  pe":"address"}],
+00017e40: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00017e50: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
+00017e60: 2266 756e 6374 696f 6e22 7d5d 270a 0a20  "function"}]'.. 
+00017e70: 2020 2023 7265 7475 726e 2071 756f 7465     #return quote
+00017e80: 0a20 2020 2023 2020 2020 7374 7275 6374  .    #    struct
+00017e90: 2051 756f 7465 207b 0a20 2020 2023 2020   Quote {.    #  
+00017ea0: 2020 2061 6464 7265 7373 5b5d 2072 6f75     address[] rou
+00017eb0: 7465 3b20 696e 2074 6f6b 656e 20e5 9ca8  te; in token ...
+00017ec0: e589 8d0a 2020 2020 2320 2020 2020 6164  ....    #     ad
+00017ed0: 6472 6573 735b 5d20 7061 6972 733b 0a20  dress[] pairs;. 
+00017ee0: 2020 2023 2020 2020 2075 696e 7432 3536     #     uint256
+00017ef0: 5b5d 2062 696e 5374 6570 733b 0a20 2020  [] binSteps;.   
+00017f00: 2023 2020 2020 2075 696e 7432 3536 5b5d   #     uint256[]
+00017f10: 2061 6d6f 756e 7473 3b20 e695 b0e7 bb84   amounts; ......
+00017f20: 2ce9 a1ba e5ba 8fe4 b88e e8b7 afe5 be84  ,...............
+00017f30: e4b8 80e8 87b4 0a20 2020 2023 2020 2020  .......    #    
+00017f40: 2075 696e 7432 3536 5b5d 2076 6972 7475   uint256[] virtu
+00017f50: 616c 416d 6f75 6e74 7357 6974 686f 7574  alAmountsWithout
+00017f60: 536c 6970 7061 6765 3b0a 2020 2020 2320  Slippage;.    # 
+00017f70: 2020 2020 7569 6e74 3235 365b 5d20 6665      uint256[] fe
+00017f80: 6573 3b0a 2020 2020 2320 7d0a 2020 2020  es;.    # }.    
+00017f90: 6465 6620 6669 6e64 5f62 6573 745f 7061  def find_best_pa
+00017fa0: 7468 5f66 6f72 5f61 6d6f 756e 745f 696e  th_for_amount_in
+00017fb0: 285f 7765 6233 3a57 6562 332c 5f71 756f  (_web3:Web3,_quo
+00017fc0: 7465 5f61 6464 7265 7373 2c5f 7175 6f74  te_address,_quot
+00017fd0: 655f 6162 692c 5f70 6174 682c 5f61 6d6f  e_abi,_path,_amo
+00017fe0: 756e 745f 696e 293a 0a20 2020 2020 2020  unt_in):.       
+00017ff0: 2072 6574 7572 6e20 5f77 6562 332e 6574   return _web3.et
+00018000: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
+00018010: 7373 3d5f 7175 6f74 655f 6164 6472 6573  ss=_quote_addres
+00018020: 732c 6162 693d 5f71 756f 7465 5f61 6269  s,abi=_quote_abi
+00018030: 292e 6675 6e63 7469 6f6e 732e 6669 6e64  ).functions.find
+00018040: 4265 7374 5061 7468 4672 6f6d 416d 6f75  BestPathFromAmou
+00018050: 6e74 496e 285f 7061 7468 2c5f 616d 6f75  ntIn(_path,_amou
+00018060: 6e74 5f69 6e29 2e63 616c 6c28 290a 2020  nt_in).call().  
+00018070: 2020 2372 6574 7572 6e20 7175 6f74 650a    #return quote.
+00018080: 2020 2020 2320 2020 2073 7472 7563 7420      #    struct 
+00018090: 5175 6f74 6520 7b0a 2020 2020 2320 2020  Quote {.    #   
+000180a0: 2020 6164 6472 6573 735b 5d20 726f 7574    address[] rout
+000180b0: 653b 206f 7574 2074 6f6b 656e e59c a8e5  e; out token....
+000180c0: 898d 0a20 2020 2023 2020 2020 2061 6464  ...    #     add
+000180d0: 7265 7373 5b5d 2070 6169 7273 3b0a 2020  ress[] pairs;.  
+000180e0: 2020 2320 2020 2020 7569 6e74 3235 365b    #     uint256[
+000180f0: 5d20 6269 6e53 7465 7073 3b0a 2020 2020  ] binSteps;.    
+00018100: 2320 2020 2020 7569 6e74 3235 365b 5d20  #     uint256[] 
+00018110: 616d 6f75 6e74 733b 0a20 2020 2023 2020  amounts;.    #  
+00018120: 2020 2075 696e 7432 3536 5b5d 2076 6972     uint256[] vir
+00018130: 7475 616c 416d 6f75 6e74 7357 6974 686f  tualAmountsWitho
+00018140: 7574 536c 6970 7061 6765 3b0a 2020 2020  utSlippage;.    
+00018150: 2320 2020 2020 7569 6e74 3235 365b 5d20  #     uint256[] 
+00018160: 6665 6573 3b0a 2020 2020 2320 7d0a 2020  fees;.    # }.  
+00018170: 2020 6465 6620 6669 6e64 5f62 6573 745f    def find_best_
+00018180: 7061 7468 5f66 6f72 5f61 6d6f 756e 745f  path_for_amount_
+00018190: 6f75 7428 5f77 6562 333a 5765 6233 2c5f  out(_web3:Web3,_
+000181a0: 7175 6f74 655f 6164 6472 6573 732c 5f71  quote_address,_q
+000181b0: 756f 7465 5f61 6269 2c5f 7061 7468 2c5f  uote_abi,_path,_
+000181c0: 616d 6f75 6e74 5f6f 7574 293a 0a20 2020  amount_out):.   
+000181d0: 2020 2020 2072 6574 7572 6e20 5f77 6562       return _web
+000181e0: 332e 6574 682e 636f 6e74 7261 6374 2861  3.eth.contract(a
+000181f0: 6464 7265 7373 3d5f 7175 6f74 655f 6164  ddress=_quote_ad
+00018200: 6472 6573 732c 6162 693d 5f71 756f 7465  dress,abi=_quote
+00018210: 5f61 6269 292e 6675 6e63 7469 6f6e 732e  _abi).functions.
+00018220: 6669 6e64 4265 7374 5061 7468 4672 6f6d  findBestPathFrom
+00018230: 416d 6f75 6e74 496e 285f 7061 7468 2c5f  AmountIn(_path,_
+00018240: 616d 6f75 6e74 5f6f 7574 292e 6361 6c6c  amount_out).call
+00018250: 2829 0a0a 0a63 6c61 7373 204a 6f65 5632  ()...class JoeV2
+00018260: 4572 6332 303a 0a20 2020 206a 6f65 5f65  Erc20:.    joe_e
+00018270: 7263 3230 5f61 6269 3d27 5b20 7b20 2261  rc20_abi='[ { "a
+00018280: 6e6f 6e79 6d6f 7573 223a 2066 616c 7365  nonymous": false
+00018290: 2c20 2269 6e70 7574 7322 3a20 5b20 7b20  , "inputs": [ { 
+000182a0: 2269 6e64 6578 6564 223a 2074 7275 652c  "indexed": true,
+000182b0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+000182c0: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
+000182d0: 6522 3a20 226f 776e 6572 222c 2022 7479  e": "owner", "ty
+000182e0: 7065 223a 2022 6164 6472 6573 7322 207d  pe": "address" }
+000182f0: 2c20 7b20 2269 6e64 6578 6564 223a 2074  , { "indexed": t
+00018300: 7275 652c 2022 696e 7465 726e 616c 5479  rue, "internalTy
+00018310: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
+00018320: 226e 616d 6522 3a20 2273 7065 6e64 6572  "name": "spender
+00018330: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
+00018340: 6573 7322 207d 2c20 7b20 2269 6e64 6578  ess" }, { "index
+00018350: 6564 223a 2066 616c 7365 2c20 2269 6e74  ed": false, "int
+00018360: 6572 6e61 6c54 7970 6522 3a20 2275 696e  ernalType": "uin
+00018370: 7432 3536 222c 2022 6e61 6d65 223a 2022  t256", "name": "
+00018380: 7661 6c75 6522 2c20 2274 7970 6522 3a20  value", "type": 
+00018390: 2275 696e 7432 3536 2220 7d20 5d2c 2022  "uint256" } ], "
+000183a0: 6e61 6d65 223a 2022 4170 7072 6f76 616c  name": "Approval
+000183b0: 222c 2022 7479 7065 223a 2022 6576 656e  ", "type": "even
+000183c0: 7422 207d 2c20 7b20 2261 6e6f 6e79 6d6f  t" }, { "anonymo
+000183d0: 7573 223a 2066 616c 7365 2c20 2269 6e70  us": false, "inp
+000183e0: 7574 7322 3a20 5b20 7b20 2269 6e64 6578  uts": [ { "index
+000183f0: 6564 223a 2074 7275 652c 2022 696e 7465  ed": true, "inte
+00018400: 726e 616c 5479 7065 223a 2022 6164 6472  rnalType": "addr
+00018410: 6573 7322 2c20 226e 616d 6522 3a20 2266  ess", "name": "f
+00018420: 726f 6d22 2c20 2274 7970 6522 3a20 2261  rom", "type": "a
+00018430: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+00018440: 6465 7865 6422 3a20 7472 7565 2c20 2269  dexed": true, "i
+00018450: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+00018460: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+00018470: 2022 746f 222c 2022 7479 7065 223a 2022   "to", "type": "
+00018480: 6164 6472 6573 7322 207d 2c20 7b20 2269  address" }, { "i
+00018490: 6e64 6578 6564 223a 2066 616c 7365 2c20  ndexed": false, 
+000184a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a20  "internalType": 
+000184b0: 2275 696e 7432 3536 222c 2022 6e61 6d65  "uint256", "name
+000184c0: 223a 2022 7661 6c75 6522 2c20 2274 7970  ": "value", "typ
+000184d0: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
+000184e0: 5d2c 2022 6e61 6d65 223a 2022 5472 616e  ], "name": "Tran
+000184f0: 7366 6572 222c 2022 7479 7065 223a 2022  sfer", "type": "
+00018500: 6576 656e 7422 207d 2c20 7b20 2269 6e70  event" }, { "inp
+00018510: 7574 7322 3a20 5b20 7b20 2269 6e74 6572  uts": [ { "inter
+00018520: 6e61 6c54 7970 6522 3a20 2261 6464 7265  nalType": "addre
+00018530: 7373 222c 2022 6e61 6d65 223a 2022 6f77  ss", "name": "ow
+00018540: 6e65 7222 2c20 2274 7970 6522 3a20 2261  ner", "type": "a
+00018550: 6464 7265 7373 2220 7d2c 207b 2022 696e  ddress" }, { "in
+00018560: 7465 726e 616c 5479 7065 223a 2022 6164  ternalType": "ad
+00018570: 6472 6573 7322 2c20 226e 616d 6522 3a20  dress", "name": 
+00018580: 2273 7065 6e64 6572 222c 2022 7479 7065  "spender", "type
+00018590: 223a 2022 6164 6472 6573 7322 207d 205d  ": "address" } ]
+000185a0: 2c20 226e 616d 6522 3a20 2261 6c6c 6f77  , "name": "allow
+000185b0: 616e 6365 222c 2022 6f75 7470 7574 7322  ance", "outputs"
+000185c0: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
+000185d0: 7970 6522 3a20 2275 696e 7432 3536 222c  ype": "uint256",
+000185e0: 2022 6e61 6d65 223a 2022 222c 2022 7479   "name": "", "ty
+000185f0: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
+00018600: 205d 2c20 2273 7461 7465 4d75 7461 6269   ], "stateMutabi
+00018610: 6c69 7479 223a 2022 7669 6577 222c 2022  lity": "view", "
+00018620: 7479 7065 223a 2022 6675 6e63 7469 6f6e  type": "function
+00018630: 2220 7d2c 207b 2022 696e 7075 7473 223a  " }, { "inputs":
+00018640: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+00018650: 7065 223a 2022 6164 6472 6573 7322 2c20  pe": "address", 
+00018660: 226e 616d 6522 3a20 2273 7065 6e64 6572  "name": "spender
+00018670: 222c 2022 7479 7065 223a 2022 6164 6472  ", "type": "addr
+00018680: 6573 7322 207d 2c20 7b20 2269 6e74 6572  ess" }, { "inter
+00018690: 6e61 6c54 7970 6522 3a20 2275 696e 7432  nalType": "uint2
+000186a0: 3536 222c 2022 6e61 6d65 223a 2022 7661  56", "name": "va
+000186b0: 6c75 6522 2c20 2274 7970 6522 3a20 2275  lue", "type": "u
+000186c0: 696e 7432 3536 2220 7d20 5d2c 2022 6e61  int256" } ], "na
+000186d0: 6d65 223a 2022 6170 7072 6f76 6522 2c20  me": "approve", 
+000186e0: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+000186f0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+00018700: 626f 6f6c 222c 2022 6e61 6d65 223a 2022  bool", "name": "
+00018710: 222c 2022 7479 7065 223a 2022 626f 6f6c  ", "type": "bool
+00018720: 2220 7d20 5d2c 2022 7374 6174 654d 7574  " } ], "stateMut
+00018730: 6162 696c 6974 7922 3a20 226e 6f6e 7061  ability": "nonpa
+00018740: 7961 626c 6522 2c20 2274 7970 6522 3a20  yable", "type": 
+00018750: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
+00018760: 2269 6e70 7574 7322 3a20 5b20 7b20 2269  "inputs": [ { "i
+00018770: 6e74 6572 6e61 6c54 7970 6522 3a20 2261  nternalType": "a
+00018780: 6464 7265 7373 222c 2022 6e61 6d65 223a  ddress", "name":
+00018790: 2022 6f77 6e65 7222 2c20 2274 7970 6522   "owner", "type"
+000187a0: 3a20 2261 6464 7265 7373 2220 7d20 5d2c  : "address" } ],
+000187b0: 2022 6e61 6d65 223a 2022 6261 6c61 6e63   "name": "balanc
+000187c0: 654f 6622 2c20 226f 7574 7075 7473 223a  eOf", "outputs":
+000187d0: 205b 207b 2022 696e 7465 726e 616c 5479   [ { "internalTy
+000187e0: 7065 223a 2022 7569 6e74 3235 3622 2c20  pe": "uint256", 
+000187f0: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
+00018800: 6522 3a20 2275 696e 7432 3536 2220 7d20  e": "uint256" } 
+00018810: 5d2c 2022 7374 6174 654d 7574 6162 696c  ], "stateMutabil
+00018820: 6974 7922 3a20 2276 6965 7722 2c20 2274  ity": "view", "t
+00018830: 7970 6522 3a20 2266 756e 6374 696f 6e22  ype": "function"
+00018840: 207d 2c20 7b20 2269 6e70 7574 7322 3a20   }, { "inputs": 
+00018850: 5b5d 2c20 226e 616d 6522 3a20 2264 6563  [], "name": "dec
+00018860: 696d 616c 7322 2c20 226f 7574 7075 7473  imals", "outputs
+00018870: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+00018880: 5479 7065 223a 2022 7569 6e74 3822 2c20  Type": "uint8", 
+00018890: 226e 616d 6522 3a20 2222 2c20 2274 7970  "name": "", "typ
+000188a0: 6522 3a20 2275 696e 7438 2220 7d20 5d2c  e": "uint8" } ],
+000188b0: 2022 7374 6174 654d 7574 6162 696c 6974   "stateMutabilit
+000188c0: 7922 3a20 2276 6965 7722 2c20 2274 7970  y": "view", "typ
+000188d0: 6522 3a20 2266 756e 6374 696f 6e22 207d  e": "function" }
+000188e0: 2c20 7b20 2269 6e70 7574 7322 3a20 5b5d  , { "inputs": []
+000188f0: 2c20 226e 616d 6522 3a20 226e 616d 6522  , "name": "name"
+00018900: 2c20 226f 7574 7075 7473 223a 205b 207b  , "outputs": [ {
+00018910: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+00018920: 2022 7374 7269 6e67 222c 2022 6e61 6d65   "string", "name
+00018930: 223a 2022 222c 2022 7479 7065 223a 2022  ": "", "type": "
+00018940: 7374 7269 6e67 2220 7d20 5d2c 2022 7374  string" } ], "st
+00018950: 6174 654d 7574 6162 696c 6974 7922 3a20  ateMutability": 
+00018960: 2276 6965 7722 2c20 2274 7970 6522 3a20  "view", "type": 
+00018970: 2266 756e 6374 696f 6e22 207d 2c20 7b20  "function" }, { 
+00018980: 2269 6e70 7574 7322 3a20 5b5d 2c20 226e  "inputs": [], "n
+00018990: 616d 6522 3a20 2273 796d 626f 6c22 2c20  ame": "symbol", 
+000189a0: 226f 7574 7075 7473 223a 205b 207b 2022  "outputs": [ { "
+000189b0: 696e 7465 726e 616c 5479 7065 223a 2022  internalType": "
+000189c0: 7374 7269 6e67 222c 2022 6e61 6d65 223a  string", "name":
+000189d0: 2022 222c 2022 7479 7065 223a 2022 7374   "", "type": "st
+000189e0: 7269 6e67 2220 7d20 5d2c 2022 7374 6174  ring" } ], "stat
+000189f0: 654d 7574 6162 696c 6974 7922 3a20 2276  eMutability": "v
+00018a00: 6965 7722 2c20 2274 7970 6522 3a20 2266  iew", "type": "f
+00018a10: 756e 6374 696f 6e22 207d 2c20 7b20 2269  unction" }, { "i
+00018a20: 6e70 7574 7322 3a20 5b5d 2c20 226e 616d  nputs": [], "nam
+00018a30: 6522 3a20 2274 6f74 616c 5375 7070 6c79  e": "totalSupply
+00018a40: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
+00018a50: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+00018a60: 3a20 2275 696e 7432 3536 222c 2022 6e61  : "uint256", "na
+00018a70: 6d65 223a 2022 222c 2022 7479 7065 223a  me": "", "type":
+00018a80: 2022 7569 6e74 3235 3622 207d 205d 2c20   "uint256" } ], 
+00018a90: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00018aa0: 223a 2022 7669 6577 222c 2022 7479 7065  ": "view", "type
+00018ab0: 223a 2022 6675 6e63 7469 6f6e 2220 7d2c  ": "function" },
+00018ac0: 207b 2022 696e 7075 7473 223a 205b 207b   { "inputs": [ {
+00018ad0: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+00018ae0: 2022 6164 6472 6573 7322 2c20 226e 616d   "address", "nam
+00018af0: 6522 3a20 2274 6f22 2c20 2274 7970 6522  e": "to", "type"
+00018b00: 3a20 2261 6464 7265 7373 2220 7d2c 207b  : "address" }, {
+00018b10: 2022 696e 7465 726e 616c 5479 7065 223a   "internalType":
+00018b20: 2022 7569 6e74 3235 3622 2c20 226e 616d   "uint256", "nam
+00018b30: 6522 3a20 2276 616c 7565 222c 2022 7479  e": "value", "ty
+00018b40: 7065 223a 2022 7569 6e74 3235 3622 207d  pe": "uint256" }
+00018b50: 205d 2c20 226e 616d 6522 3a20 2274 7261   ], "name": "tra
+00018b60: 6e73 6665 7222 2c20 226f 7574 7075 7473  nsfer", "outputs
+00018b70: 223a 205b 207b 2022 696e 7465 726e 616c  ": [ { "internal
+00018b80: 5479 7065 223a 2022 626f 6f6c 222c 2022  Type": "bool", "
+00018b90: 6e61 6d65 223a 2022 222c 2022 7479 7065  name": "", "type
+00018ba0: 223a 2022 626f 6f6c 2220 7d20 5d2c 2022  ": "bool" } ], "
+00018bb0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00018bc0: 3a20 226e 6f6e 7061 7961 626c 6522 2c20  : "nonpayable", 
+00018bd0: 2274 7970 6522 3a20 2266 756e 6374 696f  "type": "functio
+00018be0: 6e22 207d 2c20 7b20 2269 6e70 7574 7322  n" }, { "inputs"
+00018bf0: 3a20 5b20 7b20 2269 6e74 6572 6e61 6c54  : [ { "internalT
+00018c00: 7970 6522 3a20 2261 6464 7265 7373 222c  ype": "address",
+00018c10: 2022 6e61 6d65 223a 2022 6672 6f6d 222c   "name": "from",
+00018c20: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+00018c30: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
+00018c40: 6c54 7970 6522 3a20 2261 6464 7265 7373  lType": "address
+00018c50: 222c 2022 6e61 6d65 223a 2022 746f 222c  ", "name": "to",
+00018c60: 2022 7479 7065 223a 2022 6164 6472 6573   "type": "addres
+00018c70: 7322 207d 2c20 7b20 2269 6e74 6572 6e61  s" }, { "interna
+00018c80: 6c54 7970 6522 3a20 2275 696e 7432 3536  lType": "uint256
+00018c90: 222c 2022 6e61 6d65 223a 2022 7661 6c75  ", "name": "valu
+00018ca0: 6522 2c20 2274 7970 6522 3a20 2275 696e  e", "type": "uin
+00018cb0: 7432 3536 2220 7d20 5d2c 2022 6e61 6d65  t256" } ], "name
+00018cc0: 223a 2022 7472 616e 7366 6572 4672 6f6d  ": "transferFrom
+00018cd0: 222c 2022 6f75 7470 7574 7322 3a20 5b20  ", "outputs": [ 
+00018ce0: 7b20 2269 6e74 6572 6e61 6c54 7970 6522  { "internalType"
+00018cf0: 3a20 2262 6f6f 6c22 2c20 226e 616d 6522  : "bool", "name"
+00018d00: 3a20 2222 2c20 2274 7970 6522 3a20 2262  : "", "type": "b
+00018d10: 6f6f 6c22 207d 205d 2c20 2273 7461 7465  ool" } ], "state
+00018d20: 4d75 7461 6269 6c69 7479 223a 2022 6e6f  Mutability": "no
+00018d30: 6e70 6179 6162 6c65 222c 2022 7479 7065  npayable", "type
+00018d40: 223a 2022 6675 6e63 7469 6f6e 2220 7d20  ": "function" } 
+00018d50: 5d27 2020 0a0a 636c 6173 7320 4a6f 6556  ]'  ..class JoeV
+00018d60: 3252 6f75 7465 3a0a 2020 2020 6a6f 655f  2Route:.    joe_
+00018d70: 726f 7574 655f 7632 5f61 6269 3d6a 736f  route_v2_abi=jso
+00018d80: 6e2e 6c6f 6164 7328 275b 7b22 696e 7075  n.loads('[{"inpu
+00018d90: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00018da0: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+00018db0: 4c42 4661 6374 6f72 7922 2c22 6e61 6d65  LBFactory","name
+00018dc0: 223a 225f 6661 6374 6f72 7922 2c22 7479  ":"_factory","ty
+00018dd0: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+00018de0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00018df0: 636f 6e74 7261 6374 2049 4a6f 6546 6163  contract IJoeFac
+00018e00: 746f 7279 222c 226e 616d 6522 3a22 5f6f  tory","name":"_o
+00018e10: 6c64 4661 6374 6f72 7922 2c22 7479 7065  ldFactory","type
+00018e20: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+00018e30: 6e74 6572 6e61 6c54 7970 6522 3a22 636f  nternalType":"co
+00018e40: 6e74 7261 6374 2049 5741 5641 5822 2c22  ntract IWAVAX","
+00018e50: 6e61 6d65 223a 225f 7761 7661 7822 2c22  name":"_wavax","
+00018e60: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+00018e70: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+00018e80: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
+00018e90: 2c22 7479 7065 223a 2263 6f6e 7374 7275  ,"type":"constru
+00018ea0: 6374 6f72 227d 2c7b 2269 6e70 7574 7322  ctor"},{"inputs"
+00018eb0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00018ec0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00018ed0: 6522 3a22 6270 222c 2274 7970 6522 3a22  e":"bp","type":"
+00018ee0: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+00018ef0: 223a 2242 696e 4865 6c70 6572 5f5f 4269  ":"BinHelper__Bi
+00018f00: 6e53 7465 704f 7665 7266 6c6f 7773 222c  nStepOverflows",
+00018f10: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+00018f20: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
+00018f30: 6d65 223a 2242 696e 4865 6c70 6572 5f5f  me":"BinHelper__
+00018f40: 4964 4f76 6572 666c 6f77 7322 2c22 7479  IdOverflows","ty
+00018f50: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+00018f60: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+00018f70: 3a22 4a6f 654c 6962 7261 7279 5f5f 496e  :"JoeLibrary__In
+00018f80: 7375 6666 6963 6965 6e74 416d 6f75 6e74  sufficientAmount
+00018f90: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+00018fa0: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+00018fb0: 6e61 6d65 223a 224a 6f65 4c69 6272 6172  name":"JoeLibrar
+00018fc0: 795f 5f49 6e73 7566 6669 6369 656e 744c  y__InsufficientL
+00018fd0: 6971 7569 6469 7479 222c 2274 7970 6522  iquidity","type"
+00018fe0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+00018ff0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00019000: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00019010: 6e61 6d65 223a 2261 6d6f 756e 7458 4d69  name":"amountXMi
+00019020: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
+00019030: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+00019040: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00019050: 6e61 6d65 223a 2261 6d6f 756e 7458 222c  name":"amountX",
+00019060: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00019070: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00019080: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00019090: 6522 3a22 616d 6f75 6e74 594d 696e 222c  e":"amountYMin",
+000190a0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+000190b0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000190c0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+000190d0: 6522 3a22 616d 6f75 6e74 5922 2c22 7479  e":"amountY","ty
+000190e0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+000190f0: 226e 616d 6522 3a22 4c42 526f 7574 6572  "name":"LBRouter
+00019100: 5f5f 416d 6f75 6e74 536c 6970 7061 6765  __AmountSlippage
+00019110: 4361 7567 6874 222c 2274 7970 6522 3a22  Caught","type":"
+00019120: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00019130: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00019140: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00019150: 6d65 223a 2269 6422 2c22 7479 7065 223a  me":"id","type":
+00019160: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+00019170: 6522 3a22 4c42 526f 7574 6572 5f5f 4269  e":"LBRouter__Bi
+00019180: 6e52 6573 6572 7665 4f76 6572 666c 6f77  nReserveOverflow
+00019190: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
+000191a0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+000191b0: 226e 616d 6522 3a22 4c42 526f 7574 6572  "name":"LBRouter
+000191c0: 5f5f 4272 6f6b 656e 5377 6170 5361 6665  __BrokenSwapSafe
+000191d0: 7479 4368 6563 6b22 2c22 7479 7065 223a  tyCheck","type":
+000191e0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+000191f0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00019200: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00019210: 616d 6522 3a22 6465 6164 6c69 6e65 222c  ame":"deadline",
+00019220: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00019230: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00019240: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00019250: 6522 3a22 6375 7272 656e 7454 696d 6573  e":"currentTimes
+00019260: 7461 6d70 222c 2274 7970 6522 3a22 7569  tamp","type":"ui
+00019270: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+00019280: 224c 4252 6f75 7465 725f 5f44 6561 646c  "LBRouter__Deadl
+00019290: 696e 6545 7863 6565 6465 6422 2c22 7479  ineExceeded","ty
+000192a0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+000192b0: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+000192c0: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+000192d0: 222c 226e 616d 6522 3a22 7265 6369 7069  ","name":"recipi
+000192e0: 656e 7422 2c22 7479 7065 223a 2261 6464  ent","type":"add
+000192f0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+00019300: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00019310: 2c22 6e61 6d65 223a 2261 6d6f 756e 7422  ,"name":"amount"
+00019320: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+00019330: 227d 5d2c 226e 616d 6522 3a22 4c42 526f  "}],"name":"LBRo
+00019340: 7574 6572 5f5f 4661 696c 6564 546f 5365  uter__FailedToSe
+00019350: 6e64 4156 4158 222c 2274 7970 6522 3a22  ndAVAX","type":"
+00019360: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00019370: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00019380: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00019390: 6d65 223a 2269 6444 6573 6972 6564 222c  me":"idDesired",
+000193a0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+000193b0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000193c0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+000193d0: 6522 3a22 6964 536c 6970 7061 6765 222c  e":"idSlippage",
+000193e0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+000193f0: 7d5d 2c22 6e61 6d65 223a 224c 4252 6f75  }],"name":"LBRou
+00019400: 7465 725f 5f49 6444 6573 6972 6564 4f76  ter__IdDesiredOv
+00019410: 6572 666c 6f77 7322 2c22 7479 7065 223a  erflows","type":
+00019420: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00019430: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00019440: 7065 223a 2269 6e74 3235 3622 2c22 6e61  pe":"int256","na
+00019450: 6d65 223a 2269 6422 2c22 7479 7065 223a  me":"id","type":
+00019460: 2269 6e74 3235 3622 7d5d 2c22 6e61 6d65  "int256"}],"name
+00019470: 223a 224c 4252 6f75 7465 725f 5f49 644f  ":"LBRouter__IdO
+00019480: 7665 7266 6c6f 7773 222c 2274 7970 6522  verflows","type"
+00019490: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+000194a0: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+000194b0: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+000194c0: 6e61 6d65 223a 2261 6374 6976 6549 6444  name":"activeIdD
+000194d0: 6573 6972 6564 222c 2274 7970 6522 3a22  esired","type":"
+000194e0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+000194f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00019500: 3536 222c 226e 616d 6522 3a22 6964 536c  56","name":"idSl
+00019510: 6970 7061 6765 222c 2274 7970 6522 3a22  ippage","type":"
+00019520: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+00019530: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00019540: 3536 222c 226e 616d 6522 3a22 6163 7469  56","name":"acti
+00019550: 7665 4964 222c 2274 7970 6522 3a22 7569  veId","type":"ui
+00019560: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+00019570: 224c 4252 6f75 7465 725f 5f49 6453 6c69  "LBRouter__IdSli
+00019580: 7070 6167 6543 6175 6768 7422 2c22 7479  ppageCaught","ty
+00019590: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+000195a0: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+000195b0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000195c0: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
+000195d0: 4f75 744d 696e 222c 2274 7970 6522 3a22  OutMin","type":"
+000195e0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+000195f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00019600: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+00019610: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
+00019620: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+00019630: 3a22 4c42 526f 7574 6572 5f5f 496e 7375  :"LBRouter__Insu
+00019640: 6666 6963 6965 6e74 416d 6f75 6e74 4f75  fficientAmountOu
+00019650: 7422 2c22 7479 7065 223a 2265 7272 6f72  t","type":"error
+00019660: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00019670: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+00019680: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+00019690: 7772 6f6e 6754 6f6b 656e 222c 2274 7970  wrongToken","typ
+000196a0: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+000196b0: 6e61 6d65 223a 224c 4252 6f75 7465 725f  name":"LBRouter_
+000196c0: 5f49 6e76 616c 6964 546f 6b65 6e50 6174  _InvalidTokenPat
+000196d0: 6822 2c22 7479 7065 223a 2265 7272 6f72  h","type":"error
+000196e0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+000196f0: 226e 616d 6522 3a22 4c42 526f 7574 6572  "name":"LBRouter
+00019700: 5f5f 4c65 6e67 7468 734d 6973 6d61 7463  __LengthsMismatc
+00019710: 6822 2c22 7479 7065 223a 2265 7272 6f72  h","type":"error
+00019720: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00019730: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00019740: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00019750: 616d 6f75 6e74 496e 4d61 7822 2c22 7479  amountInMax","ty
+00019760: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+00019770: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00019780: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00019790: 2261 6d6f 756e 7449 6e22 2c22 7479 7065  "amountIn","type
+000197a0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+000197b0: 616d 6522 3a22 4c42 526f 7574 6572 5f5f  ame":"LBRouter__
+000197c0: 4d61 7841 6d6f 756e 7449 6e45 7863 6565  MaxAmountInExcee
+000197d0: 6465 6422 2c22 7479 7065 223a 2265 7272  ded","type":"err
+000197e0: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+000197f0: 5d2c 226e 616d 6522 3a22 4c42 526f 7574  ],"name":"LBRout
+00019800: 6572 5f5f 4e6f 7446 6163 746f 7279 4f77  er__NotFactoryOw
+00019810: 6e65 7222 2c22 7479 7065 223a 2265 7272  ner","type":"err
+00019820: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+00019830: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00019840: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00019850: 3a22 746f 6b65 6e58 222c 2274 7970 6522  :"tokenX","type"
+00019860: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+00019870: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+00019880: 7265 7373 222c 226e 616d 6522 3a22 746f  ress","name":"to
+00019890: 6b65 6e59 222c 2274 7970 6522 3a22 6164  kenY","type":"ad
+000198a0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+000198b0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000198c0: 222c 226e 616d 6522 3a22 6269 6e53 7465  ","name":"binSte
+000198d0: 7022 2c22 7479 7065 223a 2275 696e 7432  p","type":"uint2
+000198e0: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
+000198f0: 526f 7574 6572 5f5f 5061 6972 4e6f 7443  Router__PairNotC
+00019900: 7265 6174 6564 222c 2274 7970 6522 3a22  reated","type":"
+00019910: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+00019920: 223a 5b5d 2c22 6e61 6d65 223a 224c 4252  ":[],"name":"LBR
+00019930: 6f75 7465 725f 5f53 656e 6465 7249 734e  outer__SenderIsN
+00019940: 6f74 5741 5641 5822 2c22 7479 7065 223a  otWAVAX","type":
+00019950: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00019960: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00019970: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00019980: 616d 6522 3a22 6964 222c 2274 7970 6522  ame":"id","type"
+00019990: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+000199a0: 6d65 223a 224c 4252 6f75 7465 725f 5f53  me":"LBRouter__S
+000199b0: 7761 704f 7665 7266 6c6f 7773 222c 2274  wapOverflows","t
+000199c0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+000199d0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+000199e0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+000199f0: 3622 2c22 6e61 6d65 223a 2265 7863 6573  6","name":"exces
+00019a00: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
+00019a10: 3536 227d 5d2c 226e 616d 6522 3a22 4c42  56"}],"name":"LB
+00019a20: 526f 7574 6572 5f5f 546f 6f4d 7563 6854  Router__TooMuchT
+00019a30: 6f6b 656e 7349 6e22 2c22 7479 7065 223a  okensIn","type":
+00019a40: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+00019a50: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00019a60: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00019a70: 616d 6522 3a22 616d 6f75 6e74 222c 2274  ame":"amount","t
+00019a80: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+00019a90: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00019aa0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00019ab0: 3a22 7265 7365 7276 6522 2c22 7479 7065  :"reserve","type
+00019ac0: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+00019ad0: 616d 6522 3a22 4c42 526f 7574 6572 5f5f  ame":"LBRouter__
+00019ae0: 5772 6f6e 6741 6d6f 756e 7473 222c 2274  WrongAmounts","t
+00019af0: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00019b00: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00019b10: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+00019b20: 7322 2c22 6e61 6d65 223a 2274 6f6b 656e  s","name":"token
+00019b30: 5822 2c22 7479 7065 223a 2261 6464 7265  X","type":"addre
+00019b40: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+00019b50: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+00019b60: 6e61 6d65 223a 2274 6f6b 656e 5922 2c22  name":"tokenY","
+00019b70: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+00019b80: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00019b90: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00019ba0: 223a 2261 6d6f 756e 7458 222c 2274 7970  ":"amountX","typ
+00019bb0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+00019bc0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00019bd0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00019be0: 616d 6f75 6e74 5922 2c22 7479 7065 223a  amountY","type":
+00019bf0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+00019c00: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00019c10: 3235 3622 2c22 6e61 6d65 223a 226d 7367  256","name":"msg
+00019c20: 5661 6c75 6522 2c22 7479 7065 223a 2275  Value","type":"u
+00019c30: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+00019c40: 3a22 4c42 526f 7574 6572 5f5f 5772 6f6e  :"LBRouter__Wron
+00019c50: 6741 7661 784c 6971 7569 6469 7479 5061  gAvaxLiquidityPa
+00019c60: 7261 6d65 7465 7273 222c 2274 7970 6522  rameters","type"
+00019c70: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+00019c80: 7473 223a 5b5d 2c22 6e61 6d65 223a 224c  ts":[],"name":"L
+00019c90: 4252 6f75 7465 725f 5f57 726f 6e67 546f  BRouter__WrongTo
+00019ca0: 6b65 6e4f 7264 6572 222c 2274 7970 6522  kenOrder","type"
+00019cb0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+00019cc0: 7473 223a 5b5d 2c22 6e61 6d65 223a 224d  ts":[],"name":"M
+00019cd0: 6174 6831 3238 7831 3238 5f5f 4c6f 6755  ath128x128__LogU
+00019ce0: 6e64 6572 666c 6f77 222c 2274 7970 6522  nderflow","type"
+00019cf0: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+00019d00: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00019d10: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00019d20: 6e61 6d65 223a 2278 222c 2274 7970 6522  name":"x","type"
+00019d30: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+00019d40: 7465 726e 616c 5479 7065 223a 2269 6e74  ternalType":"int
+00019d50: 3235 3622 2c22 6e61 6d65 223a 2279 222c  256","name":"y",
+00019d60: 2274 7970 6522 3a22 696e 7432 3536 227d  "type":"int256"}
+00019d70: 5d2c 226e 616d 6522 3a22 4d61 7468 3132  ],"name":"Math12
+00019d80: 3878 3132 385f 5f50 6f77 6572 556e 6465  8x128__PowerUnde
+00019d90: 7266 6c6f 7722 2c22 7479 7065 223a 2265  rflow","type":"e
+00019da0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+00019db0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00019dc0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00019dd0: 6522 3a22 7072 6f64 3122 2c22 7479 7065  e":"prod1","type
+00019de0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00019df0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00019e00: 6e74 3235 3622 2c22 6e61 6d65 223a 2264  nt256","name":"d
+00019e10: 656e 6f6d 696e 6174 6f72 222c 2274 7970  enominator","typ
+00019e20: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+00019e30: 6e61 6d65 223a 224d 6174 6835 3132 4269  name":"Math512Bi
+00019e40: 7473 5f5f 4d75 6c44 6976 4f76 6572 666c  ts__MulDivOverfl
+00019e50: 6f77 222c 2274 7970 6522 3a22 6572 726f  ow","type":"erro
+00019e60: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
+00019e70: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00019e80: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00019e90: 2270 726f 6431 222c 2274 7970 6522 3a22  "prod1","type":"
+00019ea0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+00019eb0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00019ec0: 3536 222c 226e 616d 6522 3a22 6f66 6673  56","name":"offs
+00019ed0: 6574 222c 2274 7970 6522 3a22 7569 6e74  et","type":"uint
+00019ee0: 3235 3622 7d5d 2c22 6e61 6d65 223a 224d  256"}],"name":"M
+00019ef0: 6174 6835 3132 4269 7473 5f5f 4d75 6c53  ath512Bits__MulS
+00019f00: 6869 6674 4f76 6572 666c 6f77 222c 2274  hiftOverflow","t
+00019f10: 7970 6522 3a22 6572 726f 7222 7d2c 7b22  ype":"error"},{"
+00019f20: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00019f30: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+00019f40: 3622 2c22 6e61 6d65 223a 226f 6666 7365  6","name":"offse
+00019f50: 7422 2c22 7479 7065 223a 2275 696e 7432  t","type":"uint2
+00019f60: 3536 227d 5d2c 226e 616d 6522 3a22 4d61  56"}],"name":"Ma
+00019f70: 7468 3531 3242 6974 735f 5f4f 6666 7365  th512Bits__Offse
+00019f80: 744f 7665 7266 6c6f 7773 222c 2274 7970  tOverflows","typ
+00019f90: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+00019fa0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00019fb0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00019fc0: 2c22 6e61 6d65 223a 2278 222c 2274 7970  ,"name":"x","typ
+00019fd0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+00019fe0: 6e61 6d65 223a 2253 6166 6543 6173 745f  name":"SafeCast_
+00019ff0: 5f45 7863 6565 6473 3132 3842 6974 7322  _Exceeds128Bits"
+0001a000: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+0001a010: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+0001a020: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001a030: 7432 3536 222c 226e 616d 6522 3a22 7822  t256","name":"x"
+0001a040: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001a050: 227d 5d2c 226e 616d 6522 3a22 5361 6665  "}],"name":"Safe
+0001a060: 4361 7374 5f5f 4578 6365 6564 7334 3042  Cast__Exceeds40B
+0001a070: 6974 7322 2c22 7479 7065 223a 2265 7272  its","type":"err
+0001a080: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0001a090: 5d2c 226e 616d 6522 3a22 546f 6b65 6e48  ],"name":"TokenH
+0001a0a0: 656c 7065 725f 5f43 616c 6c46 6169 6c65  elper__CallFaile
+0001a0b0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
+0001a0c0: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+0001a0d0: 226e 616d 6522 3a22 546f 6b65 6e48 656c  "name":"TokenHel
+0001a0e0: 7065 725f 5f4e 6f6e 436f 6e74 7261 6374  per__NonContract
+0001a0f0: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001a100: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+0001a110: 6e61 6d65 223a 2254 6f6b 656e 4865 6c70  name":"TokenHelp
+0001a120: 6572 5f5f 5472 616e 7366 6572 4661 696c  er__TransferFail
+0001a130: 6564 222c 2274 7970 6522 3a22 6572 726f  ed","type":"erro
+0001a140: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
+0001a150: 2263 6f6d 706f 6e65 6e74 7322 3a5b 7b22  "components":[{"
+0001a160: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+0001a170: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
+0001a180: 226e 616d 6522 3a22 746f 6b65 6e58 222c  "name":"tokenX",
+0001a190: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0001a1a0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001a1b0: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
+0001a1c0: 3230 222c 226e 616d 6522 3a22 746f 6b65  20","name":"toke
+0001a1d0: 6e59 222c 2274 7970 6522 3a22 6164 6472  nY","type":"addr
+0001a1e0: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0001a1f0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001a200: 226e 616d 6522 3a22 6269 6e53 7465 7022  "name":"binStep"
+0001a210: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001a220: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001a230: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001a240: 6d65 223a 2261 6d6f 756e 7458 222c 2274  me":"amountX","t
+0001a250: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0001a260: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001a270: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001a280: 3a22 616d 6f75 6e74 5922 2c22 7479 7065  :"amountY","type
+0001a290: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+0001a2a0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001a2b0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+0001a2c0: 6d6f 756e 7458 4d69 6e22 2c22 7479 7065  mountXMin","type
+0001a2d0: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+0001a2e0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001a2f0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+0001a300: 6d6f 756e 7459 4d69 6e22 2c22 7479 7065  mountYMin","type
+0001a310: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+0001a320: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001a330: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+0001a340: 6374 6976 6549 6444 6573 6972 6564 222c  ctiveIdDesired",
+0001a350: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001a360: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001a370: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001a380: 6522 3a22 6964 536c 6970 7061 6765 222c  e":"idSlippage",
+0001a390: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001a3a0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001a3b0: 223a 2269 6e74 3235 365b 5d22 2c22 6e61  ":"int256[]","na
+0001a3c0: 6d65 223a 2264 656c 7461 4964 7322 2c22  me":"deltaIds","
+0001a3d0: 7479 7065 223a 2269 6e74 3235 365b 5d22  type":"int256[]"
+0001a3e0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001a3f0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+0001a400: 616d 6522 3a22 6469 7374 7269 6275 7469  ame":"distributi
+0001a410: 6f6e 5822 2c22 7479 7065 223a 2275 696e  onX","type":"uin
+0001a420: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
+0001a430: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001a440: 365b 5d22 2c22 6e61 6d65 223a 2264 6973  6[]","name":"dis
+0001a450: 7472 6962 7574 696f 6e59 222c 2274 7970  tributionY","typ
+0001a460: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
+0001a470: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001a480: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0001a490: 3a22 746f 222c 2274 7970 6522 3a22 6164  :"to","type":"ad
+0001a4a0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001a4b0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001a4c0: 222c 226e 616d 6522 3a22 6465 6164 6c69  ","name":"deadli
+0001a4d0: 6e65 222c 2274 7970 6522 3a22 7569 6e74  ne","type":"uint
+0001a4e0: 3235 3622 7d5d 2c22 696e 7465 726e 616c  256"}],"internal
+0001a4f0: 5479 7065 223a 2273 7472 7563 7420 494c  Type":"struct IL
+0001a500: 4252 6f75 7465 722e 4c69 7175 6964 6974  BRouter.Liquidit
+0001a510: 7950 6172 616d 6574 6572 7322 2c22 6e61  yParameters","na
+0001a520: 6d65 223a 225f 6c69 7175 6964 6974 7950  me":"_liquidityP
+0001a530: 6172 616d 6574 6572 7322 2c22 7479 7065  arameters","type
+0001a540: 223a 2274 7570 6c65 227d 5d2c 226e 616d  ":"tuple"}],"nam
+0001a550: 6522 3a22 6164 644c 6971 7569 6469 7479  e":"addLiquidity
+0001a560: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
+0001a570: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001a580: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
+0001a590: 2264 6570 6f73 6974 4964 7322 2c22 7479  "depositIds","ty
+0001a5a0: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
+0001a5b0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001a5c0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
+0001a5d0: 6d65 223a 226c 6971 7569 6469 7479 4d69  me":"liquidityMi
+0001a5e0: 6e74 6564 222c 2274 7970 6522 3a22 7569  nted","type":"ui
+0001a5f0: 6e74 3235 365b 5d22 7d5d 2c22 7374 6174  nt256[]"}],"stat
+0001a600: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
+0001a610: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
+0001a620: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0001a630: 6e70 7574 7322 3a5b 7b22 636f 6d70 6f6e  nputs":[{"compon
+0001a640: 656e 7473 223a 5b7b 2269 6e74 6572 6e61  ents":[{"interna
+0001a650: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
+0001a660: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
+0001a670: 2274 6f6b 656e 5822 2c22 7479 7065 223a  "tokenX","type":
+0001a680: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+0001a690: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+0001a6a0: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
+0001a6b0: 6d65 223a 2274 6f6b 656e 5922 2c22 7479  me":"tokenY","ty
+0001a6c0: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+0001a6d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001a6e0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001a6f0: 2262 696e 5374 6570 222c 2274 7970 6522  "binStep","type"
+0001a700: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001a710: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001a720: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0001a730: 6f75 6e74 5822 2c22 7479 7065 223a 2275  ountX","type":"u
+0001a740: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
+0001a750: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001a760: 3622 2c22 6e61 6d65 223a 2261 6d6f 756e  6","name":"amoun
+0001a770: 7459 222c 2274 7970 6522 3a22 7569 6e74  tY","type":"uint
+0001a780: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001a790: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001a7a0: 226e 616d 6522 3a22 616d 6f75 6e74 584d  "name":"amountXM
+0001a7b0: 696e 222c 2274 7970 6522 3a22 7569 6e74  in","type":"uint
+0001a7c0: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001a7d0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001a7e0: 226e 616d 6522 3a22 616d 6f75 6e74 594d  "name":"amountYM
+0001a7f0: 696e 222c 2274 7970 6522 3a22 7569 6e74  in","type":"uint
+0001a800: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001a810: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001a820: 226e 616d 6522 3a22 6163 7469 7665 4964  "name":"activeId
+0001a830: 4465 7369 7265 6422 2c22 7479 7065 223a  Desired","type":
+0001a840: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+0001a850: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001a860: 3235 3622 2c22 6e61 6d65 223a 2269 6453  256","name":"idS
+0001a870: 6c69 7070 6167 6522 2c22 7479 7065 223a  lippage","type":
+0001a880: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+0001a890: 6572 6e61 6c54 7970 6522 3a22 696e 7432  ernalType":"int2
+0001a8a0: 3536 5b5d 222c 226e 616d 6522 3a22 6465  56[]","name":"de
+0001a8b0: 6c74 6149 6473 222c 2274 7970 6522 3a22  ltaIds","type":"
+0001a8c0: 696e 7432 3536 5b5d 227d 2c7b 2269 6e74  int256[]"},{"int
+0001a8d0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001a8e0: 3235 365b 5d22 2c22 6e61 6d65 223a 2264  256[]","name":"d
+0001a8f0: 6973 7472 6962 7574 696f 6e58 222c 2274  istributionX","t
+0001a900: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+0001a910: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001a920: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+0001a930: 616d 6522 3a22 6469 7374 7269 6275 7469  ame":"distributi
+0001a940: 6f6e 5922 2c22 7479 7065 223a 2275 696e  onY","type":"uin
+0001a950: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
+0001a960: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0001a970: 7322 2c22 6e61 6d65 223a 2274 6f22 2c22  s","name":"to","
+0001a980: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+0001a990: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001a9a0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001a9b0: 223a 2264 6561 646c 696e 6522 2c22 7479  ":"deadline","ty
+0001a9c0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+0001a9d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001a9e0: 7374 7275 6374 2049 4c42 526f 7574 6572  struct ILBRouter
+0001a9f0: 2e4c 6971 7569 6469 7479 5061 7261 6d65  .LiquidityParame
+0001aa00: 7465 7273 222c 226e 616d 6522 3a22 5f6c  ters","name":"_l
+0001aa10: 6971 7569 6469 7479 5061 7261 6d65 7465  iquidityParamete
+0001aa20: 7273 222c 2274 7970 6522 3a22 7475 706c  rs","type":"tupl
+0001aa30: 6522 7d5d 2c22 6e61 6d65 223a 2261 6464  e"}],"name":"add
+0001aa40: 4c69 7175 6964 6974 7941 5641 5822 2c22  LiquidityAVAX","
+0001aa50: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+0001aa60: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001aa70: 3536 5b5d 222c 226e 616d 6522 3a22 6465  56[]","name":"de
+0001aa80: 706f 7369 7449 6473 222c 2274 7970 6522  positIds","type"
+0001aa90: 3a22 7569 6e74 3235 365b 5d22 7d2c 7b22  :"uint256[]"},{"
+0001aaa0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001aab0: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
+0001aac0: 3a22 6c69 7175 6964 6974 794d 696e 7465  :"liquidityMinte
+0001aad0: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
+0001aae0: 3536 5b5d 227d 5d2c 2273 7461 7465 4d75  56[]"}],"stateMu
+0001aaf0: 7461 6269 6c69 7479 223a 2270 6179 6162  tability":"payab
+0001ab00: 6c65 222c 2274 7970 6522 3a22 6675 6e63  le","type":"func
+0001ab10: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0001ab20: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0001ab30: 223a 2263 6f6e 7472 6163 7420 4945 5243  ":"contract IERC
+0001ab40: 3230 222c 226e 616d 6522 3a22 5f74 6f6b  20","name":"_tok
+0001ab50: 656e 5822 2c22 7479 7065 223a 2261 6464  enX","type":"add
+0001ab60: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+0001ab70: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
+0001ab80: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
+0001ab90: 225f 746f 6b65 6e59 222c 2274 7970 6522  "_tokenY","type"
+0001aba0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001abb0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001abc0: 7432 3422 2c22 6e61 6d65 223a 225f 6163  t24","name":"_ac
+0001abd0: 7469 7665 4964 222c 2274 7970 6522 3a22  tiveId","type":"
+0001abe0: 7569 6e74 3234 227d 2c7b 2269 6e74 6572  uint24"},{"inter
+0001abf0: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
+0001ac00: 222c 226e 616d 6522 3a22 5f62 696e 5374  ","name":"_binSt
+0001ac10: 6570 222c 2274 7970 6522 3a22 7569 6e74  ep","type":"uint
+0001ac20: 3136 227d 5d2c 226e 616d 6522 3a22 6372  16"}],"name":"cr
+0001ac30: 6561 7465 4c42 5061 6972 222c 226f 7574  eateLBPair","out
+0001ac40: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001ac50: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
+0001ac60: 2049 4c42 5061 6972 222c 226e 616d 6522   ILBPair","name"
+0001ac70: 3a22 7061 6972 222c 2274 7970 6522 3a22  :"pair","type":"
+0001ac80: 6164 6472 6573 7322 7d5d 2c22 7374 6174  address"}],"stat
+0001ac90: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
+0001aca0: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
+0001acb0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0001acc0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0001acd0: 3a22 6661 6374 6f72 7922 2c22 6f75 7470  :"factory","outp
+0001ace0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+0001acf0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+0001ad00: 494c 4246 6163 746f 7279 222c 226e 616d  ILBFactory","nam
+0001ad10: 6522 3a22 222c 2274 7970 6522 3a22 6164  e":"","type":"ad
+0001ad20: 6472 6573 7322 7d5d 2c22 7374 6174 654d  dress"}],"stateM
+0001ad30: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
+0001ad40: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+0001ad50: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+0001ad60: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001ad70: 2263 6f6e 7472 6163 7420 494c 4250 6169  "contract ILBPai
+0001ad80: 7222 2c22 6e61 6d65 223a 225f 4c42 5061  r","name":"_LBPa
+0001ad90: 6972 222c 2274 7970 6522 3a22 6164 6472  ir","type":"addr
+0001ada0: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0001adb0: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001adc0: 226e 616d 6522 3a22 5f70 7269 6365 222c  "name":"_price",
+0001add0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001ade0: 7d5d 2c22 6e61 6d65 223a 2267 6574 4964  }],"name":"getId
+0001adf0: 4672 6f6d 5072 6963 6522 2c22 6f75 7470  FromPrice","outp
+0001ae00: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+0001ae10: 5479 7065 223a 2275 696e 7432 3422 2c22  Type":"uint24","
+0001ae20: 6e61 6d65 223a 2222 2c22 7479 7065 223a  name":"","type":
+0001ae30: 2275 696e 7432 3422 7d5d 2c22 7374 6174  "uint24"}],"stat
+0001ae40: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
+0001ae50: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
+0001ae60: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0001ae70: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0001ae80: 223a 2263 6f6e 7472 6163 7420 494c 4250  ":"contract ILBP
+0001ae90: 6169 7222 2c22 6e61 6d65 223a 225f 4c42  air","name":"_LB
+0001aea0: 5061 6972 222c 2274 7970 6522 3a22 6164  Pair","type":"ad
+0001aeb0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001aec0: 616c 5479 7065 223a 2275 696e 7432 3422  alType":"uint24"
+0001aed0: 2c22 6e61 6d65 223a 225f 6964 222c 2274  ,"name":"_id","t
+0001aee0: 7970 6522 3a22 7569 6e74 3234 227d 5d2c  ype":"uint24"}],
+0001aef0: 226e 616d 6522 3a22 6765 7450 7269 6365  "name":"getPrice
+0001af00: 4672 6f6d 4964 222c 226f 7574 7075 7473  FromId","outputs
+0001af10: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001af20: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001af30: 6d65 223a 2222 2c22 7479 7065 223a 2275  me":"","type":"u
+0001af40: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
+0001af50: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
+0001af60: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
+0001af70: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+0001af80: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001af90: 3a22 636f 6e74 7261 6374 2049 4c42 5061  :"contract ILBPa
+0001afa0: 6972 222c 226e 616d 6522 3a22 5f4c 4250  ir","name":"_LBP
+0001afb0: 6169 7222 2c22 7479 7065 223a 2261 6464  air","type":"add
+0001afc0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+0001afd0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001afe0: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
+0001aff0: 4f75 7422 2c22 7479 7065 223a 2275 696e  Out","type":"uin
+0001b000: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+0001b010: 6c54 7970 6522 3a22 626f 6f6c 222c 226e  lType":"bool","n
+0001b020: 616d 6522 3a22 5f73 7761 7046 6f72 5922  ame":"_swapForY"
+0001b030: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
+0001b040: 2c22 6e61 6d65 223a 2267 6574 5377 6170  ,"name":"getSwap
+0001b050: 496e 222c 226f 7574 7075 7473 223a 5b7b  In","outputs":[{
+0001b060: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001b070: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001b080: 2261 6d6f 756e 7449 6e22 2c22 7479 7065  "amountIn","type
+0001b090: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+0001b0a0: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001b0b0: 6e74 3235 3622 2c22 6e61 6d65 223a 2266  nt256","name":"f
+0001b0c0: 6565 7349 6e22 2c22 7479 7065 223a 2275  eesIn","type":"u
+0001b0d0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
+0001b0e0: 4d75 7461 6269 6c69 7479 223a 2276 6965  Mutability":"vie
+0001b0f0: 7722 2c22 7479 7065 223a 2266 756e 6374  w","type":"funct
+0001b100: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+0001b110: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001b120: 3a22 636f 6e74 7261 6374 2049 4c42 5061  :"contract ILBPa
+0001b130: 6972 222c 226e 616d 6522 3a22 5f4c 4250  ir","name":"_LBP
+0001b140: 6169 7222 2c22 7479 7065 223a 2261 6464  air","type":"add
+0001b150: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+0001b160: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001b170: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
+0001b180: 496e 222c 2274 7970 6522 3a22 7569 6e74  In","type":"uint
+0001b190: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001b1a0: 5479 7065 223a 2262 6f6f 6c22 2c22 6e61  Type":"bool","na
+0001b1b0: 6d65 223a 225f 7377 6170 466f 7259 222c  me":"_swapForY",
+0001b1c0: 2274 7970 6522 3a22 626f 6f6c 227d 5d2c  "type":"bool"}],
+0001b1d0: 226e 616d 6522 3a22 6765 7453 7761 704f  "name":"getSwapO
+0001b1e0: 7574 222c 226f 7574 7075 7473 223a 5b7b  ut","outputs":[{
+0001b1f0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001b200: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001b210: 2261 6d6f 756e 744f 7574 222c 2274 7970  "amountOut","typ
+0001b220: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0001b230: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001b240: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001b250: 6665 6573 496e 222c 2274 7970 6522 3a22  feesIn","type":"
+0001b260: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
+0001b270: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
+0001b280: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
+0001b290: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+0001b2a0: 3a5b 5d2c 226e 616d 6522 3a22 6f6c 6446  :[],"name":"oldF
+0001b2b0: 6163 746f 7279 222c 226f 7574 7075 7473  actory","outputs
+0001b2c0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001b2d0: 6522 3a22 636f 6e74 7261 6374 2049 4a6f  e":"contract IJo
+0001b2e0: 6546 6163 746f 7279 222c 226e 616d 6522  eFactory","name"
+0001b2f0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
+0001b300: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
+0001b310: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+0001b320: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+0001b330: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+0001b340: 696e 7465 726e 616c 5479 7065 223a 2263  internalType":"c
+0001b350: 6f6e 7472 6163 7420 4945 5243 3230 222c  ontract IERC20",
+0001b360: 226e 616d 6522 3a22 5f74 6f6b 656e 5822  "name":"_tokenX"
+0001b370: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001b380: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001b390: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
+0001b3a0: 4332 3022 2c22 6e61 6d65 223a 225f 746f  C20","name":"_to
+0001b3b0: 6b65 6e59 222c 2274 7970 6522 3a22 6164  kenY","type":"ad
+0001b3c0: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001b3d0: 616c 5479 7065 223a 2275 696e 7431 3622  alType":"uint16"
+0001b3e0: 2c22 6e61 6d65 223a 225f 6269 6e53 7465  ,"name":"_binSte
+0001b3f0: 7022 2c22 7479 7065 223a 2275 696e 7431  p","type":"uint1
+0001b400: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0001b410: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001b420: 616d 6522 3a22 5f61 6d6f 756e 7458 4d69  ame":"_amountXMi
+0001b430: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
+0001b440: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+0001b450: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001b460: 6e61 6d65 223a 225f 616d 6f75 6e74 594d  name":"_amountYM
+0001b470: 696e 222c 2274 7970 6522 3a22 7569 6e74  in","type":"uint
+0001b480: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001b490: 5479 7065 223a 2275 696e 7432 3536 5b5d  Type":"uint256[]
+0001b4a0: 222c 226e 616d 6522 3a22 5f69 6473 222c  ","name":"_ids",
+0001b4b0: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
+0001b4c0: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
+0001b4d0: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
+0001b4e0: 226e 616d 6522 3a22 5f61 6d6f 756e 7473  "name":"_amounts
+0001b4f0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001b500: 365b 5d22 7d2c 7b22 696e 7465 726e 616c  6[]"},{"internal
+0001b510: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0001b520: 226e 616d 6522 3a22 5f74 6f22 2c22 7479  "name":"_to","ty
+0001b530: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+0001b540: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001b550: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001b560: 225f 6465 6164 6c69 6e65 222c 2274 7970  "_deadline","typ
+0001b570: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+0001b580: 6e61 6d65 223a 2272 656d 6f76 654c 6971  name":"removeLiq
+0001b590: 7569 6469 7479 222c 226f 7574 7075 7473  uidity","outputs
+0001b5a0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001b5b0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001b5c0: 6d65 223a 2261 6d6f 756e 7458 222c 2274  me":"amountX","t
+0001b5d0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0001b5e0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001b5f0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001b600: 3a22 616d 6f75 6e74 5922 2c22 7479 7065  :"amountY","type
+0001b610: 223a 2275 696e 7432 3536 227d 5d2c 2273  ":"uint256"}],"s
+0001b620: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+0001b630: 226e 6f6e 7061 7961 626c 6522 2c22 7479  "nonpayable","ty
+0001b640: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+0001b650: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0001b660: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+0001b670: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
+0001b680: 6d65 223a 225f 746f 6b65 6e22 2c22 7479  me":"_token","ty
+0001b690: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+0001b6a0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001b6b0: 7569 6e74 3136 222c 226e 616d 6522 3a22  uint16","name":"
+0001b6c0: 5f62 696e 5374 6570 222c 2274 7970 6522  _binStep","type"
+0001b6d0: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
+0001b6e0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001b6f0: 3235 3622 2c22 6e61 6d65 223a 225f 616d  256","name":"_am
+0001b700: 6f75 6e74 546f 6b65 6e4d 696e 222c 2274  ountTokenMin","t
+0001b710: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0001b720: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001b730: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001b740: 3a22 5f61 6d6f 756e 7441 5641 584d 696e  :"_amountAVAXMin
+0001b750: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001b760: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0001b770: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
+0001b780: 226e 616d 6522 3a22 5f69 6473 222c 2274  "name":"_ids","t
+0001b790: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+0001b7a0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001b7b0: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+0001b7c0: 616d 6522 3a22 5f61 6d6f 756e 7473 222c  ame":"_amounts",
+0001b7d0: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
+0001b7e0: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
+0001b7f0: 7065 223a 2261 6464 7265 7373 2070 6179  pe":"address pay
+0001b800: 6162 6c65 222c 226e 616d 6522 3a22 5f74  able","name":"_t
+0001b810: 6f22 2c22 7479 7065 223a 2261 6464 7265  o","type":"addre
+0001b820: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+0001b830: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001b840: 6e61 6d65 223a 225f 6465 6164 6c69 6e65  name":"_deadline
+0001b850: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001b860: 3622 7d5d 2c22 6e61 6d65 223a 2272 656d  6"}],"name":"rem
+0001b870: 6f76 654c 6971 7569 6469 7479 4156 4158  oveLiquidityAVAX
+0001b880: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
+0001b890: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001b8a0: 6e74 3235 3622 2c22 6e61 6d65 223a 2261  nt256","name":"a
+0001b8b0: 6d6f 756e 7454 6f6b 656e 222c 2274 7970  mountToken","typ
+0001b8c0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0001b8d0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001b8e0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001b8f0: 616d 6f75 6e74 4156 4158 222c 2274 7970  amountAVAX","typ
+0001b900: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+0001b910: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+0001b920: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+0001b930: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+0001b940: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+0001b950: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001b960: 7432 3536 222c 226e 616d 6522 3a22 5f61  t256","name":"_a
+0001b970: 6d6f 756e 744f 7574 222c 2274 7970 6522  mountOut","type"
+0001b980: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001b990: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001b9a0: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
+0001b9b0: 5f70 6169 7242 696e 5374 6570 7322 2c22  _pairBinSteps","
+0001b9c0: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
+0001b9d0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001b9e0: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
+0001b9f0: 4332 305b 5d22 2c22 6e61 6d65 223a 225f  C20[]","name":"_
+0001ba00: 746f 6b65 6e50 6174 6822 2c22 7479 7065  tokenPath","type
+0001ba10: 223a 2261 6464 7265 7373 5b5d 227d 2c7b  ":"address[]"},{
+0001ba20: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001ba30: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+0001ba40: 225f 746f 222c 2274 7970 6522 3a22 6164  "_to","type":"ad
+0001ba50: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001ba60: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001ba70: 222c 226e 616d 6522 3a22 5f64 6561 646c  ","name":"_deadl
+0001ba80: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
+0001ba90: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+0001baa0: 7377 6170 4156 4158 466f 7245 7861 6374  swapAVAXForExact
+0001bab0: 546f 6b65 6e73 222c 226f 7574 7075 7473  Tokens","outputs
+0001bac0: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+0001bad0: 6522 3a22 7569 6e74 3235 365b 5d22 2c22  e":"uint256[]","
+0001bae0: 6e61 6d65 223a 2261 6d6f 756e 7473 496e  name":"amountsIn
+0001baf0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001bb00: 365b 5d22 7d5d 2c22 7374 6174 654d 7574  6[]"}],"stateMut
+0001bb10: 6162 696c 6974 7922 3a22 7061 7961 626c  ability":"payabl
+0001bb20: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
+0001bb30: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+0001bb40: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001bb50: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001bb60: 223a 225f 616d 6f75 6e74 4f75 744d 696e  ":"_amountOutMin
+0001bb70: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001bb80: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0001bb90: 7065 223a 2275 696e 7432 3536 5b5d 222c  pe":"uint256[]",
+0001bba0: 226e 616d 6522 3a22 5f70 6169 7242 696e  "name":"_pairBin
+0001bbb0: 5374 6570 7322 2c22 7479 7065 223a 2275  Steps","type":"u
+0001bbc0: 696e 7432 3536 5b5d 227d 2c7b 2269 6e74  int256[]"},{"int
+0001bbd0: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+0001bbe0: 7261 6374 2049 4552 4332 305b 5d22 2c22  ract IERC20[]","
+0001bbf0: 6e61 6d65 223a 225f 746f 6b65 6e50 6174  name":"_tokenPat
+0001bc00: 6822 2c22 7479 7065 223a 2261 6464 7265  h","type":"addre
+0001bc10: 7373 5b5d 227d 2c7b 2269 6e74 6572 6e61  ss[]"},{"interna
+0001bc20: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+0001bc30: 2c22 6e61 6d65 223a 225f 746f 222c 2274  ,"name":"_to","t
+0001bc40: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+0001bc50: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001bc60: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001bc70: 3a22 5f64 6561 646c 696e 6522 2c22 7479  :"_deadline","ty
+0001bc80: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+0001bc90: 226e 616d 6522 3a22 7377 6170 4578 6163  "name":"swapExac
+0001bca0: 7441 5641 5846 6f72 546f 6b65 6e73 222c  tAVAXForTokens",
+0001bcb0: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
+0001bcc0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001bcd0: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
+0001bce0: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
+0001bcf0: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
+0001bd00: 654d 7574 6162 696c 6974 7922 3a22 7061  eMutability":"pa
+0001bd10: 7961 626c 6522 2c22 7479 7065 223a 2266  yable","type":"f
+0001bd20: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+0001bd30: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001bd40: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001bd50: 6e61 6d65 223a 225f 616d 6f75 6e74 4f75  name":"_amountOu
+0001bd60: 744d 696e 222c 2274 7970 6522 3a22 7569  tMin","type":"ui
+0001bd70: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0001bd80: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001bd90: 5b5d 222c 226e 616d 6522 3a22 5f70 6169  []","name":"_pai
+0001bda0: 7242 696e 5374 6570 7322 2c22 7479 7065  rBinSteps","type
+0001bdb0: 223a 2275 696e 7432 3536 5b5d 227d 2c7b  ":"uint256[]"},{
+0001bdc0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001bdd0: 636f 6e74 7261 6374 2049 4552 4332 305b  contract IERC20[
+0001bde0: 5d22 2c22 6e61 6d65 223a 225f 746f 6b65  ]","name":"_toke
+0001bdf0: 6e50 6174 6822 2c22 7479 7065 223a 2261  nPath","type":"a
+0001be00: 6464 7265 7373 5b5d 227d 2c7b 2269 6e74  ddress[]"},{"int
+0001be10: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0001be20: 6573 7322 2c22 6e61 6d65 223a 225f 746f  ess","name":"_to
+0001be30: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0001be40: 7322 7d2c 7b22 696e 7465 726e 616c 5479  s"},{"internalTy
+0001be50: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001be60: 616d 6522 3a22 5f64 6561 646c 696e 6522  ame":"_deadline"
+0001be70: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001be80: 227d 5d2c 226e 616d 6522 3a22 7377 6170  "}],"name":"swap
+0001be90: 4578 6163 7441 5641 5846 6f72 546f 6b65  ExactAVAXForToke
+0001bea0: 6e73 5375 7070 6f72 7469 6e67 4665 654f  nsSupportingFeeO
+0001beb0: 6e54 7261 6e73 6665 7254 6f6b 656e 7322  nTransferTokens"
+0001bec0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+0001bed0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001bee0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+0001bef0: 6f75 6e74 4f75 7422 2c22 7479 7065 223a  ountOut","type":
+0001bf00: 2275 696e 7432 3536 227d 5d2c 2273 7461  "uint256"}],"sta
+0001bf10: 7465 4d75 7461 6269 6c69 7479 223a 2270  teMutability":"p
+0001bf20: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
+0001bf30: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+0001bf40: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+0001bf50: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001bf60: 226e 616d 6522 3a22 5f61 6d6f 756e 7449  "name":"_amountI
+0001bf70: 6e22 2c22 7479 7065 223a 2275 696e 7432  n","type":"uint2
+0001bf80: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+0001bf90: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001bfa0: 6e61 6d65 223a 225f 616d 6f75 6e74 4f75  name":"_amountOu
+0001bfb0: 744d 696e 4156 4158 222c 2274 7970 6522  tMinAVAX","type"
+0001bfc0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001bfd0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001bfe0: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
+0001bff0: 5f70 6169 7242 696e 5374 6570 7322 2c22  _pairBinSteps","
+0001c000: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
+0001c010: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001c020: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
+0001c030: 4332 305b 5d22 2c22 6e61 6d65 223a 225f  C20[]","name":"_
+0001c040: 746f 6b65 6e50 6174 6822 2c22 7479 7065  tokenPath","type
+0001c050: 223a 2261 6464 7265 7373 5b5d 227d 2c7b  ":"address[]"},{
+0001c060: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001c070: 6164 6472 6573 7320 7061 7961 626c 6522  address payable"
+0001c080: 2c22 6e61 6d65 223a 225f 746f 222c 2274  ,"name":"_to","t
+0001c090: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+0001c0a0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001c0b0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001c0c0: 3a22 5f64 6561 646c 696e 6522 2c22 7479  :"_deadline","ty
+0001c0d0: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+0001c0e0: 226e 616d 6522 3a22 7377 6170 4578 6163  "name":"swapExac
+0001c0f0: 7454 6f6b 656e 7346 6f72 4156 4158 222c  tTokensForAVAX",
+0001c100: 226f 7574 7075 7473 223a 5b7b 2269 6e74  "outputs":[{"int
+0001c110: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001c120: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
+0001c130: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
+0001c140: 7569 6e74 3235 3622 7d5d 2c22 7374 6174  uint256"}],"stat
+0001c150: 654d 7574 6162 696c 6974 7922 3a22 6e6f  eMutability":"no
+0001c160: 6e70 6179 6162 6c65 222c 2274 7970 6522  npayable","type"
+0001c170: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+0001c180: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+0001c190: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001c1a0: 222c 226e 616d 6522 3a22 5f61 6d6f 756e  ","name":"_amoun
+0001c1b0: 7449 6e22 2c22 7479 7065 223a 2275 696e  tIn","type":"uin
+0001c1c0: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+0001c1d0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001c1e0: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
+0001c1f0: 4f75 744d 696e 4156 4158 222c 2274 7970  OutMinAVAX","typ
+0001c200: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0001c210: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001c220: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
+0001c230: 3a22 5f70 6169 7242 696e 5374 6570 7322  :"_pairBinSteps"
+0001c240: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001c250: 5b5d 227d 2c7b 2269 6e74 6572 6e61 6c54  []"},{"internalT
+0001c260: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+0001c270: 4552 4332 305b 5d22 2c22 6e61 6d65 223a  ERC20[]","name":
+0001c280: 225f 746f 6b65 6e50 6174 6822 2c22 7479  "_tokenPath","ty
+0001c290: 7065 223a 2261 6464 7265 7373 5b5d 227d  pe":"address[]"}
+0001c2a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001c2b0: 3a22 6164 6472 6573 7320 7061 7961 626c  :"address payabl
+0001c2c0: 6522 2c22 6e61 6d65 223a 225f 746f 222c  e","name":"_to",
+0001c2d0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0001c2e0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001c2f0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001c300: 6522 3a22 5f64 6561 646c 696e 6522 2c22  e":"_deadline","
+0001c310: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001c320: 5d2c 226e 616d 6522 3a22 7377 6170 4578  ],"name":"swapEx
+0001c330: 6163 7454 6f6b 656e 7346 6f72 4156 4158  actTokensForAVAX
+0001c340: 5375 7070 6f72 7469 6e67 4665 654f 6e54  SupportingFeeOnT
+0001c350: 7261 6e73 6665 7254 6f6b 656e 7322 2c22  ransferTokens","
+0001c360: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+0001c370: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001c380: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+0001c390: 6e74 4f75 7422 2c22 7479 7065 223a 2275  ntOut","type":"u
+0001c3a0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
+0001c3b0: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+0001c3c0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+0001c3d0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+0001c3e0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001c3f0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001c400: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
+0001c410: 496e 222c 2274 7970 6522 3a22 7569 6e74  In","type":"uint
+0001c420: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001c430: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001c440: 226e 616d 6522 3a22 5f61 6d6f 756e 744f  "name":"_amountO
+0001c450: 7574 4d69 6e22 2c22 7479 7065 223a 2275  utMin","type":"u
+0001c460: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
+0001c470: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001c480: 365b 5d22 2c22 6e61 6d65 223a 225f 7061  6[]","name":"_pa
+0001c490: 6972 4269 6e53 7465 7073 222c 2274 7970  irBinSteps","typ
+0001c4a0: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
+0001c4b0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+0001c4c0: 2263 6f6e 7472 6163 7420 4945 5243 3230  "contract IERC20
+0001c4d0: 5b5d 222c 226e 616d 6522 3a22 5f74 6f6b  []","name":"_tok
+0001c4e0: 656e 5061 7468 222c 2274 7970 6522 3a22  enPath","type":"
+0001c4f0: 6164 6472 6573 735b 5d22 7d2c 7b22 696e  address[]"},{"in
+0001c500: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0001c510: 7265 7373 222c 226e 616d 6522 3a22 5f74  ress","name":"_t
+0001c520: 6f22 2c22 7479 7065 223a 2261 6464 7265  o","type":"addre
+0001c530: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+0001c540: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001c550: 6e61 6d65 223a 225f 6465 6164 6c69 6e65  name":"_deadline
+0001c560: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001c570: 3622 7d5d 2c22 6e61 6d65 223a 2273 7761  6"}],"name":"swa
+0001c580: 7045 7861 6374 546f 6b65 6e73 466f 7254  pExactTokensForT
+0001c590: 6f6b 656e 7322 2c22 6f75 7470 7574 7322  okens","outputs"
+0001c5a0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0001c5b0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001c5c0: 6522 3a22 616d 6f75 6e74 4f75 7422 2c22  e":"amountOut","
+0001c5d0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001c5e0: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+0001c5f0: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
+0001c600: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+0001c610: 6e22 7d2c 7b22 696e 7075 7473 223a 5b7b  n"},{"inputs":[{
+0001c620: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001c630: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001c640: 225f 616d 6f75 6e74 496e 222c 2274 7970  "_amountIn","typ
+0001c650: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+0001c660: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001c670: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001c680: 5f61 6d6f 756e 744f 7574 4d69 6e22 2c22  _amountOutMin","
+0001c690: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001c6a0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001c6b0: 3a22 7569 6e74 3235 365b 5d22 2c22 6e61  :"uint256[]","na
+0001c6c0: 6d65 223a 225f 7061 6972 4269 6e53 7465  me":"_pairBinSte
+0001c6d0: 7073 222c 2274 7970 6522 3a22 7569 6e74  ps","type":"uint
+0001c6e0: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
+0001c6f0: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+0001c700: 7420 4945 5243 3230 5b5d 222c 226e 616d  t IERC20[]","nam
+0001c710: 6522 3a22 5f74 6f6b 656e 5061 7468 222c  e":"_tokenPath",
+0001c720: 2274 7970 6522 3a22 6164 6472 6573 735b  "type":"address[
+0001c730: 5d22 7d2c 7b22 696e 7465 726e 616c 5479  ]"},{"internalTy
+0001c740: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+0001c750: 616d 6522 3a22 5f74 6f22 2c22 7479 7065  ame":"_to","type
+0001c760: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0001c770: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001c780: 6e74 3235 3622 2c22 6e61 6d65 223a 225f  nt256","name":"_
+0001c790: 6465 6164 6c69 6e65 222c 2274 7970 6522  deadline","type"
+0001c7a0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+0001c7b0: 6d65 223a 2273 7761 7045 7861 6374 546f  me":"swapExactTo
+0001c7c0: 6b65 6e73 466f 7254 6f6b 656e 7353 7570  kensForTokensSup
+0001c7d0: 706f 7274 696e 6746 6565 4f6e 5472 616e  portingFeeOnTran
+0001c7e0: 7366 6572 546f 6b65 6e73 222c 226f 7574  sferTokens","out
+0001c7f0: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001c800: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001c810: 2c22 6e61 6d65 223a 2261 6d6f 756e 744f  ,"name":"amountO
+0001c820: 7574 222c 2274 7970 6522 3a22 7569 6e74  ut","type":"uint
+0001c830: 3235 3622 7d5d 2c22 7374 6174 654d 7574  256"}],"stateMut
+0001c840: 6162 696c 6974 7922 3a22 6e6f 6e70 6179  ability":"nonpay
+0001c850: 6162 6c65 222c 2274 7970 6522 3a22 6675  able","type":"fu
+0001c860: 6e63 7469 6f6e 227d 2c7b 2269 6e70 7574  nction"},{"input
+0001c870: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0001c880: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001c890: 616d 6522 3a22 5f61 6d6f 756e 7441 5641  ame":"_amountAVA
+0001c8a0: 584f 7574 222c 2274 7970 6522 3a22 7569  XOut","type":"ui
+0001c8b0: 6e74 3235 3622 7d2c 7b22 696e 7465 726e  nt256"},{"intern
+0001c8c0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001c8d0: 222c 226e 616d 6522 3a22 5f61 6d6f 756e  ","name":"_amoun
+0001c8e0: 7449 6e4d 6178 222c 2274 7970 6522 3a22  tInMax","type":"
+0001c8f0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0001c900: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001c910: 3536 5b5d 222c 226e 616d 6522 3a22 5f70  56[]","name":"_p
+0001c920: 6169 7242 696e 5374 6570 7322 2c22 7479  airBinSteps","ty
+0001c930: 7065 223a 2275 696e 7432 3536 5b5d 227d  pe":"uint256[]"}
+0001c940: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+0001c950: 3a22 636f 6e74 7261 6374 2049 4552 4332  :"contract IERC2
+0001c960: 305b 5d22 2c22 6e61 6d65 223a 225f 746f  0[]","name":"_to
+0001c970: 6b65 6e50 6174 6822 2c22 7479 7065 223a  kenPath","type":
+0001c980: 2261 6464 7265 7373 5b5d 227d 2c7b 2269  "address[]"},{"i
+0001c990: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+0001c9a0: 6472 6573 7320 7061 7961 626c 6522 2c22  dress payable","
+0001c9b0: 6e61 6d65 223a 225f 746f 222c 2274 7970  name":"_to","typ
+0001c9c0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001c9d0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001c9e0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001c9f0: 5f64 6561 646c 696e 6522 2c22 7479 7065  _deadline","type
+0001ca00: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+0001ca10: 616d 6522 3a22 7377 6170 546f 6b65 6e73  ame":"swapTokens
+0001ca20: 466f 7245 7861 6374 4156 4158 222c 226f  ForExactAVAX","o
+0001ca30: 7574 7075 7473 223a 5b7b 2269 6e74 6572  utputs":[{"inter
+0001ca40: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001ca50: 365b 5d22 2c22 6e61 6d65 223a 2261 6d6f  6[]","name":"amo
+0001ca60: 756e 7473 496e 222c 2274 7970 6522 3a22  untsIn","type":"
+0001ca70: 7569 6e74 3235 365b 5d22 7d5d 2c22 7374  uint256[]"}],"st
+0001ca80: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+0001ca90: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+0001caa0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+0001cab0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+0001cac0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001cad0: 3536 222c 226e 616d 6522 3a22 5f61 6d6f  56","name":"_amo
+0001cae0: 756e 744f 7574 222c 2274 7970 6522 3a22  untOut","type":"
+0001caf0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0001cb00: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001cb10: 3536 222c 226e 616d 6522 3a22 5f61 6d6f  56","name":"_amo
+0001cb20: 756e 7449 6e4d 6178 222c 2274 7970 6522  untInMax","type"
+0001cb30: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+0001cb40: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001cb50: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
+0001cb60: 5f70 6169 7242 696e 5374 6570 7322 2c22  _pairBinSteps","
+0001cb70: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
+0001cb80: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001cb90: 6522 3a22 636f 6e74 7261 6374 2049 4552  e":"contract IER
+0001cba0: 4332 305b 5d22 2c22 6e61 6d65 223a 225f  C20[]","name":"_
+0001cbb0: 746f 6b65 6e50 6174 6822 2c22 7479 7065  tokenPath","type
+0001cbc0: 223a 2261 6464 7265 7373 5b5d 227d 2c7b  ":"address[]"},{
+0001cbd0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001cbe0: 6164 6472 6573 7322 2c22 6e61 6d65 223a  address","name":
+0001cbf0: 225f 746f 222c 2274 7970 6522 3a22 6164  "_to","type":"ad
+0001cc00: 6472 6573 7322 7d2c 7b22 696e 7465 726e  dress"},{"intern
+0001cc10: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001cc20: 222c 226e 616d 6522 3a22 5f64 6561 646c  ","name":"_deadl
+0001cc30: 696e 6522 2c22 7479 7065 223a 2275 696e  ine","type":"uin
+0001cc40: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+0001cc50: 7377 6170 546f 6b65 6e73 466f 7245 7861  swapTokensForExa
+0001cc60: 6374 546f 6b65 6e73 222c 226f 7574 7075  ctTokens","outpu
+0001cc70: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001cc80: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+0001cc90: 2c22 6e61 6d65 223a 2261 6d6f 756e 7473  ,"name":"amounts
+0001cca0: 496e 222c 2274 7970 6522 3a22 7569 6e74  In","type":"uint
+0001ccb0: 3235 365b 5d22 7d5d 2c22 7374 6174 654d  256[]"}],"stateM
+0001ccc0: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
+0001ccd0: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
+0001cce0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+0001ccf0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+0001cd00: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+0001cd10: 4945 5243 3230 222c 226e 616d 6522 3a22  IERC20","name":"
+0001cd20: 5f74 6f6b 656e 222c 2274 7970 6522 3a22  _token","type":"
+0001cd30: 6164 6472 6573 7322 7d2c 7b22 696e 7465  address"},{"inte
+0001cd40: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0001cd50: 7373 222c 226e 616d 6522 3a22 5f74 6f22  ss","name":"_to"
+0001cd60: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001cd70: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+0001cd80: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001cd90: 6d65 223a 225f 616d 6f75 6e74 222c 2274  me":"_amount","t
+0001cda0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0001cdb0: 2c22 6e61 6d65 223a 2273 7765 6570 222c  ,"name":"sweep",
+0001cdc0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+0001cdd0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+0001cde0: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+0001cdf0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+0001ce00: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+0001ce10: 726e 616c 5479 7065 223a 2263 6f6e 7472  rnalType":"contr
+0001ce20: 6163 7420 494c 4254 6f6b 656e 222c 226e  act ILBToken","n
+0001ce30: 616d 6522 3a22 5f6c 6254 6f6b 656e 222c  ame":"_lbToken",
+0001ce40: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0001ce50: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001ce60: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0001ce70: 6522 3a22 5f74 6f22 2c22 7479 7065 223a  e":"_to","type":
+0001ce80: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+0001ce90: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001cea0: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
+0001ceb0: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
+0001cec0: 7432 3536 5b5d 227d 2c7b 2269 6e74 6572  t256[]"},{"inter
+0001ced0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001cee0: 365b 5d22 2c22 6e61 6d65 223a 225f 616d  6[]","name":"_am
+0001cef0: 6f75 6e74 7322 2c22 7479 7065 223a 2275  ounts","type":"u
+0001cf00: 696e 7432 3536 5b5d 227d 5d2c 226e 616d  int256[]"}],"nam
+0001cf10: 6522 3a22 7377 6565 704c 4254 6f6b 656e  e":"sweepLBToken
+0001cf20: 222c 226f 7574 7075 7473 223a 5b5d 2c22  ","outputs":[],"
+0001cf30: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+0001cf40: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+0001cf50: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+0001cf60: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+0001cf70: 616d 6522 3a22 7761 7661 7822 2c22 6f75  ame":"wavax","ou
+0001cf80: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
+0001cf90: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+0001cfa0: 7420 4957 4156 4158 222c 226e 616d 6522  t IWAVAX","name"
+0001cfb0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
+0001cfc0: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
+0001cfd0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+0001cfe0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+0001cff0: 227d 2c7b 2273 7461 7465 4d75 7461 6269  "},{"stateMutabi
+0001d000: 6c69 7479 223a 2270 6179 6162 6c65 222c  lity":"payable",
+0001d010: 2274 7970 6522 3a22 7265 6365 6976 6522  "type":"receive"
+0001d020: 7d5d 2729 0a0a 2020 2020 6465 6620 6765  }]')..    def ge
+0001d030: 745f 6964 5f66 726f 6d5f 7072 6963 6528  t_id_from_price(
+0001d040: 5f77 6562 333a 5765 6233 2c5f 726f 7574  _web3:Web3,_rout
+0001d050: 655f 6164 6472 6573 733a 7374 722c 5f72  e_address:str,_r
+0001d060: 6f75 7465 5f61 6269 2c5f 6c62 5f70 6169  oute_abi,_lb_pai
+0001d070: 722c 5f70 7269 6365 293a 0a20 2020 2020  r,_price):.     
+0001d080: 2020 2072 6574 7572 6e20 5f77 6562 332e     return _web3.
+0001d090: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
+0001d0a0: 7265 7373 3d5f 726f 7574 655f 6164 6472  ress=_route_addr
+0001d0b0: 6573 732c 2061 6269 3d5f 726f 7574 655f  ess, abi=_route_
+0001d0c0: 6162 6929 2e66 756e 6374 696f 6e73 2e67  abi).functions.g
+0001d0d0: 6574 4964 4672 6f6d 5072 6963 6528 5f6c  etIdFromPrice(_l
+0001d0e0: 625f 7061 6972 2c5f 7072 6963 6529 2e63  b_pair,_price).c
+0001d0f0: 616c 6c28 290a 0a20 2020 2064 6566 2067  all()..    def g
+0001d100: 6574 5f70 7269 6365 5f66 726f 6d5f 6964  et_price_from_id
+0001d110: 285f 7765 6233 3a57 6562 332c 5f72 6f75  (_web3:Web3,_rou
+0001d120: 7465 5f61 6464 7265 7373 3a73 7472 2c5f  te_address:str,_
+0001d130: 726f 7574 655f 6162 692c 5f6c 625f 7061  route_abi,_lb_pa
+0001d140: 6972 2c5f 6964 293a 0a20 2020 2020 2020  ir,_id):.       
+0001d150: 2072 6574 7572 6e20 5f77 6562 332e 6574   return _web3.et
+0001d160: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
+0001d170: 7373 3d5f 726f 7574 655f 6164 6472 6573  ss=_route_addres
+0001d180: 732c 2061 6269 3d5f 726f 7574 655f 6162  s, abi=_route_ab
+0001d190: 6929 2e66 756e 6374 696f 6e73 2e67 6574  i).functions.get
+0001d1a0: 5072 6963 6546 726f 6d49 6428 5f6c 625f  PriceFromId(_lb_
+0001d1b0: 7061 6972 2c5f 6964 292e 6361 6c6c 2829  pair,_id).call()
+0001d1c0: 0a0a 2020 2020 2372 6574 7572 6e20 5b61  ..    #return [a
+0001d1d0: 6d6f 756e 745f 696e 2c66 6565 5d0a 2020  mount_in,fee].  
+0001d1e0: 2020 6465 6620 6765 745f 7377 6170 5f69    def get_swap_i
+0001d1f0: 6e28 5f77 6562 333a 5765 6233 2c5f 726f  n(_web3:Web3,_ro
+0001d200: 7574 655f 6164 6472 6573 733a 7374 722c  ute_address:str,
+0001d210: 5f72 6f75 7465 5f61 6269 3a73 7472 2c5f  _route_abi:str,_
+0001d220: 6c62 5f70 6169 722c 5f61 6d6f 756e 745f  lb_pair,_amount_
+0001d230: 6f75 742c 5f73 7761 705f 666f 725f 793a  out,_swap_for_y:
+0001d240: 626f 6f6c 293a 0a20 2020 2020 2020 2072  bool):.        r
+0001d250: 6574 7572 6e20 5f77 6562 332e 6574 682e  eturn _web3.eth.
+0001d260: 636f 6e74 7261 6374 2861 6464 7265 7373  contract(address
+0001d270: 3d5f 726f 7574 655f 6164 6472 6573 732c  =_route_address,
+0001d280: 2061 6269 3d5f 726f 7574 655f 6162 6929   abi=_route_abi)
+0001d290: 2e66 756e 6374 696f 6e73 2e67 6574 5377  .functions.getSw
+0001d2a0: 6170 496e 285f 6c62 5f70 6169 722c 5f61  apIn(_lb_pair,_a
+0001d2b0: 6d6f 756e 745f 6f75 742c 5f73 7761 705f  mount_out,_swap_
+0001d2c0: 666f 725f 7929 2e63 616c 6c28 290a 2020  for_y).call().  
+0001d2d0: 2020 0a20 2020 2023 7265 7475 726e 205b    .    #return [
+0001d2e0: 616d 6f75 6e74 5f6f 7574 2c66 6565 5d0a  amount_out,fee].
+0001d2f0: 2020 2020 6465 6620 6765 745f 7377 6170      def get_swap
+0001d300: 5f6f 7574 285f 7765 6233 3a57 6562 332c  _out(_web3:Web3,
+0001d310: 5f72 6f75 7465 5f61 6464 7265 7373 3a73  _route_address:s
+0001d320: 7472 2c5f 726f 7574 655f 6162 693a 7374  tr,_route_abi:st
+0001d330: 722c 5f6c 625f 7061 6972 2c5f 616d 6f75  r,_lb_pair,_amou
+0001d340: 6e74 5f69 6e2c 5f73 7761 705f 666f 725f  nt_in,_swap_for_
+0001d350: 793a 626f 6f6c 293a 0a20 2020 2020 2020  y:bool):.       
+0001d360: 2072 6574 7572 6e20 5f77 6562 332e 6574   return _web3.et
+0001d370: 682e 636f 6e74 7261 6374 2861 6464 7265  h.contract(addre
+0001d380: 7373 3d5f 726f 7574 655f 6164 6472 6573  ss=_route_addres
+0001d390: 732c 2061 6269 3d5f 726f 7574 655f 6162  s, abi=_route_ab
+0001d3a0: 6929 2e66 756e 6374 696f 6e73 2e67 6574  i).functions.get
+0001d3b0: 5377 6170 4f75 7428 5f6c 625f 7061 6972  SwapOut(_lb_pair
+0001d3c0: 2c5f 616d 6f75 6e74 5f69 6e2c 5f73 7761  ,_amount_in,_swa
+0001d3d0: 705f 666f 725f 7929 2e63 616c 6c28 290a  p_for_y).call().
+0001d3e0: 0a20 2020 2064 6566 2073 7761 705f 6578  .    def swap_ex
+0001d3f0: 6163 745f 746f 6b65 6e73 5f66 6f72 5f74  act_tokens_for_t
+0001d400: 6f6b 656e 7328 5f77 6562 333a 5765 6233  okens(_web3:Web3
+0001d410: 2c5f 726f 7574 655f 6164 6472 6573 733a  ,_route_address:
+0001d420: 7374 722c 5f72 6f75 7465 5f61 6269 2c0a  str,_route_abi,.
+0001d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d450: 2020 2020 205f 616d 6f75 6e74 5f69 6e2c       _amount_in,
+0001d460: 5f61 6d6f 756e 745f 6f75 745f 6d69 6e2c  _amount_out_min,
+0001d470: 5f70 6169 725f 6269 6e5f 7374 6570 732c  _pair_bin_steps,
+0001d480: 5f74 6f6b 656e 5f70 6174 682c 5f74 6f2c  _token_path,_to,
+0001d490: 5f64 6561 646c 696e 652c 0a20 2020 2020  _deadline,.     
+0001d4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d4c0: 5f70 7562 6c69 635f 6b65 792c 5f70 7269  _public_key,_pri
+0001d4d0: 7661 7465 5f6b 6579 293a 0a20 2020 2020  vate_key):.     
+0001d4e0: 2020 206e 6f6e 6365 3d5f 7765 6233 2e65     nonce=_web3.e
+0001d4f0: 7468 2e67 6574 5f74 7261 6e73 6163 7469  th.get_transacti
+0001d500: 6f6e 5f63 6f75 6e74 285f 7075 626c 6963  on_count(_public
+0001d510: 5f6b 6579 290a 2020 2020 2020 2020 726f  _key).        ro
+0001d520: 7574 655f 636f 6e74 7261 6374 3d5f 7765  ute_contract=_we
+0001d530: 6233 2e65 7468 2e63 6f6e 7472 6163 7428  b3.eth.contract(
+0001d540: 6164 6472 6573 733d 5f72 6f75 7465 5f61  address=_route_a
+0001d550: 6464 7265 7373 2c20 6162 693d 5f72 6f75  ddress, abi=_rou
+0001d560: 7465 5f61 6269 290a 2020 2020 2020 2020  te_abi).        
+0001d570: 7377 6170 5f66 756e 6374 696f 6e3d 726f  swap_function=ro
+0001d580: 7574 655f 636f 6e74 7261 6374 2e66 756e  ute_contract.fun
+0001d590: 6374 696f 6e73 2e73 7761 7045 7861 6374  ctions.swapExact
+0001d5a0: 546f 6b65 6e73 466f 7254 6f6b 656e 7328  TokensForTokens(
+0001d5b0: 5f61 6d6f 756e 745f 696e 2c5f 616d 6f75  _amount_in,_amou
+0001d5c0: 6e74 5f6f 7574 5f6d 696e 2c5f 7061 6972  nt_out_min,_pair
+0001d5d0: 5f62 696e 5f73 7465 7073 2c5f 746f 6b65  _bin_steps,_toke
+0001d5e0: 6e5f 7061 7468 2c5f 746f 2c5f 6465 6164  n_path,_to,_dead
+0001d5f0: 6c69 6e65 290a 2020 2020 2020 2020 7061  line).        pa
+0001d600: 7261 6d73 3d7b 0a20 2020 2020 2020 2020  rams={.         
+0001d610: 2020 2027 6672 6f6d 273a 205f 7075 626c     'from': _publ
+0001d620: 6963 5f6b 6579 2c0a 2020 2020 2020 2020  ic_key,.        
+0001d630: 2020 2020 2776 616c 7565 273a 2030 2c0a      'value': 0,.
+0001d640: 2020 2020 2020 2020 2020 2020 276e 6f6e              'non
+0001d650: 6365 273a 206e 6f6e 6365 2c0a 2020 2020  ce': nonce,.    
+0001d660: 2020 2020 2020 2020 2774 7970 6527 3a20          'type': 
+0001d670: 2730 7832 270a 2020 2020 2020 2020 7d0a  '0x2'.        }.
+0001d680: 2020 2020 2020 2020 7369 676e 6564 5f74          signed_t
+0001d690: 7261 6e73 6163 7469 6f6e 3d5f 7765 6233  ransaction=_web3
+0001d6a0: 2e65 7468 2e61 6363 6f75 6e74 2e73 6967  .eth.account.sig
+0001d6b0: 6e5f 7472 616e 7361 6374 696f 6e28 7377  n_transaction(sw
+0001d6c0: 6170 5f66 756e 6374 696f 6e2e 6275 696c  ap_function.buil
+0001d6d0: 6454 7261 6e73 6163 7469 6f6e 2870 6172  dTransaction(par
+0001d6e0: 616d 7329 2c70 7269 7661 7465 5f6b 6579  ams),private_key
+0001d6f0: 3d5f 7072 6976 6174 655f 6b65 7929 0a20  =_private_key). 
+0001d700: 2020 2020 2020 2072 6573 706f 6e73 653d         response=
+0001d710: 5f77 6562 332e 6574 682e 7365 6e64 5f72  _web3.eth.send_r
+0001d720: 6177 5f74 7261 6e73 6163 7469 6f6e 2873  aw_transaction(s
+0001d730: 6967 6e65 645f 7472 616e 7361 6374 696f  igned_transactio
+0001d740: 6e2e 7261 7754 7261 6e73 6163 7469 6f6e  n.rawTransaction
+0001d750: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+0001d760: 2057 6562 332e 746f 4865 7828 7265 7370   Web3.toHex(resp
+0001d770: 6f6e 7365 290a 2020 2020 0a20 2020 2064  onse).    .    d
+0001d780: 6566 2073 7761 705f 746f 6b65 6e73 5f66  ef swap_tokens_f
+0001d790: 6f72 5f65 7861 6374 5f74 6f6b 656e 7328  or_exact_tokens(
+0001d7a0: 5f77 6562 333a 5765 6233 2c5f 726f 7574  _web3:Web3,_rout
+0001d7b0: 655f 6164 6472 6573 733a 7374 722c 5f72  e_address:str,_r
+0001d7c0: 6f75 7465 5f61 6269 2c0a 2020 2020 2020  oute_abi,.      
+0001d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d7e0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+0001d7f0: 616d 6f75 6e74 5f6f 7574 2c5f 616d 6f75  amount_out,_amou
+0001d800: 6e74 5f69 6e5f 6d61 782c 5f70 6169 725f  nt_in_max,_pair_
+0001d810: 6269 6e5f 7374 6570 732c 5f74 6f6b 656e  bin_steps,_token
+0001d820: 5f70 6174 682c 5f74 6f2c 5f64 6561 646c  _path,_to,_deadl
+0001d830: 696e 652c 0a20 2020 2020 2020 2020 2020  ine,.           
+0001d840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d850: 2020 2020 2020 2020 2020 5f70 7562 6c69            _publi
+0001d860: 635f 6b65 792c 5f70 7269 7661 7465 5f6b  c_key,_private_k
+0001d870: 6579 293a 0a20 2020 2020 2020 206e 6f6e  ey):.        non
+0001d880: 6365 3d5f 7765 6233 2e65 7468 2e67 6574  ce=_web3.eth.get
+0001d890: 5f74 7261 6e73 6163 7469 6f6e 5f63 6f75  _transaction_cou
+0001d8a0: 6e74 285f 7075 626c 6963 5f6b 6579 290a  nt(_public_key).
+0001d8b0: 2020 2020 2020 2020 726f 7574 655f 636f          route_co
+0001d8c0: 6e74 7261 6374 3d5f 7765 6233 2e65 7468  ntract=_web3.eth
+0001d8d0: 2e63 6f6e 7472 6163 7428 6164 6472 6573  .contract(addres
+0001d8e0: 733d 5f72 6f75 7465 5f61 6464 7265 7373  s=_route_address
+0001d8f0: 2c20 6162 693d 5f72 6f75 7465 5f61 6269  , abi=_route_abi
+0001d900: 290a 2020 2020 2020 2020 7377 6170 5f66  ).        swap_f
+0001d910: 756e 6374 696f 6e3d 726f 7574 655f 636f  unction=route_co
+0001d920: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
+0001d930: 2e73 7761 7054 6f6b 656e 7346 6f72 4578  .swapTokensForEx
+0001d940: 6163 7454 6f6b 656e 7328 5f61 6d6f 756e  actTokens(_amoun
+0001d950: 745f 6f75 742c 5f61 6d6f 756e 745f 696e  t_out,_amount_in
+0001d960: 5f6d 6178 2c5f 7061 6972 5f62 696e 5f73  _max,_pair_bin_s
+0001d970: 7465 7073 2c5f 746f 6b65 6e5f 7061 7468  teps,_token_path
+0001d980: 2c5f 746f 2c5f 6465 6164 6c69 6e65 290a  ,_to,_deadline).
+0001d990: 2020 2020 2020 2020 7061 7261 6d73 3d7b          params={
+0001d9a0: 0a20 2020 2020 2020 2020 2020 2027 6672  .            'fr
+0001d9b0: 6f6d 273a 205f 7075 626c 6963 5f6b 6579  om': _public_key
+0001d9c0: 2c0a 2020 2020 2020 2020 2020 2020 2776  ,.            'v
+0001d9d0: 616c 7565 273a 2030 2c0a 2020 2020 2020  alue': 0,.      
+0001d9e0: 2020 2020 2020 276e 6f6e 6365 273a 206e        'nonce': n
+0001d9f0: 6f6e 6365 2c0a 2020 2020 2020 2020 2020  once,.          
+0001da00: 2020 2774 7970 6527 3a20 2730 7832 270a    'type': '0x2'.
+0001da10: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+0001da20: 2020 7369 676e 6564 5f74 7261 6e73 6163    signed_transac
+0001da30: 7469 6f6e 3d5f 7765 6233 2e65 7468 2e61  tion=_web3.eth.a
+0001da40: 6363 6f75 6e74 2e73 6967 6e5f 7472 616e  ccount.sign_tran
+0001da50: 7361 6374 696f 6e28 7377 6170 5f66 756e  saction(swap_fun
+0001da60: 6374 696f 6e2e 6275 696c 6454 7261 6e73  ction.buildTrans
+0001da70: 6163 7469 6f6e 2870 6172 616d 7329 2c70  action(params),p
+0001da80: 7269 7661 7465 5f6b 6579 3d5f 7072 6976  rivate_key=_priv
+0001da90: 6174 655f 6b65 7929 0a20 2020 2020 2020  ate_key).       
+0001daa0: 2072 6573 706f 6e73 653d 5f77 6562 332e   response=_web3.
+0001dab0: 6574 682e 7365 6e64 5f72 6177 5f74 7261  eth.send_raw_tra
+0001dac0: 6e73 6163 7469 6f6e 2873 6967 6e65 645f  nsaction(signed_
+0001dad0: 7472 616e 7361 6374 696f 6e2e 7261 7754  transaction.rawT
+0001dae0: 7261 6e73 6163 7469 6f6e 290a 2020 2020  ransaction).    
+0001daf0: 2020 2020 7265 7475 726e 2057 6562 332e      return Web3.
+0001db00: 746f 4865 7828 7265 7370 6f6e 7365 290a  toHex(response).
+0001db10: 0a63 6c61 7373 204a 6f65 5632 5061 6972  .class JoeV2Pair
+0001db20: 3a0a 0a20 2020 206a 6f65 5f70 6169 725f  :..    joe_pair_
+0001db30: 7632 5f61 6269 3d6a 736f 6e2e 6c6f 6164  v2_abi=json.load
+0001db40: 7328 275b 7b22 696e 7075 7473 223a 5b7b  s('[{"inputs":[{
+0001db50: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001db60: 636f 6e74 7261 6374 2049 4c42 4661 6374  contract ILBFact
+0001db70: 6f72 7922 2c22 6e61 6d65 223a 225f 6661  ory","name":"_fa
+0001db80: 6374 6f72 7922 2c22 7479 7065 223a 2261  ctory","type":"a
+0001db90: 6464 7265 7373 227d 5d2c 2273 7461 7465  ddress"}],"state
+0001dba0: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+0001dbb0: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+0001dbc0: 2263 6f6e 7374 7275 6374 6f72 227d 2c7b  "constructor"},{
+0001dbd0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+0001dbe0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001dbf0: 3536 222c 226e 616d 6522 3a22 6270 222c  56","name":"bp",
+0001dc00: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001dc10: 7d5d 2c22 6e61 6d65 223a 2242 696e 4865  }],"name":"BinHe
+0001dc20: 6c70 6572 5f5f 4269 6e53 7465 704f 7665  lper__BinStepOve
+0001dc30: 7266 6c6f 7773 222c 2274 7970 6522 3a22  rflows","type":"
+0001dc40: 6572 726f 7222 7d2c 7b22 696e 7075 7473  error"},{"inputs
+0001dc50: 223a 5b5d 2c22 6e61 6d65 223a 2242 696e  ":[],"name":"Bin
+0001dc60: 4865 6c70 6572 5f5f 4964 4f76 6572 666c  Helper__IdOverfl
+0001dc70: 6f77 7322 2c22 7479 7065 223a 2265 7272  ows","type":"err
+0001dc80: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0001dc90: 5d2c 226e 616d 6522 3a22 4c42 5061 6972  ],"name":"LBPair
+0001dca0: 5f5f 4164 6472 6573 735a 6572 6f22 2c22  __AddressZero","
+0001dcb0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+0001dcc0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+0001dcd0: 6522 3a22 4c42 5061 6972 5f5f 4164 6472  e":"LBPair__Addr
+0001dce0: 6573 735a 6572 6f4f 7254 6869 7322 2c22  essZeroOrThis","
+0001dcf0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+0001dd00: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+0001dd10: 6522 3a22 4c42 5061 6972 5f5f 416c 7265  e":"LBPair__Alre
+0001dd20: 6164 7949 6e69 7469 616c 697a 6564 222c  adyInitialized",
+0001dd30: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+0001dd40: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0001dd50: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001dd60: 3235 3622 2c22 6e61 6d65 223a 2269 6422  256","name":"id"
+0001dd70: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001dd80: 227d 5d2c 226e 616d 6522 3a22 4c42 5061  "}],"name":"LBPa
+0001dd90: 6972 5f5f 436f 6d70 6f73 6974 696f 6e46  ir__CompositionF
+0001dda0: 6163 746f 7246 6c61 7765 6422 2c22 7479  actorFlawed","ty
+0001ddb0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+0001ddc0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0001ddd0: 3a22 4c42 5061 6972 5f5f 4469 7374 7269  :"LBPair__Distri
+0001dde0: 6275 7469 6f6e 734f 7665 7266 6c6f 7722  butionsOverflow"
+0001ddf0: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+0001de00: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+0001de10: 616d 6522 3a22 4c42 5061 6972 5f5f 466c  ame":"LBPair__Fl
+0001de20: 6173 684c 6f61 6e43 616c 6c62 6163 6b46  ashLoanCallbackF
+0001de30: 6169 6c65 6422 2c22 7479 7065 223a 2265  ailed","type":"e
+0001de40: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+0001de50: 3a5b 5d2c 226e 616d 6522 3a22 4c42 5061  :[],"name":"LBPa
+0001de60: 6972 5f5f 466c 6173 684c 6f61 6e49 6e76  ir__FlashLoanInv
+0001de70: 616c 6964 4261 6c61 6e63 6522 2c22 7479  alidBalance","ty
+0001de80: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+0001de90: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0001dea0: 3a22 4c42 5061 6972 5f5f 466c 6173 684c  :"LBPair__FlashL
+0001deb0: 6f61 6e49 6e76 616c 6964 546f 6b65 6e22  oanInvalidToken"
+0001dec0: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+0001ded0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+0001dee0: 616d 6522 3a22 4c42 5061 6972 5f5f 496e  ame":"LBPair__In
+0001def0: 7375 6666 6963 6965 6e74 416d 6f75 6e74  sufficientAmount
+0001df00: 7322 2c22 7479 7065 223a 2265 7272 6f72  s","type":"error
+0001df10: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+0001df20: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001df30: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001df40: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
+0001df50: 3235 3622 7d5d 2c22 6e61 6d65 223a 224c  256"}],"name":"L
+0001df60: 4250 6169 725f 5f49 6e73 7566 6669 6369  BPair__Insuffici
+0001df70: 656e 744c 6971 7569 6469 7479 4275 726e  entLiquidityBurn
+0001df80: 6564 222c 2274 7970 6522 3a22 6572 726f  ed","type":"erro
+0001df90: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
+0001dfa0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001dfb0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001dfc0: 2269 6422 2c22 7479 7065 223a 2275 696e  "id","type":"uin
+0001dfd0: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+0001dfe0: 4c42 5061 6972 5f5f 496e 7375 6666 6963  LBPair__Insuffic
+0001dff0: 6965 6e74 4c69 7175 6964 6974 794d 696e  ientLiquidityMin
+0001e000: 7465 6422 2c22 7479 7065 223a 2265 7272  ted","type":"err
+0001e010: 6f72 227d 2c7b 2269 6e70 7574 7322 3a5b  or"},{"inputs":[
+0001e020: 5d2c 226e 616d 6522 3a22 4c42 5061 6972  ],"name":"LBPair
+0001e030: 5f5f 4f6e 6c79 4661 6374 6f72 7922 2c22  __OnlyFactory","
+0001e040: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+0001e050: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+0001e060: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0001e070: 7373 222c 226e 616d 6522 3a22 6665 6552  ss","name":"feeR
+0001e080: 6563 6970 6965 6e74 222c 2274 7970 6522  ecipient","type"
+0001e090: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001e0a0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0001e0b0: 7265 7373 222c 226e 616d 6522 3a22 7365  ress","name":"se
+0001e0c0: 6e64 6572 222c 2274 7970 6522 3a22 6164  nder","type":"ad
+0001e0d0: 6472 6573 7322 7d5d 2c22 6e61 6d65 223a  dress"}],"name":
+0001e0e0: 224c 4250 6169 725f 5f4f 6e6c 7946 6565  "LBPair__OnlyFee
+0001e0f0: 5265 6369 7069 656e 7422 2c22 7479 7065  Recipient","type
+0001e100: 223a 2265 7272 6f72 227d 2c7b 2269 6e70  ":"error"},{"inp
+0001e110: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+0001e120: 4c42 5061 6972 5f5f 4f6e 6c79 5374 7269  LBPair__OnlyStri
+0001e130: 6374 6c79 496e 6372 6561 7369 6e67 4964  ctlyIncreasingId
+0001e140: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001e150: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0001e160: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001e170: 6e74 3235 3622 2c22 6e61 6d65 223a 226e  nt256","name":"n
+0001e180: 6577 5369 7a65 222c 2274 7970 6522 3a22  ewSize","type":"
+0001e190: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0001e1a0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001e1b0: 3536 222c 226e 616d 6522 3a22 6f72 6163  56","name":"orac
+0001e1c0: 6c65 5369 7a65 222c 2274 7970 6522 3a22  leSize","type":"
+0001e1d0: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+0001e1e0: 223a 224c 4250 6169 725f 5f4f 7261 636c  ":"LBPair__Oracl
+0001e1f0: 654e 6577 5369 7a65 546f 6f53 6d61 6c6c  eNewSizeTooSmall
+0001e200: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001e210: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+0001e220: 6e61 6d65 223a 224c 4250 6169 725f 5f57  name":"LBPair__W
+0001e230: 726f 6e67 4c65 6e67 7468 7322 2c22 7479  rongLengths","ty
+0001e240: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+0001e250: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+0001e260: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+0001e270: 222c 226e 616d 6522 3a22 6672 6f6d 222c  ","name":"from",
+0001e280: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+0001e290: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001e2a0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001e2b0: 6522 3a22 6964 222c 2274 7970 6522 3a22  e":"id","type":"
+0001e2c0: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+0001e2d0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001e2e0: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+0001e2f0: 6e74 222c 2274 7970 6522 3a22 7569 6e74  nt","type":"uint
+0001e300: 3235 3622 7d5d 2c22 6e61 6d65 223a 224c  256"}],"name":"L
+0001e310: 4254 6f6b 656e 5f5f 4275 726e 4578 6365  BToken__BurnExce
+0001e320: 6564 7342 616c 616e 6365 222c 2274 7970  edsBalance","typ
+0001e330: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+0001e340: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+0001e350: 224c 4254 6f6b 656e 5f5f 4275 726e 4672  "LBToken__BurnFr
+0001e360: 6f6d 4164 6472 6573 7330 222c 2274 7970  omAddress0","typ
+0001e370: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+0001e380: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001e390: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001e3a0: 2c22 6e61 6d65 223a 2261 6363 6f75 6e74  ,"name":"account
+0001e3b0: 734c 656e 6774 6822 2c22 7479 7065 223a  sLength","type":
+0001e3c0: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+0001e3d0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001e3e0: 3235 3622 2c22 6e61 6d65 223a 2269 6473  256","name":"ids
+0001e3f0: 4c65 6e67 7468 222c 2274 7970 6522 3a22  Length","type":"
+0001e400: 7569 6e74 3235 3622 7d5d 2c22 6e61 6d65  uint256"}],"name
+0001e410: 223a 224c 4254 6f6b 656e 5f5f 4c65 6e67  ":"LBToken__Leng
+0001e420: 7468 4d69 736d 6174 6368 222c 2274 7970  thMismatch","typ
+0001e430: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+0001e440: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+0001e450: 224c 4254 6f6b 656e 5f5f 4d69 6e74 546f  "LBToken__MintTo
+0001e460: 4164 6472 6573 7330 222c 2274 7970 6522  Address0","type"
+0001e470: 3a22 6572 726f 7222 7d2c 7b22 696e 7075  :"error"},{"inpu
+0001e480: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+0001e490: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0001e4a0: 6e61 6d65 223a 226f 776e 6572 222c 2274  name":"owner","t
+0001e4b0: 7970 6522 3a22 6164 6472 6573 7322 7d5d  ype":"address"}]
+0001e4c0: 2c22 6e61 6d65 223a 224c 4254 6f6b 656e  ,"name":"LBToken
+0001e4d0: 5f5f 5365 6c66 4170 7072 6f76 616c 222c  __SelfApproval",
+0001e4e0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+0001e4f0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0001e500: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0001e510: 6573 7322 2c22 6e61 6d65 223a 226f 776e  ess","name":"own
+0001e520: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
+0001e530: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+0001e540: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+0001e550: 226e 616d 6522 3a22 7370 656e 6465 7222  "name":"spender"
+0001e560: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001e570: 227d 5d2c 226e 616d 6522 3a22 4c42 546f  "}],"name":"LBTo
+0001e580: 6b65 6e5f 5f53 7065 6e64 6572 4e6f 7441  ken__SpenderNotA
+0001e590: 7070 726f 7665 6422 2c22 7479 7065 223a  pproved","type":
+0001e5a0: 2265 7272 6f72 227d 2c7b 2269 6e70 7574  "error"},{"input
+0001e5b0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+0001e5c0: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+0001e5d0: 616d 6522 3a22 6672 6f6d 222c 2274 7970  ame":"from","typ
+0001e5e0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+0001e5f0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001e600: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001e610: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
+0001e620: 3235 3622 7d2c 7b22 696e 7465 726e 616c  256"},{"internal
+0001e630: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001e640: 226e 616d 6522 3a22 616d 6f75 6e74 222c  "name":"amount",
+0001e650: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001e660: 7d5d 2c22 6e61 6d65 223a 224c 4254 6f6b  }],"name":"LBTok
+0001e670: 656e 5f5f 5472 616e 7366 6572 4578 6365  en__TransferExce
+0001e680: 6564 7342 616c 616e 6365 222c 2274 7970  edsBalance","typ
+0001e690: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+0001e6a0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+0001e6b0: 224c 4254 6f6b 656e 5f5f 5472 616e 7366  "LBToken__Transf
+0001e6c0: 6572 4672 6f6d 4f72 546f 4164 6472 6573  erFromOrToAddres
+0001e6d0: 7330 222c 2274 7970 6522 3a22 6572 726f  s0","type":"erro
+0001e6e0: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
+0001e6f0: 2c22 6e61 6d65 223a 224c 4254 6f6b 656e  ,"name":"LBToken
+0001e700: 5f5f 5472 616e 7366 6572 546f 5365 6c66  __TransferToSelf
+0001e710: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001e720: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0001e730: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001e740: 6e74 3235 3622 2c22 6e61 6d65 223a 2278  nt256","name":"x
+0001e750: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001e760: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+0001e770: 7065 223a 2269 6e74 3235 3622 2c22 6e61  pe":"int256","na
+0001e780: 6d65 223a 2279 222c 2274 7970 6522 3a22  me":"y","type":"
+0001e790: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+0001e7a0: 3a22 4d61 7468 3132 3878 3132 385f 5f50  :"Math128x128__P
+0001e7b0: 6f77 6572 556e 6465 7266 6c6f 7722 2c22  owerUnderflow","
+0001e7c0: 7479 7065 223a 2265 7272 6f72 227d 2c7b  type":"error"},{
+0001e7d0: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+0001e7e0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001e7f0: 3536 222c 226e 616d 6522 3a22 7072 6f64  56","name":"prod
+0001e800: 3122 2c22 7479 7065 223a 2275 696e 7432  1","type":"uint2
+0001e810: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+0001e820: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+0001e830: 6e61 6d65 223a 2264 656e 6f6d 696e 6174  name":"denominat
+0001e840: 6f72 222c 2274 7970 6522 3a22 7569 6e74  or","type":"uint
+0001e850: 3235 3622 7d5d 2c22 6e61 6d65 223a 224d  256"}],"name":"M
+0001e860: 6174 6835 3132 4269 7473 5f5f 4d75 6c44  ath512Bits__MulD
+0001e870: 6976 4f76 6572 666c 6f77 222c 2274 7970  ivOverflow","typ
+0001e880: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+0001e890: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001e8a0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001e8b0: 2c22 6e61 6d65 223a 2270 726f 6431 222c  ,"name":"prod1",
+0001e8c0: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001e8d0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001e8e0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001e8f0: 6522 3a22 6f66 6673 6574 222c 2274 7970  e":"offset","typ
+0001e900: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+0001e910: 6e61 6d65 223a 224d 6174 6835 3132 4269  name":"Math512Bi
+0001e920: 7473 5f5f 4d75 6c53 6869 6674 4f76 6572  ts__MulShiftOver
+0001e930: 666c 6f77 222c 2274 7970 6522 3a22 6572  flow","type":"er
+0001e940: 726f 7222 7d2c 7b22 696e 7075 7473 223a  ror"},{"inputs":
+0001e950: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+0001e960: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001e970: 223a 226f 6666 7365 7422 2c22 7479 7065  ":"offset","type
+0001e980: 223a 2275 696e 7432 3536 227d 5d2c 226e  ":"uint256"}],"n
+0001e990: 616d 6522 3a22 4d61 7468 3531 3242 6974  ame":"Math512Bit
+0001e9a0: 735f 5f4f 6666 7365 744f 7665 7266 6c6f  s__OffsetOverflo
+0001e9b0: 7773 222c 2274 7970 6522 3a22 6572 726f  ws","type":"erro
+0001e9c0: 7222 7d2c 7b22 696e 7075 7473 223a 5b7b  r"},{"inputs":[{
+0001e9d0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001e9e0: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001e9f0: 225f 6d69 6e54 696d 6573 7461 6d70 222c  "_minTimestamp",
+0001ea00: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001ea10: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+0001ea20: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001ea30: 6522 3a22 5f6c 6f6f 6b55 7054 696d 6573  e":"_lookUpTimes
+0001ea40: 7461 6d70 222c 2274 7970 6522 3a22 7569  tamp","type":"ui
+0001ea50: 6e74 3235 3622 7d5d 2c22 6e61 6d65 223a  nt256"}],"name":
+0001ea60: 224f 7261 636c 655f 5f4c 6f6f 6b55 7054  "Oracle__LookUpT
+0001ea70: 696d 6573 7461 6d70 546f 6f4f 6c64 222c  imestampTooOld",
+0001ea80: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+0001ea90: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
+0001eaa0: 6d65 223a 224f 7261 636c 655f 5f4e 6f74  me":"Oracle__Not
+0001eab0: 496e 6974 6961 6c69 7a65 6422 2c22 7479  Initialized","ty
+0001eac0: 7065 223a 2265 7272 6f72 227d 2c7b 2269  pe":"error"},{"i
+0001ead0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+0001eae0: 3a22 5265 656e 7472 616e 6379 4775 6172  :"ReentrancyGuar
+0001eaf0: 6455 7067 7261 6465 6162 6c65 5f5f 416c  dUpgradeable__Al
+0001eb00: 7265 6164 7949 6e69 7469 616c 697a 6564  readyInitialized
+0001eb10: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001eb20: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+0001eb30: 6e61 6d65 223a 2252 6565 6e74 7261 6e63  name":"Reentranc
+0001eb40: 7947 7561 7264 5570 6772 6164 6561 626c  yGuardUpgradeabl
+0001eb50: 655f 5f52 6565 6e74 7261 6e74 4361 6c6c  e__ReentrantCall
+0001eb60: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001eb70: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+0001eb80: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+0001eb90: 6e74 3235 3622 2c22 6e61 6d65 223a 2278  nt256","name":"x
+0001eba0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001ebb0: 3622 7d5d 2c22 6e61 6d65 223a 2253 6166  6"}],"name":"Saf
+0001ebc0: 6543 6173 745f 5f45 7863 6565 6473 3131  eCast__Exceeds11
+0001ebd0: 3242 6974 7322 2c22 7479 7065 223a 2265  2Bits","type":"e
+0001ebe0: 7272 6f72 227d 2c7b 2269 6e70 7574 7322  rror"},{"inputs"
+0001ebf0: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+0001ec00: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001ec10: 6522 3a22 7822 2c22 7479 7065 223a 2275  e":"x","type":"u
+0001ec20: 696e 7432 3536 227d 5d2c 226e 616d 6522  int256"}],"name"
+0001ec30: 3a22 5361 6665 4361 7374 5f5f 4578 6365  :"SafeCast__Exce
+0001ec40: 6564 7331 3238 4269 7473 222c 2274 7970  eds128Bits","typ
+0001ec50: 6522 3a22 6572 726f 7222 7d2c 7b22 696e  e":"error"},{"in
+0001ec60: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+0001ec70: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001ec80: 2c22 6e61 6d65 223a 2278 222c 2274 7970  ,"name":"x","typ
+0001ec90: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+0001eca0: 6e61 6d65 223a 2253 6166 6543 6173 745f  name":"SafeCast_
+0001ecb0: 5f45 7863 6565 6473 3234 4269 7473 222c  _Exceeds24Bits",
+0001ecc0: 2274 7970 6522 3a22 6572 726f 7222 7d2c  "type":"error"},
+0001ecd0: 7b22 696e 7075 7473 223a 5b7b 2269 6e74  {"inputs":[{"int
+0001ece0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001ecf0: 3235 3622 2c22 6e61 6d65 223a 2278 222c  256","name":"x",
+0001ed00: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001ed10: 7d5d 2c22 6e61 6d65 223a 2253 6166 6543  }],"name":"SafeC
+0001ed20: 6173 745f 5f45 7863 6565 6473 3430 4269  ast__Exceeds40Bi
+0001ed30: 7473 222c 2274 7970 6522 3a22 6572 726f  ts","type":"erro
+0001ed40: 7222 7d2c 7b22 696e 7075 7473 223a 5b5d  r"},{"inputs":[]
+0001ed50: 2c22 6e61 6d65 223a 2254 6f6b 656e 4865  ,"name":"TokenHe
+0001ed60: 6c70 6572 5f5f 4361 6c6c 4661 696c 6564  lper__CallFailed
+0001ed70: 222c 2274 7970 6522 3a22 6572 726f 7222  ","type":"error"
+0001ed80: 7d2c 7b22 696e 7075 7473 223a 5b5d 2c22  },{"inputs":[],"
+0001ed90: 6e61 6d65 223a 2254 6f6b 656e 4865 6c70  name":"TokenHelp
+0001eda0: 6572 5f5f 4e6f 6e43 6f6e 7472 6163 7422  er__NonContract"
+0001edb0: 2c22 7479 7065 223a 2265 7272 6f72 227d  ,"type":"error"}
+0001edc0: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+0001edd0: 616d 6522 3a22 546f 6b65 6e48 656c 7065  ame":"TokenHelpe
+0001ede0: 725f 5f54 7261 6e73 6665 7246 6169 6c65  r__TransferFaile
+0001edf0: 6422 2c22 7479 7065 223a 2265 7272 6f72  d","type":"error
+0001ee00: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+0001ee10: 226e 616d 6522 3a22 5472 6565 4d61 7468  "name":"TreeMath
+0001ee20: 5f5f 4572 726f 7244 6570 7468 5365 6172  __ErrorDepthSear
+0001ee30: 6368 222c 2274 7970 6522 3a22 6572 726f  ch","type":"erro
+0001ee40: 7222 7d2c 7b22 616e 6f6e 796d 6f75 7322  r"},{"anonymous"
+0001ee50: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
+0001ee60: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
+0001ee70: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0001ee80: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0001ee90: 3a22 6163 636f 756e 7422 2c22 7479 7065  :"account","type
+0001eea0: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0001eeb0: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
+0001eec0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0001eed0: 7265 7373 222c 226e 616d 6522 3a22 7365  ress","name":"se
+0001eee0: 6e64 6572 222c 2274 7970 6522 3a22 6164  nder","type":"ad
+0001eef0: 6472 6573 7322 7d2c 7b22 696e 6465 7865  dress"},{"indexe
+0001ef00: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+0001ef10: 616c 5479 7065 223a 2262 6f6f 6c22 2c22  alType":"bool","
+0001ef20: 6e61 6d65 223a 2261 7070 726f 7665 6422  name":"approved"
+0001ef30: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
+0001ef40: 2c22 6e61 6d65 223a 2241 7070 726f 7661  ,"name":"Approva
+0001ef50: 6c46 6f72 416c 6c22 2c22 7479 7065 223a  lForAll","type":
+0001ef60: 2265 7665 6e74 227d 2c7b 2261 6e6f 6e79  "event"},{"anony
+0001ef70: 6d6f 7573 223a 6661 6c73 652c 2269 6e70  mous":false,"inp
+0001ef80: 7574 7322 3a5b 7b22 696e 6465 7865 6422  uts":[{"indexed"
+0001ef90: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
+0001efa0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0001efb0: 6e61 6d65 223a 2273 656e 6465 7222 2c22  name":"sender","
+0001efc0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+0001efd0: 2c7b 2269 6e64 6578 6564 223a 7472 7565  ,{"indexed":true
+0001efe0: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0001eff0: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0001f000: 3a22 7265 6369 7069 656e 7422 2c22 7479  :"recipient","ty
+0001f010: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+0001f020: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
+0001f030: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+0001f040: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+0001f050: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
+0001f060: 3235 3622 7d2c 7b22 696e 6465 7865 6422  256"},{"indexed"
+0001f070: 3a66 616c 7365 2c22 696e 7465 726e 616c  :false,"internal
+0001f080: 5479 7065 223a 2275 696e 7432 3536 222c  Type":"uint256",
+0001f090: 226e 616d 6522 3a22 6665 6573 5822 2c22  "name":"feesX","
+0001f0a0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001f0b0: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+0001f0c0: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001f0d0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001f0e0: 223a 2266 6565 7359 222c 2274 7970 6522  ":"feesY","type"
+0001f0f0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+0001f100: 6d65 223a 2243 6f6d 706f 7369 7469 6f6e  me":"Composition
+0001f110: 4665 6522 2c22 7479 7065 223a 2265 7665  Fee","type":"eve
+0001f120: 6e74 227d 2c7b 2261 6e6f 6e79 6d6f 7573  nt"},{"anonymous
+0001f130: 223a 6661 6c73 652c 2269 6e70 7574 7322  ":false,"inputs"
+0001f140: 3a5b 7b22 696e 6465 7865 6422 3a74 7275  :[{"indexed":tru
+0001f150: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001f160: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0001f170: 223a 2273 656e 6465 7222 2c22 7479 7065  ":"sender","type
+0001f180: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0001f190: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
+0001f1a0: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0001f1b0: 7265 7373 222c 226e 616d 6522 3a22 7265  ress","name":"re
+0001f1c0: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
+0001f1d0: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
+0001f1e0: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
+0001f1f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001f200: 3536 222c 226e 616d 6522 3a22 6964 222c  56","name":"id",
+0001f210: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001f220: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
+0001f230: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
+0001f240: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001f250: 6522 3a22 616d 6f75 6e74 5822 2c22 7479  e":"amountX","ty
+0001f260: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+0001f270: 2269 6e64 6578 6564 223a 6661 6c73 652c  "indexed":false,
+0001f280: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+0001f290: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+0001f2a0: 2261 6d6f 756e 7459 222c 2274 7970 6522  "amountY","type"
+0001f2b0: 3a22 7569 6e74 3235 3622 7d5d 2c22 6e61  :"uint256"}],"na
+0001f2c0: 6d65 223a 2244 6570 6f73 6974 6564 546f  me":"DepositedTo
+0001f2d0: 4269 6e22 2c22 7479 7065 223a 2265 7665  Bin","type":"eve
+0001f2e0: 6e74 227d 2c7b 2261 6e6f 6e79 6d6f 7573  nt"},{"anonymous
+0001f2f0: 223a 6661 6c73 652c 2269 6e70 7574 7322  ":false,"inputs"
+0001f300: 3a5b 7b22 696e 6465 7865 6422 3a74 7275  :[{"indexed":tru
+0001f310: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001f320: 3a22 6164 6472 6573 7322 2c22 6e61 6d65  :"address","name
+0001f330: 223a 2273 656e 6465 7222 2c22 7479 7065  ":"sender","type
+0001f340: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0001f350: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
+0001f360: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+0001f370: 7265 7373 222c 226e 616d 6522 3a22 7265  ress","name":"re
+0001f380: 6369 7069 656e 7422 2c22 7479 7065 223a  cipient","type":
+0001f390: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
+0001f3a0: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+0001f3b0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001f3c0: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
+0001f3d0: 756e 7458 222c 2274 7970 6522 3a22 7569  untX","type":"ui
+0001f3e0: 6e74 3235 3622 7d2c 7b22 696e 6465 7865  nt256"},{"indexe
+0001f3f0: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+0001f400: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+0001f410: 222c 226e 616d 6522 3a22 616d 6f75 6e74  ","name":"amount
+0001f420: 5922 2c22 7479 7065 223a 2275 696e 7432  Y","type":"uint2
+0001f430: 3536 227d 5d2c 226e 616d 6522 3a22 4665  56"}],"name":"Fe
+0001f440: 6573 436f 6c6c 6563 7465 6422 2c22 7479  esCollected","ty
+0001f450: 7065 223a 2265 7665 6e74 227d 2c7b 2261  pe":"event"},{"a
+0001f460: 6e6f 6e79 6d6f 7573 223a 6661 6c73 652c  nonymous":false,
+0001f470: 2269 6e70 7574 7322 3a5b 7b22 696e 6465  "inputs":[{"inde
+0001f480: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
+0001f490: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0001f4a0: 7322 2c22 6e61 6d65 223a 2273 656e 6465  s","name":"sende
+0001f4b0: 7222 2c22 7479 7065 223a 2261 6464 7265  r","type":"addre
+0001f4c0: 7373 227d 2c7b 2269 6e64 6578 6564 223a  ss"},{"indexed":
+0001f4d0: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
+0001f4e0: 7065 223a 2263 6f6e 7472 6163 7420 494c  pe":"contract IL
+0001f4f0: 4246 6c61 7368 4c6f 616e 4361 6c6c 6261  BFlashLoanCallba
+0001f500: 636b 222c 226e 616d 6522 3a22 7265 6365  ck","name":"rece
+0001f510: 6976 6572 222c 2274 7970 6522 3a22 6164  iver","type":"ad
+0001f520: 6472 6573 7322 7d2c 7b22 696e 6465 7865  dress"},{"indexe
+0001f530: 6422 3a66 616c 7365 2c22 696e 7465 726e  d":false,"intern
+0001f540: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+0001f550: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
+0001f560: 3a22 746f 6b65 6e22 2c22 7479 7065 223a  :"token","type":
+0001f570: 2261 6464 7265 7373 227d 2c7b 2269 6e64  "address"},{"ind
+0001f580: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+0001f590: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001f5a0: 3235 3622 2c22 6e61 6d65 223a 2261 6d6f  256","name":"amo
+0001f5b0: 756e 7422 2c22 7479 7065 223a 2275 696e  unt","type":"uin
+0001f5c0: 7432 3536 227d 2c7b 2269 6e64 6578 6564  t256"},{"indexed
+0001f5d0: 223a 6661 6c73 652c 2269 6e74 6572 6e61  ":false,"interna
+0001f5e0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+0001f5f0: 2c22 6e61 6d65 223a 2266 6565 222c 2274  ,"name":"fee","t
+0001f600: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0001f610: 2c22 6e61 6d65 223a 2246 6c61 7368 4c6f  ,"name":"FlashLo
+0001f620: 616e 222c 2274 7970 6522 3a22 6576 656e  an","type":"even
+0001f630: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
+0001f640: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
+0001f650: 5b7b 2269 6e64 6578 6564 223a 6661 6c73  [{"indexed":fals
+0001f660: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001f670: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001f680: 223a 2270 7265 7669 6f75 7353 697a 6522  ":"previousSize"
+0001f690: 2c22 7479 7065 223a 2275 696e 7432 3536  ,"type":"uint256
+0001f6a0: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
+0001f6b0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
+0001f6c0: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001f6d0: 6d65 223a 226e 6577 5369 7a65 222c 2274  me":"newSize","t
+0001f6e0: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+0001f6f0: 2c22 6e61 6d65 223a 224f 7261 636c 6553  ,"name":"OracleS
+0001f700: 697a 6549 6e63 7265 6173 6564 222c 2274  izeIncreased","t
+0001f710: 7970 6522 3a22 6576 656e 7422 7d2c 7b22  ype":"event"},{"
+0001f720: 616e 6f6e 796d 6f75 7322 3a66 616c 7365  anonymous":false
+0001f730: 2c22 696e 7075 7473 223a 5b7b 2269 6e64  ,"inputs":[{"ind
+0001f740: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
+0001f750: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0001f760: 7373 222c 226e 616d 6522 3a22 7365 6e64  ss","name":"send
+0001f770: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
+0001f780: 6573 7322 7d2c 7b22 696e 6465 7865 6422  ess"},{"indexed"
+0001f790: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
+0001f7a0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0001f7b0: 6e61 6d65 223a 2272 6563 6970 6965 6e74  name":"recipient
+0001f7c0: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0001f7d0: 7322 7d2c 7b22 696e 6465 7865 6422 3a66  s"},{"indexed":f
+0001f7e0: 616c 7365 2c22 696e 7465 726e 616c 5479  alse,"internalTy
+0001f7f0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001f800: 616d 6522 3a22 616d 6f75 6e74 5822 2c22  ame":"amountX","
+0001f810: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001f820: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+0001f830: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001f840: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001f850: 223a 2261 6d6f 756e 7459 222c 2274 7970  ":"amountY","typ
+0001f860: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+0001f870: 6e61 6d65 223a 2250 726f 746f 636f 6c46  name":"ProtocolF
+0001f880: 6565 7343 6f6c 6c65 6374 6564 222c 2274  eesCollected","t
+0001f890: 7970 6522 3a22 6576 656e 7422 7d2c 7b22  ype":"event"},{"
+0001f8a0: 616e 6f6e 796d 6f75 7322 3a66 616c 7365  anonymous":false
+0001f8b0: 2c22 696e 7075 7473 223a 5b7b 2269 6e64  ,"inputs":[{"ind
+0001f8c0: 6578 6564 223a 7472 7565 2c22 696e 7465  exed":true,"inte
+0001f8d0: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+0001f8e0: 7373 222c 226e 616d 6522 3a22 7365 6e64  ss","name":"send
+0001f8f0: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
+0001f900: 6573 7322 7d2c 7b22 696e 6465 7865 6422  ess"},{"indexed"
+0001f910: 3a74 7275 652c 2269 6e74 6572 6e61 6c54  :true,"internalT
+0001f920: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+0001f930: 6e61 6d65 223a 2272 6563 6970 6965 6e74  name":"recipient
+0001f940: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+0001f950: 7322 7d2c 7b22 696e 6465 7865 6422 3a74  s"},{"indexed":t
+0001f960: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
+0001f970: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001f980: 6d65 223a 2269 6422 2c22 7479 7065 223a  me":"id","type":
+0001f990: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
+0001f9a0: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+0001f9b0: 6572 6e61 6c54 7970 6522 3a22 626f 6f6c  ernalType":"bool
+0001f9c0: 222c 226e 616d 6522 3a22 7377 6170 466f  ","name":"swapFo
+0001f9d0: 7259 222c 2274 7970 6522 3a22 626f 6f6c  rY","type":"bool
+0001f9e0: 227d 2c7b 2269 6e64 6578 6564 223a 6661  "},{"indexed":fa
+0001f9f0: 6c73 652c 2269 6e74 6572 6e61 6c54 7970  lse,"internalTyp
+0001fa00: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+0001fa10: 6d65 223a 2261 6d6f 756e 7449 6e22 2c22  me":"amountIn","
+0001fa20: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+0001fa30: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+0001fa40: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+0001fa50: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+0001fa60: 223a 2261 6d6f 756e 744f 7574 222c 2274  ":"amountOut","t
+0001fa70: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+0001fa80: 7b22 696e 6465 7865 6422 3a66 616c 7365  {"indexed":false
+0001fa90: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0001faa0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+0001fab0: 3a22 766f 6c61 7469 6c69 7479 4163 6375  :"volatilityAccu
+0001fac0: 6d75 6c61 7465 6422 2c22 7479 7065 223a  mulated","type":
+0001fad0: 2275 696e 7432 3536 227d 2c7b 2269 6e64  "uint256"},{"ind
+0001fae0: 6578 6564 223a 6661 6c73 652c 2269 6e74  exed":false,"int
+0001faf0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+0001fb00: 3235 3622 2c22 6e61 6d65 223a 2266 6565  256","name":"fee
+0001fb10: 7322 2c22 7479 7065 223a 2275 696e 7432  s","type":"uint2
+0001fb20: 3536 227d 5d2c 226e 616d 6522 3a22 5377  56"}],"name":"Sw
+0001fb30: 6170 222c 2274 7970 6522 3a22 6576 656e  ap","type":"even
+0001fb40: 7422 7d2c 7b22 616e 6f6e 796d 6f75 7322  t"},{"anonymous"
+0001fb50: 3a66 616c 7365 2c22 696e 7075 7473 223a  :false,"inputs":
+0001fb60: 5b7b 2269 6e64 6578 6564 223a 7472 7565  [{"indexed":true
+0001fb70: 2c22 696e 7465 726e 616c 5479 7065 223a  ,"internalType":
+0001fb80: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+0001fb90: 3a22 7365 6e64 6572 222c 2274 7970 6522  :"sender","type"
+0001fba0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001fbb0: 6465 7865 6422 3a74 7275 652c 2269 6e74  dexed":true,"int
+0001fbc0: 6572 6e61 6c54 7970 6522 3a22 6164 6472  ernalType":"addr
+0001fbd0: 6573 7322 2c22 6e61 6d65 223a 2266 726f  ess","name":"fro
+0001fbe0: 6d22 2c22 7479 7065 223a 2261 6464 7265  m","type":"addre
+0001fbf0: 7373 227d 2c7b 2269 6e64 6578 6564 223a  ss"},{"indexed":
+0001fc00: 7472 7565 2c22 696e 7465 726e 616c 5479  true,"internalTy
+0001fc10: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+0001fc20: 616d 6522 3a22 746f 222c 2274 7970 6522  ame":"to","type"
+0001fc30: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+0001fc40: 6465 7865 6422 3a66 616c 7365 2c22 696e  dexed":false,"in
+0001fc50: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001fc60: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
+0001fc70: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
+0001fc80: 7432 3536 5b5d 227d 2c7b 2269 6e64 6578  t256[]"},{"index
+0001fc90: 6564 223a 6661 6c73 652c 2269 6e74 6572  ed":false,"inter
+0001fca0: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+0001fcb0: 365b 5d22 2c22 6e61 6d65 223a 2261 6d6f  6[]","name":"amo
+0001fcc0: 756e 7473 222c 2274 7970 6522 3a22 7569  unts","type":"ui
+0001fcd0: 6e74 3235 365b 5d22 7d5d 2c22 6e61 6d65  nt256[]"}],"name
+0001fce0: 223a 2254 7261 6e73 6665 7242 6174 6368  ":"TransferBatch
+0001fcf0: 222c 2274 7970 6522 3a22 6576 656e 7422  ","type":"event"
+0001fd00: 7d2c 7b22 616e 6f6e 796d 6f75 7322 3a66  },{"anonymous":f
+0001fd10: 616c 7365 2c22 696e 7075 7473 223a 5b7b  alse,"inputs":[{
+0001fd20: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
+0001fd30: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+0001fd40: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+0001fd50: 7365 6e64 6572 222c 2274 7970 6522 3a22  sender","type":"
+0001fd60: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
+0001fd70: 7865 6422 3a74 7275 652c 2269 6e74 6572  xed":true,"inter
+0001fd80: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+0001fd90: 7322 2c22 6e61 6d65 223a 2266 726f 6d22  s","name":"from"
+0001fda0: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+0001fdb0: 227d 2c7b 2269 6e64 6578 6564 223a 7472  "},{"indexed":tr
+0001fdc0: 7565 2c22 696e 7465 726e 616c 5479 7065  ue,"internalType
+0001fdd0: 223a 2261 6464 7265 7373 222c 226e 616d  ":"address","nam
+0001fde0: 6522 3a22 746f 222c 2274 7970 6522 3a22  e":"to","type":"
+0001fdf0: 6164 6472 6573 7322 7d2c 7b22 696e 6465  address"},{"inde
+0001fe00: 7865 6422 3a66 616c 7365 2c22 696e 7465  xed":false,"inte
+0001fe10: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+0001fe20: 3536 222c 226e 616d 6522 3a22 6964 222c  56","name":"id",
+0001fe30: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+0001fe40: 7d2c 7b22 696e 6465 7865 6422 3a66 616c  },{"indexed":fal
+0001fe50: 7365 2c22 696e 7465 726e 616c 5479 7065  se,"internalType
+0001fe60: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+0001fe70: 6522 3a22 616d 6f75 6e74 222c 2274 7970  e":"amount","typ
+0001fe80: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+0001fe90: 6e61 6d65 223a 2254 7261 6e73 6665 7253  name":"TransferS
+0001fea0: 696e 676c 6522 2c22 7479 7065 223a 2265  ingle","type":"e
+0001feb0: 7665 6e74 227d 2c7b 2261 6e6f 6e79 6d6f  vent"},{"anonymo
+0001fec0: 7573 223a 6661 6c73 652c 2269 6e70 7574  us":false,"input
+0001fed0: 7322 3a5b 7b22 696e 6465 7865 6422 3a74  s":[{"indexed":t
+0001fee0: 7275 652c 2269 6e74 6572 6e61 6c54 7970  rue,"internalTyp
+0001fef0: 6522 3a22 6164 6472 6573 7322 2c22 6e61  e":"address","na
+0001ff00: 6d65 223a 2273 656e 6465 7222 2c22 7479  me":"sender","ty
+0001ff10: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+0001ff20: 2269 6e64 6578 6564 223a 7472 7565 2c22  "indexed":true,"
+0001ff30: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+0001ff40: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+0001ff50: 7265 6369 7069 656e 7422 2c22 7479 7065  recipient","type
+0001ff60: 223a 2261 6464 7265 7373 227d 2c7b 2269  ":"address"},{"i
+0001ff70: 6e64 6578 6564 223a 7472 7565 2c22 696e  ndexed":true,"in
+0001ff80: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+0001ff90: 7432 3536 222c 226e 616d 6522 3a22 6964  t256","name":"id
+0001ffa0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+0001ffb0: 3622 7d2c 7b22 696e 6465 7865 6422 3a66  6"},{"indexed":f
+0001ffc0: 616c 7365 2c22 696e 7465 726e 616c 5479  alse,"internalTy
+0001ffd0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+0001ffe0: 616d 6522 3a22 616d 6f75 6e74 5822 2c22  ame":"amountX","
+0001fff0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00020000: 2c7b 2269 6e64 6578 6564 223a 6661 6c73  ,{"indexed":fals
+00020010: 652c 2269 6e74 6572 6e61 6c54 7970 6522  e,"internalType"
+00020020: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00020030: 223a 2261 6d6f 756e 7459 222c 2274 7970  ":"amountY","typ
+00020040: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+00020050: 6e61 6d65 223a 2257 6974 6864 7261 776e  name":"Withdrawn
+00020060: 4672 6f6d 4269 6e22 2c22 7479 7065 223a  FromBin","type":
+00020070: 2265 7665 6e74 227d 2c7b 2269 6e70 7574  "event"},{"input
+00020080: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00020090: 7065 223a 2261 6464 7265 7373 222c 226e  pe":"address","n
+000200a0: 616d 6522 3a22 5f61 6363 6f75 6e74 222c  ame":"_account",
+000200b0: 2274 7970 6522 3a22 6164 6472 6573 7322  "type":"address"
+000200c0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000200d0: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+000200e0: 6522 3a22 5f69 6422 2c22 7479 7065 223a  e":"_id","type":
+000200f0: 2275 696e 7432 3536 227d 5d2c 226e 616d  "uint256"}],"nam
+00020100: 6522 3a22 6261 6c61 6e63 654f 6622 2c22  e":"balanceOf","
+00020110: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+00020120: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00020130: 3536 222c 226e 616d 6522 3a22 222c 2274  56","name":"","t
+00020140: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+00020150: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+00020160: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+00020170: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+00020180: 6e70 7574 7322 3a5b 7b22 696e 7465 726e  nputs":[{"intern
+00020190: 616c 5479 7065 223a 2261 6464 7265 7373  alType":"address
+000201a0: 5b5d 222c 226e 616d 6522 3a22 5f61 6363  []","name":"_acc
+000201b0: 6f75 6e74 7322 2c22 7479 7065 223a 2261  ounts","type":"a
+000201c0: 6464 7265 7373 5b5d 227d 2c7b 2269 6e74  ddress[]"},{"int
+000201d0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+000201e0: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
+000201f0: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
+00020200: 7432 3536 5b5d 227d 5d2c 226e 616d 6522  t256[]"}],"name"
+00020210: 3a22 6261 6c61 6e63 654f 6642 6174 6368  :"balanceOfBatch
+00020220: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
+00020230: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00020240: 6e74 3235 365b 5d22 2c22 6e61 6d65 223a  nt256[]","name":
+00020250: 2262 6174 6368 4261 6c61 6e63 6573 222c  "batchBalances",
+00020260: 2274 7970 6522 3a22 7569 6e74 3235 365b  "type":"uint256[
+00020270: 5d22 7d5d 2c22 7374 6174 654d 7574 6162  ]"}],"stateMutab
+00020280: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+00020290: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+000202a0: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
 000202b0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-000202c0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
-000202d0: 6f75 6e74 5922 2c22 7479 7065 223a 2275  ountY","type":"u
-000202e0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
-000202f0: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-00020300: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-00020310: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00020320: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00020330: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-00020340: 2c22 6e61 6d65 223a 225f 6163 636f 756e  ,"name":"_accoun
-00020350: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
-00020360: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-00020370: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
-00020380: 2c22 6e61 6d65 223a 225f 6964 7322 2c22  ,"name":"_ids","
-00020390: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
-000203a0: 227d 5d2c 226e 616d 6522 3a22 636f 6c6c  "}],"name":"coll
-000203b0: 6563 7446 6565 7322 2c22 6f75 7470 7574  ectFees","output
-000203c0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-000203d0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-000203e0: 616d 6522 3a22 616d 6f75 6e74 5822 2c22  ame":"amountX","
-000203f0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00020400: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00020410: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00020420: 223a 2261 6d6f 756e 7459 222c 2274 7970  ":"amountY","typ
-00020430: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-00020440: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00020450: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
-00020460: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00020470: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
-00020480: 616d 6522 3a22 636f 6c6c 6563 7450 726f  ame":"collectPro
-00020490: 746f 636f 6c46 6565 7322 2c22 6f75 7470  tocolFees","outp
-000204a0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-000204b0: 5479 7065 223a 2275 696e 7431 3238 222c  Type":"uint128",
-000204c0: 226e 616d 6522 3a22 616d 6f75 6e74 5822  "name":"amountX"
-000204d0: 2c22 7479 7065 223a 2275 696e 7431 3238  ,"type":"uint128
-000204e0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-000204f0: 6522 3a22 7569 6e74 3132 3822 2c22 6e61  e":"uint128","na
-00020500: 6d65 223a 2261 6d6f 756e 7459 222c 2274  me":"amountY","t
-00020510: 7970 6522 3a22 7569 6e74 3132 3822 7d5d  ype":"uint128"}]
-00020520: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00020530: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
-00020540: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-00020550: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
-00020560: 226e 616d 6522 3a22 6661 6374 6f72 7922  "name":"factory"
-00020570: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-00020580: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
-00020590: 7472 6163 7420 494c 4246 6163 746f 7279  tract ILBFactory
-000205a0: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-000205b0: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
-000205c0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-000205d0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-000205e0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-000205f0: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-00020600: 6665 6550 6172 616d 6574 6572 7322 2c22  feeParameters","
-00020610: 6f75 7470 7574 7322 3a5b 7b22 636f 6d70  outputs":[{"comp
-00020620: 6f6e 656e 7473 223a 5b7b 2269 6e74 6572  onents":[{"inter
-00020630: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
-00020640: 222c 226e 616d 6522 3a22 6269 6e53 7465  ","name":"binSte
-00020650: 7022 2c22 7479 7065 223a 2275 696e 7431  p","type":"uint1
-00020660: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00020670: 7065 223a 2275 696e 7431 3622 2c22 6e61  pe":"uint16","na
-00020680: 6d65 223a 2262 6173 6546 6163 746f 7222  me":"baseFactor"
-00020690: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
-000206a0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-000206b0: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-000206c0: 223a 2266 696c 7465 7250 6572 696f 6422  ":"filterPeriod"
-000206d0: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
-000206e0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-000206f0: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
-00020700: 223a 2264 6563 6179 5065 7269 6f64 222c  ":"decayPeriod",
-00020710: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
-00020720: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00020730: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
-00020740: 3a22 7265 6475 6374 696f 6e46 6163 746f  :"reductionFacto
-00020750: 7222 2c22 7479 7065 223a 2275 696e 7431  r","type":"uint1
-00020760: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00020770: 7065 223a 2275 696e 7432 3422 2c22 6e61  pe":"uint24","na
-00020780: 6d65 223a 2276 6172 6961 626c 6546 6565  me":"variableFee
-00020790: 436f 6e74 726f 6c22 2c22 7479 7065 223a  Control","type":
-000207a0: 2275 696e 7432 3422 7d2c 7b22 696e 7465  "uint24"},{"inte
-000207b0: 726e 616c 5479 7065 223a 2275 696e 7431  rnalType":"uint1
-000207c0: 3622 2c22 6e61 6d65 223a 2270 726f 746f  6","name":"proto
-000207d0: 636f 6c53 6861 7265 222c 2274 7970 6522  colShare","type"
-000207e0: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
-000207f0: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00020800: 3234 222c 226e 616d 6522 3a22 6d61 7856  24","name":"maxV
-00020810: 6f6c 6174 696c 6974 7941 6363 756d 756c  olatilityAccumul
-00020820: 6174 6564 222c 2274 7970 6522 3a22 7569  ated","type":"ui
-00020830: 6e74 3234 227d 2c7b 2269 6e74 6572 6e61  nt24"},{"interna
-00020840: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
-00020850: 226e 616d 6522 3a22 766f 6c61 7469 6c69  "name":"volatili
-00020860: 7479 4163 6375 6d75 6c61 7465 6422 2c22  tyAccumulated","
-00020870: 7479 7065 223a 2275 696e 7432 3422 7d2c  type":"uint24"},
-00020880: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00020890: 2275 696e 7432 3422 2c22 6e61 6d65 223a  "uint24","name":
-000208a0: 2276 6f6c 6174 696c 6974 7952 6566 6572  "volatilityRefer
-000208b0: 656e 6365 222c 2274 7970 6522 3a22 7569  ence","type":"ui
-000208c0: 6e74 3234 227d 2c7b 2269 6e74 6572 6e61  nt24"},{"interna
-000208d0: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
-000208e0: 226e 616d 6522 3a22 696e 6465 7852 6566  "name":"indexRef
-000208f0: 222c 2274 7970 6522 3a22 7569 6e74 3234  ","type":"uint24
-00020900: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
-00020910: 6522 3a22 7569 6e74 3430 222c 226e 616d  e":"uint40","nam
-00020920: 6522 3a22 7469 6d65 222c 2274 7970 6522  e":"time","type"
-00020930: 3a22 7569 6e74 3430 227d 5d2c 2269 6e74  :"uint40"}],"int
-00020940: 6572 6e61 6c54 7970 6522 3a22 7374 7275  ernalType":"stru
-00020950: 6374 2046 6565 4865 6c70 6572 2e46 6565  ct FeeHelper.Fee
-00020960: 5061 7261 6d65 7465 7273 222c 226e 616d  Parameters","nam
-00020970: 6522 3a22 222c 2274 7970 6522 3a22 7475  e":"","type":"tu
-00020980: 706c 6522 7d5d 2c22 7374 6174 654d 7574  ple"}],"stateMut
-00020990: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-000209a0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-000209b0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-000209c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-000209d0: 696e 7432 3422 2c22 6e61 6d65 223a 225f  int24","name":"_
-000209e0: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
-000209f0: 3234 227d 2c7b 2269 6e74 6572 6e61 6c54  24"},{"internalT
-00020a00: 7970 6522 3a22 626f 6f6c 222c 226e 616d  ype":"bool","nam
-00020a10: 6522 3a22 5f73 7761 7046 6f72 5922 2c22  e":"_swapForY","
-00020a20: 7479 7065 223a 2262 6f6f 6c22 7d5d 2c22  type":"bool"}],"
-00020a30: 6e61 6d65 223a 2266 696e 6446 6972 7374  name":"findFirst
-00020a40: 4e6f 6e45 6d70 7479 4269 6e49 6422 2c22  NonEmptyBinId","
-00020a50: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-00020a60: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00020a70: 3422 2c22 6e61 6d65 223a 2222 2c22 7479  4","name":"","ty
-00020a80: 7065 223a 2275 696e 7432 3422 7d5d 2c22  pe":"uint24"}],"
-00020a90: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-00020aa0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-00020ab0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00020ac0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00020ad0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
-00020ae0: 494c 4246 6c61 7368 4c6f 616e 4361 6c6c  ILBFlashLoanCall
-00020af0: 6261 636b 222c 226e 616d 6522 3a22 5f72  back","name":"_r
-00020b00: 6563 6569 7665 7222 2c22 7479 7065 223a  eceiver","type":
-00020b10: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-00020b20: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
-00020b30: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
-00020b40: 6d65 223a 225f 746f 6b65 6e22 2c22 7479  me":"_token","ty
-00020b50: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
-00020b60: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00020b70: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
-00020b80: 225f 616d 6f75 6e74 222c 2274 7970 6522  "_amount","type"
-00020b90: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-00020ba0: 7465 726e 616c 5479 7065 223a 2262 7974  ternalType":"byt
-00020bb0: 6573 222c 226e 616d 6522 3a22 5f64 6174  es","name":"_dat
-00020bc0: 6122 2c22 7479 7065 223a 2262 7974 6573  a","type":"bytes
-00020bd0: 227d 5d2c 226e 616d 6522 3a22 666c 6173  "}],"name":"flas
-00020be0: 684c 6f61 6e22 2c22 6f75 7470 7574 7322  hLoan","outputs"
-00020bf0: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
-00020c00: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
-00020c10: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
-00020c20: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-00020c30: 5b5d 2c22 6e61 6d65 223a 2266 6f72 6365  [],"name":"force
-00020c40: 4465 6361 7922 2c22 6f75 7470 7574 7322  Decay","outputs"
-00020c50: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
-00020c60: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
-00020c70: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
-00020c80: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
-00020c90: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00020ca0: 3a22 7569 6e74 3234 222c 226e 616d 6522  :"uint24","name"
-00020cb0: 3a22 5f69 6422 2c22 7479 7065 223a 2275  :"_id","type":"u
-00020cc0: 696e 7432 3422 7d5d 2c22 6e61 6d65 223a  int24"}],"name":
-00020cd0: 2267 6574 4269 6e22 2c22 6f75 7470 7574  "getBin","output
-00020ce0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00020cf0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00020d00: 616d 6522 3a22 7265 7365 7276 6558 222c  ame":"reserveX",
-00020d10: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
-00020d20: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
-00020d30: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
-00020d40: 6522 3a22 7265 7365 7276 6559 222c 2274  e":"reserveY","t
-00020d50: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
-00020d60: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-00020d70: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
-00020d80: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-00020d90: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-00020da0: 3a22 6765 7447 6c6f 6261 6c46 6565 7322  :"getGlobalFees"
-00020db0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-00020dc0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00020dd0: 7431 3238 222c 226e 616d 6522 3a22 6665  t128","name":"fe
-00020de0: 6573 5854 6f74 616c 222c 2274 7970 6522  esXTotal","type"
-00020df0: 3a22 7569 6e74 3132 3822 7d2c 7b22 696e  :"uint128"},{"in
-00020e00: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00020e10: 7431 3238 222c 226e 616d 6522 3a22 6665  t128","name":"fe
-00020e20: 6573 5954 6f74 616c 222c 2274 7970 6522  esYTotal","type"
-00020e30: 3a22 7569 6e74 3132 3822 7d2c 7b22 696e  :"uint128"},{"in
-00020e40: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00020e50: 7431 3238 222c 226e 616d 6522 3a22 6665  t128","name":"fe
-00020e60: 6573 5850 726f 746f 636f 6c22 2c22 7479  esXProtocol","ty
-00020e70: 7065 223a 2275 696e 7431 3238 227d 2c7b  pe":"uint128"},{
-00020e80: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-00020e90: 7569 6e74 3132 3822 2c22 6e61 6d65 223a  uint128","name":
-00020ea0: 2266 6565 7359 5072 6f74 6f63 6f6c 222c  "feesYProtocol",
-00020eb0: 2274 7970 6522 3a22 7569 6e74 3132 3822  "type":"uint128"
-00020ec0: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
-00020ed0: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
-00020ee0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00020ef0: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
-00020f00: 6522 3a22 6765 744f 7261 636c 6550 6172  e":"getOraclePar
-00020f10: 616d 6574 6572 7322 2c22 6f75 7470 7574  ameters","output
-00020f20: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
-00020f30: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00020f40: 616d 6522 3a22 6f72 6163 6c65 5361 6d70  ame":"oracleSamp
-00020f50: 6c65 4c69 6665 7469 6d65 222c 2274 7970  leLifetime","typ
-00020f60: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-00020f70: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00020f80: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00020f90: 6f72 6163 6c65 5369 7a65 222c 2274 7970  oracleSize","typ
-00020fa0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
-00020fb0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00020fc0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00020fd0: 6f72 6163 6c65 4163 7469 7665 5369 7a65  oracleActiveSize
-00020fe0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00020ff0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-00021000: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-00021010: 616d 6522 3a22 6f72 6163 6c65 4c61 7374  ame":"oracleLast
-00021020: 5469 6d65 7374 616d 7022 2c22 7479 7065  Timestamp","type
-00021030: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
-00021040: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
-00021050: 6e74 3235 3622 2c22 6e61 6d65 223a 226f  nt256","name":"o
-00021060: 7261 636c 6549 6422 2c22 7479 7065 223a  racleId","type":
-00021070: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
-00021080: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00021090: 3235 3622 2c22 6e61 6d65 223a 226d 696e  256","name":"min
-000210a0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-000210b0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
-000210c0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
-000210d0: 616d 6522 3a22 6d61 7822 2c22 7479 7065  ame":"max","type
-000210e0: 223a 2275 696e 7432 3536 227d 5d2c 2273  ":"uint256"}],"s
-000210f0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00021100: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
-00021110: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00021120: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00021130: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00021140: 6e61 6d65 223a 225f 7469 6d65 4465 6c74  name":"_timeDelt
-00021150: 6122 2c22 7479 7065 223a 2275 696e 7432  a","type":"uint2
-00021160: 3536 227d 5d2c 226e 616d 6522 3a22 6765  56"}],"name":"ge
-00021170: 744f 7261 636c 6553 616d 706c 6546 726f  tOracleSampleFro
-00021180: 6d22 2c22 6f75 7470 7574 7322 3a5b 7b22  m","outputs":[{"
-00021190: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-000211a0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-000211b0: 6375 6d75 6c61 7469 7665 4964 222c 2274  cumulativeId","t
-000211c0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
-000211d0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-000211e0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
-000211f0: 3a22 6375 6d75 6c61 7469 7665 566f 6c61  :"cumulativeVola
-00021200: 7469 6c69 7479 4163 6375 6d75 6c61 7465  tilityAccumulate
-00021210: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
-00021220: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
-00021230: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
-00021240: 6e61 6d65 223a 2263 756d 756c 6174 6976  name":"cumulativ
-00021250: 6542 696e 4372 6f73 7365 6422 2c22 7479  eBinCrossed","ty
-00021260: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
-00021270: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
-00021280: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
-00021290: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-000212a0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
-000212b0: 2267 6574 5265 7365 7276 6573 416e 6449  "getReservesAndI
-000212c0: 6422 2c22 6f75 7470 7574 7322 3a5b 7b22  d","outputs":[{"
-000212d0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-000212e0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-000212f0: 7265 7365 7276 6558 222c 2274 7970 6522  reserveX","type"
-00021300: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
-00021310: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
-00021320: 7432 3536 222c 226e 616d 6522 3a22 7265  t256","name":"re
-00021330: 7365 7276 6559 222c 2274 7970 6522 3a22  serveY","type":"
-00021340: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
-00021350: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00021360: 3536 222c 226e 616d 6522 3a22 6163 7469  56","name":"acti
-00021370: 7665 4964 222c 2274 7970 6522 3a22 7569  veId","type":"ui
-00021380: 6e74 3235 3622 7d5d 2c22 7374 6174 654d  nt256"}],"stateM
-00021390: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
-000213a0: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
-000213b0: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
-000213c0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-000213d0: 2275 696e 7431 3622 2c22 6e61 6d65 223a  "uint16","name":
-000213e0: 225f 6e65 774c 656e 6774 6822 2c22 7479  "_newLength","ty
-000213f0: 7065 223a 2275 696e 7431 3622 7d5d 2c22  pe":"uint16"}],"
-00021400: 6e61 6d65 223a 2269 6e63 7265 6173 654f  name":"increaseO
-00021410: 7261 636c 654c 656e 6774 6822 2c22 6f75  racleLength","ou
-00021420: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
-00021430: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
-00021440: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
-00021450: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
-00021460: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
-00021470: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
-00021480: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
-00021490: 225f 746f 6b65 6e58 222c 2274 7970 6522  "_tokenX","type"
-000214a0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
-000214b0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
-000214c0: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
-000214d0: 616d 6522 3a22 5f74 6f6b 656e 5922 2c22  ame":"_tokenY","
-000214e0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
-000214f0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00021500: 3a22 7569 6e74 3234 222c 226e 616d 6522  :"uint24","name"
-00021510: 3a22 5f61 6374 6976 6549 6422 2c22 7479  :"_activeId","ty
-00021520: 7065 223a 2275 696e 7432 3422 7d2c 7b22  pe":"uint24"},{"
-00021530: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00021540: 696e 7431 3622 2c22 6e61 6d65 223a 225f  int16","name":"_
-00021550: 7361 6d70 6c65 4c69 6665 7469 6d65 222c  sampleLifetime",
-00021560: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
-00021570: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-00021580: 3a22 6279 7465 7333 3222 2c22 6e61 6d65  :"bytes32","name
-00021590: 223a 225f 7061 636b 6564 4665 6550 6172  ":"_packedFeePar
-000215a0: 616d 6574 6572 7322 2c22 7479 7065 223a  ameters","type":
-000215b0: 2262 7974 6573 3332 227d 5d2c 226e 616d  "bytes32"}],"nam
-000215c0: 6522 3a22 696e 6974 6961 6c69 7a65 222c  e":"initialize",
-000215d0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
-000215e0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-000215f0: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
-00021600: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00021610: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-00021620: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-00021630: 7373 222c 226e 616d 6522 3a22 5f6f 776e  ss","name":"_own
-00021640: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
-00021650: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
-00021660: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
-00021670: 226e 616d 6522 3a22 5f73 7065 6e64 6572  "name":"_spender
-00021680: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
-00021690: 7322 7d5d 2c22 6e61 6d65 223a 2269 7341  s"}],"name":"isA
-000216a0: 7070 726f 7665 6446 6f72 416c 6c22 2c22  pprovedForAll","
-000216b0: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-000216c0: 726e 616c 5479 7065 223a 2262 6f6f 6c22  rnalType":"bool"
-000216d0: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
-000216e0: 223a 2262 6f6f 6c22 7d5d 2c22 7374 6174  ":"bool"}],"stat
-000216f0: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
-00021700: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
-00021710: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
-00021720: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
-00021730: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
-00021740: 616d 6522 3a22 5f69 6473 222c 2274 7970  ame":"_ids","typ
-00021750: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
-00021760: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00021770: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
-00021780: 6522 3a22 5f64 6973 7472 6962 7574 696f  e":"_distributio
-00021790: 6e58 222c 2274 7970 6522 3a22 7569 6e74  nX","type":"uint
-000217a0: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
-000217b0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-000217c0: 5b5d 222c 226e 616d 6522 3a22 5f64 6973  []","name":"_dis
-000217d0: 7472 6962 7574 696f 6e59 222c 2274 7970  tributionY","typ
-000217e0: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
-000217f0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00021800: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
-00021810: 3a22 5f74 6f22 2c22 7479 7065 223a 2261  :"_to","type":"a
-00021820: 6464 7265 7373 227d 5d2c 226e 616d 6522  ddress"}],"name"
-00021830: 3a22 6d69 6e74 222c 226f 7574 7075 7473  :"mint","outputs
-00021840: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
-00021850: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
-00021860: 6d65 223a 2222 2c22 7479 7065 223a 2275  me":"","type":"u
-00021870: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
-00021880: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
-00021890: 3622 2c22 6e61 6d65 223a 2222 2c22 7479  6","name":"","ty
-000218a0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
-000218b0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
-000218c0: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
-000218d0: 223a 226c 6971 7569 6469 7479 4d69 6e74  ":"liquidityMint
-000218e0: 6564 222c 2274 7970 6522 3a22 7569 6e74  ed","type":"uint
-000218f0: 3235 365b 5d22 7d5d 2c22 7374 6174 654d  256[]"}],"stateM
-00021900: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-00021910: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-00021920: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00021930: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
-00021940: 6e61 6d65 222c 226f 7574 7075 7473 223a  name","outputs":
-00021950: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-00021960: 3a22 7374 7269 6e67 222c 226e 616d 6522  :"string","name"
-00021970: 3a22 222c 2274 7970 6522 3a22 7374 7269  :"","type":"stri
-00021980: 6e67 227d 5d2c 2273 7461 7465 4d75 7461  ng"}],"stateMuta
-00021990: 6269 6c69 7479 223a 2270 7572 6522 2c22  bility":"pure","
-000219a0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
-000219b0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
-000219c0: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
-000219d0: 6472 6573 7322 2c22 6e61 6d65 223a 225f  dress","name":"_
-000219e0: 6163 636f 756e 7422 2c22 7479 7065 223a  account","type":
-000219f0: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
-00021a00: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
-00021a10: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
-00021a20: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
-00021a30: 7432 3536 5b5d 227d 5d2c 226e 616d 6522  t256[]"}],"name"
-00021a40: 3a22 7065 6e64 696e 6746 6565 7322 2c22  :"pendingFees","
-00021a50: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
-00021a60: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
-00021a70: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
-00021a80: 6e74 5822 2c22 7479 7065 223a 2275 696e  ntX","type":"uin
-00021a90: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-00021aa0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00021ab0: 2c22 6e61 6d65 223a 2261 6d6f 756e 7459  ,"name":"amountY
-00021ac0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00021ad0: 3622 7d5d 2c22 7374 6174 654d 7574 6162  6"}],"stateMutab
-00021ae0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
-00021af0: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
-00021b00: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
-00021b10: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
-00021b20: 7265 7373 222c 226e 616d 6522 3a22 5f66  ress","name":"_f
-00021b30: 726f 6d22 2c22 7479 7065 223a 2261 6464  rom","type":"add
-00021b40: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-00021b50: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
-00021b60: 2c22 6e61 6d65 223a 225f 746f 222c 2274  ,"name":"_to","t
-00021b70: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
-00021b80: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
-00021b90: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
-00021ba0: 6522 3a22 5f69 6473 222c 2274 7970 6522  e":"_ids","type"
-00021bb0: 3a22 7569 6e74 3235 365b 5d22 7d2c 7b22  :"uint256[]"},{"
-00021bc0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00021bd0: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
-00021be0: 3a22 5f61 6d6f 756e 7473 222c 2274 7970  :"_amounts","typ
-00021bf0: 6522 3a22 7569 6e74 3235 365b 5d22 7d5d  e":"uint256[]"}]
-00021c00: 2c22 6e61 6d65 223a 2273 6166 6542 6174  ,"name":"safeBat
-00021c10: 6368 5472 616e 7366 6572 4672 6f6d 222c  chTransferFrom",
-00021c20: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
-00021c30: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
-00021c40: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
-00021c50: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
-00021c60: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
-00021c70: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
-00021c80: 7373 222c 226e 616d 6522 3a22 5f66 726f  ss","name":"_fro
-00021c90: 6d22 2c22 7479 7065 223a 2261 6464 7265  m","type":"addre
-00021ca0: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
-00021cb0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
-00021cc0: 6e61 6d65 223a 225f 746f 222c 2274 7970  name":"_to","typ
-00021cd0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
-00021ce0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00021cf0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00021d00: 5f69 6422 2c22 7479 7065 223a 2275 696e  _id","type":"uin
-00021d10: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
-00021d20: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
-00021d30: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
-00021d40: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
-00021d50: 3622 7d5d 2c22 6e61 6d65 223a 2273 6166  6"}],"name":"saf
-00021d60: 6554 7261 6e73 6665 7246 726f 6d22 2c22  eTransferFrom","
-00021d70: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
-00021d80: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
-00021d90: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
-00021da0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
-00021db0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
-00021dc0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
-00021dd0: 7322 2c22 6e61 6d65 223a 225f 7370 656e  s","name":"_spen
-00021de0: 6465 7222 2c22 7479 7065 223a 2261 6464  der","type":"add
-00021df0: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
-00021e00: 6c54 7970 6522 3a22 626f 6f6c 222c 226e  lType":"bool","n
-00021e10: 616d 6522 3a22 5f61 7070 726f 7665 6422  ame":"_approved"
-00021e20: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
-00021e30: 2c22 6e61 6d65 223a 2273 6574 4170 7072  ,"name":"setAppr
-00021e40: 6f76 616c 466f 7241 6c6c 222c 226f 7574  ovalForAll","out
-00021e50: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
-00021e60: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-00021e70: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-00021e80: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00021e90: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00021ea0: 5479 7065 223a 2262 7974 6573 3332 222c  Type":"bytes32",
-00021eb0: 226e 616d 6522 3a22 5f70 6163 6b65 6446  "name":"_packedF
-00021ec0: 6565 5061 7261 6d65 7465 7273 222c 2274  eeParameters","t
-00021ed0: 7970 6522 3a22 6279 7465 7333 3222 7d5d  ype":"bytes32"}]
-00021ee0: 2c22 6e61 6d65 223a 2273 6574 4665 6573  ,"name":"setFees
-00021ef0: 5061 7261 6d65 7465 7273 222c 226f 7574  Parameters","out
-00021f00: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
-00021f10: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
-00021f20: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
-00021f30: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
-00021f40: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
-00021f50: 5479 7065 223a 2262 7974 6573 3422 2c22  Type":"bytes4","
-00021f60: 6e61 6d65 223a 225f 696e 7465 7266 6163  name":"_interfac
-00021f70: 6549 6422 2c22 7479 7065 223a 2262 7974  eId","type":"byt
-00021f80: 6573 3422 7d5d 2c22 6e61 6d65 223a 2273  es4"}],"name":"s
-00021f90: 7570 706f 7274 7349 6e74 6572 6661 6365  upportsInterface
-00021fa0: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
-00021fb0: 6e74 6572 6e61 6c54 7970 6522 3a22 626f  nternalType":"bo
-00021fc0: 6f6c 222c 226e 616d 6522 3a22 222c 2274  ol","name":"","t
-00021fd0: 7970 6522 3a22 626f 6f6c 227d 5d2c 2273  ype":"bool"}],"s
-00021fe0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
-00021ff0: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
-00022000: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
-00022010: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00022020: 7970 6522 3a22 626f 6f6c 222c 226e 616d  ype":"bool","nam
-00022030: 6522 3a22 5f73 7761 7046 6f72 5922 2c22  e":"_swapForY","
-00022040: 7479 7065 223a 2262 6f6f 6c22 7d2c 7b22  type":"bool"},{"
-00022050: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
-00022060: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
-00022070: 5f74 6f22 2c22 7479 7065 223a 2261 6464  _to","type":"add
-00022080: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
-00022090: 7377 6170 222c 226f 7574 7075 7473 223a  swap","outputs":
-000220a0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
-000220b0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-000220c0: 223a 2261 6d6f 756e 7458 4f75 7422 2c22  ":"amountXOut","
-000220d0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-000220e0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
-000220f0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
-00022100: 223a 2261 6d6f 756e 7459 4f75 7422 2c22  ":"amountYOut","
-00022110: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
-00022120: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
-00022130: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
-00022140: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
-00022150: 6e22 7d2c 7b22 696e 7075 7473 223a 5b5d  n"},{"inputs":[]
-00022160: 2c22 6e61 6d65 223a 2273 796d 626f 6c22  ,"name":"symbol"
-00022170: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
-00022180: 7465 726e 616c 5479 7065 223a 2273 7472  ternalType":"str
-00022190: 696e 6722 2c22 6e61 6d65 223a 2222 2c22  ing","name":"","
-000221a0: 7479 7065 223a 2273 7472 696e 6722 7d5d  type":"string"}]
-000221b0: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
-000221c0: 7922 3a22 7075 7265 222c 2274 7970 6522  y":"pure","type"
-000221d0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
-000221e0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
-000221f0: 3a22 746f 6b65 6e58 222c 226f 7574 7075  :"tokenX","outpu
-00022200: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
-00022210: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
-00022220: 4552 4332 3022 2c22 6e61 6d65 223a 2222  ERC20","name":""
-00022230: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
-00022240: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
-00022250: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
-00022260: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
-00022270: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
-00022280: 6d65 223a 2274 6f6b 656e 5922 2c22 6f75  me":"tokenY","ou
-00022290: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-000222a0: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
-000222b0: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
-000222c0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
-000222d0: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
-000222e0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
-000222f0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
-00022300: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
-00022310: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
-00022320: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
-00022330: 5f69 6422 2c22 7479 7065 223a 2275 696e  _id","type":"uin
-00022340: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
-00022350: 746f 7461 6c53 7570 706c 7922 2c22 6f75  totalSupply","ou
-00022360: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
-00022370: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
-00022380: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
-00022390: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
-000223a0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
-000223b0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
-000223c0: 6675 6e63 7469 6f6e 227d 5d27 290a 0a20  function"}]').. 
-000223d0: 2020 2023 2072 6574 7572 6e73 2028 7569     # returns (ui
-000223e0: 6e74 3235 3620 7265 7365 7276 6558 2c20  nt256 reserveX, 
-000223f0: 7569 6e74 3235 3620 7265 7365 7276 6559  uint256 reserveY
-00022400: 2c20 7569 6e74 3235 3620 6163 7469 7665  , uint256 active
-00022410: 4964 290a 2020 2020 6465 6620 6765 745f  Id).    def get_
-00022420: 7265 7365 7276 655f 616e 645f 6964 285f  reserve_and_id(_
-00022430: 7765 6233 3a57 6562 332c 5f70 6169 725f  web3:Web3,_pair_
-00022440: 6164 6472 6573 733a 7374 7229 3a0a 2020  address:str):.  
-00022450: 2020 2020 2020 7061 6972 5f63 6f6e 7472        pair_contr
-00022460: 6163 743d 5f77 6562 332e 6574 682e 636f  act=_web3.eth.co
-00022470: 6e74 7261 6374 2861 6464 7265 7373 3d5f  ntract(address=_
-00022480: 7061 6972 5f61 6464 7265 7373 2c20 6162  pair_address, ab
-00022490: 693d 4a6f 6556 3250 6169 722e 6a6f 655f  i=JoeV2Pair.joe_
-000224a0: 7061 6972 5f76 325f 6162 6929 0a20 2020  pair_v2_abi).   
-000224b0: 2020 2020 2072 6574 7572 6e20 7061 6972       return pair
-000224c0: 5f63 6f6e 7472 6163 742e 6675 6e63 7469  _contract.functi
-000224d0: 6f6e 732e 6765 7452 6573 6572 7665 7341  ons.getReservesA
-000224e0: 6e64 4964 2829 2e63 616c 6c28 290a 0a20  ndId().call().. 
-000224f0: 2020 2023 2066 756e 6374 696f 6e20 6765     # function ge
-00022500: 7447 6c6f 6261 6c46 6565 7328 2920 6578  tGlobalFees() ex
-00022510: 7465 726e 616c 2076 6965 7720 6f76 6572  ternal view over
-00022520: 7269 6465 2072 6574 7572 6e73 2028 7569  ride returns (ui
-00022530: 6e74 3235 3620 6665 6573 5854 6f74 616c  nt256 feesXTotal
-00022540: 2c20 7569 6e74 3235 3620 6665 6573 5954  , uint256 feesYT
-00022550: 6f74 616c 2c20 7569 6e74 3235 3620 6665  otal, uint256 fe
-00022560: 6573 5850 726f 746f 636f 6c2c 2075 696e  esXProtocol, uin
-00022570: 7432 3536 2066 6565 7359 5072 6f74 6f63  t256 feesYProtoc
-00022580: 6f6c 290a 2020 2020 6465 6620 6765 745f  ol).    def get_
-00022590: 676c 6f62 616c 5f66 6565 285f 7765 6233  global_fee(_web3
-000225a0: 3a57 6562 332c 5f70 6169 725f 6164 6472  :Web3,_pair_addr
-000225b0: 6573 733a 7374 7229 3a0a 2020 2020 2020  ess:str):.      
-000225c0: 2020 7061 6972 5f63 6f6e 7472 6163 743d    pair_contract=
-000225d0: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
-000225e0: 6374 2861 6464 7265 7373 3d5f 7061 6972  ct(address=_pair
-000225f0: 5f61 6464 7265 7373 2c20 6162 693d 4a6f  _address, abi=Jo
-00022600: 6556 3250 6169 722e 6a6f 655f 7061 6972  eV2Pair.joe_pair
-00022610: 5f76 325f 6162 6929 0a20 2020 2020 2020  _v2_abi).       
-00022620: 2072 6574 7572 6e20 7061 6972 5f63 6f6e   return pair_con
-00022630: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
-00022640: 6765 7447 6c6f 6261 6c46 6565 7328 292e  getGlobalFees().
-00022650: 6361 6c6c 2829 0a0a 2020 2020 2320 6675  call()..    # fu
-00022660: 6e63 7469 6f6e 2066 696e 6446 6972 7374  nction findFirst
-00022670: 4e6f 6e45 6d70 7479 4269 6e49 6428 7569  NonEmptyBinId(ui
-00022680: 6e74 3234 205f 6964 2c20 626f 6f6c 205f  nt24 _id, bool _
-00022690: 7377 6170 466f 7259 2920 6578 7465 726e  swapForY) extern
-000226a0: 616c 2076 6965 7720 6f76 6572 7269 6465  al view override
-000226b0: 2072 6574 7572 6e73 2028 7569 6e74 3234   returns (uint24
-000226c0: 290a 2020 2020 6465 6620 6669 6e64 5f66  ).    def find_f
-000226d0: 6972 7374 5f6e 6f6e 5f65 6d70 7479 5f62  irst_non_empty_b
-000226e0: 696e 5f69 6428 5f77 6562 333a 5765 6233  in_id(_web3:Web3
-000226f0: 2c5f 7061 6972 5f61 6464 7265 7373 3a73  ,_pair_address:s
-00022700: 7472 2c5f 6964 2c5f 7377 6170 5f66 6f72  tr,_id,_swap_for
-00022710: 5f79 293a 0a20 2020 2020 2020 2070 6169  _y):.        pai
-00022720: 725f 636f 6e74 7261 6374 3d5f 7765 6233  r_contract=_web3
-00022730: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
-00022740: 6472 6573 733d 5f70 6169 725f 6164 6472  dress=_pair_addr
-00022750: 6573 732c 2061 6269 3d4a 6f65 5632 5061  ess, abi=JoeV2Pa
-00022760: 6972 2e6a 6f65 5f70 6169 725f 7632 5f61  ir.joe_pair_v2_a
-00022770: 6269 290a 2020 2020 2020 2020 7265 7475  bi).        retu
-00022780: 726e 2070 6169 725f 636f 6e74 7261 6374  rn pair_contract
-00022790: 2e66 756e 6374 696f 6e73 2e66 696e 6446  .functions.findF
-000227a0: 6972 7374 4e6f 6e45 6d70 7479 4269 6e49  irstNonEmptyBinI
-000227b0: 6428 5f69 642c 5f73 7761 705f 666f 725f  d(_id,_swap_for_
-000227c0: 7929 2e63 616c 6c28 290a 0a20 2020 2023  y).call()..    #
-000227d0: 2066 756e 6374 696f 6e20 6765 7442 696e   function getBin
-000227e0: 2875 696e 7432 3420 5f69 6429 2065 7874  (uint24 _id) ext
-000227f0: 6572 6e61 6c20 7669 6577 206f 7665 7272  ernal view overr
-00022800: 6964 6520 7265 7475 726e 7320 2875 696e  ide returns (uin
-00022810: 7432 3536 2072 6573 6572 7665 582c 2075  t256 reserveX, u
-00022820: 696e 7432 3536 2072 6573 6572 7665 5929  int256 reserveY)
-00022830: 0a20 2020 2064 6566 2067 6574 5f62 696e  .    def get_bin
-00022840: 285f 7765 6233 3a57 6562 332c 5f70 6169  (_web3:Web3,_pai
-00022850: 725f 6164 6472 6573 733a 7374 722c 5f69  r_address:str,_i
-00022860: 6429 3a0a 2020 2020 2020 2020 7061 6972  d):.        pair
-00022870: 5f63 6f6e 7472 6163 743d 5f77 6562 332e  _contract=_web3.
-00022880: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
-00022890: 7265 7373 3d5f 7061 6972 5f61 6464 7265  ress=_pair_addre
-000228a0: 7373 2c20 6162 693d 4a6f 6556 3250 6169  ss, abi=JoeV2Pai
-000228b0: 722e 6a6f 655f 7061 6972 5f76 325f 6162  r.joe_pair_v2_ab
-000228c0: 6929 0a20 2020 2020 2020 2072 6574 7572  i).        retur
-000228d0: 6e20 7061 6972 5f63 6f6e 7472 6163 742e  n pair_contract.
-000228e0: 6675 6e63 7469 6f6e 732e 6765 7442 696e  functions.getBin
-000228f0: 285f 6964 292e 6361 6c6c 2829 0a0a 2020  (_id).call()..  
-00022900: 2020 2320 6675 6e63 7469 6f6e 2073 7761    # function swa
-00022910: 7028 626f 6f6c 205f 7377 6170 466f 7259  p(bool _swapForY
-00022920: 2c20 6164 6472 6573 7320 5f74 6f29 2065  , address _to) e
-00022930: 7874 6572 6e61 6c20 6f76 6572 7269 6465  xternal override
-00022940: 206e 6f6e 5265 656e 7472 616e 7420 7265   nonReentrant re
-00022950: 7475 726e 7320 2875 696e 7432 3536 2061  turns (uint256 a
-00022960: 6d6f 756e 7458 4f75 742c 2075 696e 7432  mountXOut, uint2
-00022970: 3536 2061 6d6f 756e 7459 4f75 7429 0a20  56 amountYOut). 
-00022980: 2020 2064 6566 2073 7761 7028 5f77 6562     def swap(_web
-00022990: 333a 5765 6233 2c5f 7061 6972 5f61 6464  3:Web3,_pair_add
-000229a0: 7265 7373 3a73 7472 2c5f 7377 6170 5f66  ress:str,_swap_f
-000229b0: 6f72 5f79 2c5f 746f 293a 0a20 2020 2020  or_y,_to):.     
-000229c0: 2020 2070 6169 725f 636f 6e74 7261 6374     pair_contract
-000229d0: 3d5f 7765 6233 2e65 7468 2e63 6f6e 7472  =_web3.eth.contr
-000229e0: 6163 7428 6164 6472 6573 733d 5f70 6169  act(address=_pai
-000229f0: 725f 6164 6472 6573 732c 2061 6269 3d4a  r_address, abi=J
-00022a00: 6f65 5632 5061 6972 2e6a 6f65 5f70 6169  oeV2Pair.joe_pai
-00022a10: 725f 7632 5f61 6269 290a 2020 2020 2020  r_v2_abi).      
-00022a20: 2020 7265 7475 726e 2070 6169 725f 636f    return pair_co
-00022a30: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
-00022a40: 2e73 7761 7028 5f73 7761 705f 666f 725f  .swap(_swap_for_
-00022a50: 792c 5f74 6f29 2e63 616c 6c28 29         y,_to).call()
+000202c0: 7432 3536 5b5d 222c 226e 616d 6522 3a22  t256[]","name":"
+000202d0: 5f69 6473 222c 2274 7970 6522 3a22 7569  _ids","type":"ui
+000202e0: 6e74 3235 365b 5d22 7d2c 7b22 696e 7465  nt256[]"},{"inte
+000202f0: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00020300: 3536 5b5d 222c 226e 616d 6522 3a22 5f61  56[]","name":"_a
+00020310: 6d6f 756e 7473 222c 2274 7970 6522 3a22  mounts","type":"
+00020320: 7569 6e74 3235 365b 5d22 7d2c 7b22 696e  uint256[]"},{"in
+00020330: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+00020340: 7265 7373 222c 226e 616d 6522 3a22 5f74  ress","name":"_t
+00020350: 6f22 2c22 7479 7065 223a 2261 6464 7265  o","type":"addre
+00020360: 7373 227d 5d2c 226e 616d 6522 3a22 6275  ss"}],"name":"bu
+00020370: 726e 222c 226f 7574 7075 7473 223a 5b7b  rn","outputs":[{
+00020380: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00020390: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+000203a0: 2261 6d6f 756e 7458 222c 2274 7970 6522  "amountX","type"
+000203b0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+000203c0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+000203d0: 7432 3536 222c 226e 616d 6522 3a22 616d  t256","name":"am
+000203e0: 6f75 6e74 5922 2c22 7479 7065 223a 2275  ountY","type":"u
+000203f0: 696e 7432 3536 227d 5d2c 2273 7461 7465  int256"}],"state
+00020400: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+00020410: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+00020420: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00020430: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00020440: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+00020450: 2c22 6e61 6d65 223a 225f 6163 636f 756e  ,"name":"_accoun
+00020460: 7422 2c22 7479 7065 223a 2261 6464 7265  t","type":"addre
+00020470: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+00020480: 7970 6522 3a22 7569 6e74 3235 365b 5d22  ype":"uint256[]"
+00020490: 2c22 6e61 6d65 223a 225f 6964 7322 2c22  ,"name":"_ids","
+000204a0: 7479 7065 223a 2275 696e 7432 3536 5b5d  type":"uint256[]
+000204b0: 227d 5d2c 226e 616d 6522 3a22 636f 6c6c  "}],"name":"coll
+000204c0: 6563 7446 6565 7322 2c22 6f75 7470 7574  ectFees","output
+000204d0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+000204e0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000204f0: 616d 6522 3a22 616d 6f75 6e74 5822 2c22  ame":"amountX","
+00020500: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00020510: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00020520: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00020530: 223a 2261 6d6f 756e 7459 222c 2274 7970  ":"amountY","typ
+00020540: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+00020550: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00020560: 3a22 6e6f 6e70 6179 6162 6c65 222c 2274  :"nonpayable","t
+00020570: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00020580: 2c7b 2269 6e70 7574 7322 3a5b 5d2c 226e  ,{"inputs":[],"n
+00020590: 616d 6522 3a22 636f 6c6c 6563 7450 726f  ame":"collectPro
+000205a0: 746f 636f 6c46 6565 7322 2c22 6f75 7470  tocolFees","outp
+000205b0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+000205c0: 5479 7065 223a 2275 696e 7431 3238 222c  Type":"uint128",
+000205d0: 226e 616d 6522 3a22 616d 6f75 6e74 5822  "name":"amountX"
+000205e0: 2c22 7479 7065 223a 2275 696e 7431 3238  ,"type":"uint128
+000205f0: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00020600: 6522 3a22 7569 6e74 3132 3822 2c22 6e61  e":"uint128","na
+00020610: 6d65 223a 2261 6d6f 756e 7459 222c 2274  me":"amountY","t
+00020620: 7970 6522 3a22 7569 6e74 3132 3822 7d5d  ype":"uint128"}]
+00020630: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+00020640: 7922 3a22 6e6f 6e70 6179 6162 6c65 222c  y":"nonpayable",
+00020650: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00020660: 227d 2c7b 2269 6e70 7574 7322 3a5b 5d2c  "},{"inputs":[],
+00020670: 226e 616d 6522 3a22 6661 6374 6f72 7922  "name":"factory"
+00020680: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+00020690: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+000206a0: 7472 6163 7420 494c 4246 6163 746f 7279  tract ILBFactory
+000206b0: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
+000206c0: 6522 3a22 6164 6472 6573 7322 7d5d 2c22  e":"address"}],"
+000206d0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+000206e0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
+000206f0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00020700: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+00020710: 6665 6550 6172 616d 6574 6572 7322 2c22  feeParameters","
+00020720: 6f75 7470 7574 7322 3a5b 7b22 636f 6d70  outputs":[{"comp
+00020730: 6f6e 656e 7473 223a 5b7b 2269 6e74 6572  onents":[{"inter
+00020740: 6e61 6c54 7970 6522 3a22 7569 6e74 3136  nalType":"uint16
+00020750: 222c 226e 616d 6522 3a22 6269 6e53 7465  ","name":"binSte
+00020760: 7022 2c22 7479 7065 223a 2275 696e 7431  p","type":"uint1
+00020770: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+00020780: 7065 223a 2275 696e 7431 3622 2c22 6e61  pe":"uint16","na
+00020790: 6d65 223a 2262 6173 6546 6163 746f 7222  me":"baseFactor"
+000207a0: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
+000207b0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+000207c0: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
+000207d0: 223a 2266 696c 7465 7250 6572 696f 6422  ":"filterPeriod"
+000207e0: 2c22 7479 7065 223a 2275 696e 7431 3622  ,"type":"uint16"
+000207f0: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00020800: 223a 2275 696e 7431 3622 2c22 6e61 6d65  ":"uint16","name
+00020810: 223a 2264 6563 6179 5065 7269 6f64 222c  ":"decayPeriod",
+00020820: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
+00020830: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00020840: 3a22 7569 6e74 3136 222c 226e 616d 6522  :"uint16","name"
+00020850: 3a22 7265 6475 6374 696f 6e46 6163 746f  :"reductionFacto
+00020860: 7222 2c22 7479 7065 223a 2275 696e 7431  r","type":"uint1
+00020870: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+00020880: 7065 223a 2275 696e 7432 3422 2c22 6e61  pe":"uint24","na
+00020890: 6d65 223a 2276 6172 6961 626c 6546 6565  me":"variableFee
+000208a0: 436f 6e74 726f 6c22 2c22 7479 7065 223a  Control","type":
+000208b0: 2275 696e 7432 3422 7d2c 7b22 696e 7465  "uint24"},{"inte
+000208c0: 726e 616c 5479 7065 223a 2275 696e 7431  rnalType":"uint1
+000208d0: 3622 2c22 6e61 6d65 223a 2270 726f 746f  6","name":"proto
+000208e0: 636f 6c53 6861 7265 222c 2274 7970 6522  colShare","type"
+000208f0: 3a22 7569 6e74 3136 227d 2c7b 2269 6e74  :"uint16"},{"int
+00020900: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00020910: 3234 222c 226e 616d 6522 3a22 6d61 7856  24","name":"maxV
+00020920: 6f6c 6174 696c 6974 7941 6363 756d 756c  olatilityAccumul
+00020930: 6174 6564 222c 2274 7970 6522 3a22 7569  ated","type":"ui
+00020940: 6e74 3234 227d 2c7b 2269 6e74 6572 6e61  nt24"},{"interna
+00020950: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
+00020960: 226e 616d 6522 3a22 766f 6c61 7469 6c69  "name":"volatili
+00020970: 7479 4163 6375 6d75 6c61 7465 6422 2c22  tyAccumulated","
+00020980: 7479 7065 223a 2275 696e 7432 3422 7d2c  type":"uint24"},
+00020990: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000209a0: 2275 696e 7432 3422 2c22 6e61 6d65 223a  "uint24","name":
+000209b0: 2276 6f6c 6174 696c 6974 7952 6566 6572  "volatilityRefer
+000209c0: 656e 6365 222c 2274 7970 6522 3a22 7569  ence","type":"ui
+000209d0: 6e74 3234 227d 2c7b 2269 6e74 6572 6e61  nt24"},{"interna
+000209e0: 6c54 7970 6522 3a22 7569 6e74 3234 222c  lType":"uint24",
+000209f0: 226e 616d 6522 3a22 696e 6465 7852 6566  "name":"indexRef
+00020a00: 222c 2274 7970 6522 3a22 7569 6e74 3234  ","type":"uint24
+00020a10: 227d 2c7b 2269 6e74 6572 6e61 6c54 7970  "},{"internalTyp
+00020a20: 6522 3a22 7569 6e74 3430 222c 226e 616d  e":"uint40","nam
+00020a30: 6522 3a22 7469 6d65 222c 2274 7970 6522  e":"time","type"
+00020a40: 3a22 7569 6e74 3430 227d 5d2c 2269 6e74  :"uint40"}],"int
+00020a50: 6572 6e61 6c54 7970 6522 3a22 7374 7275  ernalType":"stru
+00020a60: 6374 2046 6565 4865 6c70 6572 2e46 6565  ct FeeHelper.Fee
+00020a70: 5061 7261 6d65 7465 7273 222c 226e 616d  Parameters","nam
+00020a80: 6522 3a22 222c 2274 7970 6522 3a22 7475  e":"","type":"tu
+00020a90: 706c 6522 7d5d 2c22 7374 6174 654d 7574  ple"}],"stateMut
+00020aa0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+00020ab0: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00020ac0: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00020ad0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00020ae0: 696e 7432 3422 2c22 6e61 6d65 223a 225f  int24","name":"_
+00020af0: 6964 222c 2274 7970 6522 3a22 7569 6e74  id","type":"uint
+00020b00: 3234 227d 2c7b 2269 6e74 6572 6e61 6c54  24"},{"internalT
+00020b10: 7970 6522 3a22 626f 6f6c 222c 226e 616d  ype":"bool","nam
+00020b20: 6522 3a22 5f73 7761 7046 6f72 5922 2c22  e":"_swapForY","
+00020b30: 7479 7065 223a 2262 6f6f 6c22 7d5d 2c22  type":"bool"}],"
+00020b40: 6e61 6d65 223a 2266 696e 6446 6972 7374  name":"findFirst
+00020b50: 4e6f 6e45 6d70 7479 4269 6e49 6422 2c22  NonEmptyBinId","
+00020b60: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+00020b70: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00020b80: 3422 2c22 6e61 6d65 223a 2222 2c22 7479  4","name":"","ty
+00020b90: 7065 223a 2275 696e 7432 3422 7d5d 2c22  pe":"uint24"}],"
+00020ba0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+00020bb0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
+00020bc0: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00020bd0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00020be0: 5479 7065 223a 2263 6f6e 7472 6163 7420  Type":"contract 
+00020bf0: 494c 4246 6c61 7368 4c6f 616e 4361 6c6c  ILBFlashLoanCall
+00020c00: 6261 636b 222c 226e 616d 6522 3a22 5f72  back","name":"_r
+00020c10: 6563 6569 7665 7222 2c22 7479 7065 223a  eceiver","type":
+00020c20: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+00020c30: 6572 6e61 6c54 7970 6522 3a22 636f 6e74  ernalType":"cont
+00020c40: 7261 6374 2049 4552 4332 3022 2c22 6e61  ract IERC20","na
+00020c50: 6d65 223a 225f 746f 6b65 6e22 2c22 7479  me":"_token","ty
+00020c60: 7065 223a 2261 6464 7265 7373 227d 2c7b  pe":"address"},{
+00020c70: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00020c80: 7569 6e74 3235 3622 2c22 6e61 6d65 223a  uint256","name":
+00020c90: 225f 616d 6f75 6e74 222c 2274 7970 6522  "_amount","type"
+00020ca0: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+00020cb0: 7465 726e 616c 5479 7065 223a 2262 7974  ternalType":"byt
+00020cc0: 6573 222c 226e 616d 6522 3a22 5f64 6174  es","name":"_dat
+00020cd0: 6122 2c22 7479 7065 223a 2262 7974 6573  a","type":"bytes
+00020ce0: 227d 5d2c 226e 616d 6522 3a22 666c 6173  "}],"name":"flas
+00020cf0: 684c 6f61 6e22 2c22 6f75 7470 7574 7322  hLoan","outputs"
+00020d00: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
+00020d10: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
+00020d20: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
+00020d30: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+00020d40: 5b5d 2c22 6e61 6d65 223a 2266 6f72 6365  [],"name":"force
+00020d50: 4465 6361 7922 2c22 6f75 7470 7574 7322  Decay","outputs"
+00020d60: 3a5b 5d2c 2273 7461 7465 4d75 7461 6269  :[],"stateMutabi
+00020d70: 6c69 7479 223a 226e 6f6e 7061 7961 626c  lity":"nonpayabl
+00020d80: 6522 2c22 7479 7065 223a 2266 756e 6374  e","type":"funct
+00020d90: 696f 6e22 7d2c 7b22 696e 7075 7473 223a  ion"},{"inputs":
+00020da0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+00020db0: 3a22 7569 6e74 3234 222c 226e 616d 6522  :"uint24","name"
+00020dc0: 3a22 5f69 6422 2c22 7479 7065 223a 2275  :"_id","type":"u
+00020dd0: 696e 7432 3422 7d5d 2c22 6e61 6d65 223a  int24"}],"name":
+00020de0: 2267 6574 4269 6e22 2c22 6f75 7470 7574  "getBin","output
+00020df0: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00020e00: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00020e10: 616d 6522 3a22 7265 7365 7276 6558 222c  ame":"reserveX",
+00020e20: 2274 7970 6522 3a22 7569 6e74 3235 3622  "type":"uint256"
+00020e30: 7d2c 7b22 696e 7465 726e 616c 5479 7065  },{"internalType
+00020e40: 223a 2275 696e 7432 3536 222c 226e 616d  ":"uint256","nam
+00020e50: 6522 3a22 7265 7365 7276 6559 222c 2274  e":"reserveY","t
+00020e60: 7970 6522 3a22 7569 6e74 3235 3622 7d5d  ype":"uint256"}]
+00020e70: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+00020e80: 7922 3a22 7669 6577 222c 2274 7970 6522  y":"view","type"
+00020e90: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+00020ea0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+00020eb0: 3a22 6765 7447 6c6f 6261 6c46 6565 7322  :"getGlobalFees"
+00020ec0: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+00020ed0: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00020ee0: 7431 3238 222c 226e 616d 6522 3a22 6665  t128","name":"fe
+00020ef0: 6573 5854 6f74 616c 222c 2274 7970 6522  esXTotal","type"
+00020f00: 3a22 7569 6e74 3132 3822 7d2c 7b22 696e  :"uint128"},{"in
+00020f10: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00020f20: 7431 3238 222c 226e 616d 6522 3a22 6665  t128","name":"fe
+00020f30: 6573 5954 6f74 616c 222c 2274 7970 6522  esYTotal","type"
+00020f40: 3a22 7569 6e74 3132 3822 7d2c 7b22 696e  :"uint128"},{"in
+00020f50: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00020f60: 7431 3238 222c 226e 616d 6522 3a22 6665  t128","name":"fe
+00020f70: 6573 5850 726f 746f 636f 6c22 2c22 7479  esXProtocol","ty
+00020f80: 7065 223a 2275 696e 7431 3238 227d 2c7b  pe":"uint128"},{
+00020f90: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+00020fa0: 7569 6e74 3132 3822 2c22 6e61 6d65 223a  uint128","name":
+00020fb0: 2266 6565 7359 5072 6f74 6f63 6f6c 222c  "feesYProtocol",
+00020fc0: 2274 7970 6522 3a22 7569 6e74 3132 3822  "type":"uint128"
+00020fd0: 7d5d 2c22 7374 6174 654d 7574 6162 696c  }],"stateMutabil
+00020fe0: 6974 7922 3a22 7669 6577 222c 2274 7970  ity":"view","typ
+00020ff0: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00021000: 2269 6e70 7574 7322 3a5b 5d2c 226e 616d  "inputs":[],"nam
+00021010: 6522 3a22 6765 744f 7261 636c 6550 6172  e":"getOraclePar
+00021020: 616d 6574 6572 7322 2c22 6f75 7470 7574  ameters","output
+00021030: 7322 3a5b 7b22 696e 7465 726e 616c 5479  s":[{"internalTy
+00021040: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00021050: 616d 6522 3a22 6f72 6163 6c65 5361 6d70  ame":"oracleSamp
+00021060: 6c65 4c69 6665 7469 6d65 222c 2274 7970  leLifetime","typ
+00021070: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+00021080: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00021090: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000210a0: 6f72 6163 6c65 5369 7a65 222c 2274 7970  oracleSize","typ
+000210b0: 6522 3a22 7569 6e74 3235 3622 7d2c 7b22  e":"uint256"},{"
+000210c0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000210d0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000210e0: 6f72 6163 6c65 4163 7469 7665 5369 7a65  oracleActiveSize
+000210f0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00021100: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+00021110: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+00021120: 616d 6522 3a22 6f72 6163 6c65 4c61 7374  ame":"oracleLast
+00021130: 5469 6d65 7374 616d 7022 2c22 7479 7065  Timestamp","type
+00021140: 223a 2275 696e 7432 3536 227d 2c7b 2269  ":"uint256"},{"i
+00021150: 6e74 6572 6e61 6c54 7970 6522 3a22 7569  nternalType":"ui
+00021160: 6e74 3235 3622 2c22 6e61 6d65 223a 226f  nt256","name":"o
+00021170: 7261 636c 6549 6422 2c22 7479 7065 223a  racleId","type":
+00021180: 2275 696e 7432 3536 227d 2c7b 2269 6e74  "uint256"},{"int
+00021190: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+000211a0: 3235 3622 2c22 6e61 6d65 223a 226d 696e  256","name":"min
+000211b0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+000211c0: 3622 7d2c 7b22 696e 7465 726e 616c 5479  6"},{"internalTy
+000211d0: 7065 223a 2275 696e 7432 3536 222c 226e  pe":"uint256","n
+000211e0: 616d 6522 3a22 6d61 7822 2c22 7479 7065  ame":"max","type
+000211f0: 223a 2275 696e 7432 3536 227d 5d2c 2273  ":"uint256"}],"s
+00021200: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+00021210: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
+00021220: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+00021230: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00021240: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00021250: 6e61 6d65 223a 225f 7469 6d65 4465 6c74  name":"_timeDelt
+00021260: 6122 2c22 7479 7065 223a 2275 696e 7432  a","type":"uint2
+00021270: 3536 227d 5d2c 226e 616d 6522 3a22 6765  56"}],"name":"ge
+00021280: 744f 7261 636c 6553 616d 706c 6546 726f  tOracleSampleFro
+00021290: 6d22 2c22 6f75 7470 7574 7322 3a5b 7b22  m","outputs":[{"
+000212a0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000212b0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+000212c0: 6375 6d75 6c61 7469 7665 4964 222c 2274  cumulativeId","t
+000212d0: 7970 6522 3a22 7569 6e74 3235 3622 7d2c  ype":"uint256"},
+000212e0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000212f0: 2275 696e 7432 3536 222c 226e 616d 6522  "uint256","name"
+00021300: 3a22 6375 6d75 6c61 7469 7665 566f 6c61  :"cumulativeVola
+00021310: 7469 6c69 7479 4163 6375 6d75 6c61 7465  tilityAccumulate
+00021320: 6422 2c22 7479 7065 223a 2275 696e 7432  d","type":"uint2
+00021330: 3536 227d 2c7b 2269 6e74 6572 6e61 6c54  56"},{"internalT
+00021340: 7970 6522 3a22 7569 6e74 3235 3622 2c22  ype":"uint256","
+00021350: 6e61 6d65 223a 2263 756d 756c 6174 6976  name":"cumulativ
+00021360: 6542 696e 4372 6f73 7365 6422 2c22 7479  eBinCrossed","ty
+00021370: 7065 223a 2275 696e 7432 3536 227d 5d2c  pe":"uint256"}],
+00021380: 2273 7461 7465 4d75 7461 6269 6c69 7479  "stateMutability
+00021390: 223a 2276 6965 7722 2c22 7479 7065 223a  ":"view","type":
+000213a0: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+000213b0: 7075 7473 223a 5b5d 2c22 6e61 6d65 223a  puts":[],"name":
+000213c0: 2267 6574 5265 7365 7276 6573 416e 6449  "getReservesAndI
+000213d0: 6422 2c22 6f75 7470 7574 7322 3a5b 7b22  d","outputs":[{"
+000213e0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+000213f0: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00021400: 7265 7365 7276 6558 222c 2274 7970 6522  reserveX","type"
+00021410: 3a22 7569 6e74 3235 3622 7d2c 7b22 696e  :"uint256"},{"in
+00021420: 7465 726e 616c 5479 7065 223a 2275 696e  ternalType":"uin
+00021430: 7432 3536 222c 226e 616d 6522 3a22 7265  t256","name":"re
+00021440: 7365 7276 6559 222c 2274 7970 6522 3a22  serveY","type":"
+00021450: 7569 6e74 3235 3622 7d2c 7b22 696e 7465  uint256"},{"inte
+00021460: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00021470: 3536 222c 226e 616d 6522 3a22 6163 7469  56","name":"acti
+00021480: 7665 4964 222c 2274 7970 6522 3a22 7569  veId","type":"ui
+00021490: 6e74 3235 3622 7d5d 2c22 7374 6174 654d  nt256"}],"stateM
+000214a0: 7574 6162 696c 6974 7922 3a22 7669 6577  utability":"view
+000214b0: 222c 2274 7970 6522 3a22 6675 6e63 7469  ","type":"functi
+000214c0: 6f6e 227d 2c7b 2269 6e70 7574 7322 3a5b  on"},{"inputs":[
+000214d0: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+000214e0: 2275 696e 7431 3622 2c22 6e61 6d65 223a  "uint16","name":
+000214f0: 225f 6e65 774c 656e 6774 6822 2c22 7479  "_newLength","ty
+00021500: 7065 223a 2275 696e 7431 3622 7d5d 2c22  pe":"uint16"}],"
+00021510: 6e61 6d65 223a 2269 6e63 7265 6173 654f  name":"increaseO
+00021520: 7261 636c 654c 656e 6774 6822 2c22 6f75  racleLength","ou
+00021530: 7470 7574 7322 3a5b 5d2c 2273 7461 7465  tputs":[],"state
+00021540: 4d75 7461 6269 6c69 7479 223a 226e 6f6e  Mutability":"non
+00021550: 7061 7961 626c 6522 2c22 7479 7065 223a  payable","type":
+00021560: 2266 756e 6374 696f 6e22 7d2c 7b22 696e  "function"},{"in
+00021570: 7075 7473 223a 5b7b 2269 6e74 6572 6e61  puts":[{"interna
+00021580: 6c54 7970 6522 3a22 636f 6e74 7261 6374  lType":"contract
+00021590: 2049 4552 4332 3022 2c22 6e61 6d65 223a   IERC20","name":
+000215a0: 225f 746f 6b65 6e58 222c 2274 7970 6522  "_tokenX","type"
+000215b0: 3a22 6164 6472 6573 7322 7d2c 7b22 696e  :"address"},{"in
+000215c0: 7465 726e 616c 5479 7065 223a 2263 6f6e  ternalType":"con
+000215d0: 7472 6163 7420 4945 5243 3230 222c 226e  tract IERC20","n
+000215e0: 616d 6522 3a22 5f74 6f6b 656e 5922 2c22  ame":"_tokenY","
+000215f0: 7479 7065 223a 2261 6464 7265 7373 227d  type":"address"}
+00021600: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00021610: 3a22 7569 6e74 3234 222c 226e 616d 6522  :"uint24","name"
+00021620: 3a22 5f61 6374 6976 6549 6422 2c22 7479  :"_activeId","ty
+00021630: 7065 223a 2275 696e 7432 3422 7d2c 7b22  pe":"uint24"},{"
+00021640: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00021650: 696e 7431 3622 2c22 6e61 6d65 223a 225f  int16","name":"_
+00021660: 7361 6d70 6c65 4c69 6665 7469 6d65 222c  sampleLifetime",
+00021670: 2274 7970 6522 3a22 7569 6e74 3136 227d  "type":"uint16"}
+00021680: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00021690: 3a22 6279 7465 7333 3222 2c22 6e61 6d65  :"bytes32","name
+000216a0: 223a 225f 7061 636b 6564 4665 6550 6172  ":"_packedFeePar
+000216b0: 616d 6574 6572 7322 2c22 7479 7065 223a  ameters","type":
+000216c0: 2262 7974 6573 3332 227d 5d2c 226e 616d  "bytes32"}],"nam
+000216d0: 6522 3a22 696e 6974 6961 6c69 7a65 222c  e":"initialize",
+000216e0: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+000216f0: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00021700: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+00021710: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00021720: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00021730: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+00021740: 7373 222c 226e 616d 6522 3a22 5f6f 776e  ss","name":"_own
+00021750: 6572 222c 2274 7970 6522 3a22 6164 6472  er","type":"addr
+00021760: 6573 7322 7d2c 7b22 696e 7465 726e 616c  ess"},{"internal
+00021770: 5479 7065 223a 2261 6464 7265 7373 222c  Type":"address",
+00021780: 226e 616d 6522 3a22 5f73 7065 6e64 6572  "name":"_spender
+00021790: 222c 2274 7970 6522 3a22 6164 6472 6573  ","type":"addres
+000217a0: 7322 7d5d 2c22 6e61 6d65 223a 2269 7341  s"}],"name":"isA
+000217b0: 7070 726f 7665 6446 6f72 416c 6c22 2c22  pprovedForAll","
+000217c0: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+000217d0: 726e 616c 5479 7065 223a 2262 6f6f 6c22  rnalType":"bool"
+000217e0: 2c22 6e61 6d65 223a 2222 2c22 7479 7065  ,"name":"","type
+000217f0: 223a 2262 6f6f 6c22 7d5d 2c22 7374 6174  ":"bool"}],"stat
+00021800: 654d 7574 6162 696c 6974 7922 3a22 7669  eMutability":"vi
+00021810: 6577 222c 2274 7970 6522 3a22 6675 6e63  ew","type":"func
+00021820: 7469 6f6e 227d 2c7b 2269 6e70 7574 7322  tion"},{"inputs"
+00021830: 3a5b 7b22 696e 7465 726e 616c 5479 7065  :[{"internalType
+00021840: 223a 2275 696e 7432 3536 5b5d 222c 226e  ":"uint256[]","n
+00021850: 616d 6522 3a22 5f69 6473 222c 2274 7970  ame":"_ids","typ
+00021860: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
+00021870: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00021880: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
+00021890: 6522 3a22 5f64 6973 7472 6962 7574 696f  e":"_distributio
+000218a0: 6e58 222c 2274 7970 6522 3a22 7569 6e74  nX","type":"uint
+000218b0: 3235 365b 5d22 7d2c 7b22 696e 7465 726e  256[]"},{"intern
+000218c0: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+000218d0: 5b5d 222c 226e 616d 6522 3a22 5f64 6973  []","name":"_dis
+000218e0: 7472 6962 7574 696f 6e59 222c 2274 7970  tributionY","typ
+000218f0: 6522 3a22 7569 6e74 3235 365b 5d22 7d2c  e":"uint256[]"},
+00021900: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00021910: 2261 6464 7265 7373 222c 226e 616d 6522  "address","name"
+00021920: 3a22 5f74 6f22 2c22 7479 7065 223a 2261  :"_to","type":"a
+00021930: 6464 7265 7373 227d 5d2c 226e 616d 6522  ddress"}],"name"
+00021940: 3a22 6d69 6e74 222c 226f 7574 7075 7473  :"mint","outputs
+00021950: 223a 5b7b 2269 6e74 6572 6e61 6c54 7970  ":[{"internalTyp
+00021960: 6522 3a22 7569 6e74 3235 3622 2c22 6e61  e":"uint256","na
+00021970: 6d65 223a 2222 2c22 7479 7065 223a 2275  me":"","type":"u
+00021980: 696e 7432 3536 227d 2c7b 2269 6e74 6572  int256"},{"inter
+00021990: 6e61 6c54 7970 6522 3a22 7569 6e74 3235  nalType":"uint25
+000219a0: 3622 2c22 6e61 6d65 223a 2222 2c22 7479  6","name":"","ty
+000219b0: 7065 223a 2275 696e 7432 3536 227d 2c7b  pe":"uint256"},{
+000219c0: 2269 6e74 6572 6e61 6c54 7970 6522 3a22  "internalType":"
+000219d0: 7569 6e74 3235 365b 5d22 2c22 6e61 6d65  uint256[]","name
+000219e0: 223a 226c 6971 7569 6469 7479 4d69 6e74  ":"liquidityMint
+000219f0: 6564 222c 2274 7970 6522 3a22 7569 6e74  ed","type":"uint
+00021a00: 3235 365b 5d22 7d5d 2c22 7374 6174 654d  256[]"}],"stateM
+00021a10: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
+00021a20: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
+00021a30: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00021a40: 7574 7322 3a5b 5d2c 226e 616d 6522 3a22  uts":[],"name":"
+00021a50: 6e61 6d65 222c 226f 7574 7075 7473 223a  name","outputs":
+00021a60: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+00021a70: 3a22 7374 7269 6e67 222c 226e 616d 6522  :"string","name"
+00021a80: 3a22 222c 2274 7970 6522 3a22 7374 7269  :"","type":"stri
+00021a90: 6e67 227d 5d2c 2273 7461 7465 4d75 7461  ng"}],"stateMuta
+00021aa0: 6269 6c69 7479 223a 2270 7572 6522 2c22  bility":"pure","
+00021ab0: 7479 7065 223a 2266 756e 6374 696f 6e22  type":"function"
+00021ac0: 7d2c 7b22 696e 7075 7473 223a 5b7b 2269  },{"inputs":[{"i
+00021ad0: 6e74 6572 6e61 6c54 7970 6522 3a22 6164  nternalType":"ad
+00021ae0: 6472 6573 7322 2c22 6e61 6d65 223a 225f  dress","name":"_
+00021af0: 6163 636f 756e 7422 2c22 7479 7065 223a  account","type":
+00021b00: 2261 6464 7265 7373 227d 2c7b 2269 6e74  "address"},{"int
+00021b10: 6572 6e61 6c54 7970 6522 3a22 7569 6e74  ernalType":"uint
+00021b20: 3235 365b 5d22 2c22 6e61 6d65 223a 225f  256[]","name":"_
+00021b30: 6964 7322 2c22 7479 7065 223a 2275 696e  ids","type":"uin
+00021b40: 7432 3536 5b5d 227d 5d2c 226e 616d 6522  t256[]"}],"name"
+00021b50: 3a22 7065 6e64 696e 6746 6565 7322 2c22  :"pendingFees","
+00021b60: 6f75 7470 7574 7322 3a5b 7b22 696e 7465  outputs":[{"inte
+00021b70: 726e 616c 5479 7065 223a 2275 696e 7432  rnalType":"uint2
+00021b80: 3536 222c 226e 616d 6522 3a22 616d 6f75  56","name":"amou
+00021b90: 6e74 5822 2c22 7479 7065 223a 2275 696e  ntX","type":"uin
+00021ba0: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00021bb0: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00021bc0: 2c22 6e61 6d65 223a 2261 6d6f 756e 7459  ,"name":"amountY
+00021bd0: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00021be0: 3622 7d5d 2c22 7374 6174 654d 7574 6162  6"}],"stateMutab
+00021bf0: 696c 6974 7922 3a22 7669 6577 222c 2274  ility":"view","t
+00021c00: 7970 6522 3a22 6675 6e63 7469 6f6e 227d  ype":"function"}
+00021c10: 2c7b 2269 6e70 7574 7322 3a5b 7b22 696e  ,{"inputs":[{"in
+00021c20: 7465 726e 616c 5479 7065 223a 2261 6464  ternalType":"add
+00021c30: 7265 7373 222c 226e 616d 6522 3a22 5f66  ress","name":"_f
+00021c40: 726f 6d22 2c22 7479 7065 223a 2261 6464  rom","type":"add
+00021c50: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+00021c60: 6c54 7970 6522 3a22 6164 6472 6573 7322  lType":"address"
+00021c70: 2c22 6e61 6d65 223a 225f 746f 222c 2274  ,"name":"_to","t
+00021c80: 7970 6522 3a22 6164 6472 6573 7322 7d2c  ype":"address"},
+00021c90: 7b22 696e 7465 726e 616c 5479 7065 223a  {"internalType":
+00021ca0: 2275 696e 7432 3536 5b5d 222c 226e 616d  "uint256[]","nam
+00021cb0: 6522 3a22 5f69 6473 222c 2274 7970 6522  e":"_ids","type"
+00021cc0: 3a22 7569 6e74 3235 365b 5d22 7d2c 7b22  :"uint256[]"},{"
+00021cd0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00021ce0: 696e 7432 3536 5b5d 222c 226e 616d 6522  int256[]","name"
+00021cf0: 3a22 5f61 6d6f 756e 7473 222c 2274 7970  :"_amounts","typ
+00021d00: 6522 3a22 7569 6e74 3235 365b 5d22 7d5d  e":"uint256[]"}]
+00021d10: 2c22 6e61 6d65 223a 2273 6166 6542 6174  ,"name":"safeBat
+00021d20: 6368 5472 616e 7366 6572 4672 6f6d 222c  chTransferFrom",
+00021d30: 226f 7574 7075 7473 223a 5b5d 2c22 7374  "outputs":[],"st
+00021d40: 6174 654d 7574 6162 696c 6974 7922 3a22  ateMutability":"
+00021d50: 6e6f 6e70 6179 6162 6c65 222c 2274 7970  nonpayable","typ
+00021d60: 6522 3a22 6675 6e63 7469 6f6e 227d 2c7b  e":"function"},{
+00021d70: 2269 6e70 7574 7322 3a5b 7b22 696e 7465  "inputs":[{"inte
+00021d80: 726e 616c 5479 7065 223a 2261 6464 7265  rnalType":"addre
+00021d90: 7373 222c 226e 616d 6522 3a22 5f66 726f  ss","name":"_fro
+00021da0: 6d22 2c22 7479 7065 223a 2261 6464 7265  m","type":"addre
+00021db0: 7373 227d 2c7b 2269 6e74 6572 6e61 6c54  ss"},{"internalT
+00021dc0: 7970 6522 3a22 6164 6472 6573 7322 2c22  ype":"address","
+00021dd0: 6e61 6d65 223a 225f 746f 222c 2274 7970  name":"_to","typ
+00021de0: 6522 3a22 6164 6472 6573 7322 7d2c 7b22  e":"address"},{"
+00021df0: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00021e00: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00021e10: 5f69 6422 2c22 7479 7065 223a 2275 696e  _id","type":"uin
+00021e20: 7432 3536 227d 2c7b 2269 6e74 6572 6e61  t256"},{"interna
+00021e30: 6c54 7970 6522 3a22 7569 6e74 3235 3622  lType":"uint256"
+00021e40: 2c22 6e61 6d65 223a 225f 616d 6f75 6e74  ,"name":"_amount
+00021e50: 222c 2274 7970 6522 3a22 7569 6e74 3235  ","type":"uint25
+00021e60: 3622 7d5d 2c22 6e61 6d65 223a 2273 6166  6"}],"name":"saf
+00021e70: 6554 7261 6e73 6665 7246 726f 6d22 2c22  eTransferFrom","
+00021e80: 6f75 7470 7574 7322 3a5b 5d2c 2273 7461  outputs":[],"sta
+00021e90: 7465 4d75 7461 6269 6c69 7479 223a 226e  teMutability":"n
+00021ea0: 6f6e 7061 7961 626c 6522 2c22 7479 7065  onpayable","type
+00021eb0: 223a 2266 756e 6374 696f 6e22 7d2c 7b22  ":"function"},{"
+00021ec0: 696e 7075 7473 223a 5b7b 2269 6e74 6572  inputs":[{"inter
+00021ed0: 6e61 6c54 7970 6522 3a22 6164 6472 6573  nalType":"addres
+00021ee0: 7322 2c22 6e61 6d65 223a 225f 7370 656e  s","name":"_spen
+00021ef0: 6465 7222 2c22 7479 7065 223a 2261 6464  der","type":"add
+00021f00: 7265 7373 227d 2c7b 2269 6e74 6572 6e61  ress"},{"interna
+00021f10: 6c54 7970 6522 3a22 626f 6f6c 222c 226e  lType":"bool","n
+00021f20: 616d 6522 3a22 5f61 7070 726f 7665 6422  ame":"_approved"
+00021f30: 2c22 7479 7065 223a 2262 6f6f 6c22 7d5d  ,"type":"bool"}]
+00021f40: 2c22 6e61 6d65 223a 2273 6574 4170 7072  ,"name":"setAppr
+00021f50: 6f76 616c 466f 7241 6c6c 222c 226f 7574  ovalForAll","out
+00021f60: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
+00021f70: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
+00021f80: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
+00021f90: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00021fa0: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00021fb0: 5479 7065 223a 2262 7974 6573 3332 222c  Type":"bytes32",
+00021fc0: 226e 616d 6522 3a22 5f70 6163 6b65 6446  "name":"_packedF
+00021fd0: 6565 5061 7261 6d65 7465 7273 222c 2274  eeParameters","t
+00021fe0: 7970 6522 3a22 6279 7465 7333 3222 7d5d  ype":"bytes32"}]
+00021ff0: 2c22 6e61 6d65 223a 2273 6574 4665 6573  ,"name":"setFees
+00022000: 5061 7261 6d65 7465 7273 222c 226f 7574  Parameters","out
+00022010: 7075 7473 223a 5b5d 2c22 7374 6174 654d  puts":[],"stateM
+00022020: 7574 6162 696c 6974 7922 3a22 6e6f 6e70  utability":"nonp
+00022030: 6179 6162 6c65 222c 2274 7970 6522 3a22  ayable","type":"
+00022040: 6675 6e63 7469 6f6e 227d 2c7b 2269 6e70  function"},{"inp
+00022050: 7574 7322 3a5b 7b22 696e 7465 726e 616c  uts":[{"internal
+00022060: 5479 7065 223a 2262 7974 6573 3422 2c22  Type":"bytes4","
+00022070: 6e61 6d65 223a 225f 696e 7465 7266 6163  name":"_interfac
+00022080: 6549 6422 2c22 7479 7065 223a 2262 7974  eId","type":"byt
+00022090: 6573 3422 7d5d 2c22 6e61 6d65 223a 2273  es4"}],"name":"s
+000220a0: 7570 706f 7274 7349 6e74 6572 6661 6365  upportsInterface
+000220b0: 222c 226f 7574 7075 7473 223a 5b7b 2269  ","outputs":[{"i
+000220c0: 6e74 6572 6e61 6c54 7970 6522 3a22 626f  nternalType":"bo
+000220d0: 6f6c 222c 226e 616d 6522 3a22 222c 2274  ol","name":"","t
+000220e0: 7970 6522 3a22 626f 6f6c 227d 5d2c 2273  ype":"bool"}],"s
+000220f0: 7461 7465 4d75 7461 6269 6c69 7479 223a  tateMutability":
+00022100: 2276 6965 7722 2c22 7479 7065 223a 2266  "view","type":"f
+00022110: 756e 6374 696f 6e22 7d2c 7b22 696e 7075  unction"},{"inpu
+00022120: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00022130: 7970 6522 3a22 626f 6f6c 222c 226e 616d  ype":"bool","nam
+00022140: 6522 3a22 5f73 7761 7046 6f72 5922 2c22  e":"_swapForY","
+00022150: 7479 7065 223a 2262 6f6f 6c22 7d2c 7b22  type":"bool"},{"
+00022160: 696e 7465 726e 616c 5479 7065 223a 2261  internalType":"a
+00022170: 6464 7265 7373 222c 226e 616d 6522 3a22  ddress","name":"
+00022180: 5f74 6f22 2c22 7479 7065 223a 2261 6464  _to","type":"add
+00022190: 7265 7373 227d 5d2c 226e 616d 6522 3a22  ress"}],"name":"
+000221a0: 7377 6170 222c 226f 7574 7075 7473 223a  swap","outputs":
+000221b0: 5b7b 2269 6e74 6572 6e61 6c54 7970 6522  [{"internalType"
+000221c0: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+000221d0: 223a 2261 6d6f 756e 7458 4f75 7422 2c22  ":"amountXOut","
+000221e0: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+000221f0: 2c7b 2269 6e74 6572 6e61 6c54 7970 6522  ,{"internalType"
+00022200: 3a22 7569 6e74 3235 3622 2c22 6e61 6d65  :"uint256","name
+00022210: 223a 2261 6d6f 756e 7459 4f75 7422 2c22  ":"amountYOut","
+00022220: 7479 7065 223a 2275 696e 7432 3536 227d  type":"uint256"}
+00022230: 5d2c 2273 7461 7465 4d75 7461 6269 6c69  ],"stateMutabili
+00022240: 7479 223a 226e 6f6e 7061 7961 626c 6522  ty":"nonpayable"
+00022250: 2c22 7479 7065 223a 2266 756e 6374 696f  ,"type":"functio
+00022260: 6e22 7d2c 7b22 696e 7075 7473 223a 5b5d  n"},{"inputs":[]
+00022270: 2c22 6e61 6d65 223a 2273 796d 626f 6c22  ,"name":"symbol"
+00022280: 2c22 6f75 7470 7574 7322 3a5b 7b22 696e  ,"outputs":[{"in
+00022290: 7465 726e 616c 5479 7065 223a 2273 7472  ternalType":"str
+000222a0: 696e 6722 2c22 6e61 6d65 223a 2222 2c22  ing","name":"","
+000222b0: 7479 7065 223a 2273 7472 696e 6722 7d5d  type":"string"}]
+000222c0: 2c22 7374 6174 654d 7574 6162 696c 6974  ,"stateMutabilit
+000222d0: 7922 3a22 7075 7265 222c 2274 7970 6522  y":"pure","type"
+000222e0: 3a22 6675 6e63 7469 6f6e 227d 2c7b 2269  :"function"},{"i
+000222f0: 6e70 7574 7322 3a5b 5d2c 226e 616d 6522  nputs":[],"name"
+00022300: 3a22 746f 6b65 6e58 222c 226f 7574 7075  :"tokenX","outpu
+00022310: 7473 223a 5b7b 2269 6e74 6572 6e61 6c54  ts":[{"internalT
+00022320: 7970 6522 3a22 636f 6e74 7261 6374 2049  ype":"contract I
+00022330: 4552 4332 3022 2c22 6e61 6d65 223a 2222  ERC20","name":""
+00022340: 2c22 7479 7065 223a 2261 6464 7265 7373  ,"type":"address
+00022350: 227d 5d2c 2273 7461 7465 4d75 7461 6269  "}],"stateMutabi
+00022360: 6c69 7479 223a 2276 6965 7722 2c22 7479  lity":"view","ty
+00022370: 7065 223a 2266 756e 6374 696f 6e22 7d2c  pe":"function"},
+00022380: 7b22 696e 7075 7473 223a 5b5d 2c22 6e61  {"inputs":[],"na
+00022390: 6d65 223a 2274 6f6b 656e 5922 2c22 6f75  me":"tokenY","ou
+000223a0: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
+000223b0: 616c 5479 7065 223a 2263 6f6e 7472 6163  alType":"contrac
+000223c0: 7420 4945 5243 3230 222c 226e 616d 6522  t IERC20","name"
+000223d0: 3a22 222c 2274 7970 6522 3a22 6164 6472  :"","type":"addr
+000223e0: 6573 7322 7d5d 2c22 7374 6174 654d 7574  ess"}],"stateMut
+000223f0: 6162 696c 6974 7922 3a22 7669 6577 222c  ability":"view",
+00022400: 2274 7970 6522 3a22 6675 6e63 7469 6f6e  "type":"function
+00022410: 227d 2c7b 2269 6e70 7574 7322 3a5b 7b22  "},{"inputs":[{"
+00022420: 696e 7465 726e 616c 5479 7065 223a 2275  internalType":"u
+00022430: 696e 7432 3536 222c 226e 616d 6522 3a22  int256","name":"
+00022440: 5f69 6422 2c22 7479 7065 223a 2275 696e  _id","type":"uin
+00022450: 7432 3536 227d 5d2c 226e 616d 6522 3a22  t256"}],"name":"
+00022460: 746f 7461 6c53 7570 706c 7922 2c22 6f75  totalSupply","ou
+00022470: 7470 7574 7322 3a5b 7b22 696e 7465 726e  tputs":[{"intern
+00022480: 616c 5479 7065 223a 2275 696e 7432 3536  alType":"uint256
+00022490: 222c 226e 616d 6522 3a22 222c 2274 7970  ","name":"","typ
+000224a0: 6522 3a22 7569 6e74 3235 3622 7d5d 2c22  e":"uint256"}],"
+000224b0: 7374 6174 654d 7574 6162 696c 6974 7922  stateMutability"
+000224c0: 3a22 7669 6577 222c 2274 7970 6522 3a22  :"view","type":"
+000224d0: 6675 6e63 7469 6f6e 227d 5d27 290a 0a20  function"}]').. 
+000224e0: 2020 2023 2072 6574 7572 6e73 2028 7569     # returns (ui
+000224f0: 6e74 3235 3620 7265 7365 7276 6558 2c20  nt256 reserveX, 
+00022500: 7569 6e74 3235 3620 7265 7365 7276 6559  uint256 reserveY
+00022510: 2c20 7569 6e74 3235 3620 6163 7469 7665  , uint256 active
+00022520: 4964 290a 2020 2020 6465 6620 6765 745f  Id).    def get_
+00022530: 7265 7365 7276 655f 616e 645f 6964 285f  reserve_and_id(_
+00022540: 7765 6233 3a57 6562 332c 5f70 6169 725f  web3:Web3,_pair_
+00022550: 6164 6472 6573 733a 7374 7229 3a0a 2020  address:str):.  
+00022560: 2020 2020 2020 7061 6972 5f63 6f6e 7472        pair_contr
+00022570: 6163 743d 5f77 6562 332e 6574 682e 636f  act=_web3.eth.co
+00022580: 6e74 7261 6374 2861 6464 7265 7373 3d5f  ntract(address=_
+00022590: 7061 6972 5f61 6464 7265 7373 2c20 6162  pair_address, ab
+000225a0: 693d 4a6f 6556 3250 6169 722e 6a6f 655f  i=JoeV2Pair.joe_
+000225b0: 7061 6972 5f76 325f 6162 6929 0a20 2020  pair_v2_abi).   
+000225c0: 2020 2020 2072 6574 7572 6e20 7061 6972       return pair
+000225d0: 5f63 6f6e 7472 6163 742e 6675 6e63 7469  _contract.functi
+000225e0: 6f6e 732e 6765 7452 6573 6572 7665 7341  ons.getReservesA
+000225f0: 6e64 4964 2829 2e63 616c 6c28 290a 0a20  ndId().call().. 
+00022600: 2020 2023 2066 756e 6374 696f 6e20 6765     # function ge
+00022610: 7447 6c6f 6261 6c46 6565 7328 2920 6578  tGlobalFees() ex
+00022620: 7465 726e 616c 2076 6965 7720 6f76 6572  ternal view over
+00022630: 7269 6465 2072 6574 7572 6e73 2028 7569  ride returns (ui
+00022640: 6e74 3235 3620 6665 6573 5854 6f74 616c  nt256 feesXTotal
+00022650: 2c20 7569 6e74 3235 3620 6665 6573 5954  , uint256 feesYT
+00022660: 6f74 616c 2c20 7569 6e74 3235 3620 6665  otal, uint256 fe
+00022670: 6573 5850 726f 746f 636f 6c2c 2075 696e  esXProtocol, uin
+00022680: 7432 3536 2066 6565 7359 5072 6f74 6f63  t256 feesYProtoc
+00022690: 6f6c 290a 2020 2020 6465 6620 6765 745f  ol).    def get_
+000226a0: 676c 6f62 616c 5f66 6565 285f 7765 6233  global_fee(_web3
+000226b0: 3a57 6562 332c 5f70 6169 725f 6164 6472  :Web3,_pair_addr
+000226c0: 6573 733a 7374 7229 3a0a 2020 2020 2020  ess:str):.      
+000226d0: 2020 7061 6972 5f63 6f6e 7472 6163 743d    pair_contract=
+000226e0: 5f77 6562 332e 6574 682e 636f 6e74 7261  _web3.eth.contra
+000226f0: 6374 2861 6464 7265 7373 3d5f 7061 6972  ct(address=_pair
+00022700: 5f61 6464 7265 7373 2c20 6162 693d 4a6f  _address, abi=Jo
+00022710: 6556 3250 6169 722e 6a6f 655f 7061 6972  eV2Pair.joe_pair
+00022720: 5f76 325f 6162 6929 0a20 2020 2020 2020  _v2_abi).       
+00022730: 2072 6574 7572 6e20 7061 6972 5f63 6f6e   return pair_con
+00022740: 7472 6163 742e 6675 6e63 7469 6f6e 732e  tract.functions.
+00022750: 6765 7447 6c6f 6261 6c46 6565 7328 292e  getGlobalFees().
+00022760: 6361 6c6c 2829 0a0a 2020 2020 2320 6675  call()..    # fu
+00022770: 6e63 7469 6f6e 2066 696e 6446 6972 7374  nction findFirst
+00022780: 4e6f 6e45 6d70 7479 4269 6e49 6428 7569  NonEmptyBinId(ui
+00022790: 6e74 3234 205f 6964 2c20 626f 6f6c 205f  nt24 _id, bool _
+000227a0: 7377 6170 466f 7259 2920 6578 7465 726e  swapForY) extern
+000227b0: 616c 2076 6965 7720 6f76 6572 7269 6465  al view override
+000227c0: 2072 6574 7572 6e73 2028 7569 6e74 3234   returns (uint24
+000227d0: 290a 2020 2020 6465 6620 6669 6e64 5f66  ).    def find_f
+000227e0: 6972 7374 5f6e 6f6e 5f65 6d70 7479 5f62  irst_non_empty_b
+000227f0: 696e 5f69 6428 5f77 6562 333a 5765 6233  in_id(_web3:Web3
+00022800: 2c5f 7061 6972 5f61 6464 7265 7373 3a73  ,_pair_address:s
+00022810: 7472 2c5f 6964 2c5f 7377 6170 5f66 6f72  tr,_id,_swap_for
+00022820: 5f79 293a 0a20 2020 2020 2020 2070 6169  _y):.        pai
+00022830: 725f 636f 6e74 7261 6374 3d5f 7765 6233  r_contract=_web3
+00022840: 2e65 7468 2e63 6f6e 7472 6163 7428 6164  .eth.contract(ad
+00022850: 6472 6573 733d 5f70 6169 725f 6164 6472  dress=_pair_addr
+00022860: 6573 732c 2061 6269 3d4a 6f65 5632 5061  ess, abi=JoeV2Pa
+00022870: 6972 2e6a 6f65 5f70 6169 725f 7632 5f61  ir.joe_pair_v2_a
+00022880: 6269 290a 2020 2020 2020 2020 7265 7475  bi).        retu
+00022890: 726e 2070 6169 725f 636f 6e74 7261 6374  rn pair_contract
+000228a0: 2e66 756e 6374 696f 6e73 2e66 696e 6446  .functions.findF
+000228b0: 6972 7374 4e6f 6e45 6d70 7479 4269 6e49  irstNonEmptyBinI
+000228c0: 6428 5f69 642c 5f73 7761 705f 666f 725f  d(_id,_swap_for_
+000228d0: 7929 2e63 616c 6c28 290a 0a20 2020 2023  y).call()..    #
+000228e0: 2066 756e 6374 696f 6e20 6765 7442 696e   function getBin
+000228f0: 2875 696e 7432 3420 5f69 6429 2065 7874  (uint24 _id) ext
+00022900: 6572 6e61 6c20 7669 6577 206f 7665 7272  ernal view overr
+00022910: 6964 6520 7265 7475 726e 7320 2875 696e  ide returns (uin
+00022920: 7432 3536 2072 6573 6572 7665 582c 2075  t256 reserveX, u
+00022930: 696e 7432 3536 2072 6573 6572 7665 5929  int256 reserveY)
+00022940: 0a20 2020 2064 6566 2067 6574 5f62 696e  .    def get_bin
+00022950: 285f 7765 6233 3a57 6562 332c 5f70 6169  (_web3:Web3,_pai
+00022960: 725f 6164 6472 6573 733a 7374 722c 5f69  r_address:str,_i
+00022970: 6429 3a0a 2020 2020 2020 2020 7061 6972  d):.        pair
+00022980: 5f63 6f6e 7472 6163 743d 5f77 6562 332e  _contract=_web3.
+00022990: 6574 682e 636f 6e74 7261 6374 2861 6464  eth.contract(add
+000229a0: 7265 7373 3d5f 7061 6972 5f61 6464 7265  ress=_pair_addre
+000229b0: 7373 2c20 6162 693d 4a6f 6556 3250 6169  ss, abi=JoeV2Pai
+000229c0: 722e 6a6f 655f 7061 6972 5f76 325f 6162  r.joe_pair_v2_ab
+000229d0: 6929 0a20 2020 2020 2020 2072 6574 7572  i).        retur
+000229e0: 6e20 7061 6972 5f63 6f6e 7472 6163 742e  n pair_contract.
+000229f0: 6675 6e63 7469 6f6e 732e 6765 7442 696e  functions.getBin
+00022a00: 285f 6964 292e 6361 6c6c 2829 0a0a 2020  (_id).call()..  
+00022a10: 2020 2320 6675 6e63 7469 6f6e 2073 7761    # function swa
+00022a20: 7028 626f 6f6c 205f 7377 6170 466f 7259  p(bool _swapForY
+00022a30: 2c20 6164 6472 6573 7320 5f74 6f29 2065  , address _to) e
+00022a40: 7874 6572 6e61 6c20 6f76 6572 7269 6465  xternal override
+00022a50: 206e 6f6e 5265 656e 7472 616e 7420 7265   nonReentrant re
+00022a60: 7475 726e 7320 2875 696e 7432 3536 2061  turns (uint256 a
+00022a70: 6d6f 756e 7458 4f75 742c 2075 696e 7432  mountXOut, uint2
+00022a80: 3536 2061 6d6f 756e 7459 4f75 7429 0a20  56 amountYOut). 
+00022a90: 2020 2064 6566 2073 7761 7028 5f77 6562     def swap(_web
+00022aa0: 333a 5765 6233 2c5f 7061 6972 5f61 6464  3:Web3,_pair_add
+00022ab0: 7265 7373 3a73 7472 2c5f 7377 6170 5f66  ress:str,_swap_f
+00022ac0: 6f72 5f79 2c5f 746f 293a 0a20 2020 2020  or_y,_to):.     
+00022ad0: 2020 2070 6169 725f 636f 6e74 7261 6374     pair_contract
+00022ae0: 3d5f 7765 6233 2e65 7468 2e63 6f6e 7472  =_web3.eth.contr
+00022af0: 6163 7428 6164 6472 6573 733d 5f70 6169  act(address=_pai
+00022b00: 725f 6164 6472 6573 732c 2061 6269 3d4a  r_address, abi=J
+00022b10: 6f65 5632 5061 6972 2e6a 6f65 5f70 6169  oeV2Pair.joe_pai
+00022b20: 725f 7632 5f61 6269 290a 2020 2020 2020  r_v2_abi).      
+00022b30: 2020 7265 7475 726e 2070 6169 725f 636f    return pair_co
+00022b40: 6e74 7261 6374 2e66 756e 6374 696f 6e73  ntract.functions
+00022b50: 2e73 7761 7028 5f73 7761 705f 666f 725f  .swap(_swap_for_
+00022b60: 792c 5f74 6f29 2e63 616c 6c28 29         y,_to).call()
```

### Comparing `dexhub-0.6.5/dexhub/interface/joe.py` & `dexhub-0.6.6/dexhub/interface/joe.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub/util/helper.py` & `dexhub-0.6.6/dexhub/util/helper.py`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/dexhub.egg-info/PKG-INFO` & `dexhub-0.6.6/dexhub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexhub
-Version: 0.6.5
+Version: 0.6.6
 Summary: dex connector
 Home-page: https://github.com/elmtlab/aurum
 Author: elmtlab
 Author-email: elmtlab@outlook.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dexhub-0.6.5/dexhub.egg-info/SOURCES.txt` & `dexhub-0.6.6/dexhub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexhub-0.6.5/setup.py` & `dexhub-0.6.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dexhub",
-    version="0.6.5",
+    version="0.6.6",
     author="elmtlab",
     author_email="elmtlab@outlook.com",
     description="dex connector",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/elmtlab/aurum",
     packages=setuptools.find_packages(),
```

