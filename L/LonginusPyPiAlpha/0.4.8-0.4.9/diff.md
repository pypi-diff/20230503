# Comparing `tmp/LonginusPyPiAlpha-0.4.8.tar.gz` & `tmp/LonginusPyPiAlpha-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LonginusPyPiAlpha-0.4.8.tar", last modified: Wed Feb  1 13:53:08 2023, max compression
+gzip compressed data, was "LonginusPyPiAlpha-0.4.9.tar", last modified: Tue Feb  7 12:49:17 2023, max compression
```

## Comparing `LonginusPyPiAlpha-0.4.8.tar` & `LonginusPyPiAlpha-0.4.9.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-01 13:53:08.150064 LonginusPyPiAlpha-0.4.8/
-drwxrwxrwx   0        0        0        0 2023-02-01 13:53:08.129045 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/
--rw-rw-rw-   0        0        0    21094 2023-02-01 13:51:11.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/LClient.py
--rw-rw-rw-   0        0        0    27386 2023-02-01 13:49:04.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/LServer.py
--rw-rw-rw-   0        0        0     2855 2023-01-29 12:34:39.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/LonginusP.py
--rw-rw-rw-   0        0        0     1947 2023-01-21 16:23:04.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/Lshell.py
--rw-rw-rw-   0        0        0      143 2023-01-17 02:43:24.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/__init__.py
--rw-rw-rw-   0        0        0      511 2023-01-27 16:30:13.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/diffie-hellman.py
-drwxrwxrwx   0        0        0        0 2023-02-01 13:53:08.148062 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha.egg-info/
--rw-rw-rw-   0        0        0      725 2023-02-01 13:53:08.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-02-01 13:53:08.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-01 13:53:08.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-02-01 13:53:08.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-02-01 13:53:08.000000 LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      725 2023-02-01 13:53:08.149063 LonginusPyPiAlpha-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-01-18 06:04:21.000000 LonginusPyPiAlpha-0.4.8/README.md
--rw-rw-rw-   0        0        0      443 2023-02-01 13:52:50.000000 LonginusPyPiAlpha-0.4.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-01 13:53:08.150064 LonginusPyPiAlpha-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-02-01 13:52:45.000000 LonginusPyPiAlpha-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-07 12:49:17.572221 LonginusPyPiAlpha-0.4.9/
+drwxrwxrwx   0        0        0        0 2023-02-07 12:49:17.554205 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/
+-rw-rw-rw-   0        0        0    21529 2023-02-07 12:49:07.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/LClient.py
+-rw-rw-rw-   0        0        0    30391 2023-02-07 12:46:48.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/LServer.py
+-rw-rw-rw-   0        0        0     2789 2023-02-01 16:32:06.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/LonginusP.py
+-rw-rw-rw-   0        0        0     1947 2023-01-21 16:23:04.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/Lshell.py
+-rw-rw-rw-   0        0        0      143 2023-01-17 02:43:24.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-07 12:49:17.570220 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-02-07 12:49:17.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-02-07 12:49:17.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-07 12:49:17.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-02-07 12:49:17.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-02-07 12:49:17.000000 LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      725 2023-02-07 12:49:17.571220 LonginusPyPiAlpha-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-01-18 06:04:21.000000 LonginusPyPiAlpha-0.4.9/README.md
+-rw-rw-rw-   0        0        0      443 2023-02-07 12:47:29.000000 LonginusPyPiAlpha-0.4.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-02-07 12:49:17.572221 LonginusPyPiAlpha-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      681 2023-02-07 12:48:40.000000 LonginusPyPiAlpha-0.4.9/setup.py
```

### Comparing `LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/LClient.py` & `LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/LClient.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from LonginusPyPiAlpha import Longinus
 from Cryptodome.Cipher import AES #line:32
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Cipher import AES, PKCS1_OAEP
-from diffiehellman import DiffieHellman
 import subprocess,threading,sys,os
 from socket import *
 from getpass import *
 from datetime import datetime
 from asyncio import *
 from hashlib import sha256
 from argon2 import PasswordHasher
@@ -15,31 +14,34 @@
 import struct
 
 __all__=['Client']
 
 class Client:
     L=Longinus()
     ClientDB:dict=dict()
-    def __init__(self,set_addr:str='127.0.0.1',set_port:int=9997,set_version='0.4.6'):
+    def __init__(self,set_addr:str='longinuspypialpha.kro.kr',set_port:int=9997,set_version='0.4.6'):
         self.addr=set_addr;self.port=set_port;self.recv_datas=bytes();self.string_check_data=list;self.Cypherdata:bytes
         self.userid=str();self.pwrd=bytes();self.udata=bytes();self.head=bytes();self.rsa_keys:bytes=bytes()
         self.cipherdata=bytes();self.s=socket();self.token:bytes;self.atoken:bytes=bytes;self.rtoken:bytes
         self.Cypher_userid=bytes();self.Cypher_userpw=bytes();self.header=bytes();self.session_id=bytes()
         self.cookie=dict();self.temp_userid=bytes();self.temp_userpw=bytes();self.login_id='';self.set_version=set_version
         self.cookie_login_id='';self.cookie_master_key=''
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     def client_start(self):
-            self.addr=input('Enter the server address to connect to : ');self.port=int(input('Enter the server port to connect to : '))
+        if self.cookie_checker()==True:
+            self.cookie_loader()
+            self.request()
+        else:
             self.client_hello()
-            while True:
-                self.receive_function()
-                self.protocol_execution()
+        while True:
+            self.receive_function()
+            self.protocol_execution()
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     def client_hello(self):
         # try:
             self.rtoken=self.L.Random_Token_generator()
@@ -62,40 +64,39 @@
         self.json_decompress()
         self.error_detector()
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     def protocol_execution(self):
+        if not self.cookie_master_key=='':
+            self.master_key=self.cookie_master_key
+        if not self.cookie_login_id=='':
+            self.login_id=self.cookie_login_id
         if (self.content_type=='handshake' and self.protocol=='server_hello'):
             self.client_key_exchange()
         elif (self.content_type=='handshake' and self.protocol=='Change_Cipher_Spec'):
