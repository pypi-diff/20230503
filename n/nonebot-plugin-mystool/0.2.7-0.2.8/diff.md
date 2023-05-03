# Comparing `tmp/nonebot_plugin_mystool-0.2.7.tar.gz` & `tmp/nonebot_plugin_mystool-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_mystool-0.2.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_mystool-0.2.8.tar", max compression
```

## Comparing `nonebot_plugin_mystool-0.2.7.tar` & `nonebot_plugin_mystool-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1065 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/LICENSE
--rw-r--r--   0        0        0     3262 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/README.md
--rw-r--r--   0        0        0     1317 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2802 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/__init__.py
--rw-r--r--   0        0        0     2077 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/addFriend.py
--rw-r--r--   0        0        0     6914 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/address.py
--rw-r--r--   0        0        0    30682 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/bbsAPI.py
--rw-r--r--   0        0        0     7081 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/config.py
--rw-r--r--   0        0        0    15416 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/data.py
--rw-r--r--   0        0        0    22802 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/exchange.py
--rw-r--r--   0        0        0    19562 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/exchangePlan.py
--rw-r--r--   0        0        0    15148 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/gameSign.py
--rw-r--r--   0        0        0     1832 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/help.py
--rw-r--r--   0        0        0    14883 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/login.py
--rw-r--r--   0        0        0    23334 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/mybMission.py
--rw-r--r--   0        0        0    23885 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/plan.py
--rw-r--r--   0        0        0     9755 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/setting.py
--rw-r--r--   0        0        0    10836 2023-04-27 21:27:42.572339 nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/utils.py
--rw-r--r--   0        0        0     4688 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-03 20:06:50.908427 nonebot_plugin_mystool-0.2.8/LICENSE
+-rw-r--r--   0        0        0     3441 2023-05-03 20:06:50.908427 nonebot_plugin_mystool-0.2.8/README.md
+-rw-r--r--   0        0        0     1317 2023-05-03 20:06:50.908427 nonebot_plugin_mystool-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2802 2023-05-03 20:06:50.908427 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/__init__.py
+-rw-r--r--   0        0        0     2077 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/addFriend.py
+-rw-r--r--   0        0        0     6938 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/address.py
+-rw-r--r--   0        0        0    30682 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/bbsAPI.py
+-rw-r--r--   0        0        0     7081 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/config.py
+-rw-r--r--   0        0        0    15416 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/data.py
+-rw-r--r--   0        0        0    22707 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/exchange.py
+-rw-r--r--   0        0        0    19562 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/exchangePlan.py
+-rw-r--r--   0        0        0    15573 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/gameSign.py
+-rw-r--r--   0        0        0     1832 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/help.py
+-rw-r--r--   0        0        0    14907 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/login.py
+-rw-r--r--   0        0        0    23334 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/mybMission.py
+-rw-r--r--   0        0        0    23885 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/plan.py
+-rw-r--r--   0        0        0     9815 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/setting.py
+-rw-r--r--   0        0        0    10836 2023-05-03 20:06:50.912428 nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/utils.py
+-rw-r--r--   0        0        0     4867 1970-01-01 00:00:00.000000 nonebot_plugin_mystool-0.2.8/PKG-INFO
```

### Comparing `nonebot_plugin_mystool-0.2.7/LICENSE` & `nonebot_plugin_mystool-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/README.md` & `nonebot_plugin_mystool-0.2.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -67,138 +67,150 @@
 00000420: 6f74 2d70 6c75 6769 6e2d 6d79 7354 6f6f  ot-plugin-mysToo
 00000430: 6c3f 7374 796c 653d 666f 722d 7468 652d  l?style=for-the-
 00000440: 6261 6467 6522 3e0a 2020 3c2f 613e 0a3c  badge">.  </a>.<
 00000450: 2f64 6976 3e0a 0a23 206d 7973 546f 6f6c  /div>..# mysTool
 00000460: 202d 20e7 b1b3 e6b8 b8e7 a4be e8be 85e5   - .............
 00000470: 8aa9 e5b7 a5e5 85b7 e68f 92e4 bbb6 0a0a  ................
 00000480: 2a2a e789 88e6 9cac 202d 2076 302e 322e  **...... - v0.2.
-00000490: 372a 2a0a 0a23 2323 20f0 9f93 a320 e69b  7**..### .... ..
+00000490: 382a 2a0a 0a23 2323 20f0 9f93 a320 e69b  8**..### .... ..
 000004a0: b4e6 96b0 e586 85e5 aeb9 0a0a 2323 2323  ............####
