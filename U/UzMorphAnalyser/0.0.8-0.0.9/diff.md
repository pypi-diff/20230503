# Comparing `tmp/UzMorphAnalyser-0.0.8-py3-none-any.whl.zip` & `tmp/UzMorphAnalyser-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 27573 bytes, number of entries: 13
--rw-rw-rw-  2.0 fat    33589 b- defN 22-Jul-06 05:27 UzMorphAnalyser/UzMorphAnalyser.py
+Zip file size: 28973 bytes, number of entries: 13
+-rw-rw-rw-  2.0 fat    35925 b- defN 22-Aug-03 06:42 UzMorphAnalyser/UzMorphAnalyser.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Jul-06 05:15 UzMorphAnalyser/__init__.py
--rw-rw-rw-  2.0 fat    70334 b- defN 22-Jul-06 05:24 UzMorphAnalyser/affixes.csv
--rw-rw-rw-  2.0 fat     2403 b- defN 22-Jul-06 05:15 UzMorphAnalyser/exception_stems.csv
+-rw-rw-rw-  2.0 fat    75087 b- defN 22-Aug-03 06:39 UzMorphAnalyser/affixes.csv
+-rw-rw-rw-  2.0 fat     2467 b- defN 22-Jul-29 09:37 UzMorphAnalyser/exception_stems.csv
 -rw-rw-rw-  2.0 fat      316 b- defN 22-Jul-06 05:15 UzMorphAnalyser/lemma_map.csv
--rw-rw-rw-  2.0 fat      814 b- defN 22-Jul-06 05:15 UzMorphAnalyser/non_affixed_stems.csv
--rw-rw-rw-  2.0 fat      196 b- defN 22-Jul-06 05:15 UzMorphAnalyser/number_stems.csv
--rw-rw-rw-  2.0 fat       61 b- defN 22-Jul-06 05:15 UzMorphAnalyser/small_stems.csv
--rw-rw-rw-  2.0 fat     1091 b- defN 22-Jul-06 05:30 UzMorphAnalyser-0.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     4645 b- defN 22-Jul-06 05:30 UzMorphAnalyser-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 22-Jul-06 05:30 UzMorphAnalyser-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       16 b- defN 22-Jul-06 05:30 UzMorphAnalyser-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1128 b- defN 22-Jul-06 05:30 UzMorphAnalyser-0.0.8.dist-info/RECORD
-13 files, 114685 bytes uncompressed, 25661 bytes compressed:  77.6%
+-rw-rw-rw-  2.0 fat     1410 b- defN 22-Jul-28 10:58 UzMorphAnalyser/non_affixed_stems.csv
+-rw-rw-rw-  2.0 fat      196 b- defN 22-Jul-23 06:28 UzMorphAnalyser/number_stems.csv
+-rw-rw-rw-  2.0 fat       73 b- defN 22-Jul-29 12:33 UzMorphAnalyser/small_stems.csv
+-rw-rw-rw-  2.0 fat     1091 b- defN 22-Aug-03 06:44 UzMorphAnalyser-0.0.9.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4645 b- defN 22-Aug-03 06:44 UzMorphAnalyser-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 22-Aug-03 06:44 UzMorphAnalyser-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       16 b- defN 22-Aug-03 06:44 UzMorphAnalyser-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1129 b- defN 22-Aug-03 06:44 UzMorphAnalyser-0.0.9.dist-info/RECORD
+13 files, 122447 bytes uncompressed, 27061 bytes compressed:  77.9%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: UzMorphAnalyser/number_stems.csv
 Comment: 
 
 Filename: UzMorphAnalyser/small_stems.csv
 Comment: 
 
-Filename: UzMorphAnalyser-0.0.8.dist-info/LICENSE
+Filename: UzMorphAnalyser-0.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: UzMorphAnalyser-0.0.8.dist-info/METADATA
+Filename: UzMorphAnalyser-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: UzMorphAnalyser-0.0.8.dist-info/WHEEL
+Filename: UzMorphAnalyser-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: UzMorphAnalyser-0.0.8.dist-info/top_level.txt
+Filename: UzMorphAnalyser-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: UzMorphAnalyser-0.0.8.dist-info/RECORD
+Filename: UzMorphAnalyser-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## UzMorphAnalyser/UzMorphAnalyser.py