-            if self.cookie_checker()==True:
-                print('You are already logged in')
-                self.cookie_loader()
-                self.request()
+            self.session_id=self.atoken
+            cmd=input('\nPlease login or sign up (l/s) :')
+            if cmd=='l':
+                self.Join('login')
+            elif cmd=='s':
+                self.Join('Sign_Up')
             else:
-                self.session_id=self.atoken
-                cmd=input('\nPlease login or sign up (l/s) :')
-                if cmd=='l':
-                    self.Join('login')
-                elif cmd=='s':
-                    self.Join('Sign_Up')
-                else:
-                    sys.exit()
+                sys.exit()
         elif (self.content_type=='Sign_Up-report' and self.protocol=='Sign_up_complete'):
             print('\nSign up is complete')
             print('Please login\n')
             self.Join('login')
         elif (self.content_type=='login-report' and self.protocol=='welcome! '):
             print('\nlog-in succeed!')
             self.cookie_generator()
             self.request()
         elif (self.content_type=='server_master_secret' and self.protocol=='response'):
-            self.master_secret=self.decryption_aes(base64.b85decode(self.master_secret),self.cookie_master_key)
+            self.master_secret=self.decryption_aes(base64.b85decode(self.master_secret),self.master_key)
             print('Server :',self.master_secret.decode())
             self.request()
         elif (self.content_type=='return_error' and self.protocol=='error'):
             self.error_detector()
 
 #===================================================================================================================================#
 #===================================================================================================================================#
@@ -117,14 +118,16 @@
 
     def Cypher_user_data(self):
         self.injecter()
         self.string_check()
         self.Cypher_userid=base64.b85encode(self.encryption_aes(self.verified_userid.encode(),self.master_key)).decode()
         self.Cypher_userpw=base64.b85encode(self.encryption_aes(self.verified_userpw.encode(),self.master_key)).decode()
 
+
+
     def Join(self,set_protocol):
         self.Cypher_user_data()
         self.Create_json_object(content_type='client_master_secret',platform='client',version=self.set_version,
                                 addres=gethostbyname(gethostname()),protocol=set_protocol,
                                 session_id=self.session_id,session_id_length=len(self.session_id),
                                 userid=self.Cypher_userid,userpw=self.Cypher_userpw)
 
@@ -143,22 +146,24 @@
             pickle.dump(self.cookie,f)
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     def request(self):
         self.req=input('send : ')
-        self.Cypher_data=base64.b85encode(self.encryption_aes(self.req.encode(),self.cookie_master_key)).decode()
-        self.Create_json_object(content_type='client_master_secret',platform='client',version=self.set_version,
-                                        addres=gethostbyname(gethostname()),protocol='request',login_id=self.cookie_login_id,
-                                        master_secret=self.Cypher_data)
-        self.verified_jsobj_dump=self.hmac_cipher(self.jsobj_dump.encode(),self.cookie_master_key)
-        self.s=socket()
-        self.s.connect((self.addr,self.port))
-        self.send(self.verified_jsobj_dump)
+        if not (self.req == ' ' or self.req == '\n' or self.req == '    '):
+            self.Cypher_data=base64.b85encode(self.encryption_aes(self.req.encode(),self.master_key)).decode()
+            self.Create_json_object(content_type='client_master_secret',platform='client',version=self.set_version,
+                                            addres=gethostbyname(gethostname()),protocol='request',login_id=self.login_id,
+                                            master_secret=self.Cypher_data)
+            self.verified_jsobj_dump=self.hmac_cipher(self.jsobj_dump.encode(),self.master_key)
+            self.s=socket()
+            self.s.connect((self.addr,self.port))
+            self.send(self.verified_jsobj_dump)
+        else: print('Space characters cannot be transmitted')
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     def cookie_loader(self):
         with open('cookie','rb') as f:
             self.cookie=pickle.load(f)
@@ -171,70 +176,82 @@
 
     def Create_json_object(self,content_type:str=None,platform:str=None,version:str=None,
                                         addres:str=None,protocol:str=None,random_token:str=None,
                                         random_token_length:str=None,userid:str=None,userpw:str=None,
                                         pre_master_key:str=None,session_id:str=None,session_id_length:str=None,
                                         master_secret:str=None,login_id=None,login_id_length=None):
         self.jsobj={
-            'content-type':content_type, 
-            'platform':platform,
-            'version':version,
-            'addres':addres,
-            'body':{'protocol':protocol,
+            'request-head':{
+                    'content-type':content_type, 
+                    'platform':platform,
+                    'version':version,
+                    'addres':addres,
+                    'protocol':protocol,
                     'random_token':random_token,
                     'random_token_length':random_token_length,
                     'session-id':session_id,
                     'session-id_length':session_id_length,
                     'login-id':login_id,
-                    'login-id_length':login_id_length,
+                    'login-id_length':login_id_length
+                    },
+
+            'request-body':{
                     'userid':userid,
                     'userpw':userpw,
                     'pre_master_key':pre_master_key,
                     'master_secret':master_secret
-                        }
+                    }
          }
         self.jsobj_dump= json.dumps(self.jsobj,indent=2)
         return self.jsobj_dump
 
     def json_decompress(self):
         if b'.' not in self.recv_datas:
             self.jsobj = base64.b85decode(self.recv_datas).decode()
             self.jsobj = json.loads(self.jsobj)
         else:
-            self.recv_obj=self.recv_datas.decode().split('.')
-            self.jsobj = base64.b85decode(self.recv_obj[0].encode()).decode()
-            self.hmac_hash = base64.b85decode(self.recv_obj[1].encode())
-            if self.hmac_hash==hmac.digest(self.master_key,self.jsobj.encode(),sha256):
-                self.jsobj = json.loads(self.jsobj.decode())
-            elif self.hmac_hash==hmac.digest(self.cookie_master_key,self.jsobj.encode(),sha256):
-                self.jsobj = json.loads(self.jsobj)
+            try:
+                self.recv_obj=self.recv_datas.decode().split('.')
+                self.jsobj = base64.b85decode(self.recv_obj[0].encode()).decode()
+                self.hmac_hash = base64.b85decode(self.recv_obj[1].encode())
+                if self.hmac_hash==hmac.digest(self.master_key,self.jsobj.encode(),sha256):
+                    self.jsobj = json.loads(self.jsobj)
+                elif self.hmac_hash==hmac.digest(self.cookie_master_key,self.jsobj.encode(),sha256):
+                    self.jsobj = json.loads(self.jsobj)
+            except Exception as e:
+                print(e)
         self._assign_variables()
 
     def _assign_variables(self):
