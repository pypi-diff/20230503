# Comparing `tmp/KUKA_youbot-0.1.1.tar.gz` & `tmp/KUKA_youbot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KUKA_youbot-0.1.1.tar", last modified: Fri Apr  7 10:57:37 2023, max compression
+gzip compressed data, was "KUKA_youbot-0.1.2.tar", last modified: Wed May  3 11:40:56 2023, max compression
```

## Comparing `KUKA_youbot-0.1.1.tar` & `KUKA_youbot-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-04-07 10:57:37.178055 KUKA_youbot-0.1.1/
--rw-rw-r--   0 mark      (1000) mark      (1000)     1074 2023-03-18 13:45:02.000000 KUKA_youbot-0.1.1/LICENSE
--rw-rw-r--   0 mark      (1000) mark      (1000)     4449 2023-04-07 10:57:37.178055 KUKA_youbot-0.1.1/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)     3944 2023-03-18 13:50:26.000000 KUKA_youbot-0.1.1/README.md
--rw-rw-r--   0 mark      (1000) mark      (1000)      752 2023-04-07 10:56:31.000000 KUKA_youbot-0.1.1/pyproject.toml
--rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-04-07 10:57:37.178055 KUKA_youbot-0.1.1/setup.cfg
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-04-07 10:57:37.174055 KUKA_youbot-0.1.1/src/
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-04-07 10:57:37.178055 KUKA_youbot-0.1.1/src/KUKA/
--rw-rw-r--   0 mark      (1000) mark      (1000)    33949 2023-04-07 10:55:44.000000 KUKA_youbot-0.1.1/src/KUKA/KUKA.py
--rw-rw-r--   0 mark      (1000) mark      (1000)     7355 2023-04-07 10:55:54.000000 KUKA_youbot-0.1.1/src/KUKA/SSH.py
--rw-rw-r--   0 mark      (1000) mark      (1000)       24 2023-03-17 08:35:01.000000 KUKA_youbot-0.1.1/src/KUKA/__init__.py
--rw-rw-r--   0 mark      (1000) mark      (1000)      382 2023-03-18 13:10:48.000000 KUKA_youbot-0.1.1/src/KUKA/service.py
-drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-04-07 10:57:37.178055 KUKA_youbot-0.1.1/src/KUKA_youbot.egg-info/
--rw-rw-r--   0 mark      (1000) mark      (1000)     4449 2023-04-07 10:57:37.000000 KUKA_youbot-0.1.1/src/KUKA_youbot.egg-info/PKG-INFO
--rw-rw-r--   0 mark      (1000) mark      (1000)      300 2023-04-07 10:57:37.000000 KUKA_youbot-0.1.1/src/KUKA_youbot.egg-info/SOURCES.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-04-07 10:57:37.000000 KUKA_youbot-0.1.1/src/KUKA_youbot.egg-info/dependency_links.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)      103 2023-04-07 10:57:37.000000 KUKA_youbot-0.1.1/src/KUKA_youbot.egg-info/requires.txt
--rw-rw-r--   0 mark      (1000) mark      (1000)        5 2023-04-07 10:57:37.000000 KUKA_youbot-0.1.1/src/KUKA_youbot.egg-info/top_level.txt
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 11:40:56.522093 KUKA_youbot-0.1.2/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1074 2023-03-18 13:45:02.000000 KUKA_youbot-0.1.2/LICENSE
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5244 2023-05-03 11:40:56.522093 KUKA_youbot-0.1.2/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)     4821 2023-05-03 11:27:44.000000 KUKA_youbot-0.1.2/README.md
+-rw-rw-r--   0 mark      (1000) mark      (1000)      841 2023-05-03 11:40:44.000000 KUKA_youbot-0.1.2/pyproject.toml
+-rw-rw-r--   0 mark      (1000) mark      (1000)       38 2023-05-03 11:40:56.522093 KUKA_youbot-0.1.2/setup.cfg
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 11:40:56.518093 KUKA_youbot-0.1.2/src/
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 11:40:56.522093 KUKA_youbot-0.1.2/src/KUKA/
+-rw-rw-r--   0 mark      (1000) mark      (1000)    35145 2023-05-03 11:24:55.000000 KUKA_youbot-0.1.2/src/KUKA/KUKA.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     7483 2023-04-27 10:03:13.000000 KUKA_youbot-0.1.2/src/KUKA/SSH.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)      161 2023-05-03 10:52:47.000000 KUKA_youbot-0.1.2/src/KUKA/__init__.py
+-rw-rw-r--   0 mark      (1000) mark      (1000)     1452 2023-05-03 11:12:36.000000 KUKA_youbot-0.1.2/src/KUKA/service.py
+drwxrwxr-x   0 mark      (1000) mark      (1000)        0 2023-05-03 11:40:56.522093 KUKA_youbot-0.1.2/src/KUKA_youbot.egg-info/
+-rw-rw-r--   0 mark      (1000) mark      (1000)     5244 2023-05-03 11:40:56.000000 KUKA_youbot-0.1.2/src/KUKA_youbot.egg-info/PKG-INFO
+-rw-rw-r--   0 mark      (1000) mark      (1000)      300 2023-05-03 11:40:56.000000 KUKA_youbot-0.1.2/src/KUKA_youbot.egg-info/SOURCES.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        1 2023-05-03 11:40:56.000000 KUKA_youbot-0.1.2/src/KUKA_youbot.egg-info/dependency_links.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)      103 2023-05-03 11:40:56.000000 KUKA_youbot-0.1.2/src/KUKA_youbot.egg-info/requires.txt
+-rw-rw-r--   0 mark      (1000) mark      (1000)        5 2023-05-03 11:40:56.000000 KUKA_youbot-0.1.2/src/KUKA_youbot.egg-info/top_level.txt
```

### Comparing `KUKA_youbot-0.1.1/LICENSE` & `KUKA_youbot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `KUKA_youbot-0.1.1/PKG-INFO` & `KUKA_youbot-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: KUKA_youbot
-Version: 0.1.1
-Summary: package for easy KUKA-youbot control
-Author-email: ZaSKaR <mark.turkov@mail.ru>
-Project-URL: Homepage, https://github.com/MarkT5/YouBotKUKA
-Project-URL: Bug Tracker, https://github.com/MarkT5/YouBotKUKA/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Robot Framework :: Tool
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Краткий обзор класса KUKA (Python)/(User manual):
 ____
 Класс KUKA написан для удобной работы с роботом KUKA youbot с помощью языка программирования Python. В классе есть несколько основных методов для управления роботом.
 
 source: https://github.com/MarkT5/KUKAyoubot_lib
 ____
 ## Параметры при создании элемента класса
@@ -37,47 +23,58 @@
 
 ___log___ _[(str), (int)]_: [path, freq] logs odometry and lidar data to set path with set frequency
 
 ___read_from_log___ _[(str), (int)]_: [path, freq] streams odometry and lidar data from set log path with set frequency
 ___
 ## Основные Методы
 
-___move_arm(...)___ — Sets arm position\n
-        ways to set arm position:\n
-        array of values: (joint 1, joint 2, joint 3, joint 4, joint 5, grip)\n
-        
-by keywords:
+___move_arm(...)___ — Sets arm position
 
-1. ___m1, m2, m3, m4, m5___ - for joints __(all joint parameters are relative and in degrees from upright position)__
-2.    ___grip___ - (0 - 2) for grip
-3.    target - ((x, y), ang) to set arm position in cylindrical coordinates (ang - angle from last joint to horizon)
+ways to set arm position:
+
+array of values:
+- (joint 1, joint 2, joint 3, joint 4, joint 5, grip) - degrees from upright position
         
+by keywords:
+- ___m1, m2, m3, m4, m5___ - for joints __(all joint parameters are relative and in degrees from upright position)__
+- ___grip___ - (0 - 2) for grip
+     
 
 ___move_base(f, s, ang)___ — принимает:
 
 1. ___f___ — скорость движения вдоль оси по которой направлен робот, если положительное — движение вперёд, если отрицательное — назад,
 2. ___s___ — скорость движения поперёк оси по которой направлен робот
 3. ___ang___ — угловая скорость
 если вызвать этот метод без указания аргументов, то будет отправлена команда остановки
 
 ___go_to(x, y, ang)___ — отправляет робота по координатам x, y и задаёт угол от оси x до направления робота (в метрах)
 
-
-
 ___post_to_send_data(ind, msg)___ — Записывает сообщение msg в ячейку отправки ind (используется другими методами для общения с роботом, но также может использоваться для отправки пользовательских команд, если вызвана с индексом 3. 0 — скорости платформы, 1 — положения манипулятора, 2 — положение захвата)
 
 
-___arm___ (float[6]) — arm_id, joint 1 - joint 5 
+___camera/camera_BGR()___ _returns: (cv2.Mat)_- возвращает изображение в специальном сжатом формате
 
-___wheels___ (float[4]) — wheel 1 - wheel 4
+___depth_camera()___ _returns: (cv2.Mat)_ — возвращает изображение с depth камеры
 
-___lidar___ _([float[3], float[lidar_resolution]])_— возвращает массив длиной 623 с расстояниями до точек равномерно распределённых от 0 до 240 градусов и данные одометрии скрепленные с этим измерением
+### Properties:
+___arm___ _returns: float[6]_ — arm_id, joint 1 - joint 5 
 
-___increment___ _(float[3])_ — возвращает массив с положениями по оси x, y и угла от оси x до направления робота
+___wheels___ _returns: float[4]_ — wheel 1 - wheel 4
 
-___camera/camera_BGR()___ _(cv2.Mat)_- возвращает изображение в специальном сжатом формате
+___lidar___ _returns: ([float[3], float[lidar_resolution]])_— возвращает массив длиной 623 с расстояниями до точек равномерно распределённых от 0 до 240 градусов и данные одометрии скрепленные с этим измерением
 
-___depth_camera()___ _(cv2.Mat)_ — возвращает изображение с depth камеры
+___increment___ _(returns: float[3])_ — возвращает массив с положениями по оси x, y и угла от оси x до направления робота
 
 
+## SSH:
+___
+___send(msg)___ msg (string) - отправить команду через SSH
+
+___send_recv(msg)___ msg (string) - отправить команду через SSH и дождаться её завершения
+___send_wait(msg_send, wait_msg, timeout=None, timeout_msg=None, verbose=0, max_time=20):___
+- msg_send (string)- сообщение на отправку
+- wait_msg (string)- ответ, которое будет ожидаться
+- timeout (int)- максимальное время ожидания следующего ответа
+- timeout_msg (string)-сообщение, которое будет напечатано в командную строку при привышении времени ожидания
+- verbose (int)- 0-не печатать информацию, 1-печататать только важное, 2-печатать все полученные ответы
 ___
-### подробнее - читай dock-string
+### подробнее - читай dock-string
```

