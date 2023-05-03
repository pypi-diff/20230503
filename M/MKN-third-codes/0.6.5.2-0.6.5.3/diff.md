# Comparing `tmp/MKN_third_codes-0.6.5.2.tar.gz` & `tmp/MKN_third_codes-0.6.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.5.2.tar", last modified: Wed May  3 09:48:06 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.5.3.tar", last modified: Wed May  3 12:32:06 2023, max compression
```

## Comparing `MKN_third_codes-0.6.5.2.tar` & `MKN_third_codes-0.6.5.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:06.820076 MKN_third_codes-0.6.5.2/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.5.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.5.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:06.806112 MKN_third_codes-0.6.5.2/MKN_third_codes/
--rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.5.2/MKN_third_codes/__init__.py
--rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.5.2/MKN_third_codes/mkn_globals.py
--rw-rw-rw-   0        0        0     9636 2023-05-03 09:36:24.000000 MKN_third_codes-0.6.5.2/MKN_third_codes/mkn_utils.py
--rw-rw-rw-   0        0        0    27856 2023-05-03 09:41:53.000000 MKN_third_codes-0.6.5.2/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:48:06.819079 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     7700 2023-05-03 09:48:06.000000 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-03 09:48:06.000000 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:48:06.000000 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-03 09:48:06.000000 MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7700 2023-05-03 09:48:06.820076 MKN_third_codes-0.6.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     4287 2023-05-03 09:37:41.000000 MKN_third_codes-0.6.5.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 09:48:06.821074 MKN_third_codes-0.6.5.2/setup.cfg
--rw-rw-rw-   0        0        0      489 2023-05-03 09:47:56.000000 MKN_third_codes-0.6.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 12:32:06.268447 MKN_third_codes-0.6.5.3/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.5.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.5.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-03 12:32:06.263460 MKN_third_codes-0.6.5.3/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     7700 2023-05-03 12:32:06.000000 MKN_third_codes-0.6.5.3/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-03 12:32:06.000000 MKN_third_codes-0.6.5.3/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 12:32:06.000000 MKN_third_codes-0.6.5.3/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 12:32:06.000000 MKN_third_codes-0.6.5.3/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7700 2023-05-03 12:32:06.267450 MKN_third_codes-0.6.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4287 2023-05-03 09:37:41.000000 MKN_third_codes-0.6.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 12:32:06.266452 MKN_third_codes-0.6.5.3/mfcn/
+-rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.5.3/mfcn/__init__.py
+-rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.5.3/mfcn/mkn_globals.py
+-rw-rw-rw-   0        0        0     9636 2023-05-03 09:36:24.000000 MKN_third_codes-0.6.5.3/mfcn/mkn_utils.py
+-rw-rw-rw-   0        0        0    27959 2023-05-03 12:31:55.000000 MKN_third_codes-0.6.5.3/mfcn/solutions.py
+-rw-rw-rw-   0        0        0       42 2023-05-03 12:32:06.268447 MKN_third_codes-0.6.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-05-03 12:31:22.000000 MKN_third_codes-0.6.5.3/setup.py
```

### Comparing `MKN_third_codes-0.6.5.2/LICENSE.txt` & `MKN_third_codes-0.6.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.2/MKN_third_codes/mkn_globals.py` & `MKN_third_codes-0.6.5.3/mfcn/mkn_globals.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.2/MKN_third_codes/mkn_utils.py` & `MKN_third_codes-0.6.5.3/mfcn/mkn_utils.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.2/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.5.3/mfcn/solutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 import math
 import re
-from mkn_utils import *
-from mkn_globals import regular_int, regular_float
+# from mfcn import mkn_utils as utl
+# from mfcn import mkn_globals as glb
+import mkn_utils as utl
+import mkn_globals as glb
 
 def buckets_n_balls_solution(boxes):
     """
     Находит ответ для вопроса 'какова вероятность достать Белый шар из n+1 урны' для задачи о n урнах с белыми и чёрными шарами, когда из каждой урны берут Ki шаров, перекладывают их в n+1 урну.
     Для решения используется теорема гипотез
 
     Args:
         boxes (list): массив объектов класса Box
 
     Returns:
         list: [list: массив объектов Hypotes, float: итоговая пероятность искомого события]
     """
-    myHyp = Hypoteses(boxes)
+    myHyp = utl.Hypoteses(boxes)
 
     hypot_prob = myHyp.get_from_boxes()
 
     prob_final = 0
     ready_hipoteses = []
     for i in range(0, len(hypot_prob)):
-        ready_hipoteses.append(Hypotes([hypot_prob[i][1], hypot_prob[i][2]], hypot_prob[i][0], i+1))
+        ready_hipoteses.append(utl.Hypotes([hypot_prob[i][1], hypot_prob[i][2]], hypot_prob[i][0], i+1))
         prob_final += hypot_prob[i][0]*hypot_prob[i][1]/(hypot_prob[i][1]+hypot_prob[i][2])
     
     return(ready_hipoteses, prob_final)
 
 def buckets_n_balls_terminal():
     """
     Решение задачи о n урнах с белыми и чёрными шарами, когда из каждой урны берут Ki шаров, перекладывают их в n+1 урну.
     """