-000004b0: 2032 3032 332e 342e 3238 0a2d 20e4 bfae   2023.4.28.- ...
-000004c0: e5a4 8de6 8f92 e4bb b6e5 91bd e4bb a4e8  ................
-000004d0: a2ab e585 b6e4 bb96 206e 6f6e 6562 6f74  ........ nonebot
-000004e0: 20e6 8f92 e4bb b6e6 8d95 e88e b7e7 9a84   ...............
-000004f0: e997 aee9 a298 0a2d 20e5 a29e e58a a0e6  .......- .......
-00000500: 94af e68c 81e6 989f e7a9 b9e9 9381 e981  ................
-00000510: 93e7 9a84 e595 86e5 9381 e585 91e6 8da2  ................
-00000520: 0a2d 20e6 af8f e697 a5e7 adbe e588 b0e3  .- .............
-00000530: 8081 e7b1 b3e6 b8b8 e5b8 81e4 bbbb e58a  ................
-00000540: a1e6 89a7 e8a1 8ce6 97b6 e997 b4e5 9ca8  ................
-00000550: e794 a8e6 88b7 e985 8de7 bdae e79a 84e5  ................
-00000560: 9fba e7a1 80e4 b88a e5a2 9ee5 8aa0 e99a  ................
-00000570: 8fe6 9cba e5bb b6e8 bf9f 0a2d 20e4 bfae  ...........- ...
-00000580: e5a4 8de5 a4a7 e588 abe9 878e e9a2 91e9  ................
-00000590: 8193 e6af 8fe6 97a5 e4bb bbe5 8aa1 e380  ................
-000005a0: 81e7 adbe e588 b0e6 89a7 e8a1 8ce5 a4b1  ................
-000005b0: e8b4 a5e7 9a84 e997 aee9 a298 0a0a 2323  ..............##
-000005c0: 2323 2032 3032 332e 332e 3330 0a2d 20e4  ## 2023.3.30.- .
-000005d0: bfae e5a4 8de9 878d e586 99e9 858d e7bd  ................
-000005e0: aee6 9687 e4bb b620 6070 6c75 6769 6e43  ....... `pluginC
-000005f0: 6f6e 6669 672e 6a73 6f6e 6020 e4b8 8de7  onfig.json` ....
-00000600: 949f e695 88e7 9a84 e997 aee9 a298 0a2d  ...............-
-00000610: 20e4 bfae e5a4 8de5 8d95 e8b4 a6e6 88b7   ...............
-00000620: e683 85e5 86b5 e4b8 8be6 97a0 e6b3 95e5  ................
-00000630: a29e e588 a0e5 8591 e68d a2e8 aea1 e588  ................
-00000640: 92e7 9a84 e997 aee9 a298 0a2d 20e4 bfae  ...........- ...
-00000650: e5a4 8d20 602f e585 91e6 8da2 6020 e591  ... `/......` ..
-00000660: bde4 bba4 e58f afe8 83bd e4b8 8ee5 85b6  ................
-00000670: e4bb 96e6 8f92 e4bb b6e5 91bd e4bb a4e5  ................
-00000680: 86b2 e7aa 81e7 9a84 e997 aee9 a298 efbc  ................
-00000690: 8ce5 908c e697 b620 5bf0 9f94 97e7 94a8  ....... [.......
-000006a0: e6b3 95e5 8f98 e69b b45d 2868 7474 7073  .........](https
-000006b0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4c6a  ://github.com/Lj
-000006c0: 7a64 2d50 524f 2f6e 6f6e 6562 6f74 2d70  zd-PRO/nonebot-p
-000006d0: 6c75 6769 6e2d 6d79 7374 6f6f 6c2f 7769  lugin-mystool/wi
-000006e0: 6b69 2f49 6e66 6f72 6d61 7469 6f6e 2d45  ki/Information-E
-000006f0: 7863 6861 6e67 6523 e5a2 9ee5 8aa0 e588  xchange#........
-00000700: a0e9 99a4 e585 91e6 8da2 e8ae a1e5 8892  ................
-00000710: 290a 2d20 e7b2 bee7 ae80 e68e a5e6 94b6  ).- ............
-00000720: e79a 84e5 91bd e4bb a40a 2d20 e69b b4e6  ..........- ....
-00000730: ada3 2060 6465 7669 6365 5f73 6176 6560  .. `device_save`
-00000740: 2022 e8ae bee5 a487 e4bf 9de5 ad98 2220   "............" 
-00000750: e697 a5e5 bf97 e696 87e6 9cac e79a 84e9  ................
-00000760: 9499 e8af af0a 0a23 2323 2320 3230 3233  .......#### 2023
-00000770: 2e33 2e31 380a 2d20 e5a2 9ee5 8aa0 e5af  .3.18.- ........
-00000780: bce5 87ba 436f 6f6b 6965 73e5 8a9f e883  ....Cookies.....
-00000790: bd0a 2d20 e5a2 9ee5 8aa0 e588 a0e9 99a4  ..- ............
-000007a0: e8b4 a6e5 8fb7 e695 b0e6 8dae e58a 9fe8  ................
-000007b0: 83bd 0a2d 20e5 9ca8 e794 a8e6 88b7 e689  ...- ...........
-000007c0: 80e6 9c89 e8b4 a6e5 8fb7 e983 bde7 99bb  ................
-000007d0: e5bd 95e5 a4b1 e695 88e7 9a84 e683 85e5  ................
-000007e0: 86b5 e4b8 8be5 85b3 e997 ade9 809a e79f  ................
-000007f0: a50a 2d20 e4bf aee5 a48d e58e 9fe7 a59e  ..- ............
-00000800: e6b8 b8e6 888f e7ad bee5 88b0 e5a4 b1e8  ................
-00000810: b4a5 e997 aee9 a298 0a2d 20e8 a784 e88c  .........- .....
-00000820: 83e5 8c96 e4bb a3e7 a081 0a0a 2323 20e5  ............## .
-00000830: 8a9f e883 bde5 928c e789 b9e6 80a7 0a0a  ................
-00000840: 2d20 e79f ade4 bfa1 e9aa 8ce8 af81 e799  - ..............
-00000850: bbe5 bd95 efbc 8ce5 858d e68a 93e5 8c85  ................
-00000860: e88e b7e5 8f96 2043 6f6f 6b69 650a 2d20  ...... Cookie.- 
-00000870: e887 aae5 8aa8 e5ae 8ce6 8890 e6af 8fe6  ................
-00000880: 97a5 e7b1 b3e6 b8b8 e5b8 81e4 bbbb e58a  ................
-00000890: a10a 2d20 e887 aae5 8aa8 e8bf 9be8 a18c  ..- ............
-000008a0: e6b8 b8e6 888f e7ad bee5 88b0 0a2d 20e5  .............- .
-000008b0: 8faf e588 b6e5 ae9a e7b1 b3e6 b8b8 e5b8  ................
-000008c0: 81e5 9586 e593 81e5 8591 e68d a2e8 aea1  ................
-000008d0: e588 92ef bc8c e588 b0e7 82b9 e585 91e6  ................
-000008e0: 8da2 0a2d 20e5 8faf e694 afe6 8c81 e5a4  ...- ...........
-000008f0: 9ae4 b8aa 2051 5120 e8b4 a6e5 8fb7 efbc  .... QQ ........
-00000900: 8ce6 af8f e4b8 aa20 5151 20e8 b4a6 e58f  ....... QQ .....
-00000910: b7e5 8faf e7bb 91e5 ae9a e5a4 9ae4 b8aa  ................
-00000920: e7b1 b3e5 9388 e6b8 b8e8 b4a6 e688 b70a  ................
-00000930: 2d20 5151 20e6 8ea8 e980 81e6 89a7 e8a1  - QQ ...........
-00000940: 8ce7 bb93 e69e 9ce9 809a e79f a50a 2d20  ..............- 
-00000950: e58e 9fe7 a59e e6a0 91e8 8482 e380 81e6  ................
-00000960: b49e e5a4 a9e5 ae9d e992 b1e3 8081 e8b4  ................
-00000970: a8e9 878f e58f 82e5 8f98 e4bb aae5 b7b2  ................
-00000980: e6bb a1e6 97b6 e68e a8e9 8081 e980 9ae7  ................
-00000990: 9fa5 0a0a 2323 20e4 bdbf e794 a8e8 afb4  ....## .........
-000009a0: e698 8e0a 0a23 2323 20f0 9f9b a0ef b88f  .....### .......
-000009b0: 204e 6f6e 6542 6f74 3220 e69c bae5 99a8   NoneBot2 ......
-000009c0: e4ba bae9 83a8 e7bd b2e5 928c e68f 92e4  ................
-000009d0: bbb6 e5ae 89e8 a385 0a0a e8af b7e6 9fa5  ................
-000009e0: e79c 8b20 2d3e 205b f09f 9497 496e 7374  ... -> [....Inst
-000009f0: 616c 6c61 7469 6f6e 5d28 6874 7470 733a  allation](https:
-00000a00: 2f2f 6769 7468 7562 2e63 6f6d 2f4c 6a7a  //github.com/Ljz
-00000a10: 642d 5052 4f2f 6e6f 6e65 626f 742d 706c  d-PRO/nonebot-pl
-00000a20: 7567 696e 2d6d 7973 746f 6f6c 2f77 696b  ugin-mystool/wik
-00000a30: 692f 496e 7374 616c 6c61 7469 6f6e 290a  i/Installation).
-00000a40: 0a23 2323 20f0 9f93 9620 e68f 92e4 bbb6  .### .... ......
-00000a50: e585 b7e4 bd93 e4bd bfe7 94a8 e8af b4e6  ................
-00000a60: 988e 0a0a e8af b7e6 9fa5 e79c 8b20 2d3e  ............. ->
-00000a70: 205b f09f 9497 5769 6b69 20e6 9687 e6a1   [....Wiki .....
-00000a80: a35d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
-00000a90: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
-00000aa0: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
-00000ab0: 7374 6f6f 6c2f 7769 6b69 290a 0a23 2323  stool/wiki)..###
-00000ac0: 20e2 9d93 20e8 8eb7 e58f 96e6 8f92 e4bb   ... ...........
-00000ad0: b6e5 b8ae e58a a9e4 bfa1 e681 af0a 0a23  ...............#
-00000ae0: 2323 2320 e68f 92e4 bbb6 e591 bde4 bba4  ### ............
-00000af0: 0a0a 6060 600a 2fe5 b8ae e58a a90a 6060  ..```./.......``
-00000b00: 600a 0a3e 20e2 9aa0 efb8 8f20 e6b3 a8e6  `..> ...... ....
-00000b10: 848f 20e6 ada4 e5a4 84e6 b2a1 e69c 89e4  .. .............
-00000b20: bdbf e794 a820 5bf0 9f94 9720 e68f 92e4  ..... [.... ....
-00000b30: bbb6 e591 bde4 bba4 e5a4 b45d 2868 7474  ...........](htt
-00000b40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000b50: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
-00000b60: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
-00000b70: 7769 6b69 2f43 6f6e 6669 6775 7261 7469  wiki/Configurati
-00000b80: 6f6e 2d43 6f6e 6669 6723 636f 6d6d 616e  on-Config#comman
-00000b90: 645f 7374 6172 7429 0a0a 2323 20e5 85b6  d_start)..## ...
-00000ba0: e4bb 960a 0a23 2323 205b f09f 9383 e6ba  .....### [......
-00000bb0: 90e7 a081 e8af b4e6 988e 5d28 6874 7470  ..........](http
-00000bc0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4c  s://github.com/L
-00000bd0: 6a7a 642d 5052 4f2f 6e6f 6e65 626f 742d  jzd-PRO/nonebot-
-00000be0: 706c 7567 696e 2d6d 7973 746f 6f6c 2f77  plugin-mystool/w
-00000bf0: 696b 692f 536f 7572 6365 2d53 7472 7563  iki/Source-Struc
-00000c00: 7475 7265 290a 2323 2320 e980 82e9 858d  ture).### ......
-00000c10: 205b e7bb aae5 b1b1 e79c 9fe5 afbb 426f   [............Bo
-00000c20: 745d 2868 7474 7073 3a2f 2f67 6974 6875  t](https://githu
-00000c30: 622e 636f 6d2f 4869 6269 4b69 6572 2f7a  b.com/HibiKier/z
-00000c40: 6865 6e78 756e 5f62 6f74 2920 e79a 84e5  henxun_bot) ....
-00000c50: 8886 e694 af0a 2d20 6874 7470 733a 2f2f  ......- https://
-00000c60: 6769 7468 7562 2e63 6f6d 2f4d 5754 4a43  github.com/MWTJC
-00000c70: 2f7a 6865 6e78 756e 2d70 6c75 6769 6e2d  /zhenxun-plugin-
-00000c80: 6d79 7374 6f6f 6c0a 2d20 6874 7470 733a  mystool.- https:
-00000c90: 2f2f 6769 7468 7562 2e63 6f6d 2f61 7961  //github.com/aya
-00000ca0: 6b61 7375 6b69 2f6e 6f6e 6562 6f74 2d70  kasuki/nonebot-p
-00000cb0: 6c75 6769 6e2d 6d79 7374 6f6f 6c0a       lugin-mystool.
+000004b0: 2032 3032 332e 352e 340a 2d20 e5a2 9ee5   2023.5.4.- ....
+000004c0: 8aa0 e5af b9e6 989f e7a9 b9e9 9381 e981  ................
+000004d0: 93e7 9a84 e7ad bee5 88b0 e58a 9fe8 83bd  ................
+000004e0: e79a 84e6 94af e68c 8120 2d20 5b23 3839  ......... - [#89
+000004f0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000500: 2e63 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f  .com/Ljzd-PRO/no
+00000510: 6e65 626f 742d 706c 7567 696e 2d6d 7973  nebot-plugin-mys
+00000520: 746f 6f6c 2f70 756c 6c2f 3839 2920 6279  tool/pull/89) by
+00000530: 2040 6179 616b 6173 756b 690a 2d20 e4bf   @ayakasuki.- ..
+00000540: aee5 a48d e68f 92e4 bbb6 e591 bde4 bba4  ................
+00000550: e4bc 98e5 8588 e5ba a6e9 97ae e9a2 9820  ............... 
+00000560: 2d20 5b23 3838 5d28 6874 7470 733a 2f2f  - [#88](https://
+00000570: 6769 7468 7562 2e63 6f6d 2f4c 6a7a 642d  github.com/Ljzd-
+00000580: 5052 4f2f 6e6f 6e65 626f 742d 706c 7567  PRO/nonebot-plug
+00000590: 696e 2d6d 7973 746f 6f6c 2f70 756c 6c2f  in-mystool/pull/
+000005a0: 3838 2920 6279 2040 6179 616b 6173 756b  88) by @ayakasuk
+000005b0: 690a 2d20 e983 a8e5 8886 e696 87e6 9cac  i.- ............
+000005c0: e994 99e8 afaf e4bf aee6 ada3 202d 205b  ............ - [
+000005d0: 2339 305d 2868 7474 7073 3a2f 2f67 6974  #90](https://git
+000005e0: 6875 622e 636f 6d2f 4c6a 7a64 2d50 524f  hub.com/Ljzd-PRO
+000005f0: 2f6e 6f6e 6562 6f74 2d70 6c75 6769 6e2d  /nonebot-plugin-
+00000600: 6d79 7374 6f6f 6c2f 7075 6c6c 2f39 3029  mystool/pull/90)
+00000610: 2062 7920 4062 6c61 636b 2d7a 6572 6f33   by @black-zero3
+00000620: 3538 0a0a 2323 2323 2032 3032 332e 342e  58..#### 2023.4.
+00000630: 3238 0a2d 20e4 bfae e5a4 8de6 8f92 e4bb  28.- ...........
+00000640: b6e5 91bd e4bb a4e8 a2ab e585 b6e4 bb96  ................
+00000650: 206e 6f6e 6562 6f74 20e6 8f92 e4bb b6e6   nonebot .......
+00000660: 8d95 e88e b7e7 9a84 e997 aee9 a298 0a2d  ...............-
+00000670: 20e5 a29e e58a a0e6 94af e68c 81e6 989f   ...............
+00000680: e7a9 b9e9 9381 e981 93e7 9a84 e595 86e5  ................
+00000690: 9381 e585 91e6 8da2 0a2d 20e6 af8f e697  .........- .....
+000006a0: a5e7 adbe e588 b0e3 8081 e7b1 b3e6 b8b8  ................
+000006b0: e5b8 81e4 bbbb e58a a1e6 89a7 e8a1 8ce6  ................
+000006c0: 97b6 e997 b4e5 9ca8 e794 a8e6 88b7 e985  ................
+000006d0: 8de7 bdae e79a 84e5 9fba e7a1 80e4 b88a  ................
+000006e0: e5a2 9ee5 8aa0 e99a 8fe6 9cba e5bb b6e8  ................
+000006f0: bf9f 0a2d 20e4 bfae e5a4 8de5 a4a7 e588  ...- ...........
+00000700: abe9 878e e9a2 91e9 8193 e6af 8fe6 97a5  ................
+00000710: e4bb bbe5 8aa1 e380 81e7 adbe e588 b0e6  ................
+00000720: 89a7 e8a1 8ce5 a4b1 e8b4 a5e7 9a84 e997  ................
+00000730: aee9 a298 0a0a 2323 2323 2032 3032 332e  ......#### 2023.
+00000740: 332e 3330 0a2d 20e4 bfae e5a4 8de9 878d  3.30.- .........
+00000750: e586 99e9 858d e7bd aee6 9687 e4bb b620  ............... 
+00000760: 6070 6c75 6769 6e43 6f6e 6669 672e 6a73  `pluginConfig.js
+00000770: 6f6e 6020 e4b8 8de7 949f e695 88e7 9a84  on` ............
+00000780: e997 aee9 a298 0a2d 20e4 bfae e5a4 8de5  .......- .......
+00000790: 8d95 e8b4 a6e6 88b7 e683 85e5 86b5 e4b8  ................
+000007a0: 8be6 97a0 e6b3 95e5 a29e e588 a0e5 8591  ................
+000007b0: e68d a2e8 aea1 e588 92e7 9a84 e997 aee9  ................
+000007c0: a298 0a2d 20e4 bfae e5a4 8d20 602f e585  ...- ...... `/..
+000007d0: 91e6 8da2 6020 e591 bde4 bba4 e58f afe8  ....` ..........
+000007e0: 83bd e4b8 8ee5 85b6 e4bb 96e6 8f92 e4bb  ................
+000007f0: b6e5 91bd e4bb a4e5 86b2 e7aa 81e7 9a84  ................
+00000800: e997 aee9 a298 efbc 8ce5 908c e697 b620  ............... 
+00000810: 5bf0 9f94 97e7 94a8 e6b3 95e5 8f98 e69b  [...............
+00000820: b45d 2868 7474 7073 3a2f 2f67 6974 6875  .](https://githu
+00000830: 622e 636f 6d2f 4c6a 7a64 2d50 524f 2f6e  b.com/Ljzd-PRO/n
+00000840: 6f6e 6562 6f74 2d70 6c75 6769 6e2d 6d79  onebot-plugin-my
+00000850: 7374 6f6f 6c2f 7769 6b69 2f49 6e66 6f72  stool/wiki/Infor
+00000860: 6d61 7469 6f6e 2d45 7863 6861 6e67 6523  mation-Exchange#
+00000870: e5a2 9ee5 8aa0 e588 a0e9 99a4 e585 91e6  ................
+00000880: 8da2 e8ae a1e5 8892 290a 2d20 e7b2 bee7  ........).- ....
+00000890: ae80 e68e a5e6 94b6 e79a 84e5 91bd e4bb  ................
+000008a0: a40a 2d20 e69b b4e6 ada3 2060 6465 7669  ..- ...... `devi
+000008b0: 6365 5f73 6176 6560 2022 e8ae bee5 a487  ce_save` "......
+000008c0: e4bf 9de5 ad98 2220 e697 a5e5 bf97 e696  ......" ........
+000008d0: 87e6 9cac e79a 84e9 9499 e8af af0a 0a23  ...............#
+000008e0: 2320 e58a 9fe8 83bd e592 8ce7 89b9 e680  # ..............
+000008f0: a70a 0a2d 20e7 9fad e4bf a1e9 aa8c e8af  ...- ...........
+00000900: 81e7 99bb e5bd 95ef bc8c e585 8de6 8a93  ................
+00000910: e58c 85e8 8eb7 e58f 9620 436f 6f6b 6965  ......... Cookie
+00000920: 0a2d 20e8 87aa e58a a8e5 ae8c e688 90e6  .- .............
+00000930: af8f e697 a5e7 b1b3 e6b8 b8e5 b881 e4bb  ................
+00000940: bbe5 8aa1 0a2d 20e8 87aa e58a a8e8 bf9b  .....- .........
+00000950: e8a1 8ce6 b8b8 e688 8fe7 adbe e588 b00a  ................
+00000960: 2d20 e58f afe5 88b6 e5ae 9ae7 b1b3 e6b8  - ..............
+00000970: b8e5 b881 e595 86e5 9381 e585 91e6 8da2  ................
+00000980: e8ae a1e5 8892 efbc 8ce5 88b0 e782 b9e5  ................
+00000990: 8591 e68d a20a 2d20 e58f afe6 94af e68c  ......- ........
+000009a0: 81e5 a49a e4b8 aa20 5151 20e8 b4a6 e58f  ....... QQ .....
+000009b0: b7ef bc8c e6af 8fe4 b8aa 2051 5120 e8b4  .......... QQ ..
+000009c0: a6e5 8fb7 e58f afe7 bb91 e5ae 9ae5 a49a  ................
+000009d0: e4b8 aae7 b1b3 e593 88e6 b8b8 e8b4 a6e6  ................
+000009e0: 88b7 0a2d 2051 5120 e68e a8e9 8081 e689  ...- QQ ........
+000009f0: a7e8 a18c e7bb 93e6 9e9c e980 9ae7 9fa5  ................
+00000a00: 0a2d 20e5 8e9f e7a5 9ee6 a091 e884 82e3  .- .............
+00000a10: 8081 e6b4 9ee5 a4a9 e5ae 9de9 92b1 e380  ................
+00000a20: 81e8 b4a8 e987 8fe5 8f82 e58f 98e4 bbaa  ................
+00000a30: e5b7 b2e6 bba1 e697 b6e6 8ea8 e980 81e9  ................
+00000a40: 809a e79f a50a 0a23 2320 e4bd bfe7 94a8  .......## ......
+00000a50: e8af b4e6 988e 0a0a 2323 2320 f09f 9ba0  ........### ....
+00000a60: efb8 8f20 4e6f 6e65 426f 7432 20e6 9cba  ... NoneBot2 ...
+00000a70: e599 a8e4 baba e983 a8e7 bdb2 e592 8ce6  ................
+00000a80: 8f92 e4bb b6e5 ae89 e8a3 850a 0ae8 afb7  ................
+00000a90: e69f a5e7 9c8b 202d 3e20 5bf0 9f94 9749  ...... -> [....I
+00000aa0: 6e73 7461 6c6c 6174 696f 6e5d 2868 7474  nstallation](htt
+00000ab0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000ac0: 4c6a 7a64 2d50 524f 2f6e 6f6e 6562 6f74  Ljzd-PRO/nonebot
+00000ad0: 2d70 6c75 6769 6e2d 6d79 7374 6f6f 6c2f  -plugin-mystool/
+00000ae0: 7769 6b69 2f49 6e73 7461 6c6c 6174 696f  wiki/Installatio
+00000af0: 6e29 0a0a 2323 2320 f09f 9396 20e6 8f92  n)..### .... ...
+00000b00: e4bb b6e5 85b7 e4bd 93e4 bdbf e794 a8e8  ................
+00000b10: afb4 e698 8e0a 0ae8 afb7 e69f a5e7 9c8b  ................
+00000b20: 202d 3e20 5bf0 9f94 9757 696b 6920 e696   -> [....Wiki ..
+00000b30: 87e6 a1a3 5d28 6874 7470 733a 2f2f 6769  ....](https://gi
+00000b40: 7468 7562 2e63 6f6d 2f4c 6a7a 642d 5052  thub.com/Ljzd-PR
+00000b50: 4f2f 6e6f 6e65 626f 742d 706c 7567 696e  O/nonebot-plugin
+00000b60: 2d6d 7973 746f 6f6c 2f77 696b 6929 0a0a  -mystool/wiki)..
+00000b70: 2323 2320 e29d 9320 e88e b7e5 8f96 e68f  ### ... ........
+00000b80: 92e4 bbb6 e5b8 aee5 8aa9 e4bf a1e6 81af  ................
+00000b90: 0a0a 2323 2323 20e6 8f92 e4bb b6e5 91bd  ..#### .........
+00000ba0: e4bb a40a 0a60 6060 0a2f e5b8 aee5 8aa9  .....```./......
+00000bb0: 0a60 6060 0a0a 3e20 e29a a0ef b88f 20e6  .```..> ...... .
+00000bc0: b3a8 e684 8f20 e6ad a4e5 a484 e6b2 a1e6  ..... ..........
+00000bd0: 9c89 e4bd bfe7 94a8 205b f09f 9497 20e6  ........ [.... .
+00000be0: 8f92 e4bb b6e5 91bd e4bb a4e5 a4b4 5d28  ..............](
+00000bf0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000c00: 6f6d 2f4c 6a7a 642d 5052 4f2f 6e6f 6e65  om/Ljzd-PRO/none
+00000c10: 626f 742d 706c 7567 696e 2d6d 7973 746f  bot-plugin-mysto
+00000c20: 6f6c 2f77 696b 692f 436f 6e66 6967 7572  ol/wiki/Configur
+00000c30: 6174 696f 6e2d 436f 6e66 6967 2363 6f6d  ation-Config#com
+00000c40: 6d61 6e64 5f73 7461 7274 290a 0a23 2320  mand_start)..## 
+00000c50: e585 b6e4 bb96 0a0a 2323 2320 5bf0 9f93  ........### [...
+00000c60: 83e6 ba90 e7a0 81e8 afb4 e698 8e5d 2868  .............](h
+00000c70: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000c80: 6d2f 4c6a 7a64 2d50 524f 2f6e 6f6e 6562  m/Ljzd-PRO/noneb
+00000c90: 6f74 2d70 6c75 6769 6e2d 6d79 7374 6f6f  ot-plugin-mystoo
+00000ca0: 6c2f 7769 6b69 2f53 6f75 7263 652d 5374  l/wiki/Source-St
+00000cb0: 7275 6374 7572 6529 0a23 2323 20e9 8082  ructure).### ...
+00000cc0: e985 8d20 5be7 bbaa e5b1 b1e7 9c9f e5af  ... [...........
+00000cd0: bb42 6f74 5d28 6874 7470 733a 2f2f 6769  .Bot](https://gi
+00000ce0: 7468 7562 2e63 6f6d 2f48 6962 694b 6965  thub.com/HibiKie
+00000cf0: 722f 7a68 656e 7875 6e5f 626f 7429 20e7  r/zhenxun_bot) .
+00000d00: 9a84 e588 86e6 94af 0a2d 2068 7474 7073  .........- https
+00000d10: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d57  ://github.com/MW
+00000d20: 544a 432f 7a68 656e 7875 6e2d 706c 7567  TJC/zhenxun-plug
+00000d30: 696e 2d6d 7973 746f 6f6c 0a2d 2068 7474  in-mystool.- htt
+00000d40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000d50: 6179 616b 6173 756b 692f 6e6f 6e65 626f  ayakasuki/nonebo
+00000d60: 742d 706c 7567 696e 2d6d 7973 746f 6f6c  t-plugin-mystool
+00000d70: 0a                                       .
```

### Comparing `nonebot_plugin_mystool-0.2.7/pyproject.toml` & `nonebot_plugin_mystool-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-mystool"
-version = "v0.2.7"
+version = "v0.2.8"
 description = "NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒"
 license = "MIT"
 authors = [
   "Ljzd-PRO <ljzd@office.ljzd-pro.ml>",
   "Everything0519 <598139245@qq.com>"
 ]
 readme = "README.md"