### Comparing `KUKA_youbot-0.1.1/README.md` & `KUKA_youbot-0.1.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: KUKA_youbot
+Version: 0.1.2
+Summary: package for easy KUKA-youbot control
+Author-email: ZaSKaR <mark.turkov@mail.ru>
+Project-URL: Homepage, https://github.com/MarkT5/YouBotKUKA
+Project-URL: Bug Tracker, https://github.com/MarkT5/YouBotKUKA/issues
+Project-URL: repository, https://github.com/MarkT5/YouBotKUKA
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Краткий обзор класса KUKA (Python)/(User manual):
 ____
 Класс KUKA написан для удобной работы с роботом KUKA youbot с помощью языка программирования Python. В классе есть несколько основных методов для управления роботом.
 
 source: https://github.com/MarkT5/KUKAyoubot_lib
 ____
 ## Параметры при создании элемента класса
@@ -23,47 +35,58 @@
 
 ___log___ _[(str), (int)]_: [path, freq] logs odometry and lidar data to set path with set frequency
 
 ___read_from_log___ _[(str), (int)]_: [path, freq] streams odometry and lidar data from set log path with set frequency
 ___
 ## Основные Методы
 
-___move_arm(...)___ — Sets arm position\n
-        ways to set arm position:\n
-        array of values: (joint 1, joint 2, joint 3, joint 4, joint 5, grip)\n
-        
-by keywords:
+___move_arm(...)___ — Sets arm position
 
