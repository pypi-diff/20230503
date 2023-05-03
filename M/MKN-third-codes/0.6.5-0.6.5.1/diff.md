# Comparing `tmp/MKN_third_codes-0.6.5.tar.gz` & `tmp/MKN_third_codes-0.6.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.5.tar", last modified: Wed May  3 09:38:13 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.5.1.tar", last modified: Wed May  3 09:42:16 2023, max compression
```

## Comparing `MKN_third_codes-0.6.5.tar` & `MKN_third_codes-0.6.5.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:38:13.569330 MKN_third_codes-0.6.5/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.5/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.5/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-03 09:38:13.560354 MKN_third_codes-0.6.5/MKN_third_codes/
--rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.5/MKN_third_codes/mkn_globals.py
--rw-rw-rw-   0        0        0     9636 2023-05-03 09:36:24.000000 MKN_third_codes-0.6.5/MKN_third_codes/mkn_utils.py
--rw-rw-rw-   0        0        0    27980 2023-05-03 09:35:54.000000 MKN_third_codes-0.6.5/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:38:13.567336 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     7698 2023-05-03 09:38:13.000000 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-03 09:38:13.000000 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:38:13.000000 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 09:38:13.000000 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7698 2023-05-03 09:38:13.568333 MKN_third_codes-0.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     4287 2023-05-03 09:37:41.000000 MKN_third_codes-0.6.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 09:38:13.569330 MKN_third_codes-0.6.5/setup.cfg
--rw-rw-rw-   0        0        0      503 2023-05-03 09:38:08.000000 MKN_third_codes-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:42:16.820560 MKN_third_codes-0.6.5.1/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.5.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-03 09:42:16.810586 MKN_third_codes-0.6.5.1/MKN_third_codes/
+-rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.5.1/MKN_third_codes/mkn_globals.py
+-rw-rw-rw-   0        0        0     9636 2023-05-03 09:36:24.000000 MKN_third_codes-0.6.5.1/MKN_third_codes/mkn_utils.py
+-rw-rw-rw-   0        0        0    27856 2023-05-03 09:41:53.000000 MKN_third_codes-0.6.5.1/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:42:16.819562 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     7700 2023-05-03 09:42:16.000000 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-03 09:42:16.000000 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:42:16.000000 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 09:42:16.000000 MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7700 2023-05-03 09:42:16.820560 MKN_third_codes-0.6.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4287 2023-05-03 09:37:41.000000 MKN_third_codes-0.6.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:42:16.820560 MKN_third_codes-0.6.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-05-03 09:41:57.000000 MKN_third_codes-0.6.5.1/setup.py
```

### Comparing `MKN_third_codes-0.6.5/LICENSE.txt` & `MKN_third_codes-0.6.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5/MKN_third_codes/mkn_globals.py` & `MKN_third_codes-0.6.5.1/MKN_third_codes/mkn_globals.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5/MKN_third_codes/mkn_utils.py` & `MKN_third_codes-0.6.5.1/MKN_third_codes/mkn_utils.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.5.1/MKN_third_codes/solutions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import math
 import re
-import mkn_utils as utl
+from mkn_utils import *
 from mkn_globals import regular_int, regular_float
 
 def buckets_n_balls_solution(boxes):
     """
     Находит ответ для вопроса 'какова вероятность достать Белый шар из n+1 урны' для задачи о n урнах с белыми и чёрными шарами, когда из каждой урны берут Ki шаров, перекладывают их в n+1 урну.
     Для решения используется теорема гипотез
 
     Args:
         boxes (list): массив объектов класса Box
 
     Returns:
         list: [list: массив объектов Hypotes, float: итоговая пероятность искомого события]
     """
-    myHyp = utl.Hypoteses(boxes)
+    myHyp = Hypoteses(boxes)
 
     hypot_prob = myHyp.get_from_boxes()
 
     prob_final = 0
     ready_hipoteses = []
     for i in range(0, len(hypot_prob)):
-        ready_hipoteses.append(utl.Hypotes([hypot_prob[i][1], hypot_prob[i][2]], hypot_prob[i][0], i+1))
+        ready_hipoteses.append(Hypotes([hypot_prob[i][1], hypot_prob[i][2]], hypot_prob[i][0], i+1))
         prob_final += hypot_prob[i][0]*hypot_prob[i][1]/(hypot_prob[i][1]+hypot_prob[i][2])
     
     return(ready_hipoteses, prob_final)
 
 def buckets_n_balls_terminal():
     """
     Решение задачи о n урнах с белыми и чёрными шарами, когда из каждой урны берут Ki шаров, перекладывают их в n+1 урну.
     """
