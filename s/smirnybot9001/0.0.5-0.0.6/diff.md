# Comparing `tmp/smirnybot9001-0.0.5.tar.gz` & `tmp/smirnybot9001-0.0.6.tar.gz`

## Comparing `smirnybot9001-0.0.5.tar` & `smirnybot9001-0.0.6.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/TODO.md
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/pyproject.toml.mine
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/.github/workflows/pylint.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/__init__.py
--rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/chatbot.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/color_table.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/config.py
--rw-r--r--   0        0        0    16701 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/overlay.py
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/smirnyboot9001.py
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/data/__init__.py
--rw-r--r--   0        0        0   353160 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/data/happy-ending.wav
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/smirnybot9001/data/sample.conf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0   250886 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/bricklink_color_table.html
--rw-r--r--   0        0        0    10832 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/bricklink_color_table.pickle
--rw-r--r--   0        0        0    87399 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/bricklink_part_6339079.html
--rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/brickset_fig_mk003.html
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/minimal.conf
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/test.conf
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/test_bot.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/test_color_table.py
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/test_config.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/test_fig_scrape.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/test_overlay.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/test_part_scrape.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/tests/test_util.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/.gitignore
--rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/LICENSE
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/README.md
--rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/pyproject.toml
--rw-r--r--   0        0        0    42942 2020-02-02 00:00:00.000000 smirnybot9001-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/TODO.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/pyproject.toml.mine
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/__init__.py
+-rw-r--r--   0        0        0     7281 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/chatbot.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/color_table.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/config.py
+-rw-r--r--   0        0        0    17576 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/overlay.py
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/smirnyboot9001.py
+-rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/data/__init__.py
+-rw-r--r--   0        0        0   353160 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/data/happy-ending.wav
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/smirnybot9001/data/sample.conf
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0   250886 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/bricklink_color_table.html
+-rw-r--r--   0        0        0    10847 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/bricklink_color_table.pickle
+-rw-r--r--   0        0        0    87399 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/bricklink_part_6339079.html
+-rw-r--r--   0        0        0    88439 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/bricklink_set_colcol14-16.html
+-rw-r--r--   0        0        0    21578 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/brickset_fig_mk003.html
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/minimal.conf
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test.conf
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test_bot.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test_color_table.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test_config.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test_fig_scrape.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test_overlay.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test_part_scrape.py
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test_set_scrape.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/tests/test_util.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35823 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/LICENSE
+-rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/README.md
+-rw-r--r--   0        0        0     1338 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0    43619 2020-02-02 00:00:00.000000 smirnybot9001-0.0.6/PKG-INFO
```

### Comparing `smirnybot9001-0.0.5/pyproject.toml.mine` & `smirnybot9001-0.0.6/pyproject.toml.mine`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/.github/workflows/pylint.yml` & `smirnybot9001-0.0.6/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/smirnybot9001/chatbot.py` & `smirnybot9001-0.0.6/smirnybot9001/chatbot.py`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/smirnybot9001/color_table.py` & `smirnybot9001-0.0.6/smirnybot9001/color_table.py`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/smirnybot9001/config.py` & `smirnybot9001-0.0.6/smirnybot9001/config.py`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/smirnybot9001/overlay.py` & `smirnybot9001-0.0.6/smirnybot9001/overlay.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 from pathlib import Path
 import importlib.resources
 from urllib.parse import urlparse, parse_qs
 
 import socket
 import socketserver
 
-
-
 import remi
 import requests
 import typer
 from bs4 import BeautifulSoup
 from rich import print
 
 from smirnybot9001.config import SmirnyBot9001Config, create_config_and_inject_values, CONFIG_PATH_OPTION, WIDTH_OPTION, \
     HEIGHT_OPTION, ADDRESS_OPTION, PORT_OPTION, START_BROWSER_OPTION, DEBUG_OPTION, MAX_DURATION
-from smirnybot9001.util import get_with_user_agent
+from smirnybot9001.util import get_with_user_agent, parse_bricklink_meta_description
 from smirnybot9001.color_table import get_color_table
 
 
 # monkey patch socketserver.TCPServer to use IPV6 by default
 socketserver.TCPServer.address_family = socket.AF_INET6
 
 # monkey patch updated server_bind() method into socketserver.TCPServer