-1. ___m1, m2, m3, m4, m5___ - for joints __(all joint parameters are relative and in degrees from upright position)__
-2.    ___grip___ - (0 - 2) for grip
-3.    target - ((x, y), ang) to set arm position in cylindrical coordinates (ang - angle from last joint to horizon)
+ways to set arm position:
+
+array of values:
+- (joint 1, joint 2, joint 3, joint 4, joint 5, grip) - degrees from upright position
         
+by keywords:
+- ___m1, m2, m3, m4, m5___ - for joints __(all joint parameters are relative and in degrees from upright position)__
+- ___grip___ - (0 - 2) for grip
+     
 
 ___move_base(f, s, ang)___ — принимает:
 
 1. ___f___ — скорость движения вдоль оси по которой направлен робот, если положительное — движение вперёд, если отрицательное — назад,
 2. ___s___ — скорость движения поперёк оси по которой направлен робот
 3. ___ang___ — угловая скорость
 если вызвать этот метод без указания аргументов, то будет отправлена команда остановки
 
 ___go_to(x, y, ang)___ — отправляет робота по координатам x, y и задаёт угол от оси x до направления робота (в метрах)
 
-
-
 ___post_to_send_data(ind, msg)___ — Записывает сообщение msg в ячейку отправки ind (используется другими методами для общения с роботом, но также может использоваться для отправки пользовательских команд, если вызвана с индексом 3. 0 — скорости платформы, 1 — положения манипулятора, 2 — положение захвата)
 
 
-___arm___ (float[6]) — arm_id, joint 1 - joint 5 
+___camera/camera_BGR()___ _returns: (cv2.Mat)_- возвращает изображение в специальном сжатом формате
 
-___wheels___ (float[4]) — wheel 1 - wheel 4
+___depth_camera()___ _returns: (cv2.Mat)_ — возвращает изображение с depth камеры
 
-___lidar___ _([float[3], float[lidar_resolution]])_— возвращает массив длиной 623 с расстояниями до точек равномерно распределённых от 0 до 240 градусов и данные одометрии скрепленные с этим измерением
+### Properties:
+___arm___ _returns: float[6]_ — arm_id, joint 1 - joint 5 
 
-___increment___ _(float[3])_ — возвращает массив с положениями по оси x, y и угла от оси x до направления робота
+___wheels___ _returns: float[4]_ — wheel 1 - wheel 4
 
-___camera/camera_BGR()___ _(cv2.Mat)_- возвращает изображение в специальном сжатом формате
+___lidar___ _returns: ([float[3], float[lidar_resolution]])_— возвращает массив длиной 623 с расстояниями до точек равномерно распределённых от 0 до 240 градусов и данные одометрии скрепленные с этим измерением
 
