# Comparing `tmp/MKN_third_codes-0.6.4.1.tar.gz` & `tmp/MKN_third_codes-0.6.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.4.1.tar", last modified: Tue May  2 13:17:03 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.4.2.tar", last modified: Wed May  3 07:37:03 2023, max compression
```

## Comparing `MKN_third_codes-0.6.4.1.tar` & `MKN_third_codes-0.6.4.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 13:17:03.307134 MKN_third_codes-0.6.4.1/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.4.1/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.4.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-02 13:17:03.284197 MKN_third_codes-0.6.4.1/MKN_third_codes/
--rw-rw-rw-   0        0        0       62 2023-05-02 13:02:12.000000 MKN_third_codes-0.6.4.1/MKN_third_codes/global_variables.py
--rw-rw-rw-   0        0        0    28519 2023-05-02 13:02:50.000000 MKN_third_codes-0.6.4.1/MKN_third_codes/solutions.py
--rw-rw-rw-   0        0        0     9634 2023-05-02 13:00:59.000000 MKN_third_codes-0.6.4.1/MKN_third_codes/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 13:17:03.305138 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     6987 2023-05-02 13:17:03.000000 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2023-05-02 13:17:03.000000 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 13:17:03.000000 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-02 13:17:03.000000 MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     6987 2023-05-02 13:17:03.306136 MKN_third_codes-0.6.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     4362 2023-05-02 13:16:36.000000 MKN_third_codes-0.6.4.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-02 13:17:03.307134 MKN_third_codes-0.6.4.1/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-05-02 13:04:13.000000 MKN_third_codes-0.6.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:37:03.245062 MKN_third_codes-0.6.4.2/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.4.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.4.2/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-03 07:37:03.225115 MKN_third_codes-0.6.4.2/MKN_third_codes/
+drwxrwxrwx   0        0        0        0 2023-05-03 07:37:03.244064 MKN_third_codes-0.6.4.2/MKN_third_codes/constructions/
+-rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.4.2/MKN_third_codes/constructions/mkn_globals.py
+-rw-rw-rw-   0        0        0     9636 2023-05-03 07:25:08.000000 MKN_third_codes-0.6.4.2/MKN_third_codes/constructions/mkn_utils.py
+-rw-rw-rw-   0        0        0    28008 2023-05-03 07:36:34.000000 MKN_third_codes-0.6.4.2/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 07:37:03.242069 MKN_third_codes-0.6.4.2/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     7396 2023-05-03 07:37:03.000000 MKN_third_codes-0.6.4.2/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      315 2023-05-03 07:37:03.000000 MKN_third_codes-0.6.4.2/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 07:37:03.000000 MKN_third_codes-0.6.4.2/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 07:37:03.000000 MKN_third_codes-0.6.4.2/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7396 2023-05-03 07:37:03.245062 MKN_third_codes-0.6.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     4324 2023-05-03 07:35:07.000000 MKN_third_codes-0.6.4.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 07:37:03.245062 MKN_third_codes-0.6.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      505 2023-05-03 07:30:23.000000 MKN_third_codes-0.6.4.2/setup.py
```

### Comparing `MKN_third_codes-0.6.4.1/LICENSE.txt` & `MKN_third_codes-0.6.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.4.1/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.4.2/MKN_third_codes/solutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,40 @@
 import math
 import re
-from utils import Box, Hypotes, Hypoteses, EttaTable, EttaTableCell, Meetiner
-from global_variables import regular_int, regular_float
-
-def combinations(k:float=0,n:float=0):
-    """
-    Функция, считающая число сочетаний из n по k
-
-    Args:
-        k (float): аргумент k - количество повторений
-        n (float): аргумент n - всего элементов
-
-    Returns:
-        float: результат применения формулы числа сочетаний
-    """
-    if k < 0 or n < 0:
-        raise ValueError("ERROR: one or more argument's values are less than 0")
-    return math.factorial(n)/(math.factorial(k)*math.factorial(n-k))
+import constructions.mkn_utils as utl
+from constructions.mkn_globals import regular_int, regular_float
 
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
@@ -92,15 +77,15 @@
         try:
             request = [int(parameter) for parameter in re.findall(regular_int, text)]
 
             answer = []
 
             box_num = request[0]
 
