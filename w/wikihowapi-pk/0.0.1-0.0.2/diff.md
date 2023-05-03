# Comparing `tmp/wikihowapi_pk-0.0.1.tar.gz` & `tmp/wikihowapi_pk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikihowapi_pk-0.0.1.tar", last modified: Wed May  3 11:34:23 2023, max compression
+gzip compressed data, was "wikihowapi_pk-0.0.2.tar", last modified: Wed May  3 15:00:36 2023, max compression
```

## Comparing `wikihowapi_pk-0.0.1.tar` & `wikihowapi_pk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 11:34:23.204256 wikihowapi_pk-0.0.1/
--rw-r--r--   0 piko       (501) staff       (20)     1101 2023-05-03 09:56:00.000000 wikihowapi_pk-0.0.1/LICENSE
--rw-r--r--   0 piko       (501) staff       (20)     3844 2023-05-03 11:34:23.204123 wikihowapi_pk-0.0.1/PKG-INFO
--rw-r--r--   0 piko       (501) staff       (20)     3326 2023-05-03 11:30:26.000000 wikihowapi_pk-0.0.1/README.md
--rw-r--r--   0 piko       (501) staff       (20)       38 2023-05-03 11:34:23.204298 wikihowapi_pk-0.0.1/setup.cfg
--rw-r--r--   0 piko       (501) staff       (20)      791 2023-05-03 09:59:44.000000 wikihowapi_pk-0.0.1/setup.py
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 11:34:23.203309 wikihowapi_pk-0.0.1/wikihowapi_pk/
--rw-r--r--   0 piko       (501) staff       (20)    24194 2023-05-03 10:04:01.000000 wikihowapi_pk-0.0.1/wikihowapi_pk/__init__.py
--rw-r--r--   0 piko       (501) staff       (20)      194 2023-05-03 09:37:40.000000 wikihowapi_pk-0.0.1/wikihowapi_pk/exceptions.py
-drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 11:34:23.203970 wikihowapi_pk-0.0.1/wikihowapi_pk.egg-info/
--rw-r--r--   0 piko       (501) staff       (20)     3844 2023-05-03 11:34:23.000000 wikihowapi_pk-0.0.1/wikihowapi_pk.egg-info/PKG-INFO
--rw-r--r--   0 piko       (501) staff       (20)      264 2023-05-03 11:34:23.000000 wikihowapi_pk-0.0.1/wikihowapi_pk.egg-info/SOURCES.txt
--rw-r--r--   0 piko       (501) staff       (20)        1 2023-05-03 11:34:23.000000 wikihowapi_pk-0.0.1/wikihowapi_pk.egg-info/dependency_links.txt
--rw-r--r--   0 piko       (501) staff       (20)        9 2023-05-03 11:34:23.000000 wikihowapi_pk-0.0.1/wikihowapi_pk.egg-info/requires.txt
--rw-r--r--   0 piko       (501) staff       (20)       14 2023-05-03 11:34:23.000000 wikihowapi_pk-0.0.1/wikihowapi_pk.egg-info/top_level.txt
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 15:00:36.659472 wikihowapi_pk-0.0.2/
+-rw-r--r--   0 piko       (501) staff       (20)     1101 2023-05-03 09:56:00.000000 wikihowapi_pk-0.0.2/LICENSE
+-rw-r--r--   0 piko       (501) staff       (20)     3863 2023-05-03 15:00:36.659358 wikihowapi_pk-0.0.2/PKG-INFO
+-rw-r--r--   0 piko       (501) staff       (20)     3345 2023-05-03 11:59:11.000000 wikihowapi_pk-0.0.2/README.md
+-rw-r--r--   0 piko       (501) staff       (20)       38 2023-05-03 15:00:36.659505 wikihowapi_pk-0.0.2/setup.cfg
+-rw-r--r--   0 piko       (501) staff       (20)      791 2023-05-03 14:59:18.000000 wikihowapi_pk-0.0.2/setup.py
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 15:00:36.658656 wikihowapi_pk-0.0.2/wikihowapi_pk/
+-rw-r--r--   0 piko       (501) staff       (20)    25724 2023-05-03 14:57:00.000000 wikihowapi_pk-0.0.2/wikihowapi_pk/__init__.py
+-rw-r--r--   0 piko       (501) staff       (20)      194 2023-05-03 09:37:40.000000 wikihowapi_pk-0.0.2/wikihowapi_pk/exceptions.py
+drwxr-xr-x   0 piko       (501) staff       (20)        0 2023-05-03 15:00:36.659191 wikihowapi_pk-0.0.2/wikihowapi_pk.egg-info/
+-rw-r--r--   0 piko       (501) staff       (20)     3863 2023-05-03 15:00:36.000000 wikihowapi_pk-0.0.2/wikihowapi_pk.egg-info/PKG-INFO
+-rw-r--r--   0 piko       (501) staff       (20)      264 2023-05-03 15:00:36.000000 wikihowapi_pk-0.0.2/wikihowapi_pk.egg-info/SOURCES.txt
+-rw-r--r--   0 piko       (501) staff       (20)        1 2023-05-03 15:00:36.000000 wikihowapi_pk-0.0.2/wikihowapi_pk.egg-info/dependency_links.txt
+-rw-r--r--   0 piko       (501) staff       (20)        9 2023-05-03 15:00:36.000000 wikihowapi_pk-0.0.2/wikihowapi_pk.egg-info/requires.txt
+-rw-r--r--   0 piko       (501) staff       (20)       14 2023-05-03 15:00:36.000000 wikihowapi_pk-0.0.2/wikihowapi_pk.egg-info/top_level.txt
```

### Comparing `wikihowapi_pk-0.0.1/LICENSE` & `wikihowapi_pk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wikihowapi_pk-0.0.1/PKG-INFO` & `wikihowapi_pk-0.0.2/wikihowapi_pk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wikihowapi_pk
-Version: 0.0.1
+Name: wikihowapi-pk
+Version: 0.0.2
 Summary: API to extract more data from wikiHow
 Home-page: https://github.com/p1k0pan/AdaptiveStoryFinder.git
 Author: p1k0pan
 Author-email: pan.jingheng1998@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -19,23 +19,23 @@
 wikihowAPI_pk is basically base on [vigilant-umbrella/wikiHowUnofficialAPI
 ](https://github.com/vigilant-umbrella/wikiHowUnofficialAPI.git) but add more parser on it.
 
 ## New features
 
 - [x] Return map(json) format for server use
 - [x] Video Parser in Method section: each method is either one picture or video
-- [] Video Parser in section: some page would have videos after method section
-- [] Ingredients parser
-- [] Parer to show more tipps
-- [] Make `<li>` inside a Text visible after parsing
+- [ ] Video Parser in section: some page would have videos after method section
+- [ ] Ingredients parser
+- [ ] Parer to show more tipps
+- [ ] Make `<li>` inside a Text visible after parsing
 
 ## Installation
 
 ```bash
-pip install wikiHowUnofficialAPI
+pip install wikiHowUnofficialAPI, wikihowAPI-pk
 ```
 
 ## Usage
 
 ### Random HowTo
 
 Learn random stuff! Retuns a random WikiHow article URL.
```

### Comparing `wikihowapi_pk-0.0.1/README.md` & `wikihowapi_pk-0.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 wikihowAPI_pk is basically base on [vigilant-umbrella/wikiHowUnofficialAPI
 ](https://github.com/vigilant-umbrella/wikiHowUnofficialAPI.git) but add more parser on it.
 
 ## New features
 
 - [x] Return map(json) format for server use
 - [x] Video Parser in Method section: each method is either one picture or video
-- [] Video Parser in section: some page would have videos after method section
-- [] Ingredients parser
-- [] Parer to show more tipps
-- [] Make `<li>` inside a Text visible after parsing
+- [ ] Video Parser in section: some page would have videos after method section
+- [ ] Ingredients parser
+- [ ] Parer to show more tipps
+- [ ] Make `<li>` inside a Text visible after parsing
 
 ## Installation
 
 ```bash
-pip install wikiHowUnofficialAPI
+pip install wikiHowUnofficialAPI, wikihowAPI-pk
 ```
 
 ## Usage
 
 ### Random HowTo
 
 Learn random stuff! Retuns a random WikiHow article URL.
```

### Comparing `wikihowapi_pk-0.0.1/setup.py` & `wikihowapi_pk-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name='wikihowapi_pk',
-    version='0.0.1',
+    version='0.0.2',
     description='API to extract more data from wikiHow',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/p1k0pan/AdaptiveStoryFinder.git',
     author='p1k0pan',
     author_email='pan.jingheng1998@gmail.com',
     license='MIT',
```

### Comparing `wikihowapi_pk-0.0.1/wikihowapi_pk/__init__.py` & `wikihowapi_pk-0.0.2/wikihowapi_pk/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-wikiHowUnofficialAPI
+wikihowAPI_pk
 
 API to extract data from wikiHow.
 """
 
-__version__ = '0.1.1'
-__author__ = 'Aniket Sharma, Ashok Arora'
-__credits__ = 'Aniket Sharma & Ashok Arora'
+__version__ = '0.0.2'
+__author__ = 'p1k0pan'
+__credits__ = 'Aniket Sharma & Ashok Arora & p1k0pan'
 
 from bs4 import BeautifulSoup
 import urllib.request
-from wikihowunofficialapi.exceptions import *
+from wikihowapi_pk.exceptions import *
 from datetime import datetime
 import re
 
 
 class Steps:
     def __init__(self, number, title=None, description=None, picture=None):
         self._number = number
@@ -70,14 +70,32 @@
         return {
             'number': self.number,
             'title': self.title,
             'description': self.description,
             'picture': self.picture
         }
 
+class Ingredients:
+    def __init__ (self, recipe_name, recipe_stuff):
+        self._recipe_name = recipe_name
+        self._recipe_stuff = recipe_stuff
+
+    @property
+    def recipe_name(self):
+        return self._recipe_name
+
+    @property
+    def recipe_stuff(self):
+        return self._recipe_stuff
+    
+    def get(self):
+        return{
+            "recipe_name": self.recipe_name,
+            "recipe_stuff": self.recipe_stuff
+        }
 
 class Methods:
     def __init__(self, number, title):
         self._number = number
         self._title = title
         self._steps = []
 
@@ -136,14 +154,15 @@
         self._last_updated = None
         self._views = None
         self._co_authors = None
         self._references = None
         self._summary = None
         self._warnings = []
         self._tips = []
+        self._ingredients=[]
 
         self._parsed = False
         if not lazy:
             self._parse()
 
     def __repr__(self):
         return self.title
@@ -310,14 +329,55 @@
 
         Returns:
             list: Tips from a wikiHow article.
         """
         if not self._parsed:
             self._parse()
         return self._tips
+    
+    @property
+    def ingredients(self):
+
+        ingredient_list=[]
+        if not self._parsed:
+            self._parse()
+
+        for item in self._ingredients:
+            ingredient_list.append(item.get())
+        # return self._ingredients
+        return ingredient_list
+
+    def _parse(self):
+        """Method to extract useful information from a given wikiHow article.
+
+        Raises:
+            ParseError: The given article could not be parsed.
+        """
+        try:
+            content = urllib.request.urlopen(self._url)
+            read_content = content.read()
+            soup = BeautifulSoup(read_content, 'html.parser')
+            self._parse_title(soup)
+            self._parse_intro(soup)
+            self._parse_methods(soup)
+            self._parse_votes_n_helpful(soup)
+            self._parse_is_expert(soup)
+            self._parse_last_updated(soup)
+            self._parse_views(soup)
+            self._parse_co_authors(soup)
+            self._parse_references(soup)
+            self._parse_summary(soup)
+            self._parse_warnings(soup)
+            self._parse_tips(soup)
+            self._parse_ingredients(soup)
+
+            self._parsed = True
+        except Exception as e:
+            raise ParseError
+
 
     def _parse_title(self, soup):
         """Method to extract the title of a wikiHow article.
         Args:
             soup(bs4.BeautifulSoup): An instance of BeautifulSoup class for the entire article.
 
         Raises:
@@ -348,14 +408,30 @@
                     sup.decompose()
                     intro = intro_html.text
                     self._intro = intro.strip()
             else:
                 intro = intro_html.text
                 self._intro = intro.strip()
 
+    def _parse_ingredients(self, soup):
+        self._ingredients=[]
+        ingredients_html = soup.find('div', {'id': "ingredients"})
+        if not ingredients_html:
+            return
+        else:
+            recipe_tags = ingredients_html.find_all("div", {"class": "headline_container block_header in-block subheadline"})
+            for recipe in recipe_tags:
+                detail = []
+                key = recipe.find('span', {'class': 'mw-headline'}).text
+                values = recipe.find_next_sibling('ul').findAll('li')
+                for v in values:
+                    detail.append(v.text)
+                ing = Ingredients(key, detail)
+                self._ingredients.append(ing)
+
     def _parse_methods(self, soup):
         """Method to extract the methods from a wikiHow article.
         Args:
             soup(bs4.BeautifulSoup): An instance of BeautifulSoup class for the entire article.
 
         Raises:
             ParseError: The given article could not be parsed.
@@ -606,51 +682,25 @@
             else:
                 tips_html = tips_html_div.find('p')
                 if tips_html != None:
                     self._tips.append(tips_html.text)
                 else:
                     return None
 
-    def _parse(self):
-        """Method to extract useful information from a given wikiHow article.
-
-        Raises:
-            ParseError: The given article could not be parsed.
-        """
-        try:
-            content = urllib.request.urlopen(self._url)
-            read_content = content.read()
-            soup = BeautifulSoup(read_content, 'html.parser')
-            self._parse_title(soup)
-            self._parse_intro(soup)
-            self._parse_methods(soup)
-            self._parse_votes_n_helpful(soup)
-            self._parse_is_expert(soup)
-            self._parse_last_updated(soup)
-            self._parse_views(soup)
-            self._parse_co_authors(soup)
-            self._parse_references(soup)
-            self._parse_summary(soup)
-            self._parse_warnings(soup)
-            self._parse_tips(soup)
-
-            self._parsed = True
-        except Exception as e:
-            raise ParseError
-
     def get(self):
         """Method to return a dictionary of class members.
 
         Returns:
             dict: A dictionary of class members.
         """
         return {
             'url': self.url,
             'title': self.title,
             'intro': self.intro,
+            'ingredients': self.ingredients,
             'n_methods': self.n_methods,
             'methods': self.methods,
             'num_votes': self.num_votes,
             'percent_helpful': self.percent_helpful,
             'is_expert': self.is_expert,
             'last_updated': self.last_updated,
             'views': self.views,
@@ -750,7 +800,8 @@
     """
     return list(WikiHow.search(query, max_results, lang))
 
 
 if __name__ == '__main__':
     """This file can only be loaded as a module."""
     exit()
+
```

### Comparing `wikihowapi_pk-0.0.1/wikihowapi_pk.egg-info/PKG-INFO` & `wikihowapi_pk-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wikihowapi-pk
-Version: 0.0.1
+Name: wikihowapi_pk
+Version: 0.0.2
 Summary: API to extract more data from wikiHow
 Home-page: https://github.com/p1k0pan/AdaptiveStoryFinder.git
 Author: p1k0pan
 Author-email: pan.jingheng1998@gmail.com
 License: MIT
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
@@ -19,23 +19,23 @@
 wikihowAPI_pk is basically base on [vigilant-umbrella/wikiHowUnofficialAPI
 ](https://github.com/vigilant-umbrella/wikiHowUnofficialAPI.git) but add more parser on it.
 
 ## New features
 
 - [x] Return map(json) format for server use
 - [x] Video Parser in Method section: each method is either one picture or video
-- [] Video Parser in section: some page would have videos after method section
-- [] Ingredients parser
-- [] Parer to show more tipps
-- [] Make `<li>` inside a Text visible after parsing
+- [ ] Video Parser in section: some page would have videos after method section
+- [ ] Ingredients parser
+- [ ] Parer to show more tipps
+- [ ] Make `<li>` inside a Text visible after parsing
 
 ## Installation
 
 ```bash
-pip install wikiHowUnofficialAPI
+pip install wikiHowUnofficialAPI, wikihowAPI-pk
 ```
 
 ## Usage
 
 ### Random HowTo
 
 Learn random stuff! Retuns a random WikiHow article URL.
```