```diff
@@ -12,14 +12,15 @@
     __exception_stems = []  # list of exception stems from exception_stems.csv file
     __lemma_map = []  # list of lemma convertion mapping from lemma_map.csv file
     # __ambiguity_stems = []  # list of ambiguity stems from ambiguity_stems.csv file | oxiri affix bn tugaydigan asos suzlar
 
     __vovel = ['a', 'u', 'e', 'i', 'o',"o'"]
     __consonant_hard = ['b', 'd', 'g', 'j', 'l', 'm', 'n', 'r', 'v', 'y', 'z', "g'", 'ng']  # jarangli undosh
     __consonant_soft = ['f', 'h', 'k', 'p', 'q', 's', 't', 'x', 'sh', 'ch']  # jarangsiz undosh
+    __consonant = ['b', 'd', 'g', 'j', 'l', 'm', 'n', 'r', 'v', 'y', 'z', 'f', 'k', 'p', 'q', 's', 't', 'x', 's', 'c', 'h' ]  # all undosh
 
     # affixes.csv da barcha allomorphlarni qulda generate qilib yozib quyamiz, dastur yordamida qilmaymiz, chalkash joylari kup
     # bu generate funksiya faqat qavs ichida bitta harf (katta/kichik) turganda va bitta katta harf mavjud bulganda tugri keladi.
     def __GeneratedAllomorph(self, affix):  # return a list that contain all allomorphs of the current affix
         GenAff = []
         # if allomorph has omitted letter # qavsli faqat affix boshida keladi
         parentesis = False  # is exist parentesis
@@ -95,74 +96,89 @@
                     GenAff.append(affix_v2[:uc_v2] + "k" + affix_v2[uc_v2 + 1:])
                     GenAff.append(affix_v2[:uc_v2] + "q" + affix_v2[uc_v2 + 1:])
                 if affix_v2[uc_v2] == "S":  # S:s,y
                     GenAff.append(affix_v2[:uc_v2] + "s" + affix_v2[uc_v2 + 1:])
                     GenAff.append(affix_v2[:uc_v2] + "y" + affix_v2[uc_v2 + 1:])
             else:
                 GenAff.append(affix_v2)  # qavsli lekin Katta harfsiz varianti
-
         return GenAff
         # end of Generate Allmorph
 
     def __init__(self):
         self.__read_data()
 
     def __read_data(self):
         # url = 'http://u92156l3.beget.tech/affix/export.php', it couldn't be get from url
         dirname = os.path.dirname(__file__) + "/"
 
-        with open(os.path.join(dirname + "affixes.csv"), "r") as f:
+        with open(os.path.join(dirname + "affixes.csv"), "r", encoding='utf-8') as f:
             reader = csv.DictReader(f)
             self.__affixes = list(reader)
 
-        with open(os.path.join(dirname + "small_stems.csv"), "r") as f:
+        with open(os.path.join(dirname + "small_stems.csv"), "r", encoding='utf-8') as f:
             reader = csv.reader(f)
             # self.__small_stems = list(reader)
             self.__small_stems = [item for sublist in list(reader) for item in sublist]
-        with open(os.path.join(dirname + "non_affixed_stems.csv"), "r") as f:
+        with open(os.path.join(dirname + "non_affixed_stems.csv"), "r", encoding='utf-8') as f:
             reader = csv.DictReader(f)
             self.__non_affixed_stems = list(reader)
             # reader = csv.reader(f)
             # self.__non_affixed_stems = [item for sublist in list(reader) for item in sublist]
 
-        with open(os.path.join(dirname + "number_stems.csv"), "r") as f:
+        with open(os.path.join(dirname + "number_stems.csv"), "r", encoding='utf-8') as f:
             reader = csv.reader(f)
             # self.__small_stems = list(reader)
             self.__number_stems = [item for sublist in list(reader) for item in sublist]
         # with open("ambiguity_stems.csv", "r") as f:
         #    reader = csv.DictReader(f)
         #    self.__ambiguity_stems = list(reader)
-        with open(os.path.join(dirname + "exception_stems.csv"), "r") as f:
+        with open(os.path.join(dirname + "exception_stems.csv"), "r", encoding='utf-8') as f:
             reader = csv.DictReader(f)
             self.__exception_stems = list(reader)
-        with open(os.path.join(dirname + "lemma_map.csv"), "r") as f:
+        with open(os.path.join(dirname + "lemma_map.csv"), "r", encoding='utf-8') as f:
             reader = csv.DictReader(f)
             self.__lemma_map = list(reader)
 
         # generate all allomorphs for each affix and allomorph list to affixes list
         for item in self.__affixes:
             item['allomorphs'] = self.__GeneratedAllomorph(item['affix'])
 
         # enf of read_data
 
     def __check_affixation_rules(self, affix: str, word: str, i: int):
         # True = affix qirqilsin, aks holda qirqilmasin
         # 0-rule Suz harflarini joylashuviga kura suz oxirida 2ta unli yoki 2 ta bir xil harfli undosh bilan asos tugamaydi (ikki->ikk), agar bunday hol bulayotgan bulsa, undan bu qushimchani qirqishni otkaz qilamiz. 2 xil undosh bn tugashi mumkin: tort+ib
-        buf = word[i-2:i]  # suzni asosidagi oxirgi 2 ta harfni olish
-        if len(buf) == 2 and i < 4:
-            if (buf[0] in self.__vovel and buf[1] in self.__vovel) or (buf[0] not in self.__vovel and buf[0] == buf[1]):  # asosdagi oxirgi 2 harfni 2lasi xam unli yoki 2ta bir xil harfli undosh bulsa (ikk)
-                return False
+        buf = word[:i]  # suzni asosidagi oxirgi 2 ta harfni olish
+        buf = buf.replace("'", "")
+        buf = buf.replace("‘", "")
+        if len(buf) >= 3:
+            buf1 = buf[-3]  # asosni oxiridan 3-xarfi
+            buf = buf[-2:]  # suzni asosidagi oxirgi 2 ta harfni olish
+
+            if len(buf) == 2 and i < 6:
+                if (buf[0] in self.__vovel and buf[1] in self.__vovel) or (buf[0] in self.__consonant and buf[0] == buf[1]) \
+                        or (buf[0] in self.__consonant and buf[1] in self.__consonant and buf1 not in self.__vovel):  #(buf[0] in self.__consonant and buf[1] in self.__consonant and buf not in ["ch","sh", "tq", "sm"]) or  # asosdagi oxirgi 2 harfni 2lasi xam unli yoki 2ta bir xil harfli undosh bulsa (ikk)
+                    return False
+
+            if (buf[0] in self.__consonant and buf[1] in self.__consonant and buf1 not in self.__vovel):
+                # asosdagi unli va undoshla mutanosibligini tekshirish
+                vovelcnt = sum(c in self.__vovel for c in word[:i])
+                double_char = word[:i].count("ch") + word[:i].count("sh") + word[:i].count("ng") + word[:i].count("sm") + word[:i].count("tq") + word[:i].count("'") + word[:i].count("’") + word[:i].count("‘")
+                if len(word[:i]) - vovelcnt - double_char > 1:
+                    print(len(word[:i]) - vovelcnt - double_char)
+                    if vovelcnt * 2 < len(word[:i]) - vovelcnt - double_char and not (vovelcnt == 1 and len(word[:i]) - vovelcnt - double_char == 3):
+                        return False
 
         # 1.1-rule
         if affix.startswith("(i)m"):  # (i)m egalik qushimchasida, m dan oldin kupincha a harfi keladi, agar bunday bulmasa, bu m qushimchasini qirqamay utirib yuboramiz
             if word[i] == "m" and word[i-1] not in ['a','i']:  # agar oldigi harfi a ga teng bulmasa bunda m ni qirqmasin
                 return False  # don't chop, break it
         # 1.2-rule
         if affix.startswith("(s)i"):  # (s)i quchimchasidan oldin a,i harfi keladi. bunday bulmasa, bu m qushimchasini qirqamay utirib yuboramiz
-            if word[i] == "s" and word[i-1] not in ['a','i']:  # agar oldigi harfi a ga teng bulmasa bunda m ni qirqmasin
+            if word[i] == "s" and word[i-1] not in ['a','i','o','y','u']:  # agar oldigi harfi a ga teng bulmasa bunda m ni qirqmasin
                 return False  # don't chop, break it
         # 1.3-rule
         if affix.startswith("(i)b"):  # (i)b  qushimchasi a,i harflaridan keyin qushiladi faqat. aytib,kuylab
             if word[i] == "b" and word[i-1] not in ["i", "a"]:  # bulsa bunda qushimchani qirqmasin
                 return False  # don't chop, break it
         # 1.4-rule
         if affix.startswith("(i)sh"):  # (i)sh  qushimchasi a,i harflaridan keyin qushiladi odatda. uxlash,uchish
@@ -171,15 +187,15 @@
 
         # 2-rule
         if affix.startswith('G'):  # Guncha, Gani,Gan,Gancha,Gani {G=g,k,q}  qushimchasidan oldin k,q harfi kelishi kerak, agar bunday bulmasa bu qushimchani qirqamay utirib yuboramiz
             if (word[i] == "k" and word[i-1] not in ['k']) or (word[i] == "q" and word[i-1] not in ['q']):  # bulsa qushimchani qirqmasin
                 return False  # don't chop, break it
         # 3-rule
         if affix.startswith("ir"):  # ir  qushimchasi t,ch,sh harflaridan keyin qushiladi faqat. botir,ichir,shishir
-            if word[i-1] != "t" and word[i-2:i] not in ["ch", "sh"]:  # bulsa bunda qushimchani qirqmasin
+            if word[i-1] not in ["t", "p"] and word[i-2:i] not in ["ch", "sh"]:  # bulsa bunda qushimchani qirqmasin
                 return False  # don't chop, break it
         # 4-rule
         if affix.startswith("iz"):  # iz  qushimchasi q,m harflaridan keyin qushiladi faqat. oqiz, tomiz
             if word[i-1] not in ["q", "m"]:  # bulsa bunda qushimchani qirqmasin
                 return False  # don't chop, break it
         # 5-rule
         if affix.__contains__("dagi") and not affix.__contains__("dagina"):  # qirqilayotgan affixda -dagi qushimchasi bulsa, tekshiramiz, shu asos bosh harf bn yozilganmi, chunki dagi faqat atoqli otlarga qushilsa lugaviy qushimcha buladi, boshqa xollarda suz yasovchi buladi
@@ -188,14 +204,22 @@
         # 6-rule
         if word[i:].startswith("i") and word[i-3:i] == "dag":  # -dagi qushimchasidan -i qushimchasini qirqauotgan bulsa buni qirqtirmaymiz, chunki dagini tuliq uizni qirqadi yoki tugri kelmasi qirqmaydi
             return False  # don't chop, break it
         # 7-rule
         if affix.startswith("(i)l"):  # -(i)l:  bo'lgan suzida -(i)lgan qushimchasini qirqib yuboryapti, -(i)l qushimchasidan -l quchimchasi faqat unli bn tugagan asosga qushiladi, bu asoslar kamida 4 harfdan iborat buladi katta ehtimol bn: ajra+lgan
             if word[i] == "l" and i < 4:  # bulsa bunda qushimchani qirqmasin
                 return False  # don't chop, break it
+        # 8-rule
+        if affix.startswith("(i)la"):  # (i)la
+            if word[i] == "l" and word[i-1] not in ["a", "i"]:  # bulsa bunda qushimchani qirqmasin
+                return False  # don't chop, break it
+        # 9-rule
+        if affix.startswith("mlar"):  # xurmatlash manosidagi
+            if word[i-1] not in ["a"]:  # bulsa bunda qushimchani qirqmasin
+                return False  # don't chop, break it
         # 4-rule
         if affix.startswith("iz"):  # iz  qushimchasi q,m harflaridan keyin qushiladi faqat. oqiz, tomiz
             if word[i-1] not in ["q", "m"]:  # bulsa bunda qushimchani qirqmasin
                 return False  # don't chop, break it
 
         # 8-rule  -(s)i kitobi dagi -i ni qirqanda to'g'ri dagi -i ni qirqadi, -i qirqilganda undan oldingi harflarni 2tasi unli+undosh bulsa qirqilsin, aksholda otkaz
         #if affix.startswith("(s)i") and word[i] == "i" and i > 2 and word[i-2:i] not in ['ng','tr','vq','st']: # asosni oxirgi 2 harfi -ng ga teng bulmasa jang+i, metr+i,zavq+i,artist+i da qirqavarsin
@@ -204,27 +228,30 @@
 
         return True  # it is ok, go on chopping
 
     def __correction_stem(self, self1, result):
         for item in result:  # result is list
             # I-type: xarf ortishi (avzoy+im->avzo, bun+da->bu)
             # 1-rule [avzoy+im->avzo, (xarf ortishi)] mavqe,azvo,obro',mavzu
-            if item['affixed'].startswith("i") and item['stem'][-2:] in ["ey", "oy", "uy", "'y"]:
+            if item['affixed'].startswith("i") and item['stem'][-2:] in ["ey", "oy", "'y"] and len(item['stem']) > 3:
                 item['stem'] = item['stem'][:-1]
             # 2-rule [bun+da->bu, (xarf ortishi)] unda,unday,bunda,bunday,shunda,shunday, shunga,bunga
             if (item['affixed'].startswith("d") or item['affixed'].startswith("g")) and item['stem'] in ["un", "bun", "shun"]:
                 item['stem'] = item['stem'][:-1] # remove last letter which is n from stem
 
             # II-type: Xarf uzgarishi
             # 1-rule [qiyinchilig+i ->qiyinchilik (xarf uzgarishi)]
             if item['affixed'].startswith("i") and item["stem"][-3:] == "lig": # [-3:] = oxirgi 3 harf = "lig" bulsa
                 item['stem'] = item['stem'][:-1] + "k"
             # 2-rule [bilag+i ->bilak (xarf uzgarishi)]
             if item['affixed'].startswith("i") and item["stem"][-2:] == "ag": #  [-2:] = oxirgi 2 harfi = "ag" bulsa
                 item['stem'] = item['stem'][:-1] + "k"
+            # 3-rule [o'rtog'+i ->o'rtoq (xarf uzgarishi)]
+            if item['affixed'].startswith("i") and item["stem"][-3:] == "og‘": #  [-3:] = oxirgi 3 harfi = "og`" bulsa
+                item['stem'] = item['stem'][:-2] + "q"
 
         return result
         #end of correction_stem
 
     #  umumiy holda yani stem, lemma, analyse metodlaridan turib __processing metodidan foydalanamiz
 
     def __processing(self, word: str, pos: str = None, is_lemmatize: bool = False, multi_item: bool = False):