-            boxes = [Box(request[1+2*i], request[2+2*i], request[1+box_num*2+i]) for i in range(box_num)]
+            boxes = [utl.Box(request[1+2*i], request[2+2*i], request[1+box_num*2+i]) for i in range(box_num)]
 
             result = buckets_n_balls_solution(boxes)
 
             answer.append("Обозначим событие A - достать Белый шар")
 
             txt = "P(B) = "
             for hypo in result[0]:
@@ -133,23 +118,23 @@
     Решение задачи о 'невнимательной секретарше' (сколько людей получат свои вещи)
     WARNING: Очень неоптимизированное! Не рекоммендую пытаться решить для количества людей > 11
 
     Args:
         humans (int): кол-во людей
 
     Returns:
-        EttaTable: таблица ячеек таблицы
+        utl.EttaTable: таблица ячеек таблицы
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
@@ -174,23 +159,23 @@
     Суть оптимизации:
         На больших значениях n существует закономерность в значениях кол-ва перестановок для СВ равной от 2 до n-2, где СВ обозначает 'какое кол-во людей получили свои вещи'
 
     Args:
         humans (int): кол-во людей
 
     Returns:
-        EttaTable: таблица ячеек таблицы
+        utl.EttaTable: таблица ячеек таблицы
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
@@ -279,26 +264,26 @@
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
 def geometric_meeting_terminal():
     """
     Общее решение задачи о встрече двух участников
     """
     ln = float(input("Введите отрезок меры: "))