```

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/__init__.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 # mysTool - 米游社辅助工具插件
 
-**版本 - v0.2.6**
+**版本 - v0.2.8**
 
 ## 使用说明
 
 ### 🛠️ NoneBot2 机器人部署和插件安装
 
 请查看 -> [🔗Installation](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Installation)
 
@@ -35,15 +35,15 @@
 import pkgutil
 from pathlib import Path
 
 from nonebot.plugin import PluginMetadata
 
 from .data import create_files
 
-VERSION = "v0.2.6"
+VERSION = "v0.2.8"
 '''插件版本号'''
 
 __plugin_meta__ = PluginMetadata(
     name=f"❖米游社小助手插件❖\n版本 - {VERSION}\n",
     description="米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录\n",
     usage="""
     \n🔐 {HEAD}登录 ➢ 登录绑定米游社账户\
```

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/addFriend.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/addFriend.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/address.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/address.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     except Exception:
         logger.error(f"{conf.LOG_HEAD}获取地址数据 - 请求失败")
         logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
         return -3
     return address_list
 
 
-get_address = on_command(conf.COMMAND_START + '地址')
+get_address = on_command(conf.COMMAND_START + '地址', priority=4, block=True)
 
 get_address.name = '地址'
 get_address.usage = '跟随指引，获取地址ID，用于兑换米游币商品。在获取地址ID前，如果你还没有设置米游社收获地址，请前往官网或App设置'
 
 
 @get_address.handle()
 async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State):
