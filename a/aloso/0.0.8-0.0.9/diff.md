# Comparing `tmp/aloso-0.0.8-py3-none-any.whl.zip` & `tmp/aloso-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 16478 bytes, number of entries: 28
+Zip file size: 17740 bytes, number of entries: 28
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-01 10:09 domain/__init__.py
--rw-rw-r--  2.0 unx      252 b- defN 23-Jan-27 15:19 domain/certificate_management.py
--rw-rw-r--  2.0 unx      745 b- defN 22-Dec-08 13:44 domain/contact.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jan-31 15:38 domain/equipment_management.py
--rw-rw-r--  2.0 unx      106 b- defN 23-Feb-16 07:43 domain/grafana.py
--rw-rw-r--  2.0 unx      358 b- defN 22-Dec-08 14:41 domain/label.py
--rw-rw-r--  2.0 unx      413 b- defN 23-Feb-14 14:28 domain/record_dns.py
--rw-rw-r--  2.0 unx     1312 b- defN 22-Nov-30 13:02 domain/script_model.py
--rw-rw-r--  2.0 unx      389 b- defN 22-Dec-08 14:41 domain/site.py
+-rw-rw-r--  2.0 unx      571 b- defN 23-Feb-20 10:20 domain/certificate_management.py
+-rw-rw-r--  2.0 unx     1063 b- defN 23-Feb-20 10:20 domain/contact.py
+-rw-rw-r--  2.0 unx     1124 b- defN 23-Feb-20 10:20 domain/equipment_management.py
+-rw-rw-r--  2.0 unx      555 b- defN 23-Feb-20 08:49 domain/grafana.py
+-rw-rw-r--  2.0 unx      677 b- defN 23-Feb-20 10:20 domain/label.py
+-rw-rw-r--  2.0 unx      732 b- defN 23-Feb-20 10:20 domain/record_dns.py
+-rw-rw-r--  2.0 unx     1616 b- defN 23-Feb-20 10:20 domain/script_model.py
+-rw-rw-r--  2.0 unx      708 b- defN 23-Feb-20 10:20 domain/site.py
 -rw-rw-r--  2.0 unx     1126 b- defN 23-Jan-23 11:30 domain/switch_management.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-01 10:09 output/__init__.py
 -rw-rw-r--  2.0 unx     1150 b- defN 22-Sep-15 08:00 output/certificate_shell.py
 -rw-rw-r--  2.0 unx     4010 b- defN 23-Jan-24 11:46 output/contact_database.py
 -rw-rw-r--  2.0 unx     1878 b- defN 22-Dec-01 16:21 output/contact_sheet.py
 -rw-rw-r--  2.0 unx      370 b- defN 22-Dec-07 14:58 output/database_base.py
 -rw-rw-r--  2.0 unx      326 b- defN 23-Feb-10 11:23 output/directories.py
 -rw-rw-r--  2.0 unx     6293 b- defN 23-Jan-31 15:40 output/equipment_shell.py
--rw-rw-r--  2.0 unx     3120 b- defN 23-Feb-17 14:46 output/grafana_shell.py
+-rw-rw-r--  2.0 unx     4412 b- defN 23-Feb-20 10:16 output/grafana_shell.py
 -rw-rw-r--  2.0 unx     3018 b- defN 23-Jan-24 11:46 output/label_database.py
 -rw-rw-r--  2.0 unx      687 b- defN 23-Feb-14 14:28 output/record_dns_bind9.py
 -rw-rw-r--  2.0 unx     1918 b- defN 23-Feb-16 14:55 output/record_dns_infoblox.py
 -rw-rw-r--  2.0 unx     5230 b- defN 23-Jan-23 11:27 output/script_model_shell.py
 -rw-rw-r--  2.0 unx     3533 b- defN 23-Jan-25 11:03 output/site_database.py
 -rw-rw-r--  2.0 unx     4684 b- defN 23-Jan-27 14:13 output/switch_shell.py
