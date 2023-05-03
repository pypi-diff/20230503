# Comparing `tmp/spkrepo-0.2.2.tar.gz` & `tmp/spkrepo-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spkrepo-0.2.2.tar", max compression
+gzip compressed data, was "spkrepo-0.2.3.tar", max compression
```

## Comparing `spkrepo-0.2.2.tar` & `spkrepo-0.2.3.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0     1081 2022-03-12 21:08:18.295587 spkrepo-0.2.2/LICENSE
--rw-r--r--   0        0        0     3310 2022-03-12 21:08:18.295587 spkrepo-0.2.2/README.md
--rw-r--r--   0        0        0     2018 2022-03-12 21:08:18.299587 spkrepo-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      241 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/__init__.py
--rw-r--r--   0        0        0     2425 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/app.py
--rw-r--r--   0        0        0      972 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/config.py
--rw-r--r--   0        0        0      275 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/exceptions.py
--rw-r--r--   0        0        0      448 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/ext.py
--rw-r--r--   0        0        0    17387 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/models.py
--rw-r--r--   0        0        0   114012 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/css/bootstrap.min.css
--rw-r--r--   0        0        0      922 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/css/spkrepo.css
--rw-r--r--   0        0        0    20335 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0        0        0    62927 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0        0        0    41280 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0        0        0    23320 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0        0        0    34654 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/js/bootstrap.min.js
--rw-r--r--   0        0        0     2637 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/js/html5shiv.min.js
--rw-r--r--   0        0        0    84245 2022-03-12 21:08:18.299587 spkrepo-0.2.2/spkrepo/static/js/jquery-2.1.1.min.js
--rw-r--r--   0        0        0     6150 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/static/js/jquery.dotdotdot.min.js
--rw-r--r--   0        0        0     4378 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/static/js/respond.min.js
--rw-r--r--   0        0        0       67 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/static/js/spkrepo.js
--rw-r--r--   0        0        0     5441 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/_wtfhelpers.html
--rw-r--r--   0        0        0       28 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/base.html
--rw-r--r--   0        0        0      193 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/frontend/index.html
--rw-r--r--   0        0        0     1923 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/frontend/package.html
--rw-r--r--   0        0        0     1028 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/frontend/packages.html
--rw-r--r--   0        0        0      833 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/frontend/profile.html
--rw-r--r--   0        0        0     4394 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/layout.html
--rw-r--r--   0        0        0      202 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/security/change_password.html
--rw-r--r--   0        0        0      219 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/security/forgot_password.html
--rw-r--r--   0        0        0      271 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/security/login_user.html
--rw-r--r--   0        0        0      219 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/security/register_user.html
--rw-r--r--   0        0        0      200 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/security/reset_password.html
--rw-r--r--   0        0        0      221 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/templates/security/send_confirmation.html
--rw-r--r--   0        0        0      403 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/tests/__init__.py
--rw-r--r--   0        0        0    27594 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/tests/common.py
--rw-r--r--   0        0        0    12841 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/tests/test_admin.py
--rw-r--r--   0        0        0    17458 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/tests/test_api.py
--rw-r--r--   0        0        0     6135 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/tests/test_frontend.py
--rw-r--r--   0        0        0    25238 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/tests/test_nas.py
--rw-r--r--   0        0        0    14636 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/tests/test_utils.py
--rw-r--r--   0        0        0    15606 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/utils.py
--rw-r--r--   0        0        0      286 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/views/__init__.py
--rw-r--r--   0        0        0    25454 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/views/admin.py
--rw-r--r--   0        0        0    11116 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/views/api.py
--rw-r--r--   0        0        0     3341 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/views/frontend.py
--rw-r--r--   0        0        0     8310 2022-03-12 21:08:18.303588 spkrepo-0.2.2/spkrepo/views/nas.py
--rw-r--r--   0        0        0     5045 2022-03-12 21:09:31.375174 spkrepo-0.2.2/setup.py
--rw-r--r--   0        0        0     5586 2022-03-12 21:09:31.375678 spkrepo-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-03 16:42:04.523543 spkrepo-0.2.3/LICENSE
+-rw-r--r--   0        0        0     3357 2023-05-03 16:42:04.523543 spkrepo-0.2.3/README.md
+-rw-r--r--   0        0        0     2077 2023-05-03 16:42:04.523543 spkrepo-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      241 2023-05-03 16:42:04.523543 spkrepo-0.2.3/spkrepo/__init__.py
+-rw-r--r--   0        0        0     2425 2023-05-03 16:42:04.523543 spkrepo-0.2.3/spkrepo/app.py
+-rw-r--r--   0        0        0      972 2023-05-03 16:42:04.523543 spkrepo-0.2.3/spkrepo/config.py
+-rw-r--r--   0        0        0      275 2023-05-03 16:42:04.523543 spkrepo-0.2.3/spkrepo/exceptions.py
+-rw-r--r--   0        0        0      448 2023-05-03 16:42:04.523543 spkrepo-0.2.3/spkrepo/ext.py
+-rw-r--r--   0        0        0    17685 2023-05-03 16:42:04.523543 spkrepo-0.2.3/spkrepo/models.py
+-rw-r--r--   0        0        0   114012 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/css/bootstrap.min.css
+-rw-r--r--   0        0        0      922 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/css/spkrepo.css
+-rw-r--r--   0        0        0    20335 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0        0        0    62927 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0        0        0    41280 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0        0        0    23320 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0        0        0    34654 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/js/bootstrap.min.js
+-rw-r--r--   0        0        0     2637 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/js/html5shiv.min.js
+-rw-r--r--   0        0        0    84245 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/js/jquery-2.1.1.min.js
+-rw-r--r--   0        0        0     6150 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/js/jquery.dotdotdot.min.js
+-rw-r--r--   0        0        0     4378 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/js/respond.min.js
+-rw-r--r--   0        0        0       67 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/static/js/spkrepo.js
+-rw-r--r--   0        0        0     5441 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/templates/_wtfhelpers.html
+-rw-r--r--   0        0        0       28 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/templates/base.html
+-rw-r--r--   0        0        0      193 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/templates/frontend/index.html
+-rw-r--r--   0        0        0     1977 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/templates/frontend/package.html
+-rw-r--r--   0        0        0     1028 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/templates/frontend/packages.html
+-rw-r--r--   0        0        0      833 2023-05-03 16:42:04.527543 spkrepo-0.2.3/spkrepo/templates/frontend/profile.html
+-rw-r--r--   0        0        0     4394 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/templates/layout.html
+-rw-r--r--   0        0        0      202 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/templates/security/change_password.html
+-rw-r--r--   0        0        0      219 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/templates/security/forgot_password.html
+-rw-r--r--   0        0        0      294 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/templates/security/login_user.html
+-rw-r--r--   0        0        0      219 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/templates/security/register_user.html
+-rw-r--r--   0        0        0      200 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/templates/security/reset_password.html
+-rw-r--r--   0        0        0      221 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/templates/security/send_confirmation.html
+-rw-r--r--   0        0        0      403 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/tests/__init__.py
+-rw-r--r--   0        0        0    27658 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/tests/common.py
+-rw-r--r--   0        0        0    12841 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/tests/test_admin.py
+-rw-r--r--   0        0        0    17458 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/tests/test_api.py
+-rw-r--r--   0        0        0     6135 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/tests/test_frontend.py
+-rw-r--r--   0        0        0    25238 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/tests/test_nas.py
+-rw-r--r--   0        0        0    14636 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/tests/test_utils.py
+-rw-r--r--   0        0        0    15606 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/utils.py
+-rw-r--r--   0        0        0      286 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/views/__init__.py
+-rw-r--r--   0        0        0    25454 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/views/admin.py
+-rw-r--r--   0        0        0    11146 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/views/api.py
+-rw-r--r--   0        0        0     3368 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/views/frontend.py
+-rw-r--r--   0        0        0     8310 2023-05-03 16:42:04.531543 spkrepo-0.2.3/spkrepo/views/nas.py
+-rw-r--r--   0        0        0     5805 1970-01-01 00:00:00.000000 spkrepo-0.2.3/PKG-INFO
```

### Comparing `spkrepo-0.2.2/LICENSE` & `spkrepo-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/README.md` & `spkrepo-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 [![Discord](https://img.shields.io/discord/732558169863225384?color=7289DA&label=Discord&logo=Discord&logoColor=white&style=for-the-badge)](https://discord.gg/nnN9fgE7EF)
 
 
 ## Development
 ### Installation
 1. Install dependencies with `poetry install`
 2. Run the next commands in the virtual environment `poetry shell`
-3. Create the tables with `python manage.py db create`
-4. Populate the database with some fake packages with `python manage.py db populate`
+3. Create the tables with `python manage.py create`
+4. Populate the database with some fake packages with `python manage.py populate`
 5. Add an user with `python manage.py user create -u Admin -e admin@admin.adm -p adminadmin`
-6. Grant the created user with Administrator permissions `python manage.py user add_role -u admin@admin.adm -r admin`
-7. Grant the created user with Package Administrator permissions `python manage.py user add_role -u admin@admin.adm -r package_admin`
-8. Grant the created user with Developer permissions `python manage.py user add_role -u admin@admin.adm -r developer`
+6. Grant the created user with Administrator permissions `python manage.py roles add admin@admin.adm admin`
+7. Grant the created user with Package Administrator permissions `python manage.py roles add admin@admin.adm package_admin`
+8. Grant the created user with Developer permissions `python manage.py roles add admin@admin.adm developer`
 
 To reset the environment, clean up with `python manage.py clean`.
 
 ### Run
-1. Start the development server with `python manage.py runserver`
+1. Start the development server with `python manage.py run`
 2. Website is available at http://localhost:5000
 3. Admin interface is available at http://localhost:5000/admin
 4. NAS interface is available at http://localhost:5000/nas
 5. API is available at http://localhost:5000/api
 6. Run the test suite with `poetry run pytest -v`
 
 ## Docker Compose Run
@@ -75,7 +75,14 @@
 ### Serve app via [a WSGI server](https://flask.palletsprojects.com/en/1.1.x/deploying/).
 Example:
 
 ```bash
 pip install gunicorn
 SPKREPO_CONFIG="$PWD/config.py" gunicorn -w 4 'wsgi:app'
 ```
+
+## Add migration
+
+```
+cd migrations/
+alembic revision -m "update build path length"
+```
```

### Comparing `spkrepo-0.2.2/pyproject.toml` & `spkrepo-0.2.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spkrepo"
-version = "0.2.2"
+version = "0.2.3"
 description = "Synology Package Repository"
 license = "MIT"
 authors = ["Antoine Bertin <diaoulael@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/SynoCommunity/spkrepo"
 keywords = ["synology", "package", "repository"]
 homepage = "https://synocommunity.com"
@@ -20,43 +20,44 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
     "Topic :: System :: Archiving :: Packaging",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-flask = "^2.0.0"
+python = "^3.9"
+flask = "^2.2.0"
 flask-sqlalchemy = "^2.4.1"
-flask-security = "^3.0.0"
 passlib = "^1.7.2"
 flask-babelex = "^0.9.4"
 flask-wtf = "^1.0.0"
-wtforms = "^2.3.3"
+wtforms = "^3.0.1"
 flask-mail = "^0.9.1"
 configparser = "^5.0.0"
 email_validator = "^1.1.1"
 flask-principal = "^0.4.0"
 flask-admin = "^1.5.6"
 sqlalchemy = "^1.3.17"
-pillow = "^ 8.3.2"
+pillow = "^8.3.2"
 flask-restful = "^0.3.8"
-flask-login = "^0.5.0"
+flask-login = "^0.6.0"
 flask-caching = "^1.8.0"
 redis = "^4.1.0"
 python-gnupg = "^0.4.6"
 requests = "^2.23.0"
 click = "^8.0.0"
 flask-migrate = "^3.0.0"
 alembic = "^1.4.2"
-flask-script = "^2.0.6"
 text-unidecode = "^1.3"
 ipaddress = "^1.0.23"
 flask-debugtoolbar = "^0.11.0"
 bcrypt = "^3.1.7"
+Flask-CLI = "^0.4.0"
+Flask-Security-Too = {extras = ["common", "fsqla"], version = "^5.0.2"}
+Flask = "^2.2.2"
 
 [tool.poetry.dev-dependencies]
 sphinx = "^3.0.3"
 sphinx-rtd-theme = "^0.4.3"
 flask-testing = "^0.8.0"
 factory-boy = "^2.12.0"
 faker = "^4.1.0"
```

### Comparing `spkrepo-0.2.2/spkrepo/app.py` & `spkrepo-0.2.3/spkrepo/app.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/config.py` & `spkrepo-0.2.3/spkrepo/config.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/models.py` & `spkrepo-0.2.3/spkrepo/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     # Columns
     id = db.Column(db.Integer, primary_key=True)
     username = db.Column(db.Unicode(50), unique=True, nullable=False)
     email = db.Column(db.Unicode(254), unique=True, nullable=False)
     password = db.Column(db.Unicode(255), nullable=False)
     api_key = db.Column(db.Unicode(64), unique=True)
     github_access_token = db.Column(db.Unicode(255))
+    fs_uniquifier = db.Column(db.String(255), unique=True, nullable=False)
     active = db.Column(db.Boolean(), nullable=False)
     confirmed_at = db.Column(db.DateTime())
 
     # Relationships
     roles = db.relationship(
         "Role", secondary="user_role", back_populates="users", lazy=False
     )
@@ -439,14 +440,18 @@
     def beta(self):
         return self.report_url != None  # noqa: E711
 
     @hybrid_property
     def all_builds_active(self):
         return all(b.active for b in self.builds)
 
+    @hybrid_property
+    def any_builds_active(self):
+        return any(b.active for b in self.builds)
+
     @all_builds_active.expression
     def all_builds_active(cls):
         return (
             db.select([db.func.count()])
             .where(db.and_(Build.version_id == cls.id, Build.active))
             .label("active_builds")
         ) == (
@@ -527,14 +532,18 @@
         secondary="package_user_maintainer",
         back_populates="maintained_packages",
     )
 
     # Constraints
     __table_args__ = (db.UniqueConstraint(name),)
 
+    @hybrid_property
+    def any_builds_active(self):
+        return any(v.any_builds_active for v in self.versions)
+
     @classmethod
     def find(cls, name):
         return cls.query.filter(cls.name == name).first()
 
     def __str__(self):
         return self.name
```

### Comparing `spkrepo-0.2.2/spkrepo/static/css/bootstrap.min.css` & `spkrepo-0.2.3/spkrepo/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/css/spkrepo.css` & `spkrepo-0.2.3/spkrepo/static/css/spkrepo.css`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/fonts/glyphicons-halflings-regular.eot` & `spkrepo-0.2.3/spkrepo/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/fonts/glyphicons-halflings-regular.svg` & `spkrepo-0.2.3/spkrepo/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/fonts/glyphicons-halflings-regular.ttf` & `spkrepo-0.2.3/spkrepo/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/fonts/glyphicons-halflings-regular.woff` & `spkrepo-0.2.3/spkrepo/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/js/bootstrap.min.js` & `spkrepo-0.2.3/spkrepo/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/js/html5shiv.min.js` & `spkrepo-0.2.3/spkrepo/static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/js/jquery-2.1.1.min.js` & `spkrepo-0.2.3/spkrepo/static/js/jquery-2.1.1.min.js`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/js/jquery.dotdotdot.min.js` & `spkrepo-0.2.3/spkrepo/static/js/jquery.dotdotdot.min.js`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/static/js/respond.min.js` & `spkrepo-0.2.3/spkrepo/static/js/respond.min.js`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/templates/_wtfhelpers.html` & `spkrepo-0.2.3/spkrepo/templates/_wtfhelpers.html`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/templates/frontend/package.html` & `spkrepo-0.2.3/spkrepo/templates/frontend/package.html`

 * *Files 6% similar despite different names*

```diff
@@ -30,17 +30,19 @@
           <!-- Group firmware by DSM or SRM if 1.x -->
           {% if version == '1' %}
           SRM {{ version }}.x:
           {% else %}
           DSM {{ version }}.x:
           {% endif %}
           {% for build in builds %}
+          {% if build.active %}
           {% for arch in build.architectures %}
           <a href="{{ url_for('nas.data', path=build.path) }}"><span class="label label-default">{{ build.firmware.version }} {{ arch.code }}</span></a>
           {% endfor %}
+          {% endif %}
           {% endfor %}
           <br/>
           {% endfor %}
         </dd>
       </dl>
       {% endfor %}
     </div>
```

#### html2text {}

```diff
@@ -12,13 +12,14 @@
   Version {{ version.version_string | safe }}
       {{ version.changelog | safe }}
   Date
       {{ version.insert_date }}
   Architectures
       {% for (version, builds) in version.builds_per_dsm.items() %}  {% if
       version == '1' %} SRM {{ version }}.x: {% else %} DSM {{ version }}.x: {%
-      endif %} {% for build in builds %} {% for arch in build.architectures %}
-      {{_build.firmware.version_}}_{{_arch.code_}} {% endfor %} {% endfor %}
+      endif %} {% for build in builds %} {% if build.active %} {% for arch in
+      build.architectures %} {{_build.firmware.version_}}_{{_arch.code_}} {%
+      endfor %} {% endif %} {% endfor %}
       {% endfor %}
 {% endfor %}
 /div>
 {% endblock %}
```

### Comparing `spkrepo-0.2.2/spkrepo/templates/frontend/packages.html` & `spkrepo-0.2.3/spkrepo/templates/frontend/packages.html`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/templates/frontend/profile.html` & `spkrepo-0.2.3/spkrepo/templates/frontend/profile.html`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/templates/layout.html` & `spkrepo-0.2.3/spkrepo/templates/layout.html`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/tests/common.py` & `spkrepo-0.2.3/spkrepo/tests/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 
     id = factory.Sequence(lambda n: n)
     username = factory.LazyAttribute(lambda x: fake.user_name())
     email = factory.LazyAttribute(lambda x: fake.email())
     password = factory.LazyAttribute(lambda x: fake.password())
     api_key = factory.LazyAttribute(lambda x: fake.md5())
     github_access_token = None
+    fs_uniquifier = factory.LazyAttribute(lambda x: fake.md5())
     active = True
     confirmed_at = datetime.datetime.now()
 
 
 class IconFactory(SQLAlchemyModelFactory):
     class Meta:
         sqlalchemy_session = db.session
```

### Comparing `spkrepo-0.2.2/spkrepo/tests/test_admin.py` & `spkrepo-0.2.3/spkrepo/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/tests/test_api.py` & `spkrepo-0.2.3/spkrepo/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/tests/test_frontend.py` & `spkrepo-0.2.3/spkrepo/tests/test_frontend.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/tests/test_nas.py` & `spkrepo-0.2.3/spkrepo/tests/test_nas.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/tests/test_utils.py` & `spkrepo-0.2.3/spkrepo/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/utils.py` & `spkrepo-0.2.3/spkrepo/utils.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/views/admin.py` & `spkrepo-0.2.3/spkrepo/views/admin.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/spkrepo/views/api.py` & `spkrepo-0.2.3/spkrepo/views/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,23 +246,23 @@
         if current_app.config["GNUPG_PATH"] is not None:  # pragma: no cover
             try:
                 spk.sign(
                     current_app.config["GNUPG_TIMESTAMP_URL"],
                     current_app.config["GNUPG_PATH"],
                 )
             except SPKSignError as e:
-                abort(500, message="Failed to sign package", details=e.message)
+                abort(500, message="Failed to sign package", details=str(e))
 
         # save files
         try:
             data_path = current_app.config["DATA_PATH"]
             if create_package:
-                os.mkdir(os.path.join(data_path, package.name))
+                os.makedirs(os.path.join(data_path, package.name), exist_ok=True)
             if create_version:
-                os.mkdir(os.path.join(data_path, package.name, str(version.version)))
+                os.makedirs(os.path.join(data_path, package.name, str(version.version)), exist_ok=True)
                 for size, icon in build.version.icons.items():
                     icon.save(spk.icons[size])
             build.save(spk.stream)
         except Exception as e:  # pragma: no cover
             if create_package:
                 shutil.rmtree(os.path.join(data_path, package.name), ignore_errors=True)
             elif create_version:
@@ -271,15 +271,15 @@
                     ignore_errors=True,
                 )
             else:
                 try:
                     os.remove(os.path.join(data_path, build.path))
                 except OSError:
                     pass
-            abort(500, message="Failed to save files", details=e.message)
+            abort(500, message="Failed to save files", details=str(e))
 
         # insert the package into database
         db.session.add(build)
         db.session.commit()
 
         # success
         return (
```

### Comparing `spkrepo-0.2.2/spkrepo/views/frontend.py` & `spkrepo-0.2.3/spkrepo/views/frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,17 @@
         .all()
     )
     return render_template("frontend/packages.html", versions=versions)
 
 
 @frontend.route("/package/<name>")
 def package(name):
-    # TODO: show only packages with at least a version and an active build
+    # show only packages with at least a version and an active build
     package = Package.query.filter_by(name=name).first()
-    if package is None:
+    if package is None or not package.any_builds_active:
         abort(404)
     return render_template("frontend/package.html", package=package)
 
 
 def unique_user_username(form, field):
     if user_datastore.find_user(username=field.data) is not None:
         raise ValidationError("Username already taken")
```

### Comparing `spkrepo-0.2.2/spkrepo/views/nas.py` & `spkrepo-0.2.3/spkrepo/views/nas.py`

 * *Files identical despite different names*

### Comparing `spkrepo-0.2.2/PKG-INFO` & `spkrepo-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,84 +1,87 @@
 Metadata-Version: 2.1
 Name: spkrepo
-Version: 0.2.2
+Version: 0.2.3
 Summary: Synology Package Repository
 Home-page: https://synocommunity.com
 License: MIT
 Keywords: synology,package,repository
 Author: Antoine Bertin
 Author-email: diaoulael@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: System :: Archiving :: Packaging
+Requires-Dist: Flask (>=2.2.2,<3.0.0)
+Requires-Dist: Flask-CLI (>=0.4.0,<0.5.0)
+Requires-Dist: Flask-Security-Too[common,fsqla] (>=5.0.2,<6.0.0)
 Requires-Dist: alembic (>=1.4.2,<2.0.0)
 Requires-Dist: bcrypt (>=3.1.7,<4.0.0)
 Requires-Dist: click (>=8.0.0,<9.0.0)
 Requires-Dist: configparser (>=5.0.0,<6.0.0)
 Requires-Dist: email_validator (>=1.1.1,<2.0.0)
-Requires-Dist: flask (>=2.0.0,<3.0.0)
+Requires-Dist: flask (>=2.2.0,<3.0.0)
 Requires-Dist: flask-admin (>=1.5.6,<2.0.0)
 Requires-Dist: flask-babelex (>=0.9.4,<0.10.0)
 Requires-Dist: flask-caching (>=1.8.0,<2.0.0)
 Requires-Dist: flask-debugtoolbar (>=0.11.0,<0.12.0)
-Requires-Dist: flask-login (>=0.5.0,<0.6.0)
+Requires-Dist: flask-login (>=0.6.0,<0.7.0)
 Requires-Dist: flask-mail (>=0.9.1,<0.10.0)
 Requires-Dist: flask-migrate (>=3.0.0,<4.0.0)
 Requires-Dist: flask-principal (>=0.4.0,<0.5.0)
 Requires-Dist: flask-restful (>=0.3.8,<0.4.0)
-Requires-Dist: flask-script (>=2.0.6,<3.0.0)
-Requires-Dist: flask-security (>=3.0.0,<4.0.0)
 Requires-Dist: flask-sqlalchemy (>=2.4.1,<3.0.0)
 Requires-Dist: flask-wtf (>=1.0.0,<2.0.0)
 Requires-Dist: ipaddress (>=1.0.23,<2.0.0)
 Requires-Dist: passlib (>=1.7.2,<2.0.0)
-Requires-Dist: pillow
+Requires-Dist: pillow (>=8.3.2,<9.0.0)
 Requires-Dist: python-gnupg (>=0.4.6,<0.5.0)
 Requires-Dist: redis (>=4.1.0,<5.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.3.17,<2.0.0)
 Requires-Dist: text-unidecode (>=1.3,<2.0)
-Requires-Dist: wtforms (>=2.3.3,<3.0.0)
+Requires-Dist: wtforms (>=3.0.1,<4.0.0)
 Project-URL: Repository, https://github.com/SynoCommunity/spkrepo
 Description-Content-Type: text/markdown
 
 # spkrepo
 Synology Package Repository
 
 ![Build](https://img.shields.io/github/workflow/status/SynoCommunity/spkrepo/Build?style=for-the-badge)
 [![Discord](https://img.shields.io/discord/732558169863225384?color=7289DA&label=Discord&logo=Discord&logoColor=white&style=for-the-badge)](https://discord.gg/nnN9fgE7EF)
 
 
 ## Development
 ### Installation
 1. Install dependencies with `poetry install`
 2. Run the next commands in the virtual environment `poetry shell`
-3. Create the tables with `python manage.py db create`
-4. Populate the database with some fake packages with `python manage.py db populate`
+3. Create the tables with `python manage.py create`
+4. Populate the database with some fake packages with `python manage.py populate`
 5. Add an user with `python manage.py user create -u Admin -e admin@admin.adm -p adminadmin`
-6. Grant the created user with Administrator permissions `python manage.py user add_role -u admin@admin.adm -r admin`
-7. Grant the created user with Package Administrator permissions `python manage.py user add_role -u admin@admin.adm -r package_admin`
-8. Grant the created user with Developer permissions `python manage.py user add_role -u admin@admin.adm -r developer`
+6. Grant the created user with Administrator permissions `python manage.py roles add admin@admin.adm admin`
+7. Grant the created user with Package Administrator permissions `python manage.py roles add admin@admin.adm package_admin`
+8. Grant the created user with Developer permissions `python manage.py roles add admin@admin.adm developer`
 
 To reset the environment, clean up with `python manage.py clean`.
 
 ### Run
-1. Start the development server with `python manage.py runserver`
+1. Start the development server with `python manage.py run`
 2. Website is available at http://localhost:5000
 3. Admin interface is available at http://localhost:5000/admin
 4. NAS interface is available at http://localhost:5000/nas
 5. API is available at http://localhost:5000/api
 6. Run the test suite with `poetry run pytest -v`
 
 ## Docker Compose Run
@@ -131,7 +134,14 @@
 Example:
 
 ```bash
 pip install gunicorn
 SPKREPO_CONFIG="$PWD/config.py" gunicorn -w 4 'wsgi:app'
 ```
 
+## Add migration
+
+```
+cd migrations/
+alembic revision -m "update build path length"
+```
+
```

