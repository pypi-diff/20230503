# Comparing `tmp/rpa_cooperativa-1.0.50.tar.gz` & `tmp/rpa_cooperativa-1.0.51.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.50.tar", last modified: Tue May  2 17:59:17 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.51.tar", last modified: Wed May  3 11:39:17 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.50.tar` & `rpa_cooperativa-1.0.51.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 17:59:17.785340 rpa_cooperativa-1.0.50/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.50/LICENSE
--rw-rw-rw-   0        0        0     6585 2023-05-02 17:59:17.782316 rpa_cooperativa-1.0.50/PKG-INFO
--rw-rw-rw-   0        0        0     5440 2023-05-02 17:52:50.000000 rpa_cooperativa-1.0.50/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 17:59:17.637392 rpa_cooperativa-1.0.50/rpa_coop/
--rw-rw-rw-   0        0        0      568 2023-05-02 17:34:09.000000 rpa_cooperativa-1.0.50/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:59:17.729851 rpa_cooperativa-1.0.50/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.50/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.50/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.50/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.50/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.50/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.50/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.50/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.50/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.50/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.50/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.50/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0    78671 2023-05-02 17:59:03.000000 rpa_cooperativa-1.0.50/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-05-02 17:59:17.772321 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6585 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      559 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-02 17:59:17.000000 rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-02 17:59:17.786318 rpa_cooperativa-1.0.50/setup.cfg
--rw-rw-rw-   0        0        0     2323 2023-05-02 17:58:41.000000 rpa_cooperativa-1.0.50/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:39:17.606253 rpa_cooperativa-1.0.51/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.51/LICENSE
+-rw-rw-rw-   0        0        0     6670 2023-05-03 11:39:17.598061 rpa_cooperativa-1.0.51/PKG-INFO
+-rw-rw-rw-   0        0        0     5525 2023-05-03 11:36:32.000000 rpa_cooperativa-1.0.51/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 11:39:17.350176 rpa_cooperativa-1.0.51/rpa_coop/
+-rw-rw-rw-   0        0        0      568 2023-05-02 17:34:09.000000 rpa_cooperativa-1.0.51/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:39:17.515048 rpa_cooperativa-1.0.51/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.51/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.51/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.51/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-02-28 19:52:56.000000 rpa_cooperativa-1.0.51/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      382 2023-02-28 19:50:17.000000 rpa_cooperativa-1.0.51/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.51/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.51/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.51/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.51/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.51/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.51/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0    80396 2023-05-03 11:33:25.000000 rpa_cooperativa-1.0.51/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-05-03 11:39:17.583741 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6670 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      559 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-03 11:39:16.000000 rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 11:39:17.608327 rpa_cooperativa-1.0.51/setup.cfg
+-rw-rw-rw-   0        0        0     2323 2023-05-03 11:36:40.000000 rpa_cooperativa-1.0.51/setup.py
```

### Comparing `rpa_cooperativa-1.0.50/LICENSE` & `rpa_cooperativa-1.0.51/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.50/PKG-INFO` & `rpa_cooperativa-1.0.51/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.50
+Version: 1.0.51
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -34,18 +34,24 @@
 
 ```python
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
+# Melhorias da versao 1.0.51
+## - Add metodo dia_util
+## - Add metodo mail
+
 ```
 
 ## metodo dias uteis
 ```python
+from rpa_coop import dia_util
+
 util_old = dia_util.dia_util_anterior()
 print(util_old)
 
 util_next = dia_util.dia_util_posterior()
 print(util_next)
 
 util_mes = dia_util.dias_uteis_mes()
@@ -72,25 +78,25 @@
 driver.maximize_window()
 ```
 
 ## manipulacao de emails:
 ```python
 from rpa_coop import mail
 
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg')
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui')
 
 lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']
-mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')
+mail.enviar_email(lista_dest, 'titulo aqui', 'msg aqui')
 
 anexos = ['notas.txt', 'README.md']
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui', anexos)
 
 anexos = ['notas.txt', 'README.md', 'imagem.PNG']
-html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)
+html_text_img = '<html><body><h1>msg aqui</h1><img src="cid:imagem_aqui.PNG"></body></html>'
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', anexos, html_text_img)
         
 ```
 
 
 ## manipulacao da ferramenta de fluxo de trabalho: fluid
 ```python
 ########################################################
```