@@ -365,15 +392,15 @@
                 na_stem['affixed'] = ''
                 return [na_stem]
 
         ##if word in [na_stem['stem'] for na_stem in self.__non_affixed_stems]: # in self.__non_affixed_stems
         ##    return word
 
         # 2-step sat faqat ko'rsat bulganda qirqiladi (so'zni boshi ko'rsat ga teng bulganda)
-        if word[:7].casefold() == "ko'rsat":
+        if word[:7].casefold() == "ko‘rsat":
             result_items = []
             for i_affixes in affixes:  # agar kursat topilsa, undan qolgan qushimchani affixes dan qidirib topib, undagi malumotlarni olamiz
                 if word[7:] in i_affixes["allomorphs"]:
                     i_affixes['stem'], i_affixes['affixed'] = word[:4], word[4:]  # bu dictga kursat felini nisbati haqidagi informatsiyani qushib yuborsa xam buladi
                     result_items.append(i_affixes)
                     if not multi_item:
                         return result_items
@@ -422,14 +449,15 @@
         return list_item[0]['stem']    # dict['stem] == dict.get('stem')
 
     def lemmatize(self, word: str, pos: str = None):
         # print(self.__lemma_map)
         list_item = self.__processing(self.__clean_word(word), pos, is_lemmatize=True)
         # print(list_item)
         return list_item[0]['stem']  # .get('stem')