-        self.server_version=self.jsobj["version"]
-        self.token=self.jsobj['body']['random_token']
-        self.atoken=self.jsobj['body']['session-id']
-        self.login_id = self.jsobj['body']['login-id']
-        self.platform=self.jsobj["platform"]
-        self.protocol=self.jsobj['body']["protocol"]
-        self.content_type=self.jsobj["content-type"]
-        self.rsa_keys=self.jsobj['body']["public-key"]
-        self.server_error=self.jsobj['body']["server_error"]
-        self.master_secret=self.jsobj['body']['master_secret']
+        self.server_version=self.jsobj['response-head']["version"]
+        self.token=self.jsobj['response-head']['random_token']
+        self.atoken=self.jsobj['response-head']['session-id']
+        self.login_id = self.jsobj['response-head']['login-id']
+        self.platform=self.jsobj['response-head']["platform"]
+        self.protocol=self.jsobj['response-head']["protocol"]
+        self.content_type=self.jsobj['response-head']["content-type"]
+        self.rsa_keys=self.jsobj['response-body']["public-key"]
+        self.server_error=self.jsobj['response-body']["server_error"]
+        self.master_secret=self.jsobj['response-body']['master_secret']
         return {
-                'content-type':self.content_type, 
-                'platform':self.platform,
-                'body':{'protocol':self.protocol,
-                            'random_token':self.token,
-                            'session-id':self.atoken,
-                            'login-id':self.login_id,
-                            'public-key':self.rsa_keys,
-                            'master_secret':self.master_secret,
-                            'server_error':self.server_error
-                            }
+                'response-head':{
+                    'content-type':self.content_type, 
+                    'platform':self.platform,
+                    'version':self.server_version,
+                    'protocol':self.protocol,
+                    'random_token':self.token,
+                    'session-id':self.atoken,
+                    'login-id':self.login_id,
+                    },
+
+                'response-body':{
+                        'public-key':self.rsa_keys,
+                        'master_secret':self.master_secret,
+                        'server_error':self.server_error
+                        }
             }
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     def recv_head(self):
         try:
             self.header=self.s.recv(4)
@@ -329,16 +346,15 @@
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     def decryption_aes(self,set_data,master_key):
         nonce=set_data[:16]
         tag=set_data[16:32]
         ciphertext =set_data[32:-1]+set_data[len(set_data)-1:]
-        session_key = master_key
-        cipher_aes = AES.new(session_key, AES.MODE_EAX, nonce)
+        cipher_aes = AES.new(master_key, AES.MODE_EAX, nonce)
         data = cipher_aes.decrypt_and_verify(ciphertext, tag)
         self.decrypt_data=base64.b85decode(data)
         return self.decrypt_data
 
     def decryptio_rsa(self,set_prv_key:str,encrypt_data:bytes):
         private_key = RSA.import_key(set_prv_key)
         cipher_rsa = PKCS1_OAEP.new(private_key)
@@ -383,10 +399,8 @@
             else:
                 print("*",end="", flush=True)
                 self.pwrd+=self.new_char
                 self.input_num+=1
         return self.userid,self.pwrd
 
 #===================================================================================================================================#
-#===================================================================================================================================#
-
-Client().client_start()
+#===================================================================================================================================#
```

### Comparing `LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/LServer.py` & `LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/LServer.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from getpass import *
 from datetime import datetime
 from datetime import timedelta
 from asyncio import *
 from hashlib import sha256
 from argon2 import PasswordHasher
 import re,base64,requests,struct,hmac,logging,pickle,secrets
+import winreg
 from multiprocessing import Process
 
 __all__=['Server']
 
 
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
@@ -22,321 +23,360 @@
 stream_handler = logging.StreamHandler()
 stream_handler.setFormatter(formatter)
 logger.addHandler(stream_handler)
 file_handler = logging.FileHandler('server.log')
 file_handler.setFormatter(formatter)
 logger.addHandler(file_handler)
 
+class Regedit:
+    def __init__(self):
+        self.Console_key = winreg.OpenKey(winreg.HKEY_CURRENT_USER, "Console", 0, winreg.KEY_WRITE)
+        self.logger=logger
+
+    def _Set_Console_VirtualTerminalLevel(self,level=1):
+        try:
+            winreg.SetValueEx(self.Console_key, "VirtualTerminalLevel", 0, winreg.REG_DWORD, level)
+            logger.info('[ Registry value change '+'\033[32m'+'succeeded'+'\033[0m'+' ] ==> VirtualTerminalLevel ')
+        except Exception():
+            logger.info('[ Registry value change '+'\033[31m'+'failed'+'\033[0m'+'  ] ==> VirtualTerminalLevel ')
 
 class Server:
     c=''
     addr=''
     ip=''
     sessions = {}
     session_keys = {}
     login_sessions = {}
     login_session_keys = {}
     database = {}
     json_obj=''
     N=''
+    col_ip=''
     sokt=socket()
     RSA_Key:dict=Longinus().Create_RSA_key()
     prv_key:str=open(RSA_Key['private_key']).read()
     pul_key:str=open(RSA_Key['public_key']).read()
     def __init__(self,version='0.4.6',port=9997,addres='0.0.0.0'):
         self.set_port=port;self.set_addr=addres;self.cipherdata=bytes();self.decrypt_data=bytes()
         self.set_version=version
         self.logger=logger;
         self.Lock=threading.Lock()
-        if self.FileManagement()._check_session_and_database():
-            self.FileManagement().loader()
 
     def run(self):
+        self.FileManagement().loader()
+        
         Server.N=self.Network()
         self.N.bind_address(self.set_addr, self.set_port)
         Server.N.listen(0)
         self.run_service()
 
     def run_service(self):
-        while True:
-            self.N=Server.N
-            self.external_ip=Server.N.accept_connection()
-            threading.Thread(target=self.handler_connection).start()
+        self.N=Server.N
+        Server.N.accept_connection()
+        threading.Thread(target=self.handler_connection).start()
 
     def handler_connection(self):
         while True:
-            self.receive_function()
-            self.protocol_execution()
+            try:
+                self.receive_function()
+                self.protocol_execution()
+            except Exception as e:
+                self.logger.info('handler_connection')
+                self.ERROR().error_handler(str(e))
 
     def receive_function(self):
-        self.buffer_size=self.N.recv_head()
-        self.recv_data=self.N.recv(self.buffer_size)
-        self.obj=self.DATA(self.recv_data)
-        self.json_obj,self.hmac_hash=self.obj.json_decompress()
+        try:
+            self.buffer_size=self.N.recv_head()
+            self.recv_data=self.N.recv(self.buffer_size)
+            self.obj=self.DATA(self.recv_data)
+            self.json_obj,self.hmac_hash=self.obj.json_decompress()
+        except Exception as e:
+            self.logger.info('receive_function')
+            self.ERROR().error_handler(str(e))
 
     def protocol_execution(self):
-        self.SSL=self.SSLConnection('0.5.0',self.json_obj,self.external_ip)
-        self.handle=self.HANDLERS('0.5.0',self.json_obj,self.external_ip)
-        if (self.json_obj['content-type'] == 'handshake' and self.json_obj['body']['protocol'] == 'client_hello'):
-            self.SSL.server_hello()
-        elif (self.json_obj['content-type'] == 'handshake' and self.json_obj['body']['protocol'] == 'client_key_exchange'):
-            self.session_id,self.master_key=self.SSL.Create_master_secret()
-            self.SSL.ChangeCipherSpec_Finished(self.session_id)
-        elif (self.json_obj['content-type'] == 'client_master_secret' and self.json_obj['body']['protocol'] == 'Sign_Up'):
-            self.handle.Sign_Up_handler()
-        elif (self.json_obj['content-type'] == 'client_master_secret' and self.json_obj['body']['protocol'] == 'login'):
-            self.handle.login_handler()
-        elif (self.json_obj['content-type'] == 'client_master_secret' and self.json_obj['body']['protocol'] == 'request'):
-            self.handle.request_handler()
-        else: self.ERROR().error_handler('Abnormal access detected')
+        try:
+            self.SSL=self.SSLConnection('0.5.0',self.json_obj)
+            self.handle=self.HANDLERS('0.5.0',self.json_obj)
+            self.content_type=self.json_obj['request-head']['content-type']
+            self.protocol=self.json_obj['request-head']['protocol']
+            if (self.content_type == 'handshake' and self.protocol == 'client_hello'):
+                self.SSL.server_hello()
+            elif (self.content_type == 'handshake' and self.protocol == 'client_key_exchange'):
+                self.session_id,self.master_key=self.SSL.Create_master_secret()
+                self.SSL.ChangeCipherSpec_Finished(self.session_id)
+            elif (self.content_type == 'client_master_secret' and self.protocol == 'Sign_Up'):
+                self.handle.Sign_Up_handler()
+            elif (self.content_type == 'client_master_secret' and self.protocol == 'login'):
+                self.handle.login_handler()
+            elif (self.content_type == 'client_master_secret' and self.protocol == 'request'):
+                self.handle.request_handler()
+            else: self.ERROR().error_handler('Abnormal access detected')
+        except Exception as e:
+            self.logger.info('protocol_execution')
+            self.ERROR().error_handler(str(e))
+        
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     class Network:
         c=''
         addr=''
+        col_addr=''
         def __init__(self):
             self.head=bytes()
             self.recv_datas=bytes()
             self.set_version=Server().set_version
             self.logger=logger
             self.s=Server.sokt
 
         def bind_address(self,set_addr, set_port):
             self.req = requests.get("http://ipconfig.kr")
             self.req = str(re.search(r'IP Address : (\d{1,3}\.\d{1,3}\.\d{1,3}\.\d{1,3})', self.req.text)[1])
-            self.logger.info('[ Server started on '+'\033[32m'+'complete'+'\033[0m'+' : ' + self.req + ' ] ')
             self.s.bind((set_addr, set_port))
+            self.logger.info('[ Server started on '+'\033[32m'+'complete'+'\033[0m'+' ] ==> ' + self.req+':'+str(set_port))
 
         def listen(self,Volume):
             self.s.listen(Volume)
 
         def accept_connection(self):
             Server.Network.c, Server.Network.addr = self.s.accept()
-            self.ip=str(self.addr).split("'")[1]
-            self.logger.info('[ '+'\033[32m'+'Connected'+'\033[0m'+' with ]: ' + str(self.addr))
-            return self.ip
+            Server.Network.col_addr='\033[33m'+f'{self.addr}'+'\033[0m'
+            Server.ip=str(self.addr).split("'")[1]
+            Server.col_ip='('+'\033[38;5;214m'+Server.ip+'\033[0m'+')'
+            self.logger.info('[ '+'\033[32m'+'Connected'+'\033[0m'+' with ] ==> '+Server.Network.col_addr)
 
         def recv_head(self):
+
             try:
                 self.head = self.c.recv(4)
                 self.head = int(struct.unpack("I", self.head)[0])
             except OSError as e:
                 self.accept_connection()
                 self.head = self.c.recv(4)
                 self.head = int(struct.unpack("I", self.head)[0])
-            self.logger.info(f'{self.addr} [Header '+'\033[32m'+'received'+'\033[0m'+' ]: '+str(self.head))
+            self.logger.info(f'[ Header '+'\033[32m'+'received'+'\033[0m'+' ]'+Server.Network.col_addr+': '+str(self.head))
             return self.head
 
         def recv(self,buffer_size:int):
             self.head=buffer_size
             self.recv_datas = bytes()
             if self.head < 2048:
                 self.recv_datas = self.c.recv(self.head)
             else:
                 self.recv_datas = bytearray()
                 for i in range(int(self.head / 2048)):
-                    self.logger.info(f'{self.addr} ['+'\033[32m'+ 'Receiving data'+'%' +'\033[0m'+']:' +'\033[32m'+ str(2048 * i / self.head * 100)+'%' +'\033[0m')
+                    self.logger.info(f' ['+'\033[32m'+ 'Receiving data'+'%' +'\033[0m'+']'+Server.Network.col_addr+':' +'\033[32m'+ str(2048 * i / self.head * 100)+'%' +'\033[0m')
                     self.recv_datas += self.c.recv(2048)
