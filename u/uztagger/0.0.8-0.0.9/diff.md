# Comparing `tmp/uztagger-0.0.8-py3-none-any.whl.zip` & `tmp/uztagger-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 351008 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat     5554 b- defN 23-May-01 12:10 uztagger/__init__.py
--rw-rw-rw-  2.0 fat  1066063 b- defN 22-Aug-15 06:00 uztagger/lexicon.csv
+Zip file size: 351170 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat     5869 b- defN 23-May-03 09:13 uztagger/__init__.py
+-rw-rw-rw-  2.0 fat  1066063 b- defN 23-May-03 09:15 uztagger/lexicon.csv
 -rw-rw-rw-  2.0 fat     1161 b- defN 22-Aug-15 06:00 uztagger/non_affixed_word.csv
 -rw-rw-rw-  2.0 fat    85846 b- defN 22-Aug-16 08:01 uztagger/web-interface-ui.png
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4029 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      720 b- defN 23-May-01 12:28 uztagger-0.0.8.dist-info/RECORD
-9 files, 1164565 bytes uncompressed, 349778 bytes compressed:  70.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-03 09:19 uztagger-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4029 b- defN 23-May-03 09:19 uztagger-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-03 09:19 uztagger-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-03 09:19 uztagger-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      720 b- defN 23-May-03 09:19 uztagger-0.0.9.dist-info/RECORD
+9 files, 1164880 bytes uncompressed, 349940 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: uztagger/non_affixed_word.csv
 Comment: 
 
 Filename: uztagger/web-interface-ui.png
 Comment: 
 
-Filename: uztagger-0.0.8.dist-info/LICENSE
+Filename: uztagger-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: uztagger-0.0.8.dist-info/METADATA
+Filename: uztagger-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: uztagger-0.0.8.dist-info/WHEEL
+Filename: uztagger-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: uztagger-0.0.8.dist-info/top_level.txt
+Filename: uztagger-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: uztagger-0.0.8.dist-info/RECORD
+Filename: uztagger-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## uztagger/__init__.py

```diff
@@ -29,41 +29,43 @@
         with open(os.path.join(dirname + "lexicon.csv"), "r", encoding='utf-8') as f:
             df_lexicon = pd.read_csv(f)
 
         df_lexicon = df_lexicon.sort_values(by="stem", key=lambda x: x.str.len())  # sorting to stands a small one at top, after that get first item as a result
 
         uzmorph = UzMorphAnalyser()
 
-        punctuation = {'.', ',', '!', '?', ':'}  # punctuation list, set pos tag as "PUNC"
-        symbol = {'$', '*', '#', '@', '%'}  # symbol list, set pos tag as "SYM"
+        punctuation = {'.', ',', '!', '?', ':', ';', '–', '–', '—', '(', ')', '[', ']', '{', '}', '<', '>', '“', '”'}  # punctuation list, set pos tag as "PUNC"
+        symbol = {'$', '*', '#', '@', '%', '&', '⟨', '⟩', '/', '~', '\'', '^', '|'}  # symbol list, set pos tag as "SYM" (Symbol)
 
         for token in tokens:
             # 3. check from ready list
             # 3.1 check from punctuation list
             if token in punctuation:
                 tagged_text.append((token, self.POS.PUNC))  # punctuation
                 continue
-            # 3.1 check from symbol list
+            # 3.2 check from symbol list
             if token in symbol:
                 tagged_text.append((token, self.POS.SYM))  # symbol
                 continue
-            # 4. non_affixed_words check
-            df1 = df_non_aff.loc[df_non_aff['stem'] == token.lower()]
+
+            token_l = token.lower()
+            # 3.3 check from non_affixed_words
+            df1 = df_non_aff.loc[df_non_aff['stem'] == token_l]
             if not df1.empty:
                 tagged_text.append((token, df1["pos"].iloc[0]))  # "non_aff"
                 continue
-            # 5. lookup from lexicon.csv, in reverse order by remove character
-            df1 = df_lexicon[df_lexicon['stem'].str.startswith(token.lower())]
+            # 3.4. lookup from lexicon.csv, in reverse order by remove character
+            df1 = df_lexicon[df_lexicon['stem'].str.startswith(token_l)] #token bn boshlanadigan stemni topadi va shu row ni oladi
             if not df1.empty:
-                tagged_text.append((token, df1["pos"].iloc[0]))  # "lexicon"
+                tagged_text.append((token, df1["pos"].iloc[0]))  # found in "lexicon" file
                 continue
-            # 6. UzMorph check
+            # 3.5. UzMorphAnalyser checking process
             res = uzmorph.analyze(token)
             if res[0]["pos"] != None:
-                tagged_text.append((token, res[0]["pos"]))  # "uzmorph"
+                tagged_text.append((token, res[0]["pos"]))  # tagged from "uzmorph" UzMorphAnalyser
                 continue
             # 7. still can not find, make any decision
             tagged_text.append((token, self.POS.NOUN))  # other
 
         return tagged_text
 
     class POS:
@@ -82,15 +84,15 @@
         AUX = "AUX"    # Auxiliary verb
         PPN = "PPN"    # Proper noun
         PUNC = "PUNC"  # Punctuation
         SYM = "SYM"    # Symbol
 
 
     def help(self):
-        return "help of usage of metoding"
+        return "<list of tuple> pos_tag(<text>) \n  pos_tag_list()"
 
     def pos_tag_list(self):
         return [
             ('NOUN', 'Noun', 'Ot'),
             ('ADJ', 'Adjective', 'Sifat'),
             ('NUM', 'Number', 'Son'),
             ('PRON', 'Pronoun', 'Olmosh'),
```