-    boxes = [utl.Box() for _ in range(int(input("Введите количество урн: ")))]
+    boxes = [Box() for _ in range(int(input("Введите количество урн: ")))]
 
     for i in range(len(boxes)):
         boxes[i].balls[0] = int(input(f"Кол-во Б шаров в {i+1} урне: "))
         print("\033[F                                                                       ", end="\r")
         boxes[i].balls[1] = int(input(f"Кол-во Ч шаров в {i+1} урне: "))
         print("\033[F                                                                       ", end="\r")
     print("Шары заданы.")
@@ -77,15 +77,15 @@
         try:
             request = [int(parameter) for parameter in re.findall(regular_int, text)]
 
             answer = []
 
             box_num = request[0]
 
-            boxes = [utl.Box(request[1+2*i], request[2+2*i], request[1+box_num*2+i]) for i in range(box_num)]
+            boxes = [Box(request[1+2*i], request[2+2*i], request[1+box_num*2+i]) for i in range(box_num)]
 
             result = buckets_n_balls_solution(boxes)
 
             answer.append("Обозначим событие A - достать Белый шар")
 
             txt = "P(B) = "
             for hypo in result[0]:
@@ -118,23 +118,23 @@
     Решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
     WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
 
     Args:
         humans (int): кол-во людей
 
     Returns:
-        utl.EttaTable: таблица ячеек таблицы
+        EttaTable: таблица ячеек таблицы
     """
     #следующей строчкой находим количество всех перестановок
     allPerestan = math.factorial(humans)
 
     #определяем таблицу
-    myTable = utl.EttaTable(cells=[])
+    myTable = EttaTable(cells=[])
     for j in range(0, humans+1):
-        myTable.cells.append(utl.EttaTableCell(j, 0, allPerestan))
+        myTable.cells.append(EttaTableCell(j, 0, allPerestan))
 
     #Функция, проходящаяся по всем перестановкам, и записивыающая их в таблицу
     def goThrough(n, layer, used):
         if layer == humans:#раздали все предметы
             myTable.cells[n].good_th += 1
             return
         for ticket in range(0, humans):#раздаем следующий предмет
@@ -159,23 +159,23 @@
     Суть оптимизации:
         На больших значениях n существует закономерность в значениях кол-ва перестановок для СВ равной от 2 до n-2, где СВ обозначает 'какое кол-во людей получили свои вещи'
 
     Args:
         humans (int): кол-во людей
 
     Returns:
-        utl.EttaTable: таблица ячеек таблицы
+        EttaTable: таблица ячеек таблицы
     """
     #следующей строчкой находим количество всех перестановок
     allPerestan = math.factorial(humans)
 
     #определяем таблицу
-    myTable = utl.EttaTable(cells=[])
+    myTable = EttaTable(cells=[])
     for j in range(0, humans+1):
-        myTable.cells.append(utl.EttaTableCell(j, 0, allPerestan))
+        myTable.cells.append(EttaTableCell(j, 0, allPerestan))
 
     myTable.cells[0].good_th = int(round(math.factorial(humans)/math.e))
     myTable.cells[1].good_th = myTable.cells[0].good_th + (-1)**(humans+1)
     myTable.cells[-1].good_th = 1
     myTable.cells[-2].good_th = 0
 
     for id in range(2, humans-1):
@@ -264,26 +264,26 @@
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
 def geometric_meeting_terminal():
     """
     Общее решение задачи о встрече двух участников
     """
     ln = float(input("Введите отрезок меры: "))
