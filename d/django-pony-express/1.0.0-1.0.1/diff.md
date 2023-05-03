# Comparing `tmp/django-pony-express-1.0.0.tar.gz` & `tmp/django-pony-express-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pony-express-1.0.0.tar", last modified: Tue May  2 13:35:08 2023, max compression
+gzip compressed data, was "django-pony-express-1.0.1.tar", last modified: Wed May  3 13:59:39 2023, max compression
```

## Comparing `django-pony-express-1.0.0.tar` & `django-pony-express-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0     1694 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3299 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/.gitignore
--rw-r--r--   0        0        0      902 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      551 2023-05-02 10:19:39.486780 django-pony-express-1.0.0/.readthedocs.yml
--rw-r--r--   0        0        0     1088 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/LICENSE.md
--rw-r--r--   0        0        0      136 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/MANIFEST.in
--rw-r--r--   0        0        0     4291 2023-05-02 13:34:22.568180 django-pony-express-1.0.0/README.md
--rw-r--r--   0        0        0       85 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/django_pony_express/__init__.py
--rw-r--r--   0        0        0      120 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/django_pony_express/errors.py
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/django_pony_express/services/__init__.py
--rw-r--r--   0        0        0    11273 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/django_pony_express/services/base.py
--rw-r--r--   0        0        0    10121 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/django_pony_express/services/tests.py
--rw-r--r--   0        0        0      652 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/docs/Makefile
--rw-r--r--   0        0        0     2797 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/docs/conf.py
--rw-r--r--   0        0        0      167 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/docs/features/changelog.md
--rw-r--r--   0        0        0     9661 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/docs/features/mail.md
--rw-r--r--   0        0        0     5069 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/docs/features/tests.md
--rw-r--r--   0        0        0     1261 2023-05-02 12:49:25.986765 django-pony-express-1.0.0/docs/index.rst
--rwxr-xr-x   0        0        0      793 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/docs/make.bat
--rw-r--r--   0        0        0      677 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/manage.py
--rw-r--r--   0        0        0     3536 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2328 2023-05-02 10:13:55.084628 django-pony-express-1.0.0/resources/ambient_logo.svg
--rw-r--r--   0        0        0     1615 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/settings.py
--rw-r--r--   0        0        0       67 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/testapp/__init__.py
--rw-r--r--   0        0        0      145 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/testapp/templates/testapp/test_email.html
--rw-r--r--   0        0        0      148 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/testapp/templates/testapp/test_email.txt
--rw-r--r--   0        0        0      144 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/testapp/urls.py
--rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0       28 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/tests/files/testfile.txt
--rw-r--r--   0        0        0     9590 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/tests/test_email_test_service.py
--rw-r--r--   0        0        0    15614 2023-05-02 10:13:55.100253 django-pony-express-1.0.0/tests/test_mail_services.py
--rw-r--r--   0        0        0     6114 1970-01-01 00:00:00.000000 django-pony-express-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2346 2023-05-03 13:52:42.132917 django-pony-express-1.0.1/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0     1696 2023-05-03 13:52:48.910530 django-pony-express-1.0.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3299 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/.gitignore
+-rw-r--r--   0        0        0      904 2023-05-03 13:52:48.888852 django-pony-express-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      551 2023-05-03 13:52:48.888852 django-pony-express-1.0.1/.readthedocs.yml
+-rw-r--r--   0        0        0      254 2023-05-03 13:44:27.245582 django-pony-express-1.0.1/CHANGES.md
+-rw-r--r--   0        0        0     1090 2023-05-03 13:52:48.888852 django-pony-express-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0      138 2023-05-03 13:52:48.888852 django-pony-express-1.0.1/MANIFEST.in
+-rw-r--r--   0        0        0     5272 2023-05-03 13:52:48.894859 django-pony-express-1.0.1/README.md
+-rw-r--r--   0        0        0       85 2023-05-03 13:44:27.226098 django-pony-express-1.0.1/django_pony_express/__init__.py
+-rw-r--r--   0        0        0      120 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/django_pony_express/errors.py
+-rw-r--r--   0        0        0     1607 2023-05-03 13:32:01.959010 django-pony-express-1.0.1/django_pony_express/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/django_pony_express/services/__init__.py
+-rw-r--r--   0        0        0    11273 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/django_pony_express/services/base.py
+-rw-r--r--   0        0        0    10121 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/django_pony_express/services/tests.py
+-rw-r--r--   0        0        0      654 2023-05-03 13:52:48.910530 django-pony-express-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0     2819 2023-05-03 13:52:48.910530 django-pony-express-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0       33 2023-05-03 13:34:58.443495 django-pony-express-1.0.1/docs/features/changelog.rst
+-rw-r--r--   0        0        0     9661 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/docs/features/mail.md
+-rw-r--r--   0        0        0     5069 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/docs/features/tests.md
+-rw-r--r--   0        0        0      282 2023-05-03 13:49:39.022556 django-pony-express-1.0.1/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-03 13:52:48.910530 django-pony-express-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0      677 2023-05-02 10:13:55.084628 django-pony-express-1.0.1/manage.py
+-rw-r--r--   0        0        0     3575 2023-05-03 13:52:48.894859 django-pony-express-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1682 2023-05-03 13:31:21.061433 django-pony-express-1.0.1/settings.py
+-rw-r--r--   0        0        0       69 2023-05-03 13:52:48.894859 django-pony-express-1.0.1/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/testapp/__init__.py
+-rw-r--r--   0        0        0      145 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/testapp/templates/testapp/test_email.html
+-rw-r--r--   0        0        0      148 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/testapp/templates/testapp/test_email.txt
+-rw-r--r--   0        0        0      144 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/testapp/urls.py
+-rw-r--r--   0        0        0        0 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/tests/files/testfile.txt
+-rw-r--r--   0        0        0     9590 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/tests/test_email_test_service.py
+-rw-r--r--   0        0        0    15614 2023-05-02 10:13:55.100253 django-pony-express-1.0.1/tests/test_mail_services.py
+-rw-r--r--   0        0        0     7134 1970-01-01 00:00:00.000000 django-pony-express-1.0.1/PKG-INFO
```

### Comparing `django-pony-express-1.0.0/.github/workflows/ci.yml` & `django-pony-express-1.0.1/.github/workflows/ci.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,8 +56,8 @@
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install tox
         run: pip install tox
       - name: Run Tests
         env:
           TOXENV: django${{ matrix.django-version }}