@@ -109,27 +107,38 @@
     image_url = f"https://img.bricklink.com/ItemImage/PN/{bl_color_id}/{bl_part_number}.png"
     return bl_color_id, bl_part_id, name, bl_part_number, r.url, image_url
 
 
 def extract_bricklink_part_info(bricklink_html):
     soup = BeautifulSoup(bricklink_html, 'html.parser')
     description = soup.find('meta', attrs={'name': 'description'}).get('content')
-    span_name = soup.find('span', id='item-name-title').text
+    span_name = soup.find('h1', id='item-name-title').text
     match = re.match(r'^ItemName: (?P<name>.*), ItemType:.* ItemNo: (?P<bl_number>.*), Buy and sell', description)
     if match:
-        name = match.group('name')
+        name_ = match.group('name')
         bl_number = match.group('bl_number')
 
     # bricklink has  a bug in their code missing a ", i have to pick the wrong data apart here...
     borked_image_url = soup.find('div', attrs={'data-color': '-99'}).get('data-imgurl')
     default_image_url = borked_image_url.split(' ')[0]
 
     return span_name, bl_number, default_image_url
 
 
+def extract_bricklink_set_info(bricklink_html):
+    soup = BeautifulSoup(bricklink_html, 'html.parser')
+    md = soup.find('meta', attrs={'name': 'description'})
+
+    description = None
+    if md is not None:
+        md = md.get('content')
+        description, type_, nr_ = parse_bricklink_meta_description(md)
+    return description
+
+
 def extract_fig_description_and_price(brickset_html):
     soup = BeautifulSoup(brickset_html, 'html.parser')
     description = soup.find('meta', {"property": "og:title"}).get('content')
     new = soup.find('dt', text='Current value').findNext('dd').findNext('a')
     price_new = new.text
     used = new.findNext('a')
     price_used = used.text
@@ -183,14 +192,18 @@
 
     def get_description(self):
 
         page = requests.get(self.brickset_url)
         soup = BeautifulSoup(page.text, 'html.parser')
         title = soup.find('meta', {"property": "og:title"}).get('content')
         description = soup.find(property='og:description').get('content')
+        if description == '':
+            page = get_with_user_agent(self.bricklink_url)
+            description = extract_bricklink_set_info(page.text)
+
         if title == '' and description == '':
             return ''
         else:
             return f"☠{title}: {description}☠"
 
     def get_image_url(self):
         if '-' not in self.number:
@@ -331,22 +344,26 @@
         bgcolor = 'red' if debug else 'transparent'
         label_bgcolor = 'green' if debug else 'white'
         # only show controls when debug is enabled
         show_controls = debug
         self.root_vbox = remi.gui.VBox(height=height, width=width,
                                        style={'display': 'block', 'overflow': 'visible', 'text-align': 'center',
                                               'background': bgcolor})