--rw-rw-r--  2.0 unx      526 b- defN 23-Feb-17 14:46 aloso-0.0.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Feb-17 14:46 aloso-0.0.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-Feb-17 14:46 aloso-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2191 b- defN 23-Feb-17 14:46 aloso-0.0.8.dist-info/RECORD
-28 files, 44561 bytes uncompressed, 12988 bytes compressed:  70.9%
+-rw-rw-r--  2.0 unx      526 b- defN 23-Feb-20 10:21 aloso-0.0.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Feb-20 10:21 aloso-0.0.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-Feb-20 10:21 aloso-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2193 b- defN 23-Feb-20 10:21 aloso-0.0.9.dist-info/RECORD
+28 files, 48506 bytes uncompressed, 14250 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -66,20 +66,20 @@
 
 Filename: output/site_database.py
 Comment: 
 
 Filename: output/switch_shell.py
 Comment: 
 
-Filename: aloso-0.0.8.dist-info/METADATA
+Filename: aloso-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: aloso-0.0.8.dist-info/WHEEL
+Filename: aloso-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: aloso-0.0.8.dist-info/top_level.txt
+Filename: aloso-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: aloso-0.0.8.dist-info/RECORD
+Filename: aloso-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## domain/certificate_management.py

```diff
@@ -1,9 +1,18 @@
+import logging
 from dataclasses import dataclass
 
+import config
+
+logging.basicConfig(level=config.debug_level,
+                    format='%(asctime)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s',
+                    datefmt='%d/%m/%Y %H:%M:%S',
+                    filename=config.logs_file_path,
+                    filemode='a')
+
 
 @dataclass
 class Certificate:
     country: str = ""
     state: str = ""
     locality: str = ""
     organization: str = ""
```

## domain/contact.py

```diff
@@ -1,12 +1,20 @@
+import logging
 from dataclasses import dataclass
 
+import config
 from domain.label import Label
 from domain.site import Site
 
+logging.basicConfig(level=config.debug_level,
+                    format='%(asctime)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s',
+                    datefmt='%d/%m/%Y %H:%M:%S',
+                    filename=config.logs_file_path,
+                    filemode='a')
+
 
 @dataclass
 class Contact:
     last_name: str
     first_name: str
     number: str
     mail: str
```

## domain/equipment_management.py

```diff
@@ -1,13 +1,20 @@
+import logging
 from dataclasses import dataclass
 from ftplib import FTP
 from typing import ClassVar
 
 import config
 
+logging.basicConfig(level=config.debug_level,
+                    format='%(asctime)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s',
+                    datefmt='%d/%m/%Y %H:%M:%S',
+                    filename=config.logs_file_path,
+                    filemode='a')
+
 
 @dataclass
 class TypeEquipments:
     name: str = ""
 
 
 @dataclass
```

## domain/grafana.py

```diff
@@ -1,7 +1,25 @@
+import logging
 from dataclasses import dataclass
 
+import config
+
+logging.basicConfig(level=config.debug_level,
+                    format='%(asctime)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s',
+                    datefmt='%d/%m/%Y %H:%M:%S',
+                    filename=config.logs_file_path,
+                    filemode='a')
+
 
 @dataclass
 class Grafana:
-    def install_grafana(self):
+    @staticmethod
+    def install_grafana():
+        pass
+
+    @staticmethod
+    def install_loki():
+        pass
+
+    @staticmethod
+    def install_promtail():
         pass
```

## domain/label.py

```diff
@@ -1,9 +1,18 @@
+import logging
 from dataclasses import dataclass
 
+import config
+
+logging.basicConfig(level=config.debug_level,
+                    format='%(asctime)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s',
+                    datefmt='%d/%m/%Y %H:%M:%S',
+                    filename=config.logs_file_path,
+                    filemode='a')
+
 
 @dataclass
 class Label:
     label_name: str
 
     #    contacts: list[Contact]
```

## domain/record_dns.py

```diff
@@ -1,10 +1,19 @@
+import logging
 from dataclasses import dataclass, field
 from typing import List
 
+import config
+
+logging.basicConfig(level=config.debug_level,
+                    format='%(asctime)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s',
+                    datefmt='%d/%m/%Y %H:%M:%S',
+                    filename=config.logs_file_path,
+                    filemode='a')
+
 
 @dataclass
 class Alias:
     name: str = ""
     open_data: List[str] = field(default_factory=list)
 
     def get_records(self, alias_file_path: str):
```

