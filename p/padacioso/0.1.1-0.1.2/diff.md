# Comparing `tmp/padacioso-0.1.1.tar.gz` & `tmp/padacioso-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/padacioso-0.1.1.tar", last modified: Wed Apr 28 19:07:17 2021, max compression
+gzip compressed data, was "padacioso-0.1.2.tar", last modified: Sat Aug  6 23:25:16 2022, max compression
```

## Comparing `padacioso-0.1.1.tar` & `padacioso-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-28 19:07:17.409159 padacioso-0.1.1/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2021-04-28 13:13:34.000000 padacioso-0.1.1/LICENSE.md
--rw-rw-r--   0 user      (1000) user      (1000)      252 2021-04-28 19:07:17.409159 padacioso-0.1.1/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-28 19:07:17.409159 padacioso-0.1.1/padacioso/
--rw-rw-r--   0 user      (1000) user      (1000)     2814 2021-04-28 19:04:36.000000 padacioso-0.1.1/padacioso/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5647 2021-04-28 18:02:34.000000 padacioso-0.1.1/padacioso/bracket_expansion.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-28 19:07:17.409159 padacioso-0.1.1/padacioso.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      252 2021-04-28 19:07:17.000000 padacioso-0.1.1/padacioso.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      259 2021-04-28 19:07:17.000000 padacioso-0.1.1/padacioso.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2021-04-28 19:07:17.000000 padacioso-0.1.1/padacioso.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       12 2021-04-28 19:07:17.000000 padacioso-0.1.1/padacioso.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2021-04-28 19:07:17.000000 padacioso-0.1.1/padacioso.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2021-04-28 19:07:17.409159 padacioso-0.1.1/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      335 2021-04-28 18:53:55.000000 padacioso-0.1.1/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2021-04-28 19:07:17.409159 padacioso-0.1.1/test/
--rw-rw-r--   0 user      (1000) user      (1000)     4814 2021-04-28 19:05:45.000000 padacioso-0.1.1/test/test_padacioso.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-08-06 23:25:16.358305 padacioso-0.1.2/
+-rw-r--r--   0 user      (1000) user      (1000)    11357 2022-08-06 22:34:42.000000 padacioso-0.1.2/LICENSE.md
+-rw-r--r--   0 user      (1000) user      (1000)      266 2022-08-06 23:25:16.358305 padacioso-0.1.2/PKG-INFO
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-08-06 23:25:16.358305 padacioso-0.1.2/padacioso/
+-rw-r--r--   0 user      (1000) user      (1000)     3704 2022-08-06 23:23:37.000000 padacioso-0.1.2/padacioso/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5647 2022-08-06 22:34:42.000000 padacioso-0.1.2/padacioso/bracket_expansion.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-08-06 23:25:16.358305 padacioso-0.1.2/padacioso.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      266 2022-08-06 23:25:16.000000 padacioso-0.1.2/padacioso.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      259 2022-08-06 23:25:16.000000 padacioso-0.1.2/padacioso.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2022-08-06 23:25:16.000000 padacioso-0.1.2/padacioso.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)       12 2022-08-06 23:25:16.000000 padacioso-0.1.2/padacioso.egg-info/requires.txt
+-rw-r--r--   0 user      (1000) user      (1000)       10 2022-08-06 23:25:16.000000 padacioso-0.1.2/padacioso.egg-info/top_level.txt
+-rw-r--r--   0 user      (1000) user      (1000)       38 2022-08-06 23:25:16.358305 padacioso-0.1.2/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      335 2022-08-06 23:20:30.000000 padacioso-0.1.2/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2022-08-06 23:25:16.358305 padacioso-0.1.2/test/
+-rw-r--r--   0 user      (1000) user      (1000)     6887 2022-08-06 23:22:17.000000 padacioso-0.1.2/test/test_padacioso.py
```

### Comparing `padacioso-0.1.1/LICENSE.md` & `padacioso-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `padacioso-0.1.1/padacioso/__init__.py` & `padacioso-0.1.2/padacioso/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 import simplematch
 import logging
 from padacioso.bracket_expansion import expand_parentheses
 LOG = logging.getLogger('padacioso')
 
 
 class IntentContainer:
-    def __init__(self):
+    def __init__(self, fuzz=False):
         self.intent_samples, self.entity_samples = {}, {}
         self.intents, self.entities = {}, {}
+        self.fuzz = fuzz
 
     def add_intent(self, name, lines):
         expanded = []
         for l in lines:
             expanded += expand_parentheses(l)
-        self.intent_samples[name] = expanded
+        self.intent_samples[name] = list(set(expanded))
+
+    def _get_fuzzed(self, sample):
+        fuzzed = []
+        words = sample.split(" ")
+        for idx in range(0, len(words)):
+            if "{" in words[idx] or "}" in words[idx]:
+                continue
+            new_words = list(words)
+            new_words[idx] = "*"
+            fuzzed.append(" ".join(new_words))
+        return fuzzed + [f"* {sample}", f"{sample} *"]
 
     def remove_intent(self, name):
         if name in self.intent_samples:
             del self.intent_samples[name]
 
     def add_entity(self, name, lines):
         expanded = []
@@ -64,13 +76,23 @@
                             # penalize unknown samples
                             penalty += 0.05
                     yield {"entities": entities or {},
                            "conf": 1 - penalty,
                            "name": intent_name}
                     break
 
+                if self.fuzz:
+                    penalty += 0.25
+                    for f in self._get_fuzzed(r):
+                        entities = simplematch.match(f, query, case_sensitive=False)
+                        if entities is not None:
+                            yield {"entities": entities or {},
+                                   "conf": 1 - penalty,
+                                   "name": intent_name}
+                            break
+
     def calc_intent(self, query):
         return max(
             self.calc_intents(query),
             key=lambda x: x["conf"],
             default={'name': None, 'entities': {}}
         )
```