-___depth_camera()___ _(cv2.Mat)_ — возвращает изображение с depth камеры
+___increment___ _(returns: float[3])_ — возвращает массив с положениями по оси x, y и угла от оси x до направления робота
 
 
+## SSH:
+___
+___send(msg)___ msg (string) - отправить команду через SSH
+
+___send_recv(msg)___ msg (string) - отправить команду через SSH и дождаться её завершения
+___send_wait(msg_send, wait_msg, timeout=None, timeout_msg=None, verbose=0, max_time=20):___
+- msg_send (string)- сообщение на отправку
+- wait_msg (string)- ответ, которое будет ожидаться
+- timeout (int)- максимальное время ожидания следующего ответа
+- timeout_msg (string)-сообщение, которое будет напечатано в командную строку при привышении времени ожидания
+- verbose (int)- 0-не печатать информацию, 1-печататать только важное, 2-печатать все полученные ответы
 ___
-### подробнее - читай dock-string
+### подробнее - читай dock-string
```

### Comparing `KUKA_youbot-0.1.1/pyproject.toml` & `KUKA_youbot-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "KUKA_youbot"
-version = "0.1.1"
-authors = [
-  { name="ZaSKaR", email="mark.turkov@mail.ru" },
+version = "0.1.2"
+authors = [{name = "ZaSKaR", email="mark.turkov@mail.ru"} ,
 ]
+
 dependencies = [
     "setuptools >= 40.9.0",
-    "numpy >= 1.24.2",
+    "numpy >= 1.23.0",
     "opencv-python >= 4.7.0.72",
     "py-mjpeg >= 1.0.1",
     "paramiko >= 3.1.0",
     "Pillow >= 9.4.0",
 ]
 description = "package for easy KUKA-youbot control"
 readme = "README.md"
 requires-python = ">=3.8"
+
+[project.urls]
+"Homepage" = "https://github.com/MarkT5/YouBotKUKA"
+"Bug Tracker" = "https://github.com/MarkT5/YouBotKUKA/issues"
+
+repository = "https://github.com/MarkT5/YouBotKUKA"
+
+[tool.poetry]
+readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Framework :: Robot Framework :: Tool",
     "Operating System :: OS Independent",
 ]
-[project.urls]
-"Homepage" = "https://github.com/MarkT5/YouBotKUKA"
-"Bug Tracker" = "https://github.com/MarkT5/YouBotKUKA/issues"
```

### Comparing `KUKA_youbot-0.1.1/src/KUKA/KUKA.py` & `KUKA_youbot-0.1.2/src/KUKA/KUKA.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 import threading as thr
 import time
 
 import cv2
 import numpy as np
 import paramiko
 from PIL import Image
-from mjpeg.client import MJPEGClient
 from .SSH import SSH
-from .service import debug, range_cut
+from .service import debug, range_cut, test_MJPEG_client
+from mjpeg.client import MJPEGClient
+import urllib.request
+import mjpeg
 
 
 class YouBot:
     """
     KUKA youbot controller
     """
 
@@ -44,17 +46,21 @@
         :param camera_enable (bool): enables mjpeg client if True
         :param advanced (bool): disables all safety checks in the sake of time saving
         :param log [(str), (int)]: if [path, freq] logs odometry and lidar data to set path with set frequency
         :param read_from_log [(str), (int)]: if [path, freq] streams odometry and lidar data from set log path with set frequency
         """
         if advanced:
             debug("WARNING!!! ADVANCED MODE ENABLED, ALL SAFETY CHECKS ARE SUSPENDED")
-        debug("Copyright \x1b[91m©\x1b[39m 2023 \x1b[92mZaSKaR\x1b[39m (\x1b[4mTurkov Mark\x1b[24m, RTU MIREA)")
+
+        # threading
         self.threads_number = 0
         self.main_thr = thr.main_thread()
+        self.cam_rgb_lock = thr.Lock()
+        self.cam_depth_lock = thr.Lock()
+
         self.camera_enable = camera_enable
         self.read_depth = read_depth
         self.ip = ip
         self.frequency = 50  # operating frequency
         self.data_lock = thr.Lock()
         self.connected = True
 
@@ -84,17 +90,18 @@
         # dimensions (lengths of joints)
         self.m2_len = 155
         self.m3_len = 135
         self.m4_len = 200
 
         # sensor data
         self.lidar_data = None
-        self.increment_data_lidar = [0,0,0]  # the closest to lidar read increment value
-        self.increment_data = [0,0,0]
-        self.odom_speed_data = [0,0,0]
+        self.lidar_frame_count = 0
+        self.increment_data_lidar = [0, 0, 0]  # the closest to lidar read increment value
+        self.increment_data = [0, 0, 0]
+        self.odom_speed_data = [0, 0, 0]
         self.corr_arm_pos = [None, None]
         self.wheels_data = None
         self.wheels_data_lidar = None
         self.trace = 0
 
         # for position correction
         self.wheels_old = None
@@ -109,14 +116,15 @@
             return
         if offline:
             self.connected = False
             return
 
         # connection
         debug(f"connecting to {ip}")
+
         def connect_to_control():
             if self.connected:
                 debug("connecting to control channel")
                 # init socket
                 try:
                     self.conn = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                     self.conn.settimeout(5)
@@ -133,37 +141,41 @@
                 except(TimeoutError):
                     self.connected = False
                     debug("unable to connect to socket")
                     return 1
                 except(ConnectionRefusedError):
                     debug("connection refused, (re)starting ROS")
                     return 2
-
+                except(OSError):
+                    raise OSError(
+                        f"Can't find robot with ip {self.ip} in local network. Turn on the robot, and wait until full startup")
 
         if connect_to_control() == 2:
             ros = True
             ssh = True
         self.ssh = SSH(user='youbot', ip=ip, password=pwd, connect=ssh)
         if self.ssh.connected:
             ros_ssh = True
             if not advanced:
-                ros_ssh, _, _ = self.ssh.ROS_status()
+                ros_ssh, _, _ = self.ssh.ROS_status(verbose=False)
             if not ros_ssh or ros:
                 self.ssh.launch_ROS()
                 self.connected = True
                 connect_to_control()
         elif ssh:
             debug("unable to connect to SSH")
 
-
         # connecting to video server
         if self.connected and self.camera_enable:
             if self.read_depth:
-                self.init_depth_client()
-            self.init_rgb_client()
+                if not self.init_depth_client():
+                    self.read_depth = False
+            if not self.init_rgb_client():
+                self.camera_enable = False
+                debug("\x1b[33mWARNING camera is not connected or video server is not running\x1b[39m")
 
         # waiting for initial arm position
         if self.connected:
             # debug("waiting for initial arm position")
             self.corr_arm_pos = [[0, 0, 0, 0, 0], [0, 0, 0, 0, 0]]
             self.arm_pos[0][:-1] = self.corr_arm_pos[0]
             self.arm_pos[1][:-1] = self.corr_arm_pos[1]
@@ -179,33 +191,38 @@
         """
         debug("connecting to video channel")
         self.client_rgb = MJPEGClient(
             f"http://{self.ip}:8080/stream?topic=/camera/rgb/image_rect_color&width=640&height=480&quality=20")
         bufs = self.client_rgb.request_buffers(65536, 5)
         for b in bufs:
             self.client_rgb.enqueue_buffer(b)