-    boxes = [Box() for _ in range(int(input("Введите количество урн: ")))]
+    boxes = [utl.Box() for _ in range(int(input("Введите количество урн: ")))]
 
     for i in range(len(boxes)):
         boxes[i].balls[0] = int(input(f"Кол-во Б шаров в {i+1} урне: "))
         print("\033[F                                                                       ", end="\r")
         boxes[i].balls[1] = int(input(f"Кол-во Ч шаров в {i+1} урне: "))
         print("\033[F                                                                       ", end="\r")
     print("Шары заданы.")
@@ -71,15 +73,15 @@
     """
     if text == None:
         return ["""Введите количество урн (число n)
 В следующих n строках введите количество белых и чёрных шаров (пара чисел через пробел) в i-ой урне
 В последних n строках введите количество шаров, забираемых из i-ой урны"""]
     else:
         try:
-            request = [int(parameter) for parameter in re.findall(regular_int, text)]
+            request = [int(parameter) for parameter in re.findall(glb.regular_int, text)]
 
             answer = []
 
             box_num = request[0]
 
             boxes = [Box(request[1+2*i], request[2+2*i], request[1+box_num*2+i]) for i in range(box_num)]
 
@@ -124,17 +126,17 @@
     Returns:
         EttaTable: таблица ячеек таблицы
     """
     #следующей строчкой находим количество всех перестановок
     allPerestan = math.factorial(humans)
 
     #определяем таблицу
-    myTable = EttaTable(cells=[])
+    myTable = utl.EttaTable(cells=[])
     for j in range(0, humans+1):
-        myTable.cells.append(EttaTableCell(j, 0, allPerestan))
+        myTable.cells.append(utl.EttaTableCell(j, 0, allPerestan))
 
     #Функция, проходящаяся по всем перестановкам, и записивыающая их в таблицу
     def goThrough(n, layer, used):
         if layer == humans:#раздали все предметы
             myTable.cells[n].good_th += 1
             return
         for ticket in range(0, humans):#раздаем следующий предмет
@@ -165,17 +167,17 @@
     Returns:
         EttaTable: таблица ячеек таблицы
     """
     #следующей строчкой находим количество всех перестановок
     allPerestan = math.factorial(humans)
 
     #определяем таблицу
-    myTable = EttaTable(cells=[])
+    myTable = utl.EttaTable(cells=[])
     for j in range(0, humans+1):
-        myTable.cells.append(EttaTableCell(j, 0, allPerestan))
+        myTable.cells.append(utl.EttaTableCell(j, 0, allPerestan))
 
     myTable.cells[0].good_th = int(round(math.factorial(humans)/math.e))
     myTable.cells[1].good_th = myTable.cells[0].good_th + (-1)**(humans+1)
     myTable.cells[-1].good_th = 1
     myTable.cells[-2].good_th = 0
 
     for id in range(2, humans-1):
@@ -275,15 +277,15 @@
     sM = Meetiner(float(input("Введите начальный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
     float(input("Введите конечный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
     float(input("Введите, сколько времени будет ждать участник второй: ")))
 
     print("Обозначим за A - участники встретятся")
     print(f"P(A) = {geometric_meeting_solution(ln, fM, sM)}")
 
-def geometric_meeting_solution(length:float = 0, firstAim:Meetiner=None, secondAim:Meetiner=None):
+def geometric_meeting_solution(length:float = 0, firstAim:utl.Meetiner=None, secondAim:utl.Meetiner=None):
     """
     Решение задачи о встрече двух участников
 
     Args:
         length (float): длина участка меры, на которой могут встретиться участники
         firstAim (Meetiner): первый участник
         secondAim (Meetiner): второй участник
@@ -330,15 +332,15 @@
 
                 return answer
             else:
                 return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-def find_math_prediction_solution(table: EttaTable = None, degree: float = 1, ignore_errors: bool = False):
+def find_math_prediction_solution(table: utl.EttaTable = None, degree: float = 1, ignore_errors: bool = False):
     """
     Нахождение МО по таблице значений случайных величин
 
     Args:
         table (EttaTable): таблица значений случайных величин
     
     Returns:
@@ -402,15 +404,15 @@
             else:
                 answer.append(result)
 
             return answer
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-def find_dispersion_solution(table: EttaTable):
+def find_dispersion_solution(table: utl.EttaTable):
     """
     Функция, считающая дисперсию для таблицы СВ
 
     Args:
         table (EttaTable): таблица СВ
 
     Returns:
@@ -472,15 +474,15 @@
             else:
                 answer.append(result)
 
             return answer
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-def table_analysis_solution(table: EttaTable):
+def table_analysis_solution(table: utl.EttaTable):
     """
     Находит Мx и Dx для таблицы значений СВ
 
     Args:
         table (EttaTable): таблица значений СВ
 
     Returns:
```

### Comparing `MKN_third_codes-0.6.5.2/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.5.3/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.6.5.2
+Version: 0.6.5.3
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `MKN_third_codes-0.6.5.2/PKG-INFO` & `MKN_third_codes-0.6.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.6.5.2
+Version: 0.6.5.3
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `MKN_third_codes-0.6.5.2/README.md` & `MKN_third_codes-0.6.5.3/README.md`

 * *Files identical despite different names*