+        # return {'lemma': list_item[0]['stem'], 'pos': list_item[0]['pos']}  # .['stem'] ['pos']
 
     def analyze(self, word: str, pos: str = None):
         # morpheme, bound morpheme [maktablar, maktab=morphem, lar=bound morphem]
         list_item = self.__processing(self.__clean_word(word), pos, is_lemmatize=True, multi_item=True)
         # print(list_item)
         res_list_item = []
         for item in list_item:
@@ -513,45 +541,45 @@
         tokens = []
         return tokens
 
     def sent_tokenize(self, text):
         tokens = []
         return tokens
 
-# import time
-# start_time = time.time()
-# obj = UzMorphAnalyser()
-'''
-sent = "olmasi taqgandim olma taqdimmi kurs kursi gacha namuna ko'plab ular bular sizlar kuchli shanba yuztagacha yuztaga kursi eksport eksportidan masjid masjidi tuman tumani tumanimizni taqdim taqdimi barmoqi barmoq muzqaymoq"
-with open(os.path.join(os.path.dirname(__file__) + "/" + "test.txt"), 'r', encoding='utf8') as file:
-    sent1 = file.read().rstrip()
-sent1 = sent1.replace('	', ' ')
-sent1 = sent1.replace('!', ' ')
-sent1 = sent1.replace('?', ' ')
-sent1 = sent1.replace('“', ' ')
-sent1 = sent1.replace('”', ' ')
-sent1 = sent1.replace(',', ' ')
-sent1 = sent1.replace('.', ' ')
-sent1 = sent1.replace('\n', ' ')
-sent1 = sent1.replace('(', ' ')
-sent1 = sent1.replace(')', ' ')
-
-for token in sent1.split(" "):
-    token = token.lower()
-    if token == "":
-        continue
-    print(token + '\t' + obj.stem(token) + '\t' + obj.lemmatize(token) + '\t' + str(obj.analyze(token)))
-print("--- %s seconds ---" % (time.time() - start_time))
-'''
+import time
+start_time = time.time()
+obj = UzMorphAnalyser()
+
+# sent = "olmasi taqgandim olma taqdimmi kurs kursi gacha namuna ko'plab ular bular sizlar kuchli shanba yuztagacha yuztaga kursi eksport eksportidan masjid masjidi tuman tumani tumanimizni taqdim taqdimi barmoqi barmoq muzqaymoq"
+# with open(os.path.join(os.path.dirname(__file__) + "/" + "test.txt"), 'r', encoding='utf8') as file:
+#     sent1 = file.read().rstrip()
+# sent1 = sent1.replace('	', ' ')
+# sent1 = sent1.replace('!', ' ')
+# sent1 = sent1.replace('?', ' ')
+# sent1 = sent1.replace('“', ' ')
+# sent1 = sent1.replace('”', ' ')
+# sent1 = sent1.replace(',', ' ')
+# sent1 = sent1.replace('.', ' ')
+# sent1 = sent1.replace('\n', ' ')
+# sent1 = sent1.replace('(', ' ')
+# sent1 = sent1.replace(')', ' ')
+#
+# for token in sent1.split(" "):
+#     token = token.lower()
+#     if token == "":
+#         continue
+#     print(token + '\t' + obj.stem(token) + '\t' + obj.lemmatize(token) + '\t' + str(obj.analyze(token)))
+# print("--- %s seconds ---" % (time.time() - start_time))
+
 # with open(os.path.join(os.path.dirname(__file__) + "/" + "test_token.txt"), 'r', encoding='utf8') as file:
 #     for token in file:
 #         token = token.rstrip()
