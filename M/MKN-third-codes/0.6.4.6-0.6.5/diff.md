# Comparing `tmp/MKN_third_codes-0.6.4.6.tar.gz` & `tmp/MKN_third_codes-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.4.6.tar", last modified: Wed May  3 09:33:44 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.5.tar", last modified: Wed May  3 09:38:13 2023, max compression
```

## Comparing `MKN_third_codes-0.6.4.6.tar` & `MKN_third_codes-0.6.5.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 09:33:44.775917 MKN_third_codes-0.6.4.6/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.4.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.4.6/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-03 09:33:44.762952 MKN_third_codes-0.6.4.6/MKN_third_codes/
-drwxrwxrwx   0        0        0        0 2023-05-03 09:33:44.774920 MKN_third_codes-0.6.4.6/MKN_third_codes/constructions/
--rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.4.6/MKN_third_codes/constructions/mkn_globals.py
--rw-rw-rw-   0        0        0     9637 2023-05-03 09:23:06.000000 MKN_third_codes-0.6.4.6/MKN_third_codes/constructions/mkn_utils.py
--rw-rw-rw-   0        0        0    28013 2023-05-03 09:32:28.000000 MKN_third_codes-0.6.4.6/MKN_third_codes/solutions.py
-drwxrwxrwx   0        0        0        0 2023-05-03 09:33:44.772925 MKN_third_codes-0.6.4.6/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     7544 2023-05-03 09:33:44.000000 MKN_third_codes-0.6.4.6/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-05-03 09:33:44.000000 MKN_third_codes-0.6.4.6/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 09:33:44.000000 MKN_third_codes-0.6.4.6/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-03 09:33:44.000000 MKN_third_codes-0.6.4.6/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7544 2023-05-03 09:33:44.774920 MKN_third_codes-0.6.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     4322 2023-05-03 09:33:28.000000 MKN_third_codes-0.6.4.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-03 09:33:44.775917 MKN_third_codes-0.6.4.6/setup.cfg
--rw-rw-rw-   0        0        0      505 2023-05-03 09:33:16.000000 MKN_third_codes-0.6.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:38:13.569330 MKN_third_codes-0.6.5/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.5/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.5/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-03 09:38:13.560354 MKN_third_codes-0.6.5/MKN_third_codes/
+-rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.5/MKN_third_codes/mkn_globals.py
+-rw-rw-rw-   0        0        0     9636 2023-05-03 09:36:24.000000 MKN_third_codes-0.6.5/MKN_third_codes/mkn_utils.py
+-rw-rw-rw-   0        0        0    27980 2023-05-03 09:35:54.000000 MKN_third_codes-0.6.5/MKN_third_codes/solutions.py
+drwxrwxrwx   0        0        0        0 2023-05-03 09:38:13.567336 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     7698 2023-05-03 09:38:13.000000 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-03 09:38:13.000000 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 09:38:13.000000 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-03 09:38:13.000000 MKN_third_codes-0.6.5/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7698 2023-05-03 09:38:13.568333 MKN_third_codes-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4287 2023-05-03 09:37:41.000000 MKN_third_codes-0.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-03 09:38:13.569330 MKN_third_codes-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      503 2023-05-03 09:38:08.000000 MKN_third_codes-0.6.5/setup.py
```

### Comparing `MKN_third_codes-0.6.4.6/LICENSE.txt` & `MKN_third_codes-0.6.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.4.6/MKN_third_codes/constructions/mkn_globals.py` & `MKN_third_codes-0.6.5/MKN_third_codes/mkn_globals.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.4.6/MKN_third_codes/constructions/mkn_utils.py` & `MKN_third_codes-0.6.5/MKN_third_codes/mkn_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .mkn_globals import combinations
+from mkn_globals import combinations
 
 class Box():
     """
     Класс урны (коробки) для задачи об урнах
 
     Args:
         white (int): кол-во белых шаров (не является параметром)
```

### Comparing `MKN_third_codes-0.6.4.6/MKN_third_codes/solutions.py` & `MKN_third_codes-0.6.5/MKN_third_codes/solutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 import re
-from constructions import mkn_utils as utl
-from constructions.mkn_globals import regular_int, regular_float
+import mkn_utils as utl
+from mkn_globals import regular_int, regular_float
 
 def buckets_n_balls_solution(boxes):
     """
     Находит ответ для вопроса 'какова вероятность достать Белый шар из n+1 урны' для задачи о n урнах с белыми и чёрными шарами, когда из каждой урны берут Ki шаров, перекладывают их в n+1 урну.
     Для решения используется теорема гипотез
 
     Args:
```

### Comparing `MKN_third_codes-0.6.4.6/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.5/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.6.4.6
+Version: 0.6.5
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4
+# 📦 Версия: 0.6.5
 
 - Функции `buckets_n_balls` => задачи про урны
 - Функции `things_complexity` => задачи про путаницу вещей
 - Функции `geometric_meeting` => задачи про встречи
 - Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
 - Функции `find_disperion` => нахождение дисперсии для таблицы СВ
 - Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
@@ -24,17 +24,16 @@
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
 ## 📂 Структура
 ```
 ━ MKN_third_codes
-    ┣ constructions
-    ┃   ┣ mkn_utils
-    ┃   ┗ mkn_globals
+    ┣ mkn_globals
+    ┣ mkn_utils
     ┗ solutions
 ```
 ## 🔧 Функции
 - 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 - 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
@@ -57,14 +56,20 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.5 (03/05/2023)
+```
+------------------
+━ изменена структура т.к. setup файл сливал все файлы в одну папку.
+------------------
+```
 ## 0.6.4.3-6 (03/05/2023)
 ```
 ------------------
 ━ Да как нормально настроить импорты???
 ------------------
 ```
 ## 0.6.4.2 (03/05/2023)
```

### Comparing `MKN_third_codes-0.6.4.6/PKG-INFO` & `MKN_third_codes-0.6.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.6.4.6
+Version: 0.6.5
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4
+# 📦 Версия: 0.6.5
 
 - Функции `buckets_n_balls` => задачи про урны
 - Функции `things_complexity` => задачи про путаницу вещей
 - Функции `geometric_meeting` => задачи про встречи
 - Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
 - Функции `find_disperion` => нахождение дисперсии для таблицы СВ
 - Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
@@ -24,17 +24,16 @@
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
 ## 📂 Структура
 ```
 ━ MKN_third_codes
-    ┣ constructions
-    ┃   ┣ mkn_utils
-    ┃   ┗ mkn_globals
+    ┣ mkn_globals
+    ┣ mkn_utils
     ┗ solutions
 ```
 ## 🔧 Функции
 - 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 - 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
@@ -57,14 +56,20 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.5 (03/05/2023)
+```
+------------------
+━ изменена структура т.к. setup файл сливал все файлы в одну папку.
+------------------
+```
 ## 0.6.4.3-6 (03/05/2023)
 ```
 ------------------
 ━ Да как нормально настроить импорты???
 ------------------
 ```
 ## 0.6.4.2 (03/05/2023)
```

### Comparing `MKN_third_codes-0.6.4.6/README.md` & `MKN_third_codes-0.6.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.4
+# 📦 Версия: 0.6.5
 
 - Функции `buckets_n_balls` => задачи про урны
 - Функции `things_complexity` => задачи про путаницу вещей
 - Функции `geometric_meeting` => задачи про встречи
 - Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
 - Функции `find_disperion` => нахождение дисперсии для таблицы СВ
 - Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
@@ -14,17 +14,16 @@
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from MKN_third_codes import solutions`
 ## 📂 Структура
 ```
 ━ MKN_third_codes
-    ┣ constructions
-    ┃   ┣ mkn_utils
-    ┃   ┗ mkn_globals
+    ┣ mkn_globals
+    ┣ mkn_utils
     ┗ solutions
 ```
 ## 🔧 Функции
 - 📱 любая функция, решающая задачу имеет суффикс `_terminal`. Это значит, что, используя данную функцию, дополнительно ничего писать не надо, т.к. она представляет из себя готовое решение типа задач. Всё взаимодействие происходит в терминале.
 - 📲 любая функция, решающая задачу имеет суффикс `_solution`. Такая функция принимает аргументы на вход, которые ей следует предоставить. В описании каждой функции есть описание возвращаемого объекта.
 - 📨 любая функция, решающая задачу имеет суффикс `_request`. Этот тип функций позволяет взаимодействовать с ней извне, например, отсылая в качестве входного параметра ввод пользователя.
 - 📊 Некоторые функции имеют метафикс `_optimized`. Такие функции считают значения приблизительно, так как в них используются формулы, дающие значения, близкие к действительным. Используйте данные функции только если слишком долги считать некоторые значения на обычных функциях.
```