```

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/bbsAPI.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/bbsAPI.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/config.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/data.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/exchange.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,20 +147,18 @@
         """
         兑换时间
         """
         # "next_time" 为 0 表示任何时间均可兑换或兑换已结束
         # "type" 为 1 时商品只有在指定时间开放兑换；为 0 时商品任何时间均可兑换
         if self.good_dict["type"] != 1 and self.good_dict["next_time"] == 0:
             return None
-        elif self.good_dict["status"] != "not_in_sell":
-            return self.good_dict["next_time"]
         elif "sale_start_time" in self.good_dict:
             return int(self.good_dict["sale_start_time"])
         else:
-            return self.time_by_detail
+            return self.good_dict["next_time"]
 
     @property
     def num(self) -> Union[None, int]:
         """
         库存
         """
         if self.good_dict["type"] != 1 and self.good_dict["next_num"] == 0:
```

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/exchangePlan.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/exchangePlan.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/gameSign.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/gameSign.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .utils import (Subscribe, check_ds, check_login, custom_attempt_times,
                     generate_ds, logger)
 
 ACT_ID = {
     "ys": "e202009291139501",
     "bh3": "e202207181446311",
     "bh2": "e202203291431091",
+    "xq": "e202304121516551",
     "wd": "e202202251749321"
 }
 URLS = {
     "ys": {
         "reward": "https://api-takumi.mihoyo.com/event/bbs_sign_reward/home?act_id={}".format(ACT_ID["ys"]),
         "info": "".join(("https://api-takumi.mihoyo.com/event/bbs_sign_reward/info?act_id={}".format(ACT_ID["ys"]),
                          "&region={region}&uid={uid}")),
@@ -35,14 +36,20 @@
     },
     "bh2": {
         "reward": "https://api-takumi.mihoyo.com/event/luna/home?lang=zh-cn&act_id={}".format(ACT_ID["bh2"]),
         "info": "".join(("https://api-takumi.mihoyo.com/event/luna/info?lang=zh-cn&act_id={}".format(ACT_ID["bh2"]),
                          "&region={region}&uid={uid}")),
         "sign": "https://api-takumi.mihoyo.com/event/luna/sign"
     },
+    "xq": {
+        "reward": "https://api-takumi.mihoyo.com/event/luna/home?lang=zh-cn&act_id={}".format(ACT_ID["xq"]),
+        "info": "".join(("https://api-takumi.mihoyo.com/event/luna/info?lang=zh-cn&act_id={}".format(ACT_ID["xq"]),
+                         "&region={region}&uid={uid}")),
+        "sign": "https://api-takumi.mihoyo.com/event/luna/sign"
+    },
     "wd": {
         "reward": "https://api-takumi.mihoyo.com/event/luna/home?lang=zh-cn&act_id={}".format(ACT_ID["wd"]),
         "info": "".join(("https://api-takumi.mihoyo.com/event/luna/info?lang=zh-cn&act_id={}".format(ACT_ID["wd"]),
                          "&region={region}&uid={uid}")),
         "sign": "https://api-takumi.mihoyo.com/event/luna/sign"
     }
 }