+        if not test_MJPEG_client(self.client_rgb.url):
+            return False
+
         self.client_rgb.start()
-        self.cam_rgb_lock = thr.Lock()
         self.cam_rgb_thr = thr.Thread(target=self.get_frame_color, args=())
         self.threads_number += 1
         self.cam_rgb_thr.start()
+        return True
 
     def init_depth_client(self):
         """
         Starts video client thread that reads depth video
         """
         self.client_depth = MJPEGClient(f"http://{self.ip}:8080/stream?topic=/camera/depth/image_rect")
         bufsd = self.client_depth.request_buffers(65536, 5)
         for b in bufsd:
             self.client_depth.enqueue_buffer(b)
+        if not test_MJPEG_client(self.client_depth.url):
+            return False
         self.client_depth.start()
-        self.cam_depth_lock = thr.Lock()
         self.cam_depth_thr = thr.Thread(target=self.get_frame_depth, args=())
         self.threads_number += 1
         self.cam_depth_thr.start()
+        return True
 
     # receiving and parsing sensor data
 
     def post_to_send_data(self, ind, data):
         """
         Updates send queue
         :param ind: data type: 0-base, 1-arm, 2-grip
@@ -345,14 +362,15 @@
             except:
                 wheels = None
         # update data
         if write_lidar or write_increment or write_arm1 or write_arm2 or wheels:
 
             self.data_lock.acquire()
             if write_lidar:
+                self.lidar_frame_count += 1
                 self.lidar_data = write_lidar
                 self.increment_data_lidar = self.increment_data
                 self.calculated_pos_lidar = self.calculated_pos[:]
                 self.wheels_data_lidar = self.wheels_data
             if write_increment:
                 self.increment_data = write_increment
             if write_odom_speed:
@@ -407,15 +425,15 @@
                     str_data = str(self.data_buff, encoding='utf-8')
                     last = str_data.rfind("\r\n")
 
                     if last == -1:
                         leftovers = self.data_buff[:]
                     else:
 
-                        leftovers = str.encode(str_data[last+2:])
+                        leftovers = str.encode(str_data[last + 2:])
                         str_data = str_data[:last]
                         splitted = str_data.split("\r\n")
                         for i in splitted:
                             self._parse_data(i)
                 except Exception as e:
                     debug(e)
                     pass
@@ -608,17 +626,17 @@
     def move_base(self, f=0.0, s=0.0, r=0.0):
         """
         Sets moving speed
         :param f: forward speed
         :param s: sideways speed
         :param r: rotation speed
         """
-        f = range_cut(-1, 1, f)
-        s = range_cut(-1, 1, s)
-        r = range_cut(-1, 1, r)
+        f = round(range_cut(-1, 1, f), 3)
+        s = round(range_cut(-1, 1, s), 3)
+        r = round(range_cut(-1, 1, r), 3)
         self.post_to_send_data(0, bytes(f'/base:{f};{s};{r}^^^', encoding='utf-8'))
         self.move_speed = (f, s, r)
 
     # go to set coordinates
     def go_to(self, x, y, ang=0, /, prec=0.005, k=1, initial_speed=None):
         """
         Sends robot to given coordinates