### Comparing `rpa_cooperativa-1.0.50/README.md` & `rpa_cooperativa-1.0.51/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,18 +9,24 @@
 
 ```python
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
+# Melhorias da versao 1.0.51
+## - Add metodo dia_util
+## - Add metodo mail
+
 ```
 
 ## metodo dias uteis
 ```python
+from rpa_coop import dia_util
+
 util_old = dia_util.dia_util_anterior()
 print(util_old)
 
 util_next = dia_util.dia_util_posterior()
 print(util_next)
 
 util_mes = dia_util.dias_uteis_mes()
@@ -47,25 +53,25 @@
 driver.maximize_window()
 ```
 
 ## manipulacao de emails:
 ```python
 from rpa_coop import mail
 
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg')
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui')
 
 lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']
-mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')
+mail.enviar_email(lista_dest, 'titulo aqui', 'msg aqui')
 
 anexos = ['notas.txt', 'README.md']
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui', anexos)
 
 anexos = ['notas.txt', 'README.md', 'imagem.PNG']
-html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)
+html_text_img = '<html><body><h1>msg aqui</h1><img src="cid:imagem_aqui.PNG"></body></html>'
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', anexos, html_text_img)
         
 ```
 
 
 ## manipulacao da ferramenta de fluxo de trabalho: fluid
 ```python
 ########################################################
```

### Comparing `rpa_cooperativa-1.0.50/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.51/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.50/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.51/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.50/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.51/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.50/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.51/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.50/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.51/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.50/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.51/rpa_coop/rpa_coop.py`

 * *Files 2% similar despite different names*