## domain/script_model.py

```diff
@@ -1,11 +1,18 @@
+import logging
 from dataclasses import dataclass
 
 import config
 
+logging.basicConfig(level=config.debug_level,
+                    format='%(asctime)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s',
+                    datefmt='%d/%m/%Y %H:%M:%S',
+                    filename=config.logs_file_path,
+                    filemode='a')
+
 
 @dataclass
 class ScriptModel:
 
     def exec_commands_on_equipments(self, file_name: str, list_equipments: list,
                                     directory: str = config.templates_directory_path):
         pass
```

## domain/site.py

```diff
@@ -1,9 +1,18 @@
+import logging
 from dataclasses import dataclass
 
+import config
+
+logging.basicConfig(level=config.debug_level,
+                    format='%(asctime)s %(levelname)s %(pathname)s %(funcName)s %(lineno)d : %(message)s',
+                    datefmt='%d/%m/%Y %H:%M:%S',
+                    filename=config.logs_file_path,
+                    filemode='a')
+
 
 @dataclass
 class Site:
     site_name: str
 
     #    contacts: list[Contact]
```

## output/grafana_shell.py

```diff
@@ -1,7 +1,8 @@
+import logging
 from fabric import Connection, Config
 import config
 from domain.grafana import Grafana
 
 
 # Using SSH key
 # KEY_FILE = '/exnovo/etc/ssh/'
@@ -13,79 +14,122 @@
 
 class GrafanaShell(Grafana):
     @staticmethod
     def connection():
         configuration = Config(overrides={'user': config.grafana_username,
                                           'port': config.grafana_port,
                                           'sudo': {'password': config.grafana_password}})
-        conn = Connection(host=config.grafana_host, config=configuration)
-        return conn
+        try:
+            conn = Connection(host=config.grafana_host, config=configuration)
+            return conn
+        except Exception as e:
+            logging.error(f"Erreur de connexion au serveur : {e}")
 
     @staticmethod
     def install_grafana():
         conn = GrafanaShell.connection()
 
+        grafana_deb_file = config.grafana_wget_url.split("/")[-1]
+
         commands = [
-            'add-apt-repository "deb https://packages.grafana.com/oss/deb stable main"',
-            'apt update',
-            'apt -y install grafana',
-            'rm -f /etc/grafana/grafana.ini',
+            'apt-get install -y adduser libfontconfig1',
+            f'wget {config.grafana_wget_url}',
+            f'dpkg -i {grafana_deb_file}',
+            f'rm {grafana_deb_file}',
             'mv grafana.ini /etc/grafana/grafana.ini',
             'systemctl daemon-reload',
             'systemctl restart grafana-server'
         ]
 
         conn.put(config.grafana_ini_file)
-        conn.run('curl https://packages.grafana.com/gpg.key | apt-key add -', hide=True)
+        logging.info("Fichier de configuration de Grafana envoyé")
 
-        for command in commands:
-            conn.run(command)
+        try:
+            for command in commands:
+                if config.use_sudo:
+                    conn.sudo(command)
+                else:
+                    conn.run(command)
+            logging.info("Grafana installé avec succès")
+        except Exception as e:
+            logging.error(f"Erreur d'installaton de Grafana : {e}")
 
     @staticmethod
     def install_loki():
         conn = GrafanaShell.connection()
 
+        loki_zip_file = config.loki_wget_url.split("/")[-1]
+
         conn.put(config.loki_yaml_file)
         conn.put(config.loki_service_file)
 
         commands = [
-            "curl -s https://api.github.com/repos/grafana/loki/releases/latest | grep browser_download_url |  cut -d '\"' -f 4 | grep loki-linux-amd64.zip | wget -i -",
-            "unzip loki-linux-amd64.zip",
-            "rm loki-linux-amd64.zip",
+            f"wget {config.loki_wget_url}",
+            f"unzip {loki_zip_file}",
+            f"rm {loki_zip_file}",
             "mv loki-linux-amd64 /usr/local/bin/loki",
             "mkdir -p /data/loki",
             "mv loki-local-config.yaml /etc/loki-local-config.yaml",
             "mv loki.service /etc/systemd/system/loki.service",
             "systemctl daemon-reload",
             "systemctl start loki.service"
         ]
-
-        for command in commands:
-            conn.sudo(command)
+        try:
+            for command in commands:
+                if config.use_sudo:
+                    conn.sudo(command)
+                else:
+                    conn.run(command)
+            logging.info("Loki installé avec succès")
+        except Exception as e:
+            logging.error(f"Erreur d'installaton de Loki : {e}")
 
     @staticmethod
     def install_promtail():
         conn = GrafanaShell.connection()
 
+        promtail_zip_file = config.promtail_wget_url.split("/")[-1]
+
         conn.put(config.promtail_yaml_file)
         conn.put(config.promtail_service_file)
 
-        # Installation de Promtail
         commands = [
-            "curl -s https://api.github.com/repos/grafana/loki/releases/latest | grep browser_download_url |  cut -d '\"' -f 4 | grep promtail-linux-amd64.zip | wget -i -",
-            "unzip promtail-linux-amd64.zip",
-            "rm promtail-linux-amd64.zip",
+            f"wget {config.promtail_wget_url}",
+            f"unzip {promtail_zip_file}",
+            f"rm {promtail_zip_file}",
             "mv promtail-linux-amd64 /usr/local/bin/promtail",
             "mv promtail-local-config.yaml /etc/promtail-local-config.yaml",
             "mv promtail.service /etc/systemd/system/promtail.service",
             "systemctl daemon-reload",
             "systemctl start promtail.service"
         ]
+        try:
+            for command in commands:
+                if config.use_sudo:
+                    conn.sudo(command)
+                else:
+                    conn.run(command)
+            logging.info("Promtail installé avec succès")
+        except Exception as e:
+            logging.error(f"Erreur d'installaton de Promtail : {e}")
 
+    @staticmethod
+    def remove_grafana():
+        conn = GrafanaShell.connection()
+        commands = [
+            'systemctl stop grafana-server',
+            'dpkg -P grafana-enterprise',
+            'rm -r /etc/grafana',
+            'systemctl daemon-reload',
+        ]
         for command in commands:
-            conn.sudo(command)
+            if config.use_sudo:
+                conn.sudo(command)
+            else:
+                conn.run(command)
 
 
 if __name__ == "__main__":
     # GrafanaShell.install_grafana()
-    # GrafanaShell.install_loki()
-    GrafanaShell.install_promtail()
+    # GrafanaShell.remove_grafana()
+    GrafanaShell.install_loki()
+    # GrafanaShell.install_promtail()
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `aloso-0.0.8.dist-info/METADATA` & `aloso-0.0.9.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aloso
-Version: 0.0.8
+Version: 0.0.9
 Summary: Lib
 Author: Aleos
 Author-email: aae5654ae@mozmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `aloso-0.0.8.dist-info/RECORD` & `aloso-0.0.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 domain/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-domain/certificate_management.py,sha256=k3QFqZhZ76EUaL9McjB6MPuPP1yi3_olatqBojV-JRQ,252
-domain/contact.py,sha256=vlLwGoS3w8gaPTvXeAn0nADdiIfKgf6ZxE1enDPZ838,745
-domain/equipment_management.py,sha256=sqeHJRnF-zyRNWob8JGwBgh5MgPKdYpFrvjP_dy9uYY,820
-domain/grafana.py,sha256=9MrulGo1ztk5b5MmqYcGyOXKaWYV_WxPIdBszL9T0Ws,106
-domain/label.py,sha256=svTQsy2SrP5qwe-Q-CoWXvNLKx0rC_PD1JxqBXsmNB0,358
-domain/record_dns.py,sha256=-kvHdRXJf4N5p4OdejnDa4OsNgYQhLwlq_CsTNzjChQ,413
-domain/script_model.py,sha256=nV8hxTgdxWVRfwig7qapTi5e3hHHvvQzIXhL6TQTues,1312
-domain/site.py,sha256=rbP9Jcmkq8tBLGAru-tmfEATC87m4H8VjSb15pmOxKo,389
+domain/certificate_management.py,sha256=gAcA6k9TNDbUvdBd4GtkfhKvO_IIrgVRx8rPCSuiLtw,571
+domain/contact.py,sha256=IqYjyZPtFL2mcA8SvUCLC-uiI3kpKwS6ooMLQtYYlWA,1063
+domain/equipment_management.py,sha256=ncstcUgOmb8k4xohDEu-446Qizzcvw-A2IfLxKqRsT8,1124
+domain/grafana.py,sha256=0s7A8Z75OroZ9YFn_KIicb25ZdWCZpKWfzY2RxKxIZw,555
+domain/label.py,sha256=jJQ-CqJNxOmYviwAmTG46DGFF23u4LBKphGm34ihFAw,677
+domain/record_dns.py,sha256=RJNmGD58JxfxAoSJsD59dp0VP1oNW_0AXFKq2gzMn0I,732
+domain/script_model.py,sha256=GWGaUB9dfD_hFQgfBMhxQFT4s9E76ISyhrIa4q89gBA,1616
+domain/site.py,sha256=Cam1s-mZyb0C03ZT1LPLluI8iBLjZi84Cz0pGQOcoAI,708
 domain/switch_management.py,sha256=iKiAkxtxcMx9ostZ18HSNd7_HvZGz7kx1dAQ0_KWmiA,1126
 output/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 output/certificate_shell.py,sha256=02DZQobN2nVwAltpmBwmn3xm7r8aDJ9Q75xsVK64cyg,1150
 output/contact_database.py,sha256=fA0S6XV3rcCeWAaDykz1f1QHWylWFGMHX97SmdordPs,4010
 output/contact_sheet.py,sha256=kTqP1UP84Tfb2r1-BR2r-uc6CEr9-BJCCQxan6BB0nc,1878
 output/database_base.py,sha256=5g0x55LtJxkkxUAzheCrCzgxrJxMx4lNJObHLSrwfhg,370
 output/directories.py,sha256=FHym04_qRnsYERJ7-0xgkbY7me40bzavD8Z7oZ5uADI,326
 output/equipment_shell.py,sha256=uTeJS9f9QsBBoUv9liF9Ml2HDbHa5Ow_44Ig2-g86tQ,6293
-output/grafana_shell.py,sha256=fzJIjJDf-8jJiWvMmpQB4W0-8hlEuMtYHwAMiIRUyOY,3120
+output/grafana_shell.py,sha256=c1lPM_R9mFT6QpUJFmvxjY7dmoefa1VFUYS2i-2EZjM,4412
 output/label_database.py,sha256=evYVTQBoh8utMfsZ3d0Mh5DF-quwO6G9atVV8-rTlEg,3018
 output/record_dns_bind9.py,sha256=YVIg69xA5uHqHpe7FJk-lguKI1qP-IVmMSuzZ9y1nhM,687
 output/record_dns_infoblox.py,sha256=Q0q7wUxM5nkiCraIijrjj39M2MWx2RlwjWraikPxEhM,1918
 output/script_model_shell.py,sha256=KaVJqr4qLpV_9Uo_JUavAzZbHq-13U7ChkdQJklSe3k,5230
 output/site_database.py,sha256=JZQ3hPt0vQi1O9Vo-lKXboup0J585vFubMEGa-vTJHQ,3533
 output/switch_shell.py,sha256=hLknpZK_0QMbANKHsF5pmO7nuCIBxSYtqimBXChfD94,4684
-aloso-0.0.8.dist-info/METADATA,sha256=eiRNQuylTAQU11y8yxgTLFtZ51VNdfdJTjuwX0bGz5k,526
-aloso-0.0.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-aloso-0.0.8.dist-info/top_level.txt,sha256=J-8QuKpAz07atczr2fgSeuF-OirBdTsk0Hu6WIK9dD0,14
-aloso-0.0.8.dist-info/RECORD,,
+aloso-0.0.9.dist-info/METADATA,sha256=jFhn0lZYrq_-DaQR8vByYkZkdo3_mureYXY6UGb4bEQ,526
+aloso-0.0.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+aloso-0.0.9.dist-info/top_level.txt,sha256=J-8QuKpAz07atczr2fgSeuF-OirBdTsk0Hu6WIK9dD0,14
+aloso-0.0.9.dist-info/RECORD,,
```