-        run: tox
+        run: tox
```

### Comparing `django-pony-express-1.0.0/.gitignore` & `django-pony-express-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/.pre-commit-config.yaml` & `django-pony-express-1.0.1/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 
   - repo: https://github.com/adamchainz/django-upgrade
     rev: 1.13.0
     hooks:
       - id: django-upgrade
         args: [--target-version, "2.2"]
         language_version: python3.11
-        stages: [ push ]
+        stages: [ push ]
```

### Comparing `django-pony-express-1.0.0/.readthedocs.yml` & `django-pony-express-1.0.1/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/LICENSE.md` & `django-pony-express-1.0.1/LICENSE.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `django-pony-express-1.0.0/README.md` & `django-pony-express-1.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,43 @@
 [![pypi](https://img.shields.io/pypi/v/django-pony-express.svg)](https://pypi.python.org/pypi/django-pony-express/)
 [![Downloads](https://pepy.tech/badge/django-pony-express)](https://pepy.tech/project/django-pony-express)
 [![Documentation Status](https://readthedocs.org/projects/django-pony-express/badge/?version=latest)](https://django-pony-express.readthedocs.io/en/latest/?badge=latest)
 
-**Class-based emails including a test suite for Django**
+Welcome to the **django-pony-express** - class-based emails for Django shipping with a full test
+suite.
 
-Full documentation for the project is available at [readthedocs.io](https://django-pony-express.readthedocs.io/en/latest/index.html).
+Similar to class-based view in Django core, this package provides a neat, DRY and testable (!) way to handle your
+emails in Django.
 
-Created and maintained by [Ambient Digital](https://ambient.digital).
+* [PyPI](https://pypi.org/project/django-pony-express/)
+* [GitHub](https://github.com/ambient-innovation/django-pony-express)
+* [Full documentation](https://django-pony-express.readthedocs.io/en/latest/index.html)
+* Creator & Maintainer: [Ambient Digital](https://ambient.digital)
+
+## Features
+
+* Class-based structure for emails
+   * Avoid duplicate low-level setup
+   * Utilise inheritance and OOP benefits
+   * No duplicated templates for HTML and plain-text
+* Test suite to write proper unit-tests for your emails
+   * Access your test outbox like a Django queryset
+
+## Etymology
+
+> The Pony Express was an American express mail service that used relays of horse-mounted riders. [...] During its
+> 18 months of operation, the Pony Express reduced the time for messages to travel between the east and west US
+> coast to about 10 days.
+>
+> https://en.wikipedia.org/wiki/Pony_Express
 
----
+The name of this package combines the Django mascot (a pony) with a once quite successful mail service in the US.
+Ingenious, right?
 
-# Installation
+## Installation
 
 - Install the package via pip:
 
   `pip install django-pony-express`
 
   or via pipenv:
 
@@ -24,40 +47,40 @@
 
     ````
     INSTALLED_APPS = (
         ...
         'django_pony_express',
     )
      ````
-  
-# Contribute
 
-## Setup package for development
+## Contribute
+
+### Setup package for development
 
 - Create a Python virtualenv and activate it
 - Install "pip-tools" with `pip install pip-tools`
 - Compile the requirements with `pip-compile --extra dev -o requirements.txt pyproject.toml --resolver=backtracking`
 - Sync the dependencies with your virtualenv with `pip-sync`
 
-## Add functionality
+### Add functionality
 
 - Create a new branch for your feature
 - Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
   `-e /Users/workspace/django-pony-express` or via pip  `pip install -e /Users/workspace/django-pony-express`
 - Ensure the code passes the tests
 - Create a pull request
 
-## Run tests
+### Run tests
 
 - Run tests
   ````
   pytest --ds settings tests
   ````
 
-## Git hooks (via pre-commit)
+### Git hooks (via pre-commit)
 
 We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
 vain.
 
 To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once:
 
     pre-commit install -t pre-push -t pre-commit --install-hooks
@@ -74,43 +97,43 @@
 
     pre-commit run ruff --all-files --hook-stage push
 
 Example: run all hooks of pre-push stage
 
     pre-commit run --all-files --hook-stage push
 
-## Update documentation
+### Update documentation
 
 - To build the documentation run: `sphinx-build docs/ docs/_build/html/`.
 - Open `docs/_build/html/index.html` to see the documentation.
 
-## Translation files
+### Translation files
 
 If you have added custom text, make sure to wrap it in `_()` where `_` is
 gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
 
 How to create translation file:
 
-* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
+* Navigate to `django-pony-express` (the inner directory!)
 * `python manage.py makemessages -l de`
-* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
+* Have a look at the new/changed files within `django-pony-express/locale`
 
 How to compile translation files:
 
-* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
+* Navigate to `django-pony-express` (the inner directory!)
 * `python manage.py compilemessages`
-* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
+* Have a look at the new/changed files within `django-pony-express/locale`
 
-## Publish to ReadTheDocs.io
+### Publish to ReadTheDocs.io
 
 - Fetch the latest changes in GitHub mirror and push them
 - Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
   up.
 
-## Publish to PyPi
+### Publish to PyPi
 
 - Update documentation about new/changed functionality
 
 - Update the `Changelog`
 
 - Increment version in main `__init__.py`
 
@@ -122,8 +145,8 @@
   ```
 
   To publish to TestPyPI use the following ensure that you have set up your .pypirc as
   shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
 
   ```
   flit publish --repository testpypi
-  ```
+  ```
```

