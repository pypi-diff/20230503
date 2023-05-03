# Comparing `tmp/ez-parse-0.0.0.tar.gz` & `tmp/ez-parse-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ez-parse-0.0.0.tar", last modified: Wed May  3 21:06:15 2023, max compression
+gzip compressed data, was "ez-parse-0.1.1.tar", last modified: Sat Mar 25 16:04:05 2023, max compression
```

## Comparing `ez-parse-0.0.0.tar` & `ez-parse-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 shivanshsrivastava   (501) staff       (20)        0 2023-05-03 21:06:15.588554 ez-parse-0.0.0/
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      302 2023-05-03 20:57:41.000000 ez-parse-0.0.0/.bumpversion.cfg
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     1016 2023-03-25 01:04:03.000000 ez-parse-0.0.0/CONTRIBUTING.md
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     1076 2023-03-02 00:22:09.000000 ez-parse-0.0.0/LICENSE
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      395 2023-03-25 15:48:48.000000 ez-parse-0.0.0/MANIFEST.in
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     2143 2023-05-03 17:17:24.000000 ez-parse-0.0.0/Makefile
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      155 2023-05-03 21:06:15.588386 ez-parse-0.0.0/PKG-INFO
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     3052 2023-05-03 17:17:24.000000 ez-parse-0.0.0/README.md
-drwxr-xr-x   0 shivanshsrivastava   (501) staff       (20)        0 2023-05-03 21:06:15.586461 ez-parse-0.0.0/Resume-Parser/
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)       57 2023-05-03 20:57:41.000000 ez-parse-0.0.0/Resume-Parser/__init__.py
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     9289 2023-05-03 17:17:24.000000 ez-parse-0.0.0/Resume-Parser/parser.py
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)    14082 2023-05-03 17:17:24.000000 ez-parse-0.0.0/Resume-Parser/test_all.py
-drwxr-xr-x   0 shivanshsrivastava   (501) staff       (20)        0 2023-05-03 21:06:15.587445 ez-parse-0.0.0/ez_parse.egg-info/
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      155 2023-05-03 21:06:15.000000 ez-parse-0.0.0/ez_parse.egg-info/PKG-INFO
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      347 2023-05-03 21:06:15.000000 ez-parse-0.0.0/ez_parse.egg-info/SOURCES.txt
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)        1 2023-05-03 21:06:15.000000 ez-parse-0.0.0/ez_parse.egg-info/dependency_links.txt
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)        1 2023-05-03 21:06:15.000000 ez-parse-0.0.0/ez_parse.egg-info/top_level.txt
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     2205 2023-05-03 20:57:41.000000 ez-parse-0.0.0/pyproject.toml
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)       79 2023-03-25 01:18:54.000000 ez-parse-0.0.0/requirements.txt
-drwxr-xr-x   0 shivanshsrivastava   (501) staff       (20)        0 2023-05-03 21:06:15.587581 ez-parse-0.0.0/sample/
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)    48985 2023-03-25 01:04:03.000000 ez-parse-0.0.0/sample/Shivansh Srivastava.pdf
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)       38 2023-05-03 21:06:15.588746 ez-parse-0.0.0/setup.cfg
--rw-r--r--   0 shivanshsrivastava   (501) staff       (20)       54 2023-03-25 16:00:07.000000 ez-parse-0.0.0/setup.py
+drwxr-xr-x   0 shivanshsrivastava   (501) staff       (20)        0 2023-03-25 16:04:05.999363 ez-parse-0.1.1/
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      302 2023-03-25 16:01:37.000000 ez-parse-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     1016 2023-03-25 01:04:03.000000 ez-parse-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     1076 2023-03-02 00:22:09.000000 ez-parse-0.1.1/LICENSE
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      395 2023-03-25 15:48:48.000000 ez-parse-0.1.1/MANIFEST.in
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     2138 2023-03-25 15:48:48.000000 ez-parse-0.1.1/Makefile
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     3653 2023-03-25 16:04:05.999182 ez-parse-0.1.1/PKG-INFO
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     1550 2023-03-25 15:41:10.000000 ez-parse-0.1.1/README.md
+drwxr-xr-x   0 shivanshsrivastava   (501) staff       (20)        0 2023-03-25 16:04:05.997352 ez-parse-0.1.1/Resume-Parser/
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)       57 2023-03-25 16:01:37.000000 ez-parse-0.1.1/Resume-Parser/__init__.py
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     4388 2023-03-25 15:48:48.000000 ez-parse-0.1.1/Resume-Parser/parser.py
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)    10411 2023-03-25 15:48:48.000000 ez-parse-0.1.1/Resume-Parser/test_all.py
+drwxr-xr-x   0 shivanshsrivastava   (501) staff       (20)        0 2023-03-25 16:04:05.998227 ez-parse-0.1.1/ez_parse.egg-info/
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     3653 2023-03-25 16:04:05.000000 ez-parse-0.1.1/ez_parse.egg-info/PKG-INFO
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      378 2023-03-25 16:04:05.000000 ez-parse-0.1.1/ez_parse.egg-info/SOURCES.txt
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)        1 2023-03-25 16:04:05.000000 ez-parse-0.1.1/ez_parse.egg-info/dependency_links.txt
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)      175 2023-03-25 16:04:05.000000 ez-parse-0.1.1/ez_parse.egg-info/requires.txt
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)        7 2023-03-25 16:04:05.000000 ez-parse-0.1.1/ez_parse.egg-info/top_level.txt
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)     2205 2023-03-25 16:01:37.000000 ez-parse-0.1.1/pyproject.toml
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)       79 2023-03-25 01:18:54.000000 ez-parse-0.1.1/requirements.txt
+drwxr-xr-x   0 shivanshsrivastava   (501) staff       (20)        0 2023-03-25 16:04:05.998371 ez-parse-0.1.1/sample/
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)    48985 2023-03-25 01:04:03.000000 ez-parse-0.1.1/sample/Shivansh Srivastava.pdf
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)       38 2023-03-25 16:04:05.999412 ez-parse-0.1.1/setup.cfg
+-rw-r--r--   0 shivanshsrivastava   (501) staff       (20)       54 2023-03-25 16:00:07.000000 ez-parse-0.1.1/setup.py
```

### Comparing `ez-parse-0.0.0/CONTRIBUTING.md` & `ez-parse-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ez-parse-0.0.0/LICENSE` & `ez-parse-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ez-parse-0.0.0/Makefile` & `ez-parse-0.1.1/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 	python -m pip install .
 
 #########
 # LINTS #
 #########
 lint:  ## run static analysis with black and flake8
 	python -m black --check Resume-Parser setup.py