```diff
@@ -985,92 +985,116 @@
                 {"type": "text", "text": texto}   
                 ]
             }
         response = requests.post(self.url_api_sms, headers=headers, json=body)
         cod_response  = response.status_code
         return cod_response
     
-   
-   
+    
 class Emails:
     import smtplib
     from email.mime.multipart import MIMEMultipart
     from email.mime.text import MIMEText
     from email.mime.application import MIMEApplication
     
     def __init__(self):
         self.user_mail = gerador_pwd('api_email', 'usuario')
         self.password_mail = gerador_pwd('api_email', 'sistema')
         self.smtpsrv = gerador_pwd('api_email', 'ip_host')
 
 
-    def enviar_email(self, destinatarios, assunto: str, mensagem: str, anexo=None, html_text_img=None, cc=None, cco=None):
+    def enviar_email(self, destinatarios, assunto: str, mensagem='', anexo=None, html_text_img=None, cc=None, cco=None):
         '''
-        mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg') \n\n
+        mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui') \n\n
         
         lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']\n
-        mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')\n\n
+        mail.enviar_email(lista_dest, 'titulo aqui', 'msg aqui')\n\n
         
         anexos = ['notas.txt', 'README.md']\n
-        mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)\n\n
+        mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui', anexos)\n\n
         
         anexos = ['notas.txt', 'README.md', 'imagem.PNG']\n
-        html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'\n
-        mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)\n
+        html_text_img = '<html><body><h1>msg aqui</h1><img src="cid:imagem_aqui.PNG"></body></html>'\n
+        mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', anexos, html_text_img)\n
         '''
         mail_content = mensagem
         smtpserver = self.smtplib.SMTP(self.smtpsrv,587)
         msg = self.MIMEMultipart('mixed')
         msg = self.MIMEMultipart('alternative')
-        
+        if cco: 
+            msg['Bcc'] = cco if type(cco) == str else ", ".join(cco)
+        if cc: 
+            msg['Cc'] = cc if type(cc) == str else ", ".join(cc)
+            
         msg['Subject'] = assunto
         msg['From'] = self.user_mail 
-        msg['To'] = destinatarios if type(destinatarios) == str else ",".join(destinatarios)
+        msg['To'] = destinatarios if type(destinatarios) == str else ", ".join(destinatarios)
 
-        if cc: 
-            print('existe com copia')
-            msg['Cc'] = cc if type(cc) == str else ",".join(cc)
-        if cco: 
-            print('existe copia oculta')
-            msg['Bcc'] = cco if type(cco) == str else ",".join(cco)
-        msg.attach(self.MIMEText(mail_content,'plain','utf8'))
-
-        msg.attach(self.MIMEText(html_text_img, 'html', 'utf-8'))
-        
-        if type(anexo) == str:
-            if anexo:
-                attachmentPath = anexo
-                try:
-                    with open(attachmentPath, "rb") as attachment:
-                        p = self.MIMEApplication(attachment.read(),_subtype="png")	
-                        p.add_header('Content-Disposition', "attachment; filename= %s" % attachmentPath) 
-                        msg.attach(p)
-                except Exception as e:
-                    print(str(e))
-        elif type(anexo) == list:
-            for attachmentPath in anexo:
-                try:
-                    with open(attachmentPath, "rb") as attachment:
-                        p = self.MIMEApplication(attachment.read(),_subtype="png")	
-                        p.add_header('Content-Disposition', "attachment; filename= %s" % attachmentPath) 
-                        msg.attach(p)
-                except Exception as e:
-                    print(str(e))
+        
+        if html_text_img:
+            msg.attach(self.MIMEText(mail_content + html_text_img, 'html', 'utf-8'))
+        else:
+            msg.attach(self.MIMEText(mail_content,'plain','utf8'))      
+        
+        if anexo:
+            if type(anexo) == str:
+                if anexo:
+                    attachmentPath = anexo
+                    try:
+                        with open(attachmentPath, "rb") as attachment:
+                            p = self.MIMEApplication(attachment.read(),_subtype="png")	
+                            p.add_header('Content-Disposition', "attachment; filename= %s" % attachmentPath) 
+                            msg.attach(p)
+                    except Exception as e:
+                        print(str(e))
+            elif type(anexo) == list:
+                for attachmentPath in anexo:
+                    try:
+                        with open(attachmentPath, "rb") as attachment:
+                            p = self.MIMEApplication(attachment.read(),_subtype="png")	
+                            p.add_header('Content-Disposition', "attachment; filename= %s" % attachmentPath) 
+                            msg.attach(p)
+                    except Exception as e:
+                        print(str(e))
             
-                
-
         #Send the Email Message
         smtpserver.ehlo()
         smtpserver.starttls()
         smtpserver.login(self.user_mail , self.password_mail)
-        smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=destinatarios)
-        smtpserver.close()
-
-
 
+        todos_destinos = []
+        if destinatarios and cc and cco:
+            if isinstance(destinatarios, list): todos_destinos.extend(destinatarios)
+            if isinstance(destinatarios, str): todos_destinos.append(destinatarios)
+            if isinstance(cc, list): todos_destinos.extend(cc)
+            if isinstance(cc, str): todos_destinos.append(cc)
+            if isinstance(cco, list): todos_destinos.extend(cco)
+            if isinstance(cco, str): todos_destinos.append(cco) 
+            smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=todos_destinos)
+        elif destinatarios and cc:
+            if isinstance(destinatarios, list): todos_destinos.extend(destinatarios)
+            if isinstance(destinatarios, str): todos_destinos.append(destinatarios)
+            if isinstance(cc, list): todos_destinos.extend(cc)
+            if isinstance(cc, str): todos_destinos.append(cc)
+            smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=todos_destinos)
+        elif destinatarios and cco:
+            if isinstance(destinatarios, list): todos_destinos.extend(destinatarios)
+            if isinstance(destinatarios, str): todos_destinos.append(destinatarios)
+            if isinstance(cco, list): todos_destinos.extend(cco)
+            if isinstance(cco, str): todos_destinos.append(cco) 
+            smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=todos_destinos)
+        else:
+            if isinstance(destinatarios, list): todos_destinos.extend(destinatarios)
+            if isinstance(destinatarios, str): todos_destinos.append(destinatarios)
+            smtpserver.send_message (msg, from_addr=self.user_mail, to_addrs=todos_destinos)
+            
+        smtpserver.close()
+        
+                
+        
 class Acc:
     import pyautogui as p
     import subprocess
     import pyperclip
     
     
     def __init__(self):
@@ -1256,15 +1280,14 @@
             if tentativas == max_tentativas:
                 resultado = False
         print(resultado)
         if resultado == False and continua_seerro == False:
             raise Exception(f'Execução pausada. O texto: "{texto_esperado}" não foi localizado durante a execução do robô.')
         return resultado
  
-   
            
 class Monitorar:
         
     import socket
     import paramiko
     from dateutil.relativedelta import relativedelta
          
@@ -1368,16 +1391,15 @@
         else:
             df = self.dados.consultar_banco_dados(self.conexao, f"SELECT * FROM rpa_fila WHERE status_rpa='{tipo_status}'")
         df = df[['cod_rpa', 'executar_na_vm', 'status_rpa']]
         print(df)
         print()
         return df
     
-            
-              
+                          
 class Escrever_por_extenso:  
             
     def __init__(self):
         self.url_api_escreve_por_extenso = str(gerador_pwd('por_extenso', 'senha'))
    
     
     def numero_por_extenso(self, valor:str):
@@ -1440,16 +1462,15 @@
             if 'VALOR NÃO SUPORTADO' in str(texto_e): texto_e = 'ZERO'
             res = requests.post(url, data={"Valor": f'{valor_d}', "Monetario": "Não"})
             texto_d =  res.json()['Valor'].upper()
             if 'VALOR NÃO SUPORTADO' in str(texto_d): texto_d = 'ZERO'
         taxa_extenso = texto_e + ' virgula ' + texto_d + ' por cento'    
         return taxa_extenso.upper()
         
-            
-             
+                     
 class Gerador_de_codigo:
     
     def __init__(self):
         pass
     
     
     def comentar_linha(self, path:str, search:str):
@@ -1529,15 +1550,14 @@
         
         file = open(script_file_path, 'a')
         file.write(txt)
         file.close()        
         self.comentar_linha(script_file_path, 'gerador_de_codigo.')
         
            
-  
 class Selenium:
     
     def __init__(self):
         pass
     
     from selenium import webdriver
     from selenium.webdriver.common.by import By
```