## Comparing `uztagger-0.0.8.dist-info/LICENSE` & `uztagger-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `uztagger-0.0.8.dist-info/METADATA` & `uztagger-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uztagger
-Version: 0.0.8
+Version: 0.0.9
 Summary: uztagger | Uzbek Morphological Part of Speech (POS) Tagging on Python
 Home-page: https://github.com/UlugbekSalaev/uztagger
 Author: Ulugbek Salaev
 Author-email: ulugbek0302@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/uztagger/issues
 Keywords: mophology,uzbek-language,pos tagging,morphological tagging
```

## Comparing `uztagger-0.0.8.dist-info/RECORD` & `uztagger-0.0.9.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-uztagger/__init__.py,sha256=iVj5najfigCoRWvE1DMytiLwjAQzv0yLLyh4kQ3uwBc,5554
+uztagger/__init__.py,sha256=9uAhB325-xJsOh6nBvUB-qQGH2DpsspCTu7DW2S0dRg,5869
 uztagger/lexicon.csv,sha256=MkiosgciuDdZeh0MPdTW-Di1FMA8WTRNBrAwQEljj7Y,1066063
 uztagger/non_affixed_word.csv,sha256=iECecb6vWMajPm_L2gxpDJ2_PcnQuXBLNoOjfEFSQls,1161
 uztagger/web-interface-ui.png,sha256=IxLn0GkjC_79JfupXUGGUVc5l2G2-TlDxW4eH9naoA0,85846
-uztagger-0.0.8.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-uztagger-0.0.8.dist-info/METADATA,sha256=15ELScVJ-aoNgupFxtLcGwYNZQLWNFMu7XN3QiII12k,4029
-uztagger-0.0.8.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-uztagger-0.0.8.dist-info/top_level.txt,sha256=uaDS85LyY_8T_MoTYuGFvsBD0UwQ90m7jhWirfybf1M,9
-uztagger-0.0.8.dist-info/RECORD,,
+uztagger-0.0.9.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+uztagger-0.0.9.dist-info/METADATA,sha256=vKhav0_fSBuxFwYZC2Oxq5rkIEV15GZg-UVF-KbBifI,4029
+uztagger-0.0.9.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+uztagger-0.0.9.dist-info/top_level.txt,sha256=uaDS85LyY_8T_MoTYuGFvsBD0UwQ90m7jhWirfybf1M,9
+uztagger-0.0.9.dist-info/RECORD,,
```