-    fM = Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
+    fM = utl.Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
     float(input("Введите конечный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
     float(input("Введите, сколько времени будет ждать участник первый: ")))
 
-    sM = Meetiner(float(input("Введите начальный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
+    sM = utl.Meetiner(float(input("Введите начальный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
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
@@ -331,29 +316,29 @@
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
             if len(request) == 7:
                 answer = []
 
                 ln = request[0]
-                fM = Meetiner(request[1], request[2], request[3])
-                sM = Meetiner(request[4], request[5], request[6])
+                fM = utl.Meetiner(request[1], request[2], request[3])
+                sM = utl.Meetiner(request[4], request[5], request[6])
 
                 result = geometric_meeting_solution(ln, fM, sM)
 
                 answer.append("Обозначим за A - участники встретятся")
                 answer.append(f"P(A) = {result}")
 
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
@@ -372,18 +357,18 @@
         return str(matP)
 
 def find_math_prediction_terminal():
     """
     Нахождение МО по таблице значений случайных величин
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = EttaTable()
+    table = utl.EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
-        table.cells.append(EttaTableCell(etta_value=v, probability=p))
+        table.cells.append(utl.EttaTableCell(etta_value=v, probability=p))
     result = find_math_prediction_solution(table)
     if "ошибка" not in result.lower():
         print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result}")
     else:
         print(result)
 
 def find_math_prediction_request(text: str = None):
@@ -400,32 +385,32 @@
         return ["""Введите количество значений таблицы (число n)
 В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
 
             n = int(request[0])
-            table = EttaTable()
+            table = utl.EttaTable()
 
             for i in range(0, n):
-                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
+                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
             result = find_math_prediction_solution(table)
             if "ошибка" not in result.lower():
                 answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {find_math_prediction_solution(table)}")
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
@@ -442,18 +427,18 @@
             return "Ошибка при вычислении мат. ожидания. Проверьте коррекность введённых данных. (error code: 1)"
 
 def find_dispersion_terminal():
     """
     Функция, считающая дисперсию для таблицы СВ
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = EttaTable()
+    table = utl.EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
-        table.cells.append(EttaTableCell(etta_value=v, probability=p))
+        table.cells.append(utl.EttaTableCell(etta_value=v, probability=p))
     result = find_dispersion_solution(table)
     if "ошибка" not in result.lower():
         print(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result}")
     else:
         print(result)
 
 def find_dispersion_request(text: str = None):
@@ -470,32 +455,32 @@
         return ["""Введите количество значений таблицы (число n)
 В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
 
             n = int(request[0])
-            table = EttaTable()
+            table = utl.EttaTable()
 
             for i in range(0, n):
-                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
+                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
             result = find_dispersion_solution(table)
             if "ошибка" not in result.lower():
                 answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result}")
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
@@ -507,18 +492,18 @@
     return [mat_prediction, dispersion]
 
 def table_analysis_terminal():
     """
     Функция, считающая дисперсию и математическое ожидание для таблицы СВ
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = EttaTable()
+    table = utl.EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения: ").split())
-        table.cells.append(EttaTableCell(etta_value=v, probability=max(p,0)))
+        table.cells.append(utl.EttaTableCell(etta_value=v, probability=max(p,0)))
         
     result = table_analysis_solution(table)
 
     if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
         print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}\nDx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
     else:
         print("Возникла ошибка при вычислении. Проверьте коррекность введённых данных.")
@@ -540,18 +525,18 @@
         return ["""Введите количество значений таблицы (число n)
 В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
     else:
         try:
             request = [float(parameter) for parameter in re.findall(regular_float, text)]
             print(request)
             n = int(request[0])
-            table = EttaTable()
+            table = utl.EttaTable()
 
             for i in range(0, n):
-                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=max(request[2+i*2],0)))
+                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=max(request[2+i*2],0)))
                 print(table.cells[i].probability, table.cells[i].etta_value)
 
             answer = []
             result = table_analysis_solution(table)
             
             if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
                 answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}")
```

### Comparing `MKN_third_codes-0.6.4.1/MKN_third_codes/utils.py` & `MKN_third_codes-0.6.4.2/MKN_third_codes/constructions/mkn_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from solutions import combinations
+from mkn_globals import combinations
 
 class Box():
     """
     Класс урны (коробки) для задачи об урнах
 
     Args:
         white (int): кол-во белых шаров (не является параметром)
```

### Comparing `MKN_third_codes-0.6.4.1/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.4.2/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.6.4.1
+Version: 0.6.4.2
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4.1
+# 📦 Версия: 0.6.4.2
 
-- Функции buckets_n_balls => задачи про урны
-- Функции things_complexity => задачи про путаницу вещей
-- Функции geometric_meeting => задачи про встречи
-- Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
-- Функции find_disperion => нахождение дисперсии для таблицы СВ
-- Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
-- Функция combinations => число сочетаний
+- Функции `buckets_n_balls` => задачи про урны
+- Функции `things_complexity` => задачи про путаницу вещей
+- Функции `geometric_meeting` => задачи про встречи
+- Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
+- Функции `find_disperion` => нахождение дисперсии для таблицы СВ
+- Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
+- Функция `combinations` => число сочетаний
 
 ### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
-## Структура
-- модуль `solutions` - методы
-- модуль `utils` - классы
-- модуль `global_variables` - глобальные переменные библиотеки
-## 🕹 Функции
+## 📂 Структура
+```
+━ MKN_third_codes
+    ┣ constructions
+    ┃   ┣ mkn_utils
+    ┃   ┗ mkn_globals
+    ┗ solutions
+```
+## 🔧 Функции
 - 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 - 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
@@ -53,14 +57,25 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.4.2 (02/05/2023)
+```
+------------------
+┏ исправленная структуризация проекта
+┃   ┣ global_variables -переименовано-> mkn_globals
+┃   ┣ utils -переименовано-> mkn_utils
+┃   ┗ combinations перемещено в mkn_globals
+┗ структура изменена
+    ┗ mkn_globals, mkn_utils содержатся в constructions
+------------------
+```
 ## 0.6.4.1 (02/05/2023)
 ```
 ------------------
 ━ структуризация проекта на модули utils, global_variables и solutions
 ------------------
 ```
 ## 0.6.4 (02/05/2023)
```

### Comparing `MKN_third_codes-0.6.4.1/PKG-INFO` & `MKN_third_codes-0.6.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.6.4.1
+Version: 0.6.4.2
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4.1
+# 📦 Версия: 0.6.4.2
 
-- Функции buckets_n_balls => задачи про урны
-- Функции things_complexity => задачи про путаницу вещей
-- Функции geometric_meeting => задачи про встречи
-- Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
-- Функции find_disperion => нахождение дисперсии для таблицы СВ
-- Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
-- Функция combinations => число сочетаний
+- Функции `buckets_n_balls` => задачи про урны
+- Функции `things_complexity` => задачи про путаницу вещей
+- Функции `geometric_meeting` => задачи про встречи
+- Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
+- Функции `find_disperion` => нахождение дисперсии для таблицы СВ
+- Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
+- Функция `combinations` => число сочетаний
 
 ### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
-## Структура
-- модуль `solutions` - методы
-- модуль `utils` - классы
-- модуль `global_variables` - глобальные переменные библиотеки
-## 🕹 Функции
+## 📂 Структура
+```
+━ MKN_third_codes
+    ┣ constructions
+    ┃   ┣ mkn_utils
+    ┃   ┗ mkn_globals
+    ┗ solutions
+```
+## 🔧 Функции
 - 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 - 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
 
@@ -53,14 +57,25 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.4.2 (02/05/2023)
+```
+------------------
+┏ исправленная структуризация проекта
+┃   ┣ global_variables -переименовано-> mkn_globals
+┃   ┣ utils -переименовано-> mkn_utils
+┃   ┗ combinations перемещено в mkn_globals
+┗ структура изменена
+    ┗ mkn_globals, mkn_utils содержатся в constructions
+------------------
+```
 ## 0.6.4.1 (02/05/2023)
 ```
 ------------------
 ━ структуризация проекта на модули utils, global_variables и solutions
 ------------------
 ```
 ## 0.6.4 (02/05/2023)
```

### Comparing `MKN_third_codes-0.6.4.1/README.md` & `MKN_third_codes-0.6.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4.1
+# 📦 Версия: 0.6.4.2
 
-- Функции buckets_n_balls => задачи про урны
-- Функции things_complexity => задачи про путаницу вещей
-- Функции geometric_meeting => задачи про встречи
-- Функции find_math_prediction => нахождение математического ожидания для таблицы СВ
-- Функции find_disperion => нахождение дисперсии для таблицы СВ
-- Функции table_analysis => нахождение МО и Дисперсии для таблицы СВ
-- Функция combinations => число сочетаний
+- Функции `buckets_n_balls` => задачи про урны
+- Функции `things_complexity` => задачи про путаницу вещей
+- Функции `geometric_meeting` => задачи про встречи
+- Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
+- Функции `find_disperion` => нахождение дисперсии для таблицы СВ
+- Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
+- Функция `combinations` => число сочетаний
 
 ### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
-## Структура
-- модуль `solutions` - методы
-- модуль `utils` - классы
-- модуль `global_variables` - глобальные переменные библиотеки
-## 🕹 Функции
+## 📂 Структура
+```
+━ MKN_third_codes
+    ┣ constructions
+    ┃   ┣ mkn_utils
+    ┃   ┗ mkn_globals
+    ┗ solutions
+```
+## 🔧 Функции
 - 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 - 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
 ## 🧱 Классы
 - Классы данной библиотеки можно использовать вне функций, предоставляемых данной библиотекой, но т.к. классы заточены под неё, то ими возможно будет неудобно пользоваться.
```

