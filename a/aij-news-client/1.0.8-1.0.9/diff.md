# Comparing `tmp/aij-news-client-1.0.8.tar.gz` & `tmp/aij-news-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-news-client-1.0.8.tar", last modified: Wed May  3 06:01:26 2023, max compression
+gzip compressed data, was "aij-news-client-1.0.9.tar", last modified: Wed May  3 10:07:49 2023, max compression
```

## Comparing `aij-news-client-1.0.8.tar` & `aij-news-client-1.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/
--rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-client-1.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0     4302 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-client-1.0.8/README.md
--rw-rw-rw-   0        0        0     6238 2023-05-03 06:01:12.000000 aij-news-client-1.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/aij_news_client.egg-info/
--rw-rw-rw-   0        0        0     4302 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/aij_news_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      357 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/aij_news_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/aij_news_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/aij_news_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/aij_news_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/aij_news_client.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 06:01:28.000000 aij-news-client-1.0.8/src/news_client/
--rw-rw-rw-   0        0        0      710 2023-05-03 05:53:28.000000 aij-news-client-1.0.8/src/news_client/__init__.py
--rw-rw-rw-   0        0        0      975 2023-05-03 05:54:26.000000 aij-news-client-1.0.8/src/news_client/news_consumer.py
+drwxrwxrwx   0        0        0        0 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/
+-rw-rw-rw-   0        0        0     1100 2023-05-02 19:19:00.000000 aij-news-client-1.0.9/LICENSE.txt
+-rw-rw-rw-   0        0        0     4302 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1843 2023-05-02 19:19:00.000000 aij-news-client-1.0.9/README.md
+-rw-rw-rw-   0        0        0     6238 2023-05-03 10:07:30.000000 aij-news-client-1.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/aij_news_client.egg-info/
+-rw-rw-rw-   0        0        0     4302 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/aij_news_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      357 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/aij_news_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/aij_news_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/aij_news_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/aij_news_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/aij_news_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-03 10:07:50.000000 aij-news-client-1.0.9/src/news_client/
+-rw-rw-rw-   0        0        0      710 2023-05-03 05:53:28.000000 aij-news-client-1.0.9/src/news_client/__init__.py
+-rw-rw-rw-   0        0        0     1156 2023-05-03 10:07:16.000000 aij-news-client-1.0.9/src/news_client/news_consumer.py
```

### Comparing `aij-news-client-1.0.8/LICENSE.txt` & `aij-news-client-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-news-client-1.0.8/PKG-INFO` & `aij-news-client-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI Journalist News Client package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-client-1.0.8/README.md` & `aij-news-client-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aij-news-client-1.0.8/pyproject.toml` & `aij-news-client-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-news-client"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.0.8"
+version = "1.0.9"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist News Client package"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-news-client-1.0.8/src/aij_news_client.egg-info/PKG-INFO` & `aij-news-client-1.0.9/src/aij_news_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-news-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: AI Journalist News Client package
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-news-client-1.0.8/src/news_client/__init__.py` & `aij-news-client-1.0.9/src/news_client/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-news-client-1.0.8/src/news_client/news_consumer.py` & `aij-news-client-1.0.9/src/news_client/news_consumer.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,34 @@
 
 
 class NewsConsumer:
     """
     This class implements a RabbitMQ consumer.
     """
     def __init__(self, host, callback_function):
+        """
+        This method initializes the consumer.
+        """
         self.connection = pika.BlockingConnection(pika.ConnectionParameters(host))
         self.channel = self.connection.channel()
         self.channel.queue_declare(queue='news_stream')
         self.callback_function = callback_function
 
     def consume(self):
         """
         This method starts consuming messages from the RabbitMQ queue.
         """
         self.channel.basic_consume(queue='news_stream', on_message_callback=self.callback, auto_ack=True)
         self.channel.start_consuming()
 
     def callback(self, ch, method, properties, body):
-        self.callback_function(method.routing_key, body) 
+        """
+        This method is called when a message is received from the RabbitMQ queue.
+        """
+        self.callback_function(method.routing_key, body)
 
     def destroy(self):
         """
         This method closes the connection to the RabbitMQ server.
         """
         if self.connection.is_open:
             self.connection.close()
```