-                self.logger.info(f'{self.addr} [Receiving data]: '+'\033[32m'+'100%'+'\033[0m')
-            self.logger.info(f'{self.addr} [Data '+'\033[32m'+'received'+'\033[0m'+' ]: '+str(len(self.recv_datas))+' bytes')
+                self.logger.info(f' [ Receiving data]: '+'\033[32m'+'100%'+'\033[0m')
+            self.logger.info(f'[ Data '+'\033[32m'+'received'+'\033[0m'+' ]'+Server.Network.col_addr+': '+str(len(self.recv_datas))+' bytes')
             return self.recv_datas
 
         def send(self, data: bytes):
             head = struct.pack("I", len(data))
             self.c.sendall(head + data)
-            self.logger.info(f'{self.addr} [Data '+'\033[32m'+'sent'+'\033[0m'+' ]: '+str(len(data))+' bytes')
+            self.logger.info(f'[ Data '+'\033[32m'+'sent'+'\033[0m'+' ]'+Server.Network.col_addr+': '+str(len(data))+' bytes')
 
         def send_and_close(self, data: bytes):
             head = struct.pack("I", len(data))
             self.c.sendall(head + data)
-            self.logger.info(f'{self.addr} [Data '+'\033[32m'+'sent'+'\033[0m'+' ]: '+str(len(data))+' bytes')
+            self.logger.info(f'[ Data '+'\033[32m'+'sent'+'\033[0m'+' ]'+Server.Network.col_addr+': '+str(len(data))+' bytes')
             self.c.close()
-            self.logger.info(f'{self.addr} [socket '+'\033[31m'+'Closed'+'\033[0m'+' ]')
+            self.logger.info(f'[ socket '+'\033[31m'+'Closed'+'\033[0m'+' ]'+Server.Network.col_addr+'')
 
 
     class DATA:
         def __init__(self,data=bytes()):
             self.data=data
             self.hmac_hash =bytes()
             self.jsobj=str()
             self.logger=logger
 
         def json_decompress(self):
             try:
                 self.compression_data = self.data
                 if b'.' not in self.compression_data:
                     self.jsobj = base64.b85decode(self.compression_data).decode()
-                    self.logger.info('[ Data decompressed '+'\033[32m'+'complete'+'\033[0m'+' ]: \n'+str(self.jsobj))
+                    self.logger.info('[ Data decompressed '+'\033[32m'+'complete'+'\033[0m'+' ] ==> \n'+str(self.jsobj))
                     self.jsobj = json.loads(self.jsobj)
                 else:
                     self.recv_obj=self.compression_data.decode().split('.')
                     self.jsobj = base64.b85decode(self.recv_obj[0].encode())
                     self.hmac_hash = base64.b85decode(self.recv_obj[1].encode())
-                    self.logger.info('[ hmac hash found '+'\033[32m'+'successful'+'\033[0m'+' ]: '+str(self.hmac_hash))
+                    self.logger.info('[ hmac hash found '+'\033[32m'+'successful'+'\033[0m'+' ]'+Server.col_ip+': '+str(self.hmac_hash))
                     self.jsobj = json.loads(self.jsobj)
                     if not self.request_credentials(self.hmac_hash,self.jsobj):
                         Server().ERROR().error_handler('Tampering, forged false request')
                         return 'Tampering, forged false request'
                 return self.jsobj,self.hmac_hash
-            except Exception:
-                print(self.compression_data)
+            except Exception as e:
+                self.logger.info(str(e))
+                self.logger.info(str(self.compression_data))
                 Server().Network().send(b'thank you! Server test was successful thanks to you, This message is a temporary message written to convey thanks to you, and it is a disclaimer that the server is operating normally.')
 
         def master_key_selector(self,json_obj):
-            self.session_id=json_obj['body']['session-id']
-            if json_obj['body']['login-id'] !=None:
-                self.master_key=Server.login_session_keys[json_obj['body']['login-id']]
+            self.session_id=json_obj['request-head']['session-id']
+            self.login_id=json_obj['request-head']['login-id']
+            if self.login_id !=None:
+                self.master_key=Server.login_session_keys[json_obj['request-head']['login-id']]
                 return self.master_key
             elif self.session_id !=None:
                 self.master_key=Server.session_keys[self.session_id]
                 return self.master_key
             else:
                 return None
 
         def request_credentials(self,hmac_hash,json_obj):
             self.master_key=self.master_key_selector(json_obj)
             if (hmac_hash==hmac.digest(self.master_key,json.dumps(self.jsobj,indent=2).encode(),sha256)):
-                logger.info(f'[ Session Credentials '+'\033[32m'+'complete'+'\033[0m'+' ]: '+str(hmac_hash))
+                logger.info(f'[ Session Credentials '+'\033[32m'+'complete'+'\033[0m'+' ]'+Server.col_ip+': '+str(hmac_hash))
                 return True
             else:
                 return False
 
         def Create_json_object(self,content_type=None,platform=None,version=None,
                                             protocol=None,random_token=None,random_token_length=None,
                                             public_key=None,public_key_length=None,server_error=None,
                                             session_id=None,session_id_length=None,master_secret=None,
                                             login_id=None,login_id_length=None):
             self.jsobj={
-                'content-type':content_type, 
-                'platform':platform,
-                'version':version,
-                'body':{'protocol':protocol,
-                            'random_token':random_token,
-                            'random_token_length':random_token_length,
-                            'session-id':session_id,
-                            'session-id_length':session_id_length,
-                            'login-id':login_id,
-                            'login-id_length':login_id_length,
-                            'public-key':public_key,
-                            'public-key_length':public_key_length,
-                            'master_secret':master_secret,
-                            'server_error':server_error
-                            }
+                'response-head':{
+                    'content-type':content_type, 
+                    'platform':platform,
+                    'version':version,
+                    'protocol':protocol,
+                    'random_token':random_token,
+                    'random_token_length':random_token_length,
+                    'session-id':session_id,
+                    'session-id_length':session_id_length,
+                    'login-id':login_id,
+                    'login-id_length':login_id_length,
+                    },
+
+                'response-body':{
+                        'public-key':public_key,
+                        'public-key_length':public_key_length,
+                        'master_secret':master_secret,
+                        'server_error':server_error
+                        }
             }
             self.jsobj_dump= json.dumps(self.jsobj,indent=2)