-#         print(token + '\t' + obj.stem(token) + '\t' + obj.lemmatize(token) + '\t' + str(obj.analyze(token)))
+#         # print(token + '\t' + obj.stem(token) + '\t' + obj.lemmatize(token) + '\t' + str(obj.analyze(token)))
 # print("--- %s seconds ---" % (time.time() - start_time))
-#
+
 # while (True):
 #     s = input()#.lower()
 #     print(s + '\t' + obj.stem(s) + '\t' + obj.lemmatize(s) + '\t' + str(obj.analyze(s)))
 
 # print(analyzer.lemmatize('benim'))
 # [('benim', ['ben'])]
 
@@ -576,7 +604,8 @@
 '''
 
 #(i)t kirit, (i)l ko'ril, (i)n ko'rin, Y{bora,kuylay}, (a)r{borar,kuylar} qo'shimchalarini uchiramiz bazadan, chunki bir xarfli qushimchalar suzlarni oxirini kup qirqib yuboradi
 
 # test file statistics:
 # source:daryo.uz, category:4, documents for each category: 10
 # 5,288 unique words of 11,952 total (44.24%):
+
```

## UzMorphAnalyser/affixes.csv

 * *Ordering differences only*

```diff
@@ -1 +1 @@
-id,root,affix,info,pos,tense,person,possession,cases,verb_voice,verb_func,impulsion,copula,singular,plural,question,negative,lexical_affixes,syntactical_affixes
+id,root,affix,info,pos,tense,person,possession,cases,verb_voice,verb_func,impulsion,copula,singular,plural,question,negative,lexical_affixes,syntactical_affixes
```

## UzMorphAnalyser/exception_stems.csv

```diff
@@ -75,8 +75,12 @@
 hujum,NOUN,{opa(m) m quhsimchani qirqadi}
 malham,NOUN,{m ni qirqadi}
 shart,NOUN,{t ni qirqadi}
 balans,MOUN,{si ni qirqadi}
 aholi,NOUN,{i ni qirqadi}
 ravish,NOUN,{}
 tashqari,ADV,{}
-dollar,NOUN,{}
+dollar,NOUN,{}
+olim,NOUN,{}
+shaxsan,NOUN,{}
+qancha,NOUN,{}
+kelgusi,NOUN,{}
```

## UzMorphAnalyser/non_affixed_stems.csv

```diff
@@ -1,110 +1,124 @@
 stem,pos
 va,CNJ
 lekin,CNJ
 biroq,CNJ
-juda
-ushbu,
-asta
-sekin
-yana
-balki
-nafaqat
-mana
-ana
-g'oyat
-bag'oyat
-nihoyat
-nihoyatda
-tufayli
-holda
-uchun
-va
-hamda
-ammo
-lekin
-biroq
-yoki
-yohud
-yo
-dam
-goh
-ba'zan
-xoh
-gohida
-ya'ni
-chunki
-negaki
-sababki
-zero
-zeroki
-toki
-agar
-agarda
-gar
-basharti
-mabodo
-garchi
-garchand
-lek
-vale
-sababli
-tufayli
-yoinki
-minan
-go'yo
-nahotki
-axir
-g'irt
-hech
-sira
-aslo
-zinhor
-xuddi
-naq
-go'yo
-go'yoki
-faqat
-xolos
-atigi
-hatto
-hattoki
-ham
-nahot
-bilan
-uchun
-singari
-kabi
-yanglig'
-sari
-sayin
-beri
-haqida
-haqda
-qadar
-uzra
-tufayli
-to
-doir
-oid
-bo'yicha
-kabi
-qarshi
-o'zga
-boshqa
-bo'lak
-sababli
-orqali
-ilgari
-burun
-tomon
-ko'ra
-yarasha
-chog'li
-binoan
-asosan
-buyon
-shuningdek
-tomonlama
-deyarli
-turli
-o'shanda
+juda,PRT
+ushbu,PRON
+asta,ADV
+sekin,ADV
+yana,ADV
+balki,MOD
+nafaqat,PRT
+mana,PRON
+ana,PRON
+g‘oyat,PRT
+bag‘oyat,PRT
+nihoyat,PRT
+nihoyatda,PRT
+tufayli,PRT
+holda,PRT
+uchun,ADP
+hamda,CNJ
+ammo,CNJ
+lekin,CNJ
+yoki,CNJ
+yohud,CNJ
+yo,CNJ
+dam,CNJ
+goh,CNJ
+ba’zan,CNJ
+xoh,CNJ
+gohida,CNJ
+ya’ni,CNJ
+chunki,CNJ
+negaki,CNJ
+sababki,CNJ
+zero,CNJ
+zeroki,CNJ
+toki,CNJ
+agar,CNJ
+agarda,CNJ
+gar,CNJ
+basharti,CNJ
+mabodo,CNJ
+garchi,CNJ
+garchand,CNJ
+lek,CNJ
+vale,CNJ
+sababli,ADP
+tufayli,ADP
+yoinki,CNJ
+minan,ADP
+nahotki,PRT
+axir,PRT
+g‘irt,PRT
+hech,PRT
+sira,PRT
+aslo,PRT
+zinhor,PRT
+xuddi,PRT
+naq,PRT
+go‘yo,PRT
+go‘yoki,PRT
+faqat,PRT
+xolos,PRT
+atigi,PRT
+hatto,PRT
+hattoki,PRT
+ham,PRT
+nahot,PRT
+bilan,ADP
+uchun,ADP
+singari,ADP
+kabi,ADP
+yanglig‘,ADP
+sari,ADP
+sayin,ADP
+beri,ADP
+haqida,ADP
+haqda,ADP
+qadar,ADP
+uzra,ADP
+tufayli,ADP
+to,ADP
+doir,ADP
+oid,ADP
+bo‘yicha,ADP
+kabi,ADP
+qarshi,ADP
+bo‘lak,ADP
+sababli,ADP
+orqali,ADP
+ilgari,ADP
+burun,ADP
+tomon,ADP
+ko‘ra,ADP
+yarasha,ADP
+chog‘li,ADP
+binoan,ADP
+buyon,ADP
+shuningdek,MOD
+deyarli,ADP
+o‘shanda,PRON
+asosan,MOD
+o‘zga,ADJ
+boshqa,ADJ
+ko‘plab,
+endi,
+ya’ni,
+xususan,
+qo‘shimcha,
+pastki,
+borada,
+umuman,
+tayanib,
+haligacha,
+hali,
+dastlabki,
+dastlab,
+borasida,
+ba’zi,
+targ‘ib,
+kungi,
+alohida,
+o‘laroq,
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## UzMorphAnalyser/small_stems.csv

```diff
@@ -9,8 +9,11 @@
 ur
 un
 ot
 de
 oq
 uq
 en
-oy
+oy
+ye
+uz
+er
```

## Comparing `UzMorphAnalyser-0.0.8.dist-info/LICENSE` & `UzMorphAnalyser-0.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `UzMorphAnalyser-0.0.8.dist-info/METADATA` & `UzMorphAnalyser-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: UzMorphAnalyser
-Version: 0.0.8
+Version: 0.0.9
 Summary: UzMorphAnalyser | Uzbek Morphological Analyser on Python
 Home-page: https://github.com/UlugbekSalaev/UzMorphAnalyser
 Author: Ulugbek Salaev
 Author-email: ulugbek0302@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/UlugbekSalaev/UzMorphAnalyser/issues
 Keywords: mophology,uzbek-language,stemmer,lemmatize,morphological analysis
```