-        self.image_vbox = remi.gui.VBox(height='95%', width='99%',
+        self.image_vbox = remi.gui.VBox(height='99%', width='99%',
                                         style={'display': 'block', 'overflow': 'visible', 'text-align': 'center',
                                                'background': bgcolor})
         self.inputs_vbox = remi.gui.VBox(height=height / 10, width=width,
                                          style={'display': 'block', 'overflow': 'auto', 'text-align': 'center',
                                                 'background': bgcolor})
 
-        self.image = remi.gui.Image(APOCALYPSEBURG, height='85%', margin='10px')
+        self.image = remi.gui.Image(APOCALYPSEBURG, style={'object-fit': 'contain',
+                                                           'height': '85%',
+                                                           'width': '98%',
+                                                           'animation-name': 'sk-rotateplane',
+                                                           'animation-duration': '4s'})
         self.image_description_label = remi.gui.Label(width='100%', height='15%',
                                                       style={'display': 'block', 'overflow': 'visible',
                                                              'text-align': 'center', 'background': 'rgba(0,0,0,.6)',
                                                              'color': 'white', 'font-family': 'cursive',
                                                              'font-size': '40px', })
         self.set_description_text('🐸🐸🐸🐸 HELLO CHILLIBRIE 🐸🐸🐸🐸 ' * 2)
```

### Comparing `smirnybot9001-0.0.5/smirnybot9001/smirnyboot9001.py` & `smirnybot9001-0.0.6/smirnybot9001/smirnyboot9001.py`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/smirnybot9001/data/happy-ending.wav` & `smirnybot9001-0.0.6/smirnybot9001/data/happy-ending.wav`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/smirnybot9001/data/sample.conf` & `smirnybot9001-0.0.6/smirnybot9001/data/sample.conf`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/tests/bricklink_color_table.html` & `smirnybot9001-0.0.6/tests/bricklink_color_table.html`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/tests/bricklink_color_table.pickle` & `smirnybot9001-0.0.6/tests/bricklink_color_table.pickle`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 8004 9545 2a00 0000 0000 007d 9428 8c05  ...E*......}.(..
+00000000: 8004 9554 2a00 0000 0000 007d 9428 8c05  ...T*......}.(..
 00000010: 7768 6974 6594 4b01 4b01 6801 8c0f 7665  white.K.K.h...ve
 00000020: 7279 206c 6967 6874 2067 7261 7994 4b31  ry light gray.K1
 00000030: 8c0d 7665 7279 6c69 6768 7467 7261 7994  ..verylightgray.
 00000040: 4b31 8c0f 7665 7279 2d6c 6967 6874 2d67  K1..very-light-g
 00000050: 7261 7994 4b31 4b31 6802 8c16 7665 7279  ray.K1K1h...very
 00000060: 206c 6967 6874 2062 6c75 6973 6820 6772   light bluish gr
 00000070: 6179 944b 638c 1376 6572 796c 6967 6874  ay.Kc..verylight
@@ -670,8 +670,9 @@
 000029d0: 0000 8c0e 6d78 2066 6f69 6c20 7965 6c6c  ....mx foil yell
 000029e0: 6f77 944b da8c 0c6d 7866 6f69 6c79 656c  ow.K...mxfoilyel
 000029f0: 6c6f 7794 4bda 8c0e 6d78 2d66 6f69 6c2d  low.K...mx-foil-
 00002a00: 7965 6c6c 6f77 944b da4b da6a 1302 0000  yellow.K.K.j....
 00002a10: 8c0e 6d78 2066 6f69 6c20 6f72 616e 6765  ..mx foil orange
 00002a20: 944b db8c 0c6d 7866 6f69 6c6f 7261 6e67  .K...mxfoilorang
 00002a30: 6594 4bdb 8c0e 6d78 2d66 6f69 6c2d 6f72  e.K...mx-foil-or
-00002a40: 616e 6765 944b db4b db6a 1602 0000 752e  ange.K.K.j....u.
+00002a40: 616e 6765 944b db4b db6a 1602 0000 4a9d  ange.K.K.j....J.
+00002a50: ffff ff8c 074e 4f43 4f4c 4f52 9475 2e    .....NOCOLOR.u.
```

### Comparing `smirnybot9001-0.0.5/tests/bricklink_part_6339079.html` & `smirnybot9001-0.0.6/tests/bricklink_part_6339079.html`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/tests/brickset_fig_mk003.html` & `smirnybot9001-0.0.6/tests/brickset_fig_mk003.html`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/tests/test_bot.py` & `smirnybot9001-0.0.6/tests/test_bot.py`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/tests/test_color_table.py` & `smirnybot9001-0.0.6/tests/test_color_table.py`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/tests/test_config.py` & `smirnybot9001-0.0.6/tests/test_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 def test_create_minimal_config_obj():
     config = SmirnyBot9001Config.from_file_path(MINIMAL_CONF)
     assert isinstance(config, SmirnyBot9001Config)
     assert config.width == 1920
     assert config.height == 1080
-    assert config.address == '127.0.0.1'
+    assert config.address == '::'
     assert config.port == 4711
     assert config.channel is None
     assert config.token == 'TOPSECRET'
     assert config.display_wav_abs_path is None
     assert config.debug is False
     assert config.start_browser is False
```

### Comparing `smirnybot9001-0.0.5/tests/test_part_scrape.py` & `smirnybot9001-0.0.6/tests/test_set_scrape.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 from pathlib import Path
 
-import pytest
-from bs4 import BeautifulSoup
-
-from smirnybot9001.overlay import extract_bricklink_part_info
+from smirnybot9001.overlay import extract_bricklink_set_info
+from smirnybot9001.util import get_with_user_agent
 
 MYDIR = Path(__file__).resolve().parent
-TEST_HTML = MYDIR / 'bricklink_part_6339079.html'
+SET_NUM = 'col14-16'
+SET_URL = f"https://www.bricklink.com/v2/catalog/catalogitem.page?S={SET_NUM}"
+TEST_HTML = MYDIR / f"bricklink_set_col{SET_NUM}.html"
+
+
+def atest_write():
+    r = get_with_user_agent(SET_URL)
+    with open(TEST_HTML, 'w', encoding='utf-8') as of:
+        of.write(r.text)
 
 
 def test_read():
     r = open(TEST_HTML).read()
-    name, bl_number, url = extract_bricklink_part_info(r)
-    assert name == 'Minifigure, Head Dual Sided Black Eyebrows, Moustache, Open Mouth Grin, White Teeth / Bandage on Forehead Pattern - Hollow Stud'
-    assert bl_number == '3626cpb2900'
-    assert url == '//img.bricklink.com/ItemImage/PN/3/3626cpb2900.png'
+    description = extract_bricklink_set_info(r)
+    assert description == 'Spider Lady, Series 14 (Complete Set with Stand and Accessories)'
```

### Comparing `smirnybot9001-0.0.5/.gitignore` & `smirnybot9001-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/LICENSE` & `smirnybot9001-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `smirnybot9001-0.0.5/README.md` & `smirnybot9001-0.0.6/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 # smirnybot9001
 A twitch chatbot for displaying LEGO sets, minifigs and parts on an HTML overlay
 
 ## Installation - Windows
 
 1. Download and Install Python https://www.python.org/downloads/
-2. Select a directory to install a Python virtualenv and open a command line
-3. Create the venv: `python -m venv VENVDIR`
-4. Activate the venv: `VENVDIR/Scripts/activate.bat`
-5. Install the SmirnyBot into the venv `python -m pip install smirnybot9001`
+2. Select a directory to install a Python virtualenv and open a command line with the
+following instructions
+3. Using Command line, create the venv: `python -m venv VENVDIR`. e.g. `C:\Users\***User***\>python -m venv Smirny_Venv`
+4. Activate the venv: `VENVDIR/Scripts/activate.bat` e.g. `C:\Users\***User***\Smirny_Venv\Scripts>activate.bat` 
+5. Install the SmirnyBot into the venv `python -m pip install smirnybot9001` e.g. `C:\Users\***User***\Smirny_Venv\Scripts>python -m pip install smirnybot9001`
 6. Check that the Bot executables are installed in `VENVDIR/Scripts  smirnyboot9001.exe overlay.exe chatbot.exe`
-7. Run `smirnyboot.exe --help` and note the default location of the config file (Usually ` HOMEDIR\smirnybot9001.conf`)
-8. Copy the sample config file from `VENVDIR\Lib\site-packages\smirnybot9001\data\sample.conf` to the location noted above
+7. Run `smirnyboot.exe --help` and note the default location of the config file (Usually ` HOMEDIR\smirnybot9001.conf`) e.g. `C:\Users\***User***\Smirny_Venv\Scripts>smirnyboot.exe -h` 
+8. Copy the sample config file from `VENVDIR\Lib\site-packages\smirnybot9001\data\sample.conf` to the location noted above (from running `smirnyboot.exe --help`)
 9. Create a token for your chatbot twitch user (we recommend using a different user than your personal one) by visiting: https://twitchtokengenerator.com/
-10. Configure your newly created token and your channel name (Usually your personal username) in the config file
+10. Configure your newly created token and your channel name (Usually your personal username) in the config file leaving double quotation marks in place
 11. Start the bot and overlay using the `smirnyboot9001.exe` executable
-12. Browse to http://127.0.0.1:4711 to ensure that the overlay is running
+12. Browse to http://127.0.0.1:4711 using any browser to ensure that the overlay is running
 13. Create a Browser Source in OBS and set the URL to: http://127.0.0.1:4711. Make sure the "Control audio via OBS option is set"
 14. Test the bot! Enter `!set 10228` in your chat and see if the overlay displays the wanted set.
 
 
 
 ## Installation - Linux
 
 The Bot has not been tested under Linux but should work just fine
 
 
+## Updating
 
-## ‍☠
+To update the Bot simply use pip in the location you installed it:
+
+1. Update the SmirnyBot inside the venv `python -m pip install --upgrade smirnybot9001` e.g. `C:\Users\***User***\Smirny_Venv\Scripts>python -m pip install --upgrade smirnybot9001`
 
+
+## ‍☠
```

### Comparing `smirnybot9001-0.0.5/pyproject.toml` & `smirnybot9001-0.0.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 #build-backend = "flit_core.buildapi"
 
 #requires = ["pdm-pep517"]
 #build-backend = "pdm.pep517.api"
 
 [project]
 name = "smirnybot9001"
-version = "0.0.5"
+version = "0.0.6"
 description = "A twitch chatbot for displaying LEGO sets, minifigs and parts on an HTML overlay"
 authors = [
   { name="Bricks Mental", email="bricks.mental@gmail.com" },
 ]
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `smirnybot9001-0.0.5/PKG-INFO` & `smirnybot9001-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smirnybot9001
-Version: 0.0.5
+Version: 0.0.6
 Summary: A twitch chatbot for displaying LEGO sets, minifigs and parts on an HTML overlay
 Project-URL: Homepage, https://github.com/BricksMental/smirnybot9001
 Project-URL: Bug Tracker, https://github.com/BricksMental/smirnybot9001/issues
 Author-email: Bricks Mental <bricks.mental@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -697,31 +697,37 @@
 
 # smirnybot9001
 A twitch chatbot for displaying LEGO sets, minifigs and parts on an HTML overlay
 
 ## Installation - Windows
 
 1. Download and Install Python https://www.python.org/downloads/
-2. Select a directory to install a Python virtualenv and open a command line
-3. Create the venv: `python -m venv VENVDIR`
-4. Activate the venv: `VENVDIR/Scripts/activate.bat`
-5. Install the SmirnyBot into the venv `python -m pip install smirnybot9001`
+2. Select a directory to install a Python virtualenv and open a command line with the
+following instructions
+3. Using Command line, create the venv: `python -m venv VENVDIR`. e.g. `C:\Users\***User***\>python -m venv Smirny_Venv`
+4. Activate the venv: `VENVDIR/Scripts/activate.bat` e.g. `C:\Users\***User***\Smirny_Venv\Scripts>activate.bat` 
+5. Install the SmirnyBot into the venv `python -m pip install smirnybot9001` e.g. `C:\Users\***User***\Smirny_Venv\Scripts>python -m pip install smirnybot9001`
 6. Check that the Bot executables are installed in `VENVDIR/Scripts  smirnyboot9001.exe overlay.exe chatbot.exe`
-7. Run `smirnyboot.exe --help` and note the default location of the config file (Usually ` HOMEDIR\smirnybot9001.conf`)
-8. Copy the sample config file from `VENVDIR\Lib\site-packages\smirnybot9001\data\sample.conf` to the location noted above
+7. Run `smirnyboot.exe --help` and note the default location of the config file (Usually ` HOMEDIR\smirnybot9001.conf`) e.g. `C:\Users\***User***\Smirny_Venv\Scripts>smirnyboot.exe -h` 
+8. Copy the sample config file from `VENVDIR\Lib\site-packages\smirnybot9001\data\sample.conf` to the location noted above (from running `smirnyboot.exe --help`)
 9. Create a token for your chatbot twitch user (we recommend using a different user than your personal one) by visiting: https://twitchtokengenerator.com/
-10. Configure your newly created token and your channel name (Usually your personal username) in the config file
+10. Configure your newly created token and your channel name (Usually your personal username) in the config file leaving double quotation marks in place
 11. Start the bot and overlay using the `smirnyboot9001.exe` executable
-12. Browse to http://127.0.0.1:4711 to ensure that the overlay is running
+12. Browse to http://127.0.0.1:4711 using any browser to ensure that the overlay is running
 13. Create a Browser Source in OBS and set the URL to: http://127.0.0.1:4711. Make sure the "Control audio via OBS option is set"
 14. Test the bot! Enter `!set 10228` in your chat and see if the overlay displays the wanted set.
 
 
 
 ## Installation - Linux
 
 The Bot has not been tested under Linux but should work just fine
 
 
+## Updating
 
-## ‍☠
+To update the Bot simply use pip in the location you installed it:
+
+1. Update the SmirnyBot inside the venv `python -m pip install --upgrade smirnybot9001` e.g. `C:\Users\***User***\Smirny_Venv\Scripts>python -m pip install --upgrade smirnybot9001`
 
+
+## ‍☠
```