-            self.logger.info(f' Create_json_object : \n {str(self.jsobj_dump)}')
+            self.logger.info('[ Create json object '+'\033[32m'+'complete'+'\033[0m'+ ' ]'+Server.col_ip+f': \n {str(self.jsobj_dump)}')
             return self.jsobj_dump
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     class SSLConnection:
-        def __init__(self,set_version,json_obj,external_ip):
+        def __init__(self,set_version,json_obj):
             self.set_version=set_version
             self.SD=Server().DATA()
             Server.N=Server().Network()
             self.SC=Server().Crypto('')
             self.logger=logger
             self.json_obj=json_obj
-            self.external_ip=external_ip
 
         def server_hello(self):
             self.token=Longinus().Random_Token_generator()
             self.jsobj_dump=self.SD.Create_json_object(content_type='handshake',platform='server',version=self.set_version,
                                                 protocol='server_hello',random_token=self.token.decode(),random_token_length=len(self.token),
                                                 public_key=Server.pul_key,public_key_length=len(Server.pul_key))
             Server.N.send(base64.b85encode(self.jsobj_dump.encode()))
-            self.logger.info(f'[ | {self.external_ip} | server hello transmission '+'\033[32m'+'complete'+'\033[0m'+'] ')
+            self.logger.info(f'[ server hello transmission '+'\033[32m'+'complete'+'\033[0m'+']'+Server.col_ip)
 
         def Create_master_secret(self):
-            self.master_key=self.SC._decrypt_rsa(Server.prv_key,base64.b85decode(self.json_obj['body']['pre_master_key']))
-            self.session_id=Server().SessionManager(self.external_ip,self.json_obj).session_creation(self.master_key)
-            self.logger.info(f'[ | {self.external_ip} | Master secret creation '+'\033[32m'+'complete'+'\033[0m'+' ]: ' +str(self.session_id))
+            self.master_key=self.SC._decrypt_rsa(Server.prv_key,base64.b85decode(self.json_obj['request-body']['pre_master_key']))
+            self.session_id=Server().SessionManager(self.json_obj).session_creation(self.master_key)
+            self.logger.info(f'[ Master secret creation '+'\033[32m'+'complete'+'\033[0m'+' ]'+Server.col_ip+': ' +str(self.session_id))
             return self.session_id,self.master_key
 
         def ChangeCipherSpec_Finished(self,session_id=None):
             self.jsobj_dump=self.SD.Create_json_object(content_type='handshake',platform='server',version=self.set_version,
                                                 protocol='Change_Cipher_Spec',
                                                 session_id=session_id,session_id_length=len(session_id))
-            self.logger.info(f'[ | {self.external_ip} | Change Cipher Spec-'+'\033[32m'+'Finished'+'\033[0m'+' ] ')
+            self.logger.info(f'[ Change Cipher Spec-'+'\033[32m'+'Finished'+'\033[0m'+' ]'+Server.col_ip+' ')
             Server.N.send_and_close(base64.b85encode(self.jsobj_dump.encode()))
 
+
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     class HANDLERS:
-        def __init__(self,set_version,json_obj,external_ip):
+        def __init__(self,set_version,json_obj):
             self.json_obj=json_obj
-            self.session_id=json_obj['body']['session-id']
+            self.session_id=json_obj['request-head']['session-id']
             self.master_key=Server().DATA().master_key_selector(json_obj)
+            Server().FileManagement().loader()
             if (self.master_key!=None):
-                self.UserID,self.Userpw=self.json_obj['body']['userid'],self.json_obj['body']['userpw']
+                self.UserID,self.Userpw=self.json_obj['request-body']['userid'],self.json_obj['request-body']['userpw']
                 if not (self.Userpw==None or self.UserID==None):
                     self.UserID,self.Userpw=Server().Crypto(self.master_key).Decrypt_user_data(self.UserID,self.Userpw)
                     self.SU=Server().User(self.UserID.decode(),self.Userpw.decode())
                     self.verified_Userid,self.verified_Userpw=self.SU.verify_credentials()
             self.set_version = set_version
-            self.external_ip=external_ip
             self.logger=logger
             Server.N=Server().Network()
             self.SD=Server().DATA()
 
         def Sign_Up_handler(self):
             if self.SU._name_duplicate_check():
                 Server().ERROR().error_handler("This user already exists.")
                 return "This user already exists."
             self.verified_Userpw=self.SU.pwd_hashing(self.verified_Userpw)
-            if (Server.sessions[self.session_id]['external_ip']==self.external_ip):
-                if Server().User(self.verified_Userid,self.verified_Userpw)._permission_checker(self.external_ip):
-                    Server().DBManagement(group='__administrator__').new_database_definition(self.verified_Userid,self.verified_Userpw,self.external_ip)
-                Server().DBManagement(group='__user__').new_database_definition(self.verified_Userid,self.verified_Userpw,self.external_ip)
-                self.logger.info(f'[ | {self.external_ip} |  User info update '+'\033[32m'+'complete'+'\033[0m'+' ]: '+self.verified_Userid)
+            if (Server.sessions[self.session_id]['external_ip']==Server.ip):
+                if Server().User(self.verified_Userid,self.verified_Userpw)._permission_checker(Server.ip):
+                    Server().DBManagement(group='__administrator__').new_database_definition(self.verified_Userid,self.verified_Userpw,0)
+                Server().DBManagement(group='__user__').new_database_definition(self.verified_Userid,self.verified_Userpw,1)
+                Server().FileManagement().save_database()
+                self.logger.info(f'[ User info update '+'\033[32m'+'complete'+'\033[0m'+' ]'+Server.col_ip+': '+self.verified_Userid)
                 self.jsobj_dump=self.SD.Create_json_object(content_type='Sign_Up-report',platform='server',version=self.set_version,
                                             protocol='Sign_up_complete')
                 self.verified_jsobj_dump=Server().Crypto(self.master_key).hmac_cipher(self.jsobj_dump.encode())
                 Server.N.send_and_close(self.verified_jsobj_dump)
 
         def login_handler(self):                 
             for DB_id,DB_val in Server().database.items():
                 if DB_val['user_id']==self.verified_Userid:
                     #try:
                         if PasswordHasher().verify(DB_val['user_pw'],self.verified_Userpw):
