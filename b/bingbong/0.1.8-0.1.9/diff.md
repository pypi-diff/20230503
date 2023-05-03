# Comparing `tmp/bingbong-0.1.8-py3-none-any.whl.zip` & `tmp/bingbong-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 11979 bytes, number of entries: 16
--rw-rw-r--  2.0 unx       53 b- defN 23-Apr-20 20:04 pingpong/__init__.py
--rw-rw-r--  2.0 unx     1681 b- defN 23-Apr-20 19:34 pingpong/alpaca.py
--rw-rw-r--  2.0 unx     1287 b- defN 23-Apr-20 19:34 pingpong/dolly.py
--rw-rw-r--  2.0 unx     1399 b- defN 23-Apr-20 19:47 pingpong/gradio.py
--rw-rw-r--  2.0 unx     1212 b- defN 23-Apr-20 19:34 pingpong/pingpong.py
--rw-rw-r--  2.0 unx     1496 b- defN 23-Apr-20 19:59 pingpong/stablelm.py
--rw-rw-r--  2.0 unx      173 b- defN 23-Apr-20 19:34 pingpong/context/__init__.py
--rw-rw-r--  2.0 unx      589 b- defN 23-Apr-20 19:34 pingpong/context/auto_summary_strategy.py
--rw-rw-r--  2.0 unx      789 b- defN 23-Apr-20 19:34 pingpong/context/last_window_strategy.py
--rw-rw-r--  2.0 unx      840 b- defN 23-Apr-20 19:34 pingpong/context/search_window_strategy.py
--rw-rw-r--  2.0 unx      119 b- defN 23-Apr-20 19:34 pingpong/context/strategy.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3346 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1303 b- defN 23-Apr-20 20:04 bingbong-0.1.8.dist-info/RECORD
-16 files, 25745 bytes uncompressed, 9829 bytes compressed:  61.8%
+Zip file size: 11745 bytes, number of entries: 16
+-rw-r--r--  2.0 unx       53 b- defN 23-Apr-20 15:06 pingpong/__init__.py
+-rw-r--r--  2.0 unx      959 b- defN 23-Apr-20 15:04 pingpong/alpaca.py
+-rw-r--r--  2.0 unx     1287 b- defN 23-Apr-20 14:58 pingpong/dolly.py
+-rw-r--r--  2.0 unx     1399 b- defN 23-Apr-20 14:58 pingpong/gradio.py
+-rw-r--r--  2.0 unx     1212 b- defN 23-Apr-20 14:58 pingpong/pingpong.py
+-rw-r--r--  2.0 unx     1496 b- defN 23-Apr-20 14:58 pingpong/stablelm.py
+-rw-r--r--  2.0 unx      173 b- defN 23-Apr-20 14:58 pingpong/context/__init__.py
+-rw-r--r--  2.0 unx      589 b- defN 23-Apr-20 14:58 pingpong/context/auto_summary_strategy.py
+-rw-r--r--  2.0 unx      789 b- defN 23-Apr-20 14:58 pingpong/context/last_window_strategy.py
+-rw-r--r--  2.0 unx      840 b- defN 23-Apr-20 14:58 pingpong/context/search_window_strategy.py
+-rw-r--r--  2.0 unx      119 b- defN 23-Apr-20 14:58 pingpong/context/strategy.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Apr-20 15:07 bingbong-0.1.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3346 b- defN 23-Apr-20 15:07 bingbong-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 15:07 bingbong-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Apr-20 15:07 bingbong-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1302 b- defN 23-Apr-20 15:07 bingbong-0.1.9.dist-info/RECORD
+16 files, 25022 bytes uncompressed, 9595 bytes compressed:  61.7%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.1.8.dist-info/LICENSE
+Filename: bingbong-0.1.9.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.1.8.dist-info/METADATA
+Filename: bingbong-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.1.8.dist-info/WHEEL
+Filename: bingbong-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.1.8.dist-info/top_level.txt
+Filename: bingbong-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.1.8.dist-info/RECORD
+Filename: bingbong-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 from .pingpong import PingPong
```

## pingpong/alpaca.py

```diff
@@ -3,54 +3,32 @@
 
 class AlpacaPromptFmt(PromptFmt):
   @classmethod
   def ctx(cls, context):
     if context is None or context == "":
       return ""
     else:
-      return f"""### Input:
-{context}
+      return f"""{context}
 
 """
 
   @classmethod
   def prompt(cls, pingpong, truncate_size):
     return f"""### Instruction:
 {pingpong.ping[:truncate_size]}
 
 ### Response:
 {"" if pingpong.pong is None else pingpong.pong[:truncate_size]}"""
 
 class AlpacaChatPPManager(PPManager):
-  def add_ping(self, ping, fmt: PromptFmt=AlpacaPromptFmt):
-    allowed = super().add_ping(ping, fmt)
-
-    if allowed:
-      if self.ctx == "":
-        prompts = "Below is an instruction that describes a task. Write a response that appropriately completes the request. You are LLaMA which is a large language model created by Facebook."
-      else:
-        prompts = "Below is an instruction that describes a task, paired with an input that provides further context. Write a response that appropriately completes the request. You are LLaMA which is a large language model created by Facebook."
-
-      prompts += f"""
-      
-### Instruction:
-{ping}
-{fmt.ctx(self.ctx)}
-### Response:
-"""
-      return prompts
-
-    return None
-
-
   def build_prompts(self, from_idx: int=0, to_idx: int=-1, fmt: PromptFmt=AlpacaPromptFmt, truncate_size: int=None):
     if to_idx == -1 or to_idx >= len(self.pingpongs):
       to_idx = len(self.pingpongs)
 
-    results = ""
+    results = fmt.ctx(self.ctx)
 
     for idx, pingpong in enumerate(self.pingpongs[from_idx:to_idx]):
       results += fmt.prompt(pingpong, truncate_size=truncate_size)
 
       if from_idx+idx != to_idx-1:
         results += """
```

## Comparing `bingbong-0.1.8.dist-info/LICENSE` & `bingbong-0.1.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.1.8.dist-info/METADATA` & `bingbong-0.1.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.1.8
+Version: 0.1.9
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `bingbong-0.1.8.dist-info/RECORD` & `bingbong-0.1.9.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-pingpong/__init__.py,sha256=7HuUZUYPXV1B8IQ_7l4c1F_V-NdBC7QKOqwKUNZIOLI,53
-pingpong/alpaca.py,sha256=NLRBCMfyXmgL9S5SmVRUPPDsEjsw9Kv0iFYPTrPZVgs,1681
+pingpong/__init__.py,sha256=J6600qowLbmcGP-yuYuvRLFZ2uIMHPCgYDRBDrv9avw,53
+pingpong/alpaca.py,sha256=BIDnzZUyXoHeFsYON6EHvyBOZUltcFsuFvZor3QOhWk,959
 pingpong/dolly.py,sha256=vMbHiwgeewzRAsruuMVnQc2w3KEKhWJUdOmaBbyazQo,1287
 pingpong/gradio.py,sha256=K474EiQbNmyvPhfnx-0yTBFrU2X61sVy5v7JcQivQHI,1399
 pingpong/pingpong.py,sha256=XfCYe-OdNkyrKOhAEaL4Q-HhZx829_i-ohDlY2GF7gM,1212
 pingpong/stablelm.py,sha256=UlFLilnxUuJpYwcA_aANTVkQERMSK44ULx1kl-K-L6k,1496
 pingpong/context/__init__.py,sha256=ksYP7nq8inYK7SHDwpd7Hs_h87gPKdP9Ac6E5w0X6zM,173
 pingpong/context/auto_summary_strategy.py,sha256=s2lrlGKzLFNBGdLMAkaC6d2VY8aJSdgtrwa_Rvmt3Fc,589
 pingpong/context/last_window_strategy.py,sha256=JN7pFDD2C8nGMUx-H3aHNQrXCT0E0S-FlBunOrQGX-w,789
 pingpong/context/search_window_strategy.py,sha256=OPd2xxiI9FrzU4w2R5luaDEKiNEj4KYr_EF53Qi6l_Q,840
 pingpong/context/strategy.py,sha256=xGoy7T92gYubrwekz0Kz2Vxv10njgXG44K48bC9BqAU,119
-bingbong-0.1.8.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-bingbong-0.1.8.dist-info/METADATA,sha256=uZWiwivUq2GMwe4MgvfrjmraWdCNDg-cm2TNKvksCz8,3346
-bingbong-0.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-bingbong-0.1.8.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
-bingbong-0.1.8.dist-info/RECORD,,
+bingbong-0.1.9.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+bingbong-0.1.9.dist-info/METADATA,sha256=SRPCRLPhsW5atxV6C70o6UQRyHfxCAdvh1qsMf4w4Cg,3346
+bingbong-0.1.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bingbong-0.1.9.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
+bingbong-0.1.9.dist-info/RECORD,,
```