-    fM = utl.Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
+    fM = Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
     float(input("Введите конечный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
     float(input("Введите, сколько времени будет ждать участник первый: ")))
 
-    sM = utl.Meetiner(float(input("Введите начальный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
+    sM = Meetiner(float(input("Введите начальный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
     float(input("Введите конечный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
     float(input("Введите, сколько времени будет ждать участник второй: ")))
 
     print("Обозначим за A - участники встретятся")
     print(f"P(A) = {geometric_meeting_solution(ln, fM, sM)}")
 
-def geometric_meeting_solution(length:float = 0, firstAim:utl.Meetiner=None, secondAim:utl.Meetiner=None):
+def geometric_meeting_solution(length:float = 0, firstAim:Meetiner=None, secondAim:Meetiner=None):
     """
     Решение задачи о встрече двух участников
 
     Args:
         length (float): длина участка меры, на которой могут встретиться участники
         firstAim (Meetiner): первый участник
         secondAim (Meetiner): второй участник
@@ -316,29 +316,29 @@
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
             if len(request) == 7:
                 answer = []
 
                 ln = request[0]
-                fM = utl.Meetiner(request[1], request[2], request[3])
-                sM = utl.Meetiner(request[4], request[5], request[6])
+                fM = Meetiner(request[1], request[2], request[3])
+                sM = Meetiner(request[4], request[5], request[6])
 
                 result = geometric_meeting_solution(ln, fM, sM)
 
                 answer.append("Обозначим за A - участники встретятся")
                 answer.append(f"P(A) = {result}")
 
                 return answer
             else:
                 return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-def find_math_prediction_solution(table: utl.EttaTable = None, degree: float = 1, ignore_errors: bool = False):
+def find_math_prediction_solution(table: EttaTable = None, degree: float = 1, ignore_errors: bool = False):
     """
     Нахождение МО по таблице значений случайных величин
 
     Args:
         table (EttaTable): таблица значений случайных величин
     
     Returns:
@@ -357,18 +357,18 @@
         return str(matP)
 
 def find_math_prediction_terminal():
     """
     Нахождение МО по таблице значений случайных величин
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = utl.EttaTable()
+    table = EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
-        table.cells.append(utl.EttaTableCell(etta_value=v, probability=p))
+        table.cells.append(EttaTableCell(etta_value=v, probability=p))
     result = find_math_prediction_solution(table)
     if "ошибка" not in result.lower():
         print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result}")
     else:
         print(result)
 
 def find_math_prediction_request(text: str = None):
@@ -385,32 +385,32 @@
         return ["""Введите количество значений таблицы (число n)
 В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
 
             n = int(request[0])
-            table = utl.EttaTable()
+            table = EttaTable()
 
             for i in range(0, n):
-                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
+                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
             result = find_math_prediction_solution(table)
             if "ошибка" not in result.lower():
                 answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {find_math_prediction_solution(table)}")
             else:
                 answer.append(result)
 
             return answer
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-def find_dispersion_solution(table: utl.EttaTable):
+def find_dispersion_solution(table: EttaTable):
     """
     Функция, считающая дисперсию для таблицы СВ
 
     Args:
         table (EttaTable): таблица СВ
 
     Returns:
@@ -427,18 +427,18 @@
             return "Ошибка при вычислении мат. ожидания. Проверьте коррекность введённых данных. (error code: 1)"
 
 def find_dispersion_terminal():
     """
     Функция, считающая дисперсию для таблицы СВ
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = utl.EttaTable()
+    table = EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
-        table.cells.append(utl.EttaTableCell(etta_value=v, probability=p))
+        table.cells.append(EttaTableCell(etta_value=v, probability=p))
     result = find_dispersion_solution(table)
     if "ошибка" not in result.lower():
         print(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result}")
     else:
         print(result)
 
 def find_dispersion_request(text: str = None):
@@ -455,32 +455,32 @@
         return ["""Введите количество значений таблицы (число n)
 В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
 
             n = int(request[0])
-            table = utl.EttaTable()
+            table = EttaTable()
 
             for i in range(0, n):
-                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
+                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
             result = find_dispersion_solution(table)
             if "ошибка" not in result.lower():
                 answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result}")
             else:
                 answer.append(result)
 
             return answer
         except:
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
-def table_analysis_solution(table: utl.EttaTable):
+def table_analysis_solution(table: EttaTable):
     """
     Находит Мx и Dx для таблицы значений СВ
 
     Args:
         table (EttaTable): таблица значений СВ
 
     Returns:
@@ -492,18 +492,18 @@
     return [mat_prediction, dispersion]
 
 def table_analysis_terminal():
     """
     Функция, считающая дисперсию и математическое ожидание для таблицы СВ
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = utl.EttaTable()
+    table = EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения: ").split())
-        table.cells.append(utl.EttaTableCell(etta_value=v, probability=max(p,0)))
+        table.cells.append(EttaTableCell(etta_value=v, probability=max(p,0)))
         
     result = table_analysis_solution(table)
 
     if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
         print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}\nDx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
     else:
         print("Возникла ошибка при вычислении. Проверьте коррекность введённых данных.")
@@ -525,18 +525,18 @@
         return ["""Введите количество значений таблицы (число n)
 В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
             print(request)
             n = int(request[0])
-            table = utl.EttaTable()
+            table = EttaTable()
 
             for i in range(0, n):
-                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=max(request[2+i*2],0)))
+                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=max(request[2+i*2],0)))
                 print(table.cells[i].probability, table.cells[i].etta_value)
 
             answer = []
             result = table_analysis_solution(table)
             
             if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
                 answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}")
```

### Comparing `MKN_third_codes-0.6.5/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.5.1/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.6.5
+Version: 0.6.5.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `MKN_third_codes-0.6.5/PKG-INFO` & `MKN_third_codes-0.6.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.6.5
+Version: 0.6.5.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `MKN_third_codes-0.6.5/README.md` & `MKN_third_codes-0.6.5.1/README.md`

 * *Files identical despite different names*