### Comparing `rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.50
+Version: 1.0.51
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
@@ -34,18 +34,24 @@
 
 ```python
 # Melhorias da versao 1.0.31
 ## - Add libs webdriver as service
 ## - Add libs dependencia para todos projetos da VM
 ## - Add acesso gerador de senhas
 ## - Melhoria metodos da classe fluid, exceptions caso nao retorne 200
+# Melhorias da versao 1.0.51
+## - Add metodo dia_util
+## - Add metodo mail
+
 ```
 
 ## metodo dias uteis
 ```python
+from rpa_coop import dia_util
+
 util_old = dia_util.dia_util_anterior()
 print(util_old)
 
 util_next = dia_util.dia_util_posterior()
 print(util_next)
 
 util_mes = dia_util.dias_uteis_mes()
@@ -72,25 +78,25 @@
 driver.maximize_window()
 ```
 
 ## manipulacao de emails:
 ```python
 from rpa_coop import mail
 
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg')
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui')
 
 lista_dest = ['usuario@dominio.com.br','appuser@dominio.com.br']
-mail.enviar_email(lista_dest, 'teste titulo2', 'teste msg')
+mail.enviar_email(lista_dest, 'titulo aqui', 'msg aqui')
 
 anexos = ['notas.txt', 'README.md']
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos)
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', 'msg aqui', anexos)
 
 anexos = ['notas.txt', 'README.md', 'imagem.PNG']
-html_text_img = '<html><body><h1>Teste img + texto</h1><img src="cid:imagem.PNG"></body></html>'
-mail.enviar_email('usuario@dominio.com.br', 'teste titulo2', 'teste msg', anexos, html_text_img)
+html_text_img = '<html><body><h1>msg aqui</h1><img src="cid:imagem_aqui.PNG"></body></html>'
+mail.enviar_email('usuario@dominio.com.br', 'titulo aqui', anexos, html_text_img)
         
 ```
 
 
 ## manipulacao da ferramenta de fluxo de trabalho: fluid
 ```python
 ########################################################
```

### Comparing `rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.50/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.51/rpa_cooperativa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.50/setup.py` & `rpa_cooperativa-1.0.51/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.50",
+    version="1.0.51",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
```