@@ -155,25 +162,25 @@
         return self.info_dict["sign_cnt_missed"]
 
 
 class GameSign:
     """
     游戏签到相关(需先初始化对象)
     """
-    SUPPORTED_GAMES = ["ys", "bh3", "bh2", "wd"]
+    SUPPORTED_GAMES = ["ys", "bh3", "bh2", "xq", "wd"]
     '''目前支持签到的游戏'''
 
     def __init__(self, account: UserAccount) -> None:
         self.cookie = account.cookie
         self.account = account
         self.signResult: dict = {}
         '''签到返回结果'''
 
     @staticmethod
-    async def reward(game: Literal["ys", "bh3"], retry: bool = True):
+    async def reward(game: Literal["ys", "bh3", "xq"], retry: bool = True):
         """
         获取签到奖励信息，若返回`None`说明失败
 
         :param game: 目标游戏缩写
         :param retry: 是否允许重试
         """
         try:
@@ -193,15 +200,15 @@
             logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
         except Exception:
             logger.error(f"{conf.LOG_HEAD}获取签到奖励信息 - 请求失败")
             if isinstance(res, httpx.Response):
                 logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
             logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
 
-    async def info(self, game: Literal["ys", "bh3"], game_uid: str, region: str = None, retry: bool = True) -> Union[
+    async def info(self, game: Literal["ys", "bh3", "xq"], game_uid: str, region: str = None, retry: bool = True) -> Union[
         Info, Literal[-1, -2, -3, -4]]:
         """
         获取签到记录，返回Info对象
 
         :param game: 目标游戏缩写
         :param game_uid: 用户游戏UID
         :param region: 用户游戏区服(若为`None`将会自动获取)
@@ -260,15 +267,15 @@
         except Exception:
             logger.error(f"{conf.LOG_HEAD}获取签到记录 - 请求失败")
             if isinstance(res, httpx.Response):
                 logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
             logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
             return -3
 
-    async def sign(self, game: Literal["ys", "bh3", "bh2", "wd"], game_uid: str,
+    async def sign(self, game: Literal["ys", "bh3", "xq", "bh2", "wd"], game_uid: str,
                    platform: Literal["ios", "android"] = "ios", retry: bool = True) -> Literal[
         1, -1, -2, -3, -4, -5, -6]:
         """
         签到
 
         :param game: 目标游戏缩写
         :param game_uid: 用户游戏UID
@@ -338,15 +345,15 @@
                             headers["DS"] = generate_ds()
                         else:
                             headers["User-Agent"] = conf.device.USER_AGENT_ANDROID
                             headers["DS"] = generate_ds(platform="android")
                     self.signResult = res.json()
                     if game == "ys" and self.signResult["message"] == "旅行者，你已经签到过了":
                         return 1
-                    if game not in ["bh3", "wd", "bh2"] and self.signResult["data"]["risk_code"] != 0:
+                    if game not in ["bh3", "xq", "wd", "bh2"] and self.signResult["data"]["risk_code"] != 0:
                         logger.warning(
                             f"{conf.LOG_HEAD}签到 - 用户 {self.account.phone} 可能被验证码阻拦")
                         logger.debug(f"{conf.LOG_HEAD}网络请求返回: {res.text}")
                         return -5
                     return 1
         except KeyError and ValueError and TypeError:
             logger.error(f"{conf.LOG_HEAD}签到 - 服务器没有正确返回")
```

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/help.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/help.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/login.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/login.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                     return 1
         except tenacity.RetryError:
             logger.error(f"{conf.LOG_HEAD}登录米哈游账号 - 获取第三次Cookie: 网络请求失败")
             logger.debug(f"{conf.LOG_HEAD}{traceback.format_exc()}")
             return -2
 
 
-get_cookie = on_command(conf.COMMAND_START + '登录')
+get_cookie = on_command(conf.COMMAND_START + '登录', priority=4, block=True)
 get_cookie.name = '登录'
 get_cookie.usage = '跟随指引，通过电话获取短信方式绑定米游社账户，配置完成后会自动开启签到、米游币任务，后续可制定米游币自动兑换计划。'
 
 
 @get_cookie.handle()
 async def handle_first_receive(event: Union[GroupMessageEvent, PrivateMessageEvent]):
     if isinstance(event, GroupMessageEvent):
```

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/mybMission.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/mybMission.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/plan.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
                         (isinstance(sign_info, Info) and not sign_info.is_sign) or (
                         isinstance(sign_info, int) and sign_info != -1)):
                     sign_flag = await gamesign.sign(sign_game, record.uid, account.platform)
                     if sign_flag != 1:
                         if sign_flag == -1:
                             message = f"⚠️账户 {account.phone if not group_event else blur(account.phone)} 🎮『{game_name}』签到时服务器返回登录失效，请尝试重新登录绑定账户"
                         elif sign_flag == -5:
-                            message = f"⚠️账户 {account.phone if not group_event else blur(account.phone)} 🎮『{game_name}』签到时可能遇到验证码拦截，请尝试使用命令『/账户设置』更改设备平台，若仍失败请手动前往米游社签到"
+                            message = f"⚠️账户 {account.phone if not group_event else blur(account.phone)} 🎮『{game_name}』签到时可能遇到验证码拦截，请尝试使用命令『/账号设置』更改设备平台，若仍失败请手动前往米游社签到"
                         else:
                             message = f"⚠️账户 {account.phone if not group_event else blur(account.phone)} 🎮『{game_name}』签到失败，请稍后再试"
                         if UserData.is_notice(qq) or not is_auto:
                             if group_event:
                                 await bot.send(event=group_event, at_sender=True, message=message)
                             else:
                                 await bot.send_msg(
```

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/setting.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/setting.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
 from .bbsAPI import GameInfo
 from .config import config as conf
 from .data import UserAccount, UserData
 from .mybMission import GAME_ID
 from .utils import COMMAND_BEGIN
 
-setting = on_command(conf.COMMAND_START + '设置')
+setting = on_command(conf.COMMAND_START + '设置', priority=4)
 setting.name = "设置"
 setting.usage = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令。\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令。'
 
 
 @setting.handle()
 async def _(event: MessageEvent):
     msg = f'如需配置是否开启每日任务、设备平台、频道任务等相关选项，请使用『{COMMAND_BEGIN}账号设置』命令\n如需设置米游币任务和游戏签到后是否进行QQ通知，请使用『{COMMAND_BEGIN}通知设置』命令'
     await setting.send(msg)
 
 
-account_setting = on_command(conf.COMMAND_START + '账号设置')
+account_setting = on_command(conf.COMMAND_START + '账号设置', priority=5, block=True)
 account_setting.name = "账号设置"
 account_setting.usage = "配置游戏自动签到、米游币任务是否开启、设备平台、频道任务相关选项"
 
 
 @account_setting.handle()
 async def _(event: Union[PrivateMessageEvent, GroupMessageEvent], matcher: Matcher, state: T_State):
     """
@@ -169,15 +169,15 @@
             account.missionGame.append(list(filter(
                 lambda game_tuple: game_tuple[1] == game_input, GameInfo.ABBR_TO_ID.values()))[0][0])
     UserData.set_account(account, event.user_id, account.phone)
     arg = arg.replace(" ", "、")
     await account_setting.finish(f"💬执行米游币任务的频道已更改为『{arg}』")
 
 
-global_setting = on_command(conf.COMMAND_START + '通知设置')
+global_setting = on_command(conf.COMMAND_START + '通知设置', priority=5, block=True)
 global_setting.name = "通知设置"
 global_setting.usage = "设置每日签到后是否进行QQ通知"
 
 
 @global_setting.handle()
 async def _(event: MessageEvent, matcher: Matcher):
     """
```

### Comparing `nonebot_plugin_mystool-0.2.7/src/nonebot_plugin_mystool/utils.py` & `nonebot_plugin_mystool-0.2.8/src/nonebot_plugin_mystool/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_mystool-0.2.7/PKG-INFO` & `nonebot_plugin_mystool-0.2.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-mystool
-Version: 0.2.7
+Version: 0.2.8
 Summary: NoneBot2插件|米游社工具-每日米游币任务、游戏签到、商品兑换、免抓包登录、原神树脂提醒
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool
 License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO
 Author-email: ljzd@office.ljzd-pro.ml
 Requires-Python: >=3.9,<4.0
@@ -46,38 +46,36 @@
   <a href="https://github.com/Ljzd-PRO/nonebot-plugin-mystool/commits/" target="_blank">
     <img alt="最后提交" src="https://img.shields.io/github/last-commit/Ljzd-PRO/nonebot-plugin-mysTool?style=for-the-badge">
   </a>
 </div>
 
 # mysTool - 米游社辅助工具插件
 
-**版本 - v0.2.7**
+**版本 - v0.2.8**
 
 ### 📣 更新内容
 
+#### 2023.5.4
+- 增加对星穹铁道的签到功能的支持 - [#89](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/89) by @ayakasuki
+- 修复插件命令优先度问题 - [#88](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/88) by @ayakasuki
+- 部分文本错误修正 - [#90](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/90) by @black-zero358
+
 #### 2023.4.28
 - 修复插件命令被其他 nonebot 插件捕获的问题
 - 增加支持星穹铁道的商品兑换
 - 每日签到、米游币任务执行时间在用户配置的基础上增加随机延迟
 - 修复大别野频道每日任务、签到执行失败的问题
 
 #### 2023.3.30
 - 修复重写配置文件 `pluginConfig.json` 不生效的问题
 - 修复单账户情况下无法增删兑换计划的问题
 - 修复 `/兑换` 命令可能与其他插件命令冲突的问题，同时 [🔗用法变更](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-Exchange#增加删除兑换计划)
 - 精简接收的命令
 - 更正 `device_save` "设备保存" 日志文本的错误
 
-#### 2023.3.18
-- 增加导出Cookies功能
-- 增加删除账号数据功能
-- 在用户所有账号都登录失效的情况下关闭通知
-- 修复原神游戏签到失败问题
-- 规范化代码
-
 ## 功能和特性
 
 - 短信验证登录，免抓包获取 Cookie
 - 自动完成每日米游币任务
 - 自动进行游戏签到
 - 可制定米游币商品兑换计划，到点兑换
 - 可支持多个 QQ 账号，每个 QQ 账号可绑定多个米哈游账户
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-mystool Version: 0.2.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-mystool Version: 0.2.8 Summary:
 NoneBot2æä»¶|ç±³æ¸¸ç¤¾å·¥å·-
 æ¯æ¥ç±³æ¸¸å¸ä»»å¡ãæ¸¸æç­¾å°ãåååæ¢ãåæåç»å½ãåç¥æ èæé
 Home-page: https://github.com/Ljzd-PRO/nonebot-plugin-mystool License: MIT
 Keywords: bot,qq,qqbot,onebotv11,onebot,nonebot2,nonebot,mihoyo,mihoyobbs
 Author: Ljzd-PRO Author-email: ljzd@office.ljzd-pro.ml Requires-Python:
 >=3.9,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -19,28 +19,30 @@
 Repository, https://github.com/Ljzd-PRO/nonebot-plugin-mystool Description-
 Content-Type: text/markdown ``` __ __ __ __ ______ ______ ______ ______ __ /
 \ "-./ \ /\ \_\ \ /\ ___\ /\__ _\ /\ __ \ /\ __ \ /\ \ \ \ \-./\ \ \ \____ \ \
 \___ \ \/_/\ \/ \ \ \/\ \ \ \ \/\ \ \ \ \____ \ \_\ \ \_\ \/\_____\ \/\_____\ \
 \_\ \ \_____\ \ \_____\ \ \_____\ \/_/ \/_/ \/_____/ \/_____/ \/_/ \/_____/ \/
 _____/ \/_____/ ```
 [CodeFactor] [ææ°åè¡ç] [æåæäº¤]
-# mysTool - ç±³æ¸¸ç¤¾è¾å©å·¥å·æä»¶ **çæ¬ - v0.2.7** ### ð£
-æ´æ°åå®¹ #### 2023.4.28 - ä¿®å¤æä»¶å½ä»¤è¢«å¶ä» nonebot
+# mysTool - ç±³æ¸¸ç¤¾è¾å©å·¥å·æä»¶ **çæ¬ - v0.2.8** ### ð£
+æ´æ°åå®¹ #### 2023.5.4 - å¢å å¯¹æç©¹ééçç­¾å°åè½çæ¯æ -
+[#89](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/89) by @ayakasuki
+- ä¿®å¤æä»¶å½ä»¤ä¼ååº¦é®é¢ - [#88](https://github.com/Ljzd-PRO/
+nonebot-plugin-mystool/pull/88) by @ayakasuki - é¨åææ¬éè¯¯ä¿®æ­£ -
+[#90](https://github.com/Ljzd-PRO/nonebot-plugin-mystool/pull/90) by @black-
+zero358 #### 2023.4.28 - ä¿®å¤æä»¶å½ä»¤è¢«å¶ä» nonebot
 æä»¶æè·çé®é¢ - å¢å æ¯ææç©¹ééçåååæ¢ -
 æ¯æ¥ç­¾å°ãç±³æ¸¸å¸ä»»å¡æ§è¡æ¶é´å¨ç¨æ·éç½®çåºç¡ä¸å¢å éæºå»¶è¿
 - ä¿®å¤å¤§å«éé¢éæ¯æ¥ä»»å¡ãç­¾å°æ§è¡å¤±è´¥çé®é¢ ####
 2023.3.30 - ä¿®å¤éåéç½®æä»¶ `pluginConfig.json` ä¸çæçé®é¢ -
 ä¿®å¤åè´¦æ·æåµä¸æ æ³å¢å åæ¢è®¡åçé®é¢ - ä¿®å¤ `/åæ¢`
 å½ä»¤å¯è½ä¸å¶ä»æä»¶å½ä»¤å²çªçé®é¢ï¼åæ¶ [ðç¨æ³åæ´]
 (https://github.com/Ljzd-PRO/nonebot-plugin-mystool/wiki/Information-
 Exchange#å¢å å é¤åæ¢è®¡å) - ç²¾ç®æ¥æ¶çå½ä»¤ - æ´æ­£
-`device_save` "è®¾å¤ä¿å­" æ¥å¿ææ¬çéè¯¯ #### 2023.3.18 -
-å¢å å¯¼åºCookiesåè½ - å¢å å é¤è´¦å·æ°æ®åè½ -
-å¨ç¨æ·ææè´¦å·é½ç»å½å¤±æçæåµä¸å³é­éç¥ -
-ä¿®å¤åç¥æ¸¸æç­¾å°å¤±è´¥é®é¢ - è§èåä»£ç  ## åè½åç¹æ§ -
+`device_save` "è®¾å¤ä¿å­" æ¥å¿ææ¬çéè¯¯ ## åè½åç¹æ§ -
 ç­ä¿¡éªè¯ç»å½ï¼åæåè·å Cookie - èªå¨å®ææ¯æ¥ç±³æ¸¸å¸ä»»å¡
 - èªå¨è¿è¡æ¸¸æç­¾å° -
 å¯å¶å®ç±³æ¸¸å¸åååæ¢è®¡åï¼å°ç¹åæ¢ - å¯æ¯æå¤ä¸ª QQ
 è´¦å·ï¼æ¯ä¸ª QQ è´¦å·å¯ç»å®å¤ä¸ªç±³åæ¸¸è´¦æ· - QQ
 æ¨éæ§è¡ç»æéç¥ -
 åç¥æ èãæ´å¤©å®é±ãè´¨éååä»ªå·²æ»¡æ¶æ¨ééç¥ ##
 ä½¿ç¨è¯´æ ### ð ï¸ NoneBot2 æºå¨äººé¨ç½²åæä»¶å®è£ è¯·æ¥ç ->
```