-                            self.SM=Server().SessionManager(self.external_ip,self.json_obj)
+                            self.SM=Server().SessionManager(self.json_obj)
                             self.login_id=self.SM.login_session_creation(DB_id)
                             self.SM.discard_session(self.session_id)
-                            Server().FileManagement().saver()
+                            Server().FileManagement().save_session()
                             self.jsobj_dump=self.SD.Create_json_object(content_type='login-report',platform='server',version=self.set_version,
                                                         protocol='welcome! ',
                                                         login_id=self.login_id,login_id_length=len(self.login_id))
                             self.verified_jsobj_dump=Server().Crypto(self.master_key).hmac_cipher(self.jsobj_dump.encode())
+                            self.logger.info(f'[ Login '+'\033[32m'+'successful'+'\033[0m'+' ]'+Server.col_ip+': '+str(self.login_id))
                             Server.N.send_and_close(self.verified_jsobj_dump)
-                            self.logger.info(f'[ | {self.external_ip} | Login '+'\033[32m'+'successful'+'\033[0m'+' ]: '+str(self.login_id))
                     #except Exception: Server().ERROR().error_handler('The password does not match the supplied hash')
                 else: Server().ERROR().error_handler('The user could not be found. Please proceed to sign up')
 
         def request_handler(self):
-            self.reqdata=Server().Crypto(self.master_key)._decrypt_aes(base64.b85decode(self.json_obj['body']['master_secret']))
-            self.logger.info(f'[ | {self.external_ip} | \033[32m'+'get request'+'\033[0m'+' ]:' f' {self.reqdata.decode()}')
+            self.reqdata=Server().Crypto(self.master_key)._decrypt_aes(base64.b85decode(self.json_obj['request-body']['master_secret']))
+            self.logger.info('[ \033[32m'+'get request'+'\033[0m'+' ]'+Server.col_ip+':' f' {self.reqdata.decode()}')
             self.jsobj_dump=self.SD.Create_json_object(content_type='server_master_secret',platform='server',version=self.set_version,
                                         protocol='response',master_secret=base64.b85encode(Server().Crypto(self.master_key)._encrypt_aes(self.reqdata)).decode())
             self.verified_jsobj_dump=Server().Crypto(self.master_key).hmac_cipher(self.jsobj_dump.encode())
             Server.N.send_and_close(self.verified_jsobj_dump)
 
     class ERROR:
         def error_handler(self,msg,set_version=''):
-            self.logger=logger
-            Server.N=Server().Network()
-            self.SD=Server().DATA()
-            self.logger.info('[ '+'\033[31m'+'unexpected error'+'\033[0m'+ ' ]: ' +msg)
-            self.jsobj_dump=self.SD.Create_json_object(content_type='return_error',platform='server',version=set_version,
-                                                protocol='error',
-                                                server_error=' [ unexpected error ]: '+msg)
-            Server.N.send_and_close(self.jsobj_dump.encode())
+            try:
+                self.logger=logger
+                Server.N=Server().Network()
+                self.SD=Server().DATA()
+                self.logger.info('[ '+'\033[31m'+'unexpected error'+'\033[0m'+ ' ]: ' +msg)
+                self.jsobj_dump=self.SD.Create_json_object(content_type='return_error',platform='server',version=set_version,
+                                                    protocol='error',
+                                                    server_error=' [ unexpected error ]: '+msg)
+                Server.N.send_and_close(self.jsobj_dump.encode())
+            except Exception as e:
+                self.logger.info('[ unexpected error ]:' ,e)
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     class DBManagement:
         def __init__(self,group='__user__'):
             self.logger=logger
@@ -348,77 +388,111 @@
             self.permission_lv=permission_lv
             self.database_creation()
 
         def database_creation(self):
             token=Longinus().Random_Token_generator(8)
             new_database = {'user_id': self.verified_UserID, 'user_pw': self.verified_Userpw, 'permission_lv': self.permission_lv, 'group': self.group}
             Server.database[token.decode()]=new_database
-            self.logger.info(f'[ New user database creation '+'\033[32m'+'complete'+'\033[0m'+' ]: '+str(new_database))
+            self.logger.info(f'[ New user database creation '+'\033[32m'+'complete'+'\033[0m'+' ] ==> '+str(new_database))
             return new_database
 
     class SessionManager:
-        def __init__(self,external_ip,json_obj):
+        def __init__(self,json_obj):
             self.logger=logger
             self.json_obj=json_obj
-            self.session_id=json_obj['body']['session-id']
-            self.internal_ip=json_obj['addres']
-            self.external_ip=external_ip
+            self.session_id=json_obj['request-head']['session-id']
+            self.internal_ip=json_obj['request-head']['addres']
 
         def session_creation(self, master_key):
             session_id, session_info = self.session_generator()
             Server.sessions[session_id]=session_info
             Server.session_keys[session_id]=master_key
-            self.logger.info(f'[ | {self.external_ip} | Session assignment '+'\033[32m'+'complete'+'\033[0m'+' ]: '+str(session_id))
+            self.logger.info(f'[ Session assignment '+'\033[32m'+'complete'+'\033[0m'+' ]'+Server.col_ip+': '+str(session_id))
             return session_id
 
         def login_session_creation(self, data):
             login_id, session_info = self.session_generator()
             new_login_session = {login_id: {'data':data, 'session_info':session_info}}
             Server.login_sessions.update(new_login_session)
             Server.login_session_keys[login_id]=Server.session_keys[self.session_id]
-            self.logger.info(f'[ | {self.external_ip} | login Session assignment '+'\033[32m'+'complete'+'\033[0m'+' ]: '+str(login_id))
+            self.logger.info(f'[ login Session assignment '+'\033[32m'+'complete'+'\033[0m'+' ]'+Server.col_ip+': '+str(login_id))
             return login_id
 
         def session_generator(self,length=32,session_validity=7):
             token = base64.b85encode(secrets.token_bytes(length)).decode()
             now = datetime.now()
             now_after = now + timedelta(days=session_validity)