@@ -656,20 +674,28 @@
             loc_y = y - inc[1]
             rob_ang = inc[2]
             dist = math.sqrt(loc_x ** 2 + loc_y ** 2)
             speed = min(initial_speed, dist * k)
 
             targ_ang = math.atan2(loc_y, loc_x)
             loc_ang = targ_ang - rob_ang
-            if dist < prec and (ang - rob_ang) < prec:
+            if dist < prec and abs(ang - rob_ang) < prec:
                 break
             fov_speed = speed * math.cos(loc_ang)
             side_speed = -speed * math.sin(loc_ang)
             total_speed = math.sqrt(fov_speed ** 2 + side_speed ** 2)
-            ang_speed = -(ang - rob_ang) / (dist / total_speed)
+            delta_ang = ang - rob_ang
+            if delta_ang > math.pi:
+                delta_ang -= 2 * math.pi
+            elif delta_ang < -math.pi:
+                delta_ang += 2 * math.pi
+            if dist / total_speed != 0:
+                ang_speed = -delta_ang / (dist / total_speed)
+            else:
+                ang_speed = -delta_ang * 0.3
             self.move_base(fov_speed, side_speed, ang_speed)
             time.sleep(1 / self.frequency)
         self.move_base(0, 0, 0)
         time.sleep(0.01)
         self.move_base(0, 0, 0)
         self.going_to_target_pos = False
         self.threads_number -= 1
@@ -705,29 +731,31 @@
             self.arm_pos[self.arm_ID][2] = kwargs["m3"]
         if list(kwargs.keys()).count("m4") > 0:
             self.arm_pos[self.arm_ID][3] = kwargs["m4"]
         if list(kwargs.keys()).count("m5") > 0:
             self.arm_pos[self.arm_ID][4] = kwargs["m5"]
         if list(kwargs.keys()).count("grip") > 0:
             self.arm_pos[self.arm_ID][5] = kwargs["grip"]
-            self.post_to_send_data(2, bytes(f'/grip:{self.arm_ID};{self.arm_pos[self.arm_ID][5]}^^^', encoding='utf-8'))
+            self.post_to_send_data(2, bytes(f'/grip:{self.arm_ID};{round(self.arm_pos[self.arm_ID][5])}^^^',
+                                            encoding='utf-8'))
         if grip:
             self.arm_pos[self.arm_ID][5] = args[-1]
-            self.post_to_send_data(2, bytes(f'/grip:{self.arm_ID};{self.arm_pos[self.arm_ID][5]}^^^', encoding='utf-8'))
+            self.post_to_send_data(2, bytes(f'/grip:{self.arm_ID};{round(self.arm_pos[self.arm_ID][5])}^^^',
+                                            encoding='utf-8'))
 
         if list(kwargs.keys()).count("target") > 0:
             if len(kwargs["target"][0]) == 2:
                 m2, m3, m4, _ = self.solve_arm(kwargs["target"])
                 self.arm_pos[self.arm_ID][1:4] = m2, m3, m4
 
-        m1 = range_cut(11, 302, -self.arm_pos[self.arm_ID][0] + 168)
-        m2 = range_cut(3, 150, -self.arm_pos[self.arm_ID][1] + 66)
-        m3 = range_cut(-260, -15, -self.arm_pos[self.arm_ID][2] - 150)
-        m4 = range_cut(10, 195, -self.arm_pos[self.arm_ID][3] + 105)
-        m5 = range_cut(21, 292, self.arm_pos[self.arm_ID][4] + 166)
+        m1 = round(range_cut(11, 302, -self.arm_pos[self.arm_ID][0] + 168), 3)
+        m2 = round(range_cut(3, 150, -self.arm_pos[self.arm_ID][1] + 66), 3)
+        m3 = round(range_cut(-260, -15, -self.arm_pos[self.arm_ID][2] - 150), 3)
+        m4 = round(range_cut(10, 195, -self.arm_pos[self.arm_ID][3] + 105), 3)
+        m5 = round(range_cut(21, 292, self.arm_pos[self.arm_ID][4] + 166), 3)
         self.post_to_send_data(1, bytes(f'/arm:{self.arm_ID};{m1};{m2};{m3};{m4};{m5}^^^', encoding='utf-8'))
 
     def set_arm_vel(self, *args, **kwargs):
         """
         Sets arm velocities\n
         ways to set arm velocities:\n
         array of values: (joint 1, joint 2, joint 3, joint 4, joint 5)\n
@@ -751,19 +779,19 @@
         if list(kwargs.keys()).count("m3") > 0:
             self.arm_vel[self.arm_ID][2] = kwargs["m3"]
         if list(kwargs.keys()).count("m4") > 0:
             self.arm_vel[self.arm_ID][3] = kwargs["m4"]
         if list(kwargs.keys()).count("m5") > 0:
             self.arm_vel[self.arm_ID][4] = kwargs["m5"]
 
-        m1 = range_cut(-90, 90, self.arm_vel[self.arm_ID][0])
-        m2 = range_cut(-90, 90, self.arm_vel[self.arm_ID][1])
-        m3 = range_cut(-90, 90, self.arm_vel[self.arm_ID][2])
-        m4 = range_cut(-90, 90, self.arm_vel[self.arm_ID][3])
-        m5 = range_cut(-90, 90, self.arm_vel[self.arm_ID][4])
+        m1 = round(range_cut(-90, 90, self.arm_vel[self.arm_ID][0]), 3)
+        m2 = round(range_cut(-90, 90, self.arm_vel[self.arm_ID][1]), 3)
+        m3 = round(range_cut(-90, 90, self.arm_vel[self.arm_ID][2]), 3)
+        m4 = round(range_cut(-90, 90, self.arm_vel[self.arm_ID][3]), 3)
+        m5 = round(range_cut(-90, 90, self.arm_vel[self.arm_ID][4]), 3)
         self.post_to_send_data(1, bytes(f'/arm_vel:{self.arm_ID};{m1};{m2};{m3};{m4};{m5}^^^', encoding='utf-8'))
 
     # solve inverse kinetic
     def solve_arm(self, target, cartesian=False):
         """
         Solves inverse kinematics
         :param target: ((x, y), ang) to set arm position in cylindrical coordinates (ang - angle from last joint to horizon)