-	python -m flake8 Resume-Parser setup.py --ignore=E501,F401,F841
+	python -m flake8 Resume-Parser setup.py --ignore=E501,F401
 
 # Alias
 lints: lint
 
 format:  ## run autoformatting with black
 	python -m black Resume-Parser/ setup.py
```

### Comparing `ez-parse-0.0.0/Resume-Parser/test_all.py` & `ez-parse-0.1.1/Resume-Parser/test_all.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,16 @@
-import json
 from parser import (
     extract_pdf,
     get_contact,
     get_skills,
     get_certifications,
     get_honors,
     get_summary,
     get_languages,
     get_many,
-    get_json,
 )
 
 
 def test_get_contact():
     li = ["999-999-9999", "Email", "URL", "Top Skills"]
     res = {"contact": ["999-999-9999", "Email", "URL"]}
     assert get_contact(li, -1)[0] == res["contact"]
@@ -298,130 +296,14 @@
         ],
         "summary": [
             "Hi, I'm Shivansh! I'm a senior at Columbia Engineering studying computer science. I'm interested in AI/ML, computer vision, and NLP. Feel free to reach out to me at ss5945@columbia.edu."
         ],
     }
 
 
-def test_get_json():
-    li = [
-        "Contact",
-        "5202620535 ",
-        "ss5945@columbia.edu",
-        "",
-        "www.linkedin.com/in/shivansh-",
-        "srivastava-cs001 ",
-        "",
-        "Top Skills",
-        "Public Speaking",
-        "Python (Programming Language)",
-        "HTML",
-        "",
-        "Languages",
-        "Hindi (Native or Bilingual)",
-        "English (Native or Bilingual)",
-        "Spanish (Professional Working)",
-        "",
-        "Certifications",
-        "Gold Seal of Biliteracy in Spanish",
-        "Software Engineering Virtual",
-        "Experience",
-        "",
-        "Honors-Awards",
-        "Gold Seal of Bilteracy",
-        "SARSEF Grand Award",
-        "Excellence in Engineering",
-        "Scholarship",
-        "2019 Coca-Cola Scholar Semifinalist",
-        "Columbia Computer Science",
-        "Emerging Scholar of 2020",
-        "",
-        "Publications",
-        "India: Facts, Faith and Festivals",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "Shivansh Srivastava",
-        "",
-        "SWE Intern @ Meta (Facebook) | CS @ Columbia",
-        "New York City Metropolitan Area",
-        "",
-        "Summary",
-        "Hi, I'm Shivansh! I'm a senior at Columbia Engineering studying",
-        "computer science. I'm interested in AI/ML, computer vision, and NLP.",
-        "Feel free to reach out to me at ss5945@columbia.edu.",
-        "",
-        "Experience",
-        "",
-        "Meta",
-        "Software Engineer",
-        "May 2022-Present(11 months)",
-        "Menlo Park, California, United States",
-        "Integrity Observation Platform",
-        "",
-        "Columbia Build Lab",
-        "Vice President of Community",
-        "February 2021-Present(2 years 2 months)",
-        "New York City Metropolitan Area",
-        "- Interview and match 30+ MBA startup founders with 50+ \
-            undergrad and",
-        "graduate SWE, PD, and PM interns each semester",
-        "- Manage a semester budget of $144k to pay student interns \
-            and organize",
-        "workshops and networking events",
-        "- Work with the Eugene M. Lang Entrepreneurship Center and \
-            the CS",
-        "Department to design academic guidelines for students",
-        "",
-        "Skye",
-        "Software Engineer",
-        "February 2021-May 2022(1 year 4 months)",
-        "New York City Metropolitan Area",
-        "- Develop a full-stack web application for professional \
-            coaching services",
-        "- Implement Firebase back-end infrastructure for the React \
-            web app’s server to",
-        "reduce costs",
-        "- Design a novel matching algorithm to match 80+ clients to \
-            their personalized",
-        "coaches",
-        "- Clean data from 6700+ schools in the U.S. to train the matching \
-            algorithm on",
-        "",
-        "Page 1 of 2",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "",
-        "Education",
-        "Columbia University in the City of New York",
-        "Bachelor of Science - BS,Computer Science(2019-2023)",
-        "",
-        "Catalina Foothills High School",
-        "Honors Diploma(2015-2019)",
-        "",
-        "Page 2 of 2",
-        "",
-        "",
-    ]
-    res = get_json(li)
-    try:
-        json.loads(res)
-    except ValueError as err:
-        assert False
-    assert True
-
-
 def test_integrated():
     li = extract_pdf('sample/Shivansh Srivastava.pdf')
     res = get_many(li)
 
     assert res == {
         "contact": [
             "5202620535",
@@ -448,18 +330,7 @@
             "Columbia Computer Science",
             "Emerging Scholar of 2020",
         ],
         "summary": [
             "Hi, I'm Shivansh! I'm a senior at Columbia Engineering studying computer science. I'm interested in AI/ML, computer vision, and NLP. Feel free to reach out to me at ss5945@columbia.edu."
         ],
     }
-
-
-def test_integrated_json():
-    li = extract_pdf('sample/Shivansh Srivastava.pdf')
-    res = get_json(li)
-
-    try:
-        json.loads(res)
-    except ValueError as err:
-        assert False
-    assert True
```

### Comparing `ez-parse-0.0.0/pyproject.toml` & `ez-parse-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "ez-parse"
 authors = [{name = "Shivansh Srivastava", email = "ss5945@columbia.edu"}]
 description="A Python library for parsing PDFs of LinkedIn profiles"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.1"
 requires-python = ">=3.7"
 
 dependencies = [
     "pdfminer>=20191125",
 ]
 
 classifiers = [
```

### Comparing `ez-parse-0.0.0/sample/Shivansh Srivastava.pdf` & `ez-parse-0.1.1/sample/Shivansh Srivastava.pdf`

 * *Files identical despite different names*