-            token_data = {'external_ip': self.external_ip, 'internal_ip': self.internal_ip, 'timestamp': str(now), 'validity': str(now_after)}
+            token_data = {'external_ip': Server.ip, 'internal_ip': self.internal_ip, 'timestamp': str(now), 'validity': str(now_after)}
             return token, token_data
 
         def discard_session(self, session_id):
-            self.logger.info(f'[ Session '+'\033[31m'+'discarded'+'\033[0m'+']: '+str(session_id))
+            self.logger.info(f'[ Session '+'\033[31m'+'discarded'+'\033[0m'+'] '+Server.col_ip+': '+str(session_id))
             if Server.sessions:
                 del Server.sessions[session_id]
                 del Server.session_keys[session_id]
 
         def validate_session(self):
             pass
 
     class FileManagement:
-        def saver(self):
-            self.save_session_and_database()
 
         def loader(self):
-            Server.login_sessions,Server.login_session_keys,Server.database = self.load_session_and_database()
+            if (Server.login_sessions=={} and Server.login_session_keys=={} and Server.database =={}):
+                if (self._check_database() and self._check_session()):
+                    self.load_session_and_database()
+                    return 'load_session_and_database'
+            elif (Server.login_sessions=={} and Server.login_session_keys=={}):
+                if self._check_session():
+                    Server.login_sessions,Server.login_session_keys=self.load_sessione()
+                    return 'load_sessione'
+            elif Server.database=={}:
+                if self._check_database():
+                    Server.database=self.load_database()
+                    return 'load_database'
 
-        def save_session_and_database(self):
-            with open('session_and_database', 'wb') as f:
-                pickle.dump({'login_sessions':Server.login_sessions, 'login_session_keys': Server.login_session_keys, 'database': Server.database}, f)
-            logger.info('[ Database and session data saved '+'\033[32m'+'completed'+'\033[0m'+' ]')
 
         def load_session_and_database(self):
-            with open('session_and_database', 'rb') as f:
+            self.load_session()
+            self.load_database()
+
+        def load_session_and_database(self):
+            Server.login_sessions,Server.login_session_keys=self.load_sessione()
+            Server.database = self.load_database()
+
+        def save_session(self):
+            with open('Server.sessions', 'wb') as f:
+                pickle.dump({'login_sessions':Server.login_sessions, 'login_session_keys': Server.login_session_keys}, f)
+            logger.info('[ Session data saved '+'\033[32m'+'completed'+'\033[0m'+' ]')
+
+        def load_sessione(self):
+            with open('Server.sessions', 'rb') as f:
                 session_setup = pickle.load(f)
-            return session_setup['login_sessions'], session_setup['login_session_keys'], session_setup['database']
+            logger.info('[ sessione data load '+'\033[32m'+'completed'+'\033[0m'+' ]')
+            return session_setup['login_sessions'], session_setup['login_session_keys']
+
+        def save_database(self):
+            with open('Server.DB', 'wb') as f:
+                pickle.dump(Server.database, f)
+            logger.info('[ Database data saved '+'\033[32m'+'completed'+'\033[0m'+' ]')
+
+        def load_database(self):
+            with open('Server.DB', 'rb') as f:
+                database_setup = pickle.load(f)
+            logger.info('[ Database data load '+'\033[32m'+'completed'+'\033[0m'+' ]')
+            return database_setup
 
-        def _check_session_and_database(self):
+        def _check_database(self):
             self.dir=os.listdir(os.getcwd())
-            if ('session_and_database' in self.dir):
-                self.loader()
+            if ('Server.DB' in self.dir):
+                return True
+            else: return False
+
+        def _check_session(self):
+            self.dir=os.listdir(os.getcwd())
+            if ('Server.sessions' in self.dir):
                 return True
             else: return False
 
 #===================================================================================================================================#
 #===================================================================================================================================#
 
     class Crypto:
@@ -501,10 +575,8 @@
         def pwd_hashing(self,verified_Userpw):
             while True:
                 temp=self.ph.hash(verified_Userpw)
                 if (self.ph.verify(temp,verified_Userpw) and self.ph.check_needs_rehash(temp)!=True):
                     break
             return temp
 #===================================================================================================================================#
-#===================================================================================================================================#
-
-Server().run()
+#===================================================================================================================================#
```

### Comparing `LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/LonginusP.py` & `LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/LonginusP.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from Cryptodome.Cipher import AES
 from Cryptodome.PublicKey import RSA
 from Cryptodome.Cipher import PKCS1_OAEP
 import os
 from socket import *
 from getpass import *
-from datetime import datetime
 from asyncio import *
 from hashlib import blake2b
-from argon2 import PasswordHasher
 import secrets,base64
 
 
 __all__=['Longinus']
 
 class Longinus:
     def __init__(self):
```

### Comparing `LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha/Lshell.py` & `LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha/Lshell.py`

 * *Files identical despite different names*

### Comparing `LonginusPyPiAlpha-0.4.8/LonginusPyPiAlpha.egg-info/PKG-INFO` & `LonginusPyPiAlpha-0.4.9/LonginusPyPiAlpha.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LonginusPyPiAlpha
-Version: 0.4.8
+Version: 0.4.9
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/LonginusPYPI
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/LonginusPYPI
 Project-URL: Bug Tracker, https://github.com/projectlonginus/LonginusPYPI/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `LonginusPyPiAlpha-0.4.8/PKG-INFO` & `LonginusPyPiAlpha-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LonginusPyPiAlpha
-Version: 0.4.8
+Version: 0.4.9
 Summary: A small example package
 Home-page: https://github.com/projectlonginus/LonginusPYPI
 Author: Example Author
 Author-email: Longinus <team.longinus.project@gmail.com>
 Project-URL: Homepage, https://github.com/projectlonginus/LonginusPYPI
 Project-URL: Bug Tracker, https://github.com/projectlonginus/LonginusPYPI/issues
 Classifier: Programming Language :: Python :: 3
```