### Comparing `padacioso-0.1.1/padacioso/bracket_expansion.py` & `padacioso-0.1.2/padacioso/bracket_expansion.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.1.1/test/test_padacioso.py` & `padacioso-0.1.2/test/test_padacioso.py`

 * *Files 20% similar despite different names*

```diff
@@ -109,7 +109,57 @@
              'entities': {'number': 3}, 'name': 'test_int'})
 
         container.add_intent('test_float', ['* float {number:float}'])
         self.assertEqual(
             container.calc_intent('i want float 3'),
             {'conf': 0.8,   # wildcard + unseen entity example
              'entities': {'number': 3.0}, 'name': 'test_float'})
+
+    def test_no_fuzz(self):
+        container = IntentContainer(fuzz=False)
+        container.add_intent('test', ['this is a test',
+                                      'test the intent',
+                                      'execute test'])
+        container.add_intent('test2', ['tell me about {thing}',
+                                       'what is {thing}'])
+        # exact match
+        intent = container.calc_intent("this is a test")
+        self.assertEqual(intent["name"], "test")
+
+        # regex match
+        intent = container.calc_intent("tell me about Mycroft")
+        self.assertEqual(intent["name"], "test2")
+        self.assertEqual(intent["entities"], {'thing': 'Mycroft'})
+
+        # fuzzy match - failure case (no fuzz)
+        intent = container.calc_intent("this is test")
+        self.assertTrue(intent["name"] is None)
+
+        # fuzzy regex match - failure case (no fuzz)
+        intent = container.calc_intent("tell me everything about Mycroft")
+        self.assertTrue(intent["name"] is None)
+
+    def test_fuzz(self):
+        container = IntentContainer(fuzz=True)
+        container.add_intent('test', ['this is a test',
+                                      'test the intent',
+                                      'execute test'])
+        container.add_intent('test2', ['tell me about {thing}',
+                                       'what is {thing}'])
+        # exact match
+        intent = container.calc_intent("this is a test")
+        self.assertEqual(intent["name"], "test")
+
+        # regex match
+        intent = container.calc_intent("tell me about Mycroft")
+        self.assertEqual(intent["name"], "test2")
+        self.assertEqual(intent["entities"], {'thing': 'Mycroft'})
+
+        # fuzzy match
+        intent = container.calc_intent("this is test")
+        self.assertEqual(intent["name"], "test")
+
+        # fuzzy regex match
+        intent = container.calc_intent("tell me everything about Mycroft")
+        self.assertEqual(intent["name"], "test2")
+        self.assertEqual(intent["entities"], {'thing': 'Mycroft'})
+
```