### Comparing `django-pony-express-1.0.0/django_pony_express/services/base.py` & `django-pony-express-1.0.1/django_pony_express/services/base.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/django_pony_express/services/tests.py` & `django-pony-express-1.0.1/django_pony_express/services/tests.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/docs/Makefile` & `django-pony-express-1.0.1/docs/Makefile`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
 
 .PHONY: help Makefile
 
 # Catch-all target: route all unknown targets to Sphinx using the new
 # "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
 %: Makefile
-	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
+	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
```

### Comparing `django-pony-express-1.0.0/docs/conf.py` & `django-pony-express-1.0.1/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #
 import os
 import sys
 
 import django
 from django.conf import settings
 
-sys.path.insert(0, os.path.abspath('..'))  # so that we can access the package
+sys.path.insert(0, os.path.abspath('..'))  # so that we can access the "django_pony_express" package
 settings.configure(
     INSTALLED_APPS=[
         'django.contrib.admin',
         'django.contrib.auth',
         'django.contrib.contenttypes',
         'django.contrib.sessions',
         'django.contrib.messages',
```

### Comparing `django-pony-express-1.0.0/docs/features/mail.md` & `django-pony-express-1.0.1/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/docs/features/tests.md` & `django-pony-express-1.0.1/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/docs/make.bat` & `django-pony-express-1.0.1/docs/make.bat`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -28,8 +28,8 @@
 %SPHINXBUILD% -M %1 %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 goto end
 
 :help
 %SPHINXBUILD% -M help %SOURCEDIR% %BUILDDIR% %SPHINXOPTS% %O%
 
 :end
-popd
+popd
```

### Comparing `django-pony-express-1.0.0/manage.py` & `django-pony-express-1.0.1/manage.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/pyproject.toml` & `django-pony-express-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -45,14 +45,15 @@
    'pre-commit~=3.2',
    'black~=23.3',
    'Django~=3.2',
    'sphinx==4.2.0',
    'sphinx-rtd-theme==1.0.0',
    'm2r2==0.3.1',
    'mistune<2.0.0',
+   'ambient-package-update~=23.5.1',
 ]
 
 [tool.flit.module]
 name = "django_pony_express"
 
 [project.urls]
 'Documentation' = 'https://django-pony-express.readthedocs.io/en/latest/index.html'
@@ -70,15 +71,15 @@
 [tool.ruff]
 # Enable pycodestyle (`E`) and Pyflakes (`F`) codes by default.
 select = ["E", "F", "W", "N", "I", "B", "A", "DTZ", "DJ"]
 ignore = [
     'N999', # Project name contains underscore, not fixable
     'A003', # Django attributes shadow python builtins
     'DJ001', # Django model text-based fields shouldn't be nullable
-    'B905', # Django model text-based fields shouldn't be nullable
+    'B905', # Can be enabled when Python <=3.9 support is dropped
 ]
 
 # Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable =["E", "F", "W", "N", "I", "B", "A", "DTZ", "DJ"]
 unfixable = []
 
 exclude = [
@@ -134,8 +135,8 @@
 
 [gh-actions]
 python =
     3.8: py38
     3.9: py39
     3.10: py310
     3.11: py311
-"""
+"""
```

### Comparing `django-pony-express-1.0.0/settings.py` & `django-pony-express-1.0.1/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,7 +54,9 @@
     'django.middleware.csrf.CsrfViewMiddleware',
     'django.contrib.auth.middleware.AuthenticationMiddleware',
     'django.contrib.messages.middleware.MessageMiddleware',
     'django.middleware.clickjacking.XFrameOptionsMiddleware',
 )
 
 TIME_ZONE = 'UTC'
+
+LOCALE_PATHS = [str(BASE_PATH) + '/django_pony_express/locale']
```

### Comparing `django-pony-express-1.0.0/tests/test_email_test_service.py` & `django-pony-express-1.0.1/tests/test_email_test_service.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/tests/test_mail_services.py` & `django-pony-express-1.0.1/tests/test_mail_services.py`

 * *Files identical despite different names*

### Comparing `django-pony-express-1.0.0/PKG-INFO` & `django-pony-express-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pony-express
-Version: 1.0.0
+Version: 1.0.1
 Summary: Class-based emails including a test suite for Django
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
@@ -31,33 +31,57 @@
 Requires-Dist: pre-commit~=3.2 ; extra == "dev"
 Requires-Dist: black~=23.3 ; extra == "dev"
 Requires-Dist: Django~=3.2 ; extra == "dev"
 Requires-Dist: sphinx==4.2.0 ; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.0.0 ; extra == "dev"
 Requires-Dist: m2r2==0.3.1 ; extra == "dev"
 Requires-Dist: mistune<2.0.0 ; extra == "dev"
+Requires-Dist: ambient-package-update~=23.5.1 ; extra == "dev"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/django-pony-express/issues
 Project-URL: Changelog, https://django-pony-express.readthedocs.io/en/latest/features/changelog.html
 Project-URL: Documentation, https://django-pony-express.readthedocs.io/en/latest/index.html
 Project-URL: Maintained by, https://ambient.digital/
 Provides-Extra: dev
 
 [![pypi](https://img.shields.io/pypi/v/django-pony-express.svg)](https://pypi.python.org/pypi/django-pony-express/)
 [![Downloads](https://pepy.tech/badge/django-pony-express)](https://pepy.tech/project/django-pony-express)
 [![Documentation Status](https://readthedocs.org/projects/django-pony-express/badge/?version=latest)](https://django-pony-express.readthedocs.io/en/latest/?badge=latest)
 
-**Class-based emails including a test suite for Django**
+Welcome to the **django-pony-express** - class-based emails for Django shipping with a full test
+suite.
 
-Full documentation for the project is available at [readthedocs.io](https://django-pony-express.readthedocs.io/en/latest/index.html).
+Similar to class-based view in Django core, this package provides a neat, DRY and testable (!) way to handle your
+emails in Django.
 
-Created and maintained by [Ambient Digital](https://ambient.digital).
+* [PyPI](https://pypi.org/project/django-pony-express/)
+* [GitHub](https://github.com/ambient-innovation/django-pony-express)
+* [Full documentation](https://django-pony-express.readthedocs.io/en/latest/index.html)
+* Creator & Maintainer: [Ambient Digital](https://ambient.digital)
+
+## Features
+
+* Class-based structure for emails
+   * Avoid duplicate low-level setup
+   * Utilise inheritance and OOP benefits
+   * No duplicated templates for HTML and plain-text
+* Test suite to write proper unit-tests for your emails
+   * Access your test outbox like a Django queryset
+
+## Etymology
+
+> The Pony Express was an American express mail service that used relays of horse-mounted riders. [...] During its
+> 18 months of operation, the Pony Express reduced the time for messages to travel between the east and west US
+> coast to about 10 days.
+>
+> https://en.wikipedia.org/wiki/Pony_Express
 
----
+The name of this package combines the Django mascot (a pony) with a once quite successful mail service in the US.
+Ingenious, right?
 
-# Installation
+## Installation
 
 - Install the package via pip:
 
   `pip install django-pony-express`
 
   or via pipenv:
 
@@ -67,40 +91,40 @@
 
     ````
     INSTALLED_APPS = (
         ...
         'django_pony_express',
     )
      ````
-  
-# Contribute
 
-## Setup package for development
+## Contribute
+
+### Setup package for development
 
 - Create a Python virtualenv and activate it
 - Install "pip-tools" with `pip install pip-tools`
 - Compile the requirements with `pip-compile --extra dev -o requirements.txt pyproject.toml --resolver=backtracking`
 - Sync the dependencies with your virtualenv with `pip-sync`
 
-## Add functionality
+### Add functionality
 
 - Create a new branch for your feature
 - Change the dependency in your requirements.txt to a local (editable) one that points to your local file system:
   `-e /Users/workspace/django-pony-express` or via pip  `pip install -e /Users/workspace/django-pony-express`
 - Ensure the code passes the tests
 - Create a pull request
 
-## Run tests
+### Run tests
 
 - Run tests
   ````
   pytest --ds settings tests
   ````
 
-## Git hooks (via pre-commit)
+### Git hooks (via pre-commit)
 
 We use pre-push hooks to ensure that only linted code reaches our remote repository and pipelines aren't triggered in
 vain.
 
 To enable the configured pre-push hooks, you need to [install](https://pre-commit.com/) pre-commit and run once:
 
     pre-commit install -t pre-push -t pre-commit --install-hooks
@@ -117,43 +141,43 @@
 
     pre-commit run ruff --all-files --hook-stage push
 
 Example: run all hooks of pre-push stage
 
     pre-commit run --all-files --hook-stage push
 
-## Update documentation
+### Update documentation
 
 - To build the documentation run: `sphinx-build docs/ docs/_build/html/`.
 - Open `docs/_build/html/index.html` to see the documentation.
 
-## Translation files
+### Translation files
 
 If you have added custom text, make sure to wrap it in `_()` where `_` is
 gettext_lazy (`from django.utils.translation import gettext_lazy as _`).
 
 How to create translation file:
 
-* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
+* Navigate to `django-pony-express` (the inner directory!)
 * `python manage.py makemessages -l de`
-* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
+* Have a look at the new/changed files within `django-pony-express/locale`
 
 How to compile translation files:
 
-* Navigate to `ai_django_core/ai_django_core` (the inner directory!)
+* Navigate to `django-pony-express` (the inner directory!)
 * `python manage.py compilemessages`
-* Have a look at the new/changed files within `ai_django_core/ai_django_core/locale`
+* Have a look at the new/changed files within `django-pony-express/locale`
 
-## Publish to ReadTheDocs.io
+### Publish to ReadTheDocs.io
 
 - Fetch the latest changes in GitHub mirror and push them
 - Trigger new build at ReadTheDocs.io (follow instructions in admin panel at RTD) if the GitHub webhook is not yet set
   up.
 
-## Publish to PyPi
+### Publish to PyPi
 
 - Update documentation about new/changed functionality
 
 - Update the `Changelog`
 
 - Increment version in main `__init__.py`
 
@@ -166,7 +190,8 @@
 
   To publish to TestPyPI use the following ensure that you have set up your .pypirc as
   shown [here](https://flit.readthedocs.io/en/latest/upload.html#using-pypirc) and use the following command:
 
   ```
   flit publish --repository testpypi
   ```
+
```