@@ -893,9 +921,7 @@
                 pass
 
 
 if __name__ == "__main__":
     robot = YouBot('192.168.88.21', ros=False, offline=False, camera_enable=True, advanced=False)
     print(robot.ssh.send_wait("echo 123", "root"))
     time.sleep(1)
-
-
```

### Comparing `KUKA_youbot-0.1.1/src/KUKA/SSH.py` & `KUKA_youbot-0.1.2/src/KUKA/SSH.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Rases when there is an attempt to comunicate via SSH, but no client is initialised
     """
     pass
 
 
 
 class SSH:
-    def __init__(self, /, user='youbot', ip="192.168.88.21", password=None, timeout=3, connect=True):
+    def __init__(self, /, user='youbot', ip="192.168.88.21", password=None, timeout=5, connect=True):
         """
         Connects to KUKA youbot via SSH client and starts ROS
         :param user: youbot by default
         :param ip: youbot ip address
         :param password: 111111 by default
         """
         port = 22
@@ -61,19 +61,23 @@
         init_time = time.time()
         max_time_time = time.time()
         msg = ''
         self.ssh_var.send(msg_send.encode("utf-8") + b"\n")
         while not msg.count(wait_msg):
             if self.ssh_var.recv_ready():
                 init_time = time.time()
-                read_char = self.ssh_var.recv(1).decode("utf-8")
-                if read_char != chr(0):
-                    msg += read_char
-                    if verbose:
-                        debug(read_char, end='')
+                ch = self.ssh_var.recv(1)
+                try:
+                    read_char = ch.decode("utf-8")
+                    if read_char != chr(0):
+                        msg += read_char
+                        if verbose:
+                            debug(read_char, end='')
+                except:
+                    pass
             else:
                 time.sleep(0.001)
             if time.time() - max_time_time > max_time:
                 break
             elif time.time() - init_time > timeout:
                 if timeout_msg != None:
                     debug(timeout_msg, end='')
@@ -111,23 +115,23 @@
         else:
             ROS = True
             self.last_status['ROS'] = 1
 
         if rostopic.count("camera/rgb/image_raw"):
             camera_RGB = True
             if verbose:
-                debug("RGB camera is active")
+                debug("RGB camera topic is active")
             self.last_status['RGB'] = 1
         else:
             if verbose:
                 debug("WARN: RGB camera is inactive")
             self.last_status['RGB'] = 0
         if rostopic.count("camera/depth/image"):
             if verbose:
-                debug("depth camera is active")
+                debug("depth camera topic is active")
             self.last_status['depth'] = 1
             camera_depth = True
         else:
             if verbose:
                 debug("WARN: depth camera is inactive")
             self.last_status['depth'] = 0
         if verbose == 2:
@@ -143,15 +147,15 @@
         debug("cleaning screen...")
         self.send_wait("pkill screen", "root@youbot:")
         self.send_wait("screen -S roslaunch", "root@youbot:")
         debug("launching ROS... (it may take up to 20sec)")
         ssh_msg = self.send_wait("roslaunch youbot_tl_test ytl_2arm.launch", "4rfdxc34rc3x", timeout=7, timeout_msg="",
                                  verbose=int(verbose-0.5))
         self.send_wait(chr(1) + chr(4), "root@youbot:", timeout_msg="", timeout=0.1)
-        self.send_wait("echo ZaSKaR was here", "root@youbot:", timeout_msg="SSH error, please restart", timeout=1)
+        self.send_wait("echo ZaSKaR was here", "root@youbot:", timeout_msg="SSH error, please restart\n", timeout=1)
         if ssh_msg.count("First ROS iter OK"):
             debug("ROS started\n")
         else:
             debug("ROS startup error!\nplease restart the program")
         ssh_msg = ssh_msg.split('\r')
         ssh_msg.append('')
         ros_error_msg = True
```

### Comparing `KUKA_youbot-0.1.1/src/KUKA_youbot.egg-info/PKG-INFO` & `KUKA_youbot-0.1.2/src/KUKA_youbot.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: KUKA-youbot
-Version: 0.1.1
+Version: 0.1.2
 Summary: package for easy KUKA-youbot control
 Author-email: ZaSKaR <mark.turkov@mail.ru>
 Project-URL: Homepage, https://github.com/MarkT5/YouBotKUKA
 Project-URL: Bug Tracker, https://github.com/MarkT5/YouBotKUKA/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: Framework :: Robot Framework :: Tool
-Classifier: Operating System :: OS Independent
+Project-URL: repository, https://github.com/MarkT5/YouBotKUKA
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Краткий обзор класса KUKA (Python)/(User manual):
 ____
 Класс KUKA написан для удобной работы с роботом KUKA youbot с помощью языка программирования Python. В классе есть несколько основных методов для управления роботом.
@@ -37,47 +35,58 @@
 
 ___log___ _[(str), (int)]_: [path, freq] logs odometry and lidar data to set path with set frequency
 
 ___read_from_log___ _[(str), (int)]_: [path, freq] streams odometry and lidar data from set log path with set frequency
 ___
 ## Основные Методы
 
-___move_arm(...)___ — Sets arm position\n
-        ways to set arm position:\n
-        array of values: (joint 1, joint 2, joint 3, joint 4, joint 5, grip)\n
-        
-by keywords:
+___move_arm(...)___ — Sets arm position
 
-1. ___m1, m2, m3, m4, m5___ - for joints __(all joint parameters are relative and in degrees from upright position)__
-2.    ___grip___ - (0 - 2) for grip
-3.    target - ((x, y), ang) to set arm position in cylindrical coordinates (ang - angle from last joint to horizon)
+ways to set arm position:
+
+array of values:
+- (joint 1, joint 2, joint 3, joint 4, joint 5, grip) - degrees from upright position
         
+by keywords:
+- ___m1, m2, m3, m4, m5___ - for joints __(all joint parameters are relative and in degrees from upright position)__
+- ___grip___ - (0 - 2) for grip
+     
 
 ___move_base(f, s, ang)___ — принимает:
 
 1. ___f___ — скорость движения вдоль оси по которой направлен робот, если положительное — движение вперёд, если отрицательное — назад,
 2. ___s___ — скорость движения поперёк оси по которой направлен робот
 3. ___ang___ — угловая скорость
 если вызвать этот метод без указания аргументов, то будет отправлена команда остановки
 
 ___go_to(x, y, ang)___ — отправляет робота по координатам x, y и задаёт угол от оси x до направления робота (в метрах)
 
-
-
 ___post_to_send_data(ind, msg)___ — Записывает сообщение msg в ячейку отправки ind (используется другими методами для общения с роботом, но также может использоваться для отправки пользовательских команд, если вызвана с индексом 3. 0 — скорости платформы, 1 — положения манипулятора, 2 — положение захвата)
 
 
-___arm___ (float[6]) — arm_id, joint 1 - joint 5 
+___camera/camera_BGR()___ _returns: (cv2.Mat)_- возвращает изображение в специальном сжатом формате
 
-___wheels___ (float[4]) — wheel 1 - wheel 4
+___depth_camera()___ _returns: (cv2.Mat)_ — возвращает изображение с depth камеры
 
-___lidar___ _([float[3], float[lidar_resolution]])_— возвращает массив длиной 623 с расстояниями до точек равномерно распределённых от 0 до 240 градусов и данные одометрии скрепленные с этим измерением
+### Properties:
+___arm___ _returns: float[6]_ — arm_id, joint 1 - joint 5 
 
-___increment___ _(float[3])_ — возвращает массив с положениями по оси x, y и угла от оси x до направления робота
+___wheels___ _returns: float[4]_ — wheel 1 - wheel 4
 
-___camera/camera_BGR()___ _(cv2.Mat)_- возвращает изображение в специальном сжатом формате
+___lidar___ _returns: ([float[3], float[lidar_resolution]])_— возвращает массив длиной 623 с расстояниями до точек равномерно распределённых от 0 до 240 градусов и данные одометрии скрепленные с этим измерением
 
-___depth_camera()___ _(cv2.Mat)_ — возвращает изображение с depth камеры
+___increment___ _(returns: float[3])_ — возвращает массив с положениями по оси x, y и угла от оси x до направления робота
 
 
+## SSH:
+___
+___send(msg)___ msg (string) - отправить команду через SSH
+
+___send_recv(msg)___ msg (string) - отправить команду через SSH и дождаться её завершения
+___send_wait(msg_send, wait_msg, timeout=None, timeout_msg=None, verbose=0, max_time=20):___
+- msg_send (string)- сообщение на отправку
+- wait_msg (string)- ответ, которое будет ожидаться
+- timeout (int)- максимальное время ожидания следующего ответа
+- timeout_msg (string)-сообщение, которое будет напечатано в командную строку при привышении времени ожидания
+- verbose (int)- 0-не печатать информацию, 1-печататать только важное, 2-печатать все полученные ответы
 ___
 ### подробнее - читай dock-string
```

