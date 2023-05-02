# Comparing `tmp/djangocms-simple-admin-style-0.3.1.tar.gz` & `tmp/djangocms-simple-admin-style-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-simple-admin-style-0.3.1.tar", last modified: Tue May  2 10:21:21 2023, max compression
+gzip compressed data, was "djangocms-simple-admin-style-0.4.0.tar", last modified: Tue May  2 22:02:57 2023, max compression
```

## Comparing `djangocms-simple-admin-style-0.3.1.tar` & `djangocms-simple-admin-style-0.4.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.383315 djangocms-simple-admin-style-0.3.1/
--rw-r--r--   0 fsbraun    (501) staff       (20)     1479 2023-04-30 16:44:00.000000 djangocms-simple-admin-style-0.3.1/LICENSE
--rw-r--r--   0 fsbraun    (501) staff       (20)      218 2023-04-30 14:54:14.000000 djangocms-simple-admin-style-0.3.1/MANIFEST.in
--rw-r--r--   0 fsbraun    (501) staff       (20)     4244 2023-05-02 10:21:21.383393 djangocms-simple-admin-style-0.3.1/PKG-INFO
--rw-r--r--   0 fsbraun    (501) staff       (20)     2354 2023-05-02 07:52:30.000000 djangocms-simple-admin-style-0.3.1/README.rst
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.381301 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/
--rw-r--r--   0 fsbraun    (501) staff       (20)       22 2023-05-02 08:30:51.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/__init__.py
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.379922 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/static/
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.379972 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.382619 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/
--rw-r--r--   0 fsbraun    (501) staff       (20)     7096 2023-05-02 10:20:05.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.min.css
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.380091 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/templates/
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.382982 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/templates/admin/
--rw-r--r--   0 fsbraun    (501) staff       (20)      594 2023-05-02 07:50:11.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/templates/admin/base_site.html
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.383217 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/templates/admin/inc/
--rw-r--r--   0 fsbraun    (501) staff       (20)        0 2023-05-02 07:48:40.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/templates/admin/inc/extrastyle.html
-drwxr-xr-x   0 fsbraun    (501) staff       (20)        0 2023-05-02 10:21:21.382460 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/
--rw-r--r--   0 fsbraun    (501) staff       (20)     4244 2023-05-02 10:21:21.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/PKG-INFO
--rw-r--r--   0 fsbraun    (501) staff       (20)      625 2023-05-02 10:21:21.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/SOURCES.txt
--rw-r--r--   0 fsbraun    (501) staff       (20)        1 2023-05-02 10:21:21.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/dependency_links.txt
--rw-r--r--   0 fsbraun    (501) staff       (20)        1 2023-04-30 14:56:39.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/not-zip-safe
--rw-r--r--   0 fsbraun    (501) staff       (20)       11 2023-05-02 10:21:21.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/requires.txt
--rw-r--r--   0 fsbraun    (501) staff       (20)       29 2023-05-02 10:21:21.000000 djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/top_level.txt
--rw-r--r--   0 fsbraun    (501) staff       (20)      559 2023-05-02 10:21:21.383670 djangocms-simple-admin-style-0.3.1/setup.cfg
--rw-r--r--   0 fsbraun    (501) staff       (20)     2309 2023-04-30 16:49:33.000000 djangocms-simple-admin-style-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.116835 djangocms-simple-admin-style-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-05-02 22:02:39.000000 djangocms-simple-admin-style-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-02 22:02:39.000000 djangocms-simple-admin-style-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-02 22:02:57.116835 djangocms-simple-admin-style-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-02 22:02:39.000000 djangocms-simple-admin-style-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.116835 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 22:02:39.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.112835 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.112835 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.116835 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-05-02 22:02:39.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.112835 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.116835 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/templates/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-02 22:02:39.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/templates/admin/base_site.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.116835 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/templates/admin/inc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:39.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/templates/admin/inc/extrastyle.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 22:02:57.116835 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-02 22:02:57.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-02 22:02:57.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:02:57.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 22:02:56.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 22:02:57.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 22:02:57.000000 djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-02 22:02:57.120835 djangocms-simple-admin-style-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-02 22:02:39.000000 djangocms-simple-admin-style-0.4.0/setup.py
```

### Comparing `djangocms-simple-admin-style-0.3.1/LICENSE` & `djangocms-simple-admin-style-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.3.1/PKG-INFO` & `djangocms-simple-admin-style-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-simple-admin-style
-Version: 0.3.1
+Version: 0.4.0
 Summary: Adds pretty CSS styles for the django CMS admin interface.
 Home-page: https://github.com/fsbraun/djangocms-simple-admin-style
 Author: Fabian Braun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -89,15 +89,15 @@
 Contributions are highly welcome! Install the development environment by typing
 
 .. code-block::
 
     nvm use
     npm install
 
-Changes are made in the `private/djangocms-simple-admin.css` file. Minify the file using `. ./build` command.
+Changes are made in the `private/djangocms-simple-admin.css` file. Minify the file using `. ./minify-css` command.
 
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-simple-admin-style.svg
     :target: http://badge.fury.io/py/djangocms-simple-admin-style
 .. |django| image:: https://img.shields.io/badge/django-2.2%2B-blue.svg
     :target: https://www.djangoproject.com/
 .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.6%2B-blue.svg
```

### Comparing `djangocms-simple-admin-style-0.3.1/README.rst` & `djangocms-simple-admin-style-0.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 Contributions are highly welcome! Install the development environment by typing
 
 .. code-block::
 
     nvm use
     npm install
 
-Changes are made in the `private/djangocms-simple-admin.css` file. Minify the file using `. ./build` command.
+Changes are made in the `private/djangocms-simple-admin.css` file. Minify the file using `. ./minify-css` command.
 
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-simple-admin-style.svg
     :target: http://badge.fury.io/py/djangocms-simple-admin-style
 .. |django| image:: https://img.shields.io/badge/django-2.2%2B-blue.svg
     :target: https://www.djangoproject.com/
 .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.6%2B-blue.svg
```

### Comparing `djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.min.css` & `djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/static/djangocms_simple_admin_style/css/djangocms-simple-admin.min.css`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-:root,body{--font-family-primary:Helvetica,Arial,sans-serif;--primary:var(--dca-primary);--secondary:var(--dca-white);--accent:var(--primary);--primary-fg:var(--dca-white);--body-fg:var(--dca-gray-darkest);--body-bg:var(--dca-white);--header-color:var(--dca-black);--header-branding-color:var(--accent);--header-bg:var(--secondary);--header-link-color:var(--body-fg);--breadcrumbs-fg:var(--dca-gray);--breadcrumbs-link-fg:var(--dca-primary);--breadcrumbs-bg:var(--dca-gray-lightest);--link-fg:var(--dca-primary);--darkened-bg:var(--dca-gray-lightest);--button-fg:var(--dca-gray-darker);--button-bg:var(--dca-white);--button-hover-bg:var(--dca-gray-lighter);--default-button-fg:var(--dca-white);--default-button-bg:var(--dca-primary);--object-tools-fg:var(--body-fg);--object-tools-bg:vaR(--dca-white);--object-tools-hover-bg:var(--dca-gray-lighter)}:root[data-color-scheme=light],:root[data-theme=light],html,html[data-color-scheme=light],html[data-theme=light],root{--dca-light-mode:1;--dca-dark-mode:0;--dca-white:#fff;--dca-black:#000;--dca-primary:#0bf;--dca-gray:#666;--dca-gray-lightest:#f2f2f2;--dca-gray-lighter:#ddd;--dca-gray-light:#999;--dca-gray-darker:#454545;--dca-gray-darkest:#333;--dca-gray-super-lightest:#f7f7f7;color-scheme:light}@media (prefers-color-scheme:dark){:root{--dca-light-mode:0;--dca-dark-mode:1;--dca-white:#2a2c2e;--dca-black:#fff;--dca-primary:#58d1fc;--dca-gray:#999;--dca-gray-lightest:#444;--dca-gray-lighter:#666;--dca-gray-light:#888;--dca-gray-darker:#aaa;--dca-gray-darkest:#eee;--dca-gray-super-lightest:#333;--active-brightness:2;--focus-brightness:1.5;color-scheme:dark}}:root[data-theme=dark],html[data-color-scheme=dark],html[data-theme=dark],root[data-color-scheme=dark]{--dca-light-mode:0;--dca-dark-mode:1;--dca-white:#2a2c2e;--dca-black:#fff;--dca-primary:#58d1fc;--dca-gray:#999;--dca-gray-lightest:#444;--dca-gray-lighter:#666;--dca-gray-light:#888;--dca-gray-darker:#aaa;--dca-gray-darkest:#eee;--dca-gray-super-lightest:#333;--active-brightness:2;--focus-brightness:1.5;color-scheme:dark}.dashboard #content{width:calc(100% - 340px)}h1{font-size:1.4rem}h2{font-size:1.25rem}h3{font-size:1rem}.inline-group h2,.module caption,h4,td,th{font-size:.875rem}.help,.small,div.help,div.help li,form div.help,form p.help,h5,p.help{font-size:.75rem}.mini{font-size:.6815rem}dd,dt,li{font-size:.875rem;line-height:1.4rem}.inline-group h2,.module caption,.module h2{background:var(--body-bg);color:var(--body-fg)}#nav-sidebar .module caption{background:var(--primary)}#nav-sidebar .current-app .section:link,#nav-sidebar .current-app .section:visited,#nav-sidebar .section:link,#nav-sidebar .section:visited{color:var(--dca-white)}#nav-sidebar a{color:var(--body-fg)}.submit-row{background:var(--dca-white,#fff)}.button.default,.submit-row a.deletelink,.submit-row input.default,input[type=submit].default{color:var(--dca-white,#fff)}.object-tools a{border:1px solid var(--dca-gray-lighter);border-radius:3px}.object-tools a.addlink{background-color:var(--default-button-bg);border-color:var(--default-button-fg);color:var(--default-button-fg)}.object-tools a.addlink:focus,.object-tools a.addlink:hover{background-color:var(--default-button-hover-bg)}body.djangocms-simple-admin-style #page_form_lang_tabs input[type=button].language_button.selected{background-color:var(--default-button-bg);border-color:var(--default-button-bg);color:var(--default-button-fg)}th{font-weight:400}.aligned label,.inline-group h2,.module caption,.module h2{font-weight:600}.aligned label{color:var(--body-fg);display:block;float:unset;width:unset}.aligned .fieldBox>label:first-child,.flex-container,.form-row>div>label{display:block}.required label:not(.vCheckboxLabel):after,label.required:not(.vCheckboxLabel):after{color:var(--delete-button-bg);content:"*"}form .aligned div.help,form .aligned p.help{margin-left:0;padding-left:0}form button{background-color:var(--default-button-bg);border:1px solid var(--default-button-bg);border-radius:3px;color:var(--default-button-fg);font-family:var(--font-family-primary);font-size:.8125rem;font-weight:400;margin:2px 0;padding:5px 6px;vertical-align:middle}.aligned label+div.help,.aligned label+div.readonly,.aligned label+p,form .aligned input+div.help,form .aligned input+p.help,form .aligned select+div.help,form .aligned select+p.help,form .aligned textarea+div.help,form .aligned textarea+p.help{margin-left:0}.button,.submit-row input,a.btn,a.button,input[type=button],input[type=submit]{border:1px solid var(--dca-gray-lighter,#ddd)}a.btn{color:var(--body-fg)}.colM .aligned .vLargeTextField,.colM .aligned .vXMLLargeTextField,.flex-container textarea,.vLargeTextField,.vTextField,.vURLField,.vUUIDField,.vXMLLargeTextField,input[type=text]{width:calc(100% - 10px)}#changelist-search input[type=text]{width:unset}.form-row p,form .button,input,select,textarea{font-family:unset}div.form-row{display:flex;flex:1 0 0}.form-row>div{max-width:100%;width:100%}fieldset.collapse.collapsed .form-row{display:none}.select2{width:calc(100% - 40px)!important}.flex-container .related-widget-wrapper,.flex-container .select2-container,.flex-container select{width:100%}.related-widget-wrappxer select{width:calc(100% - 92px)}.colMS .aligned .vLargeTextField,.colMS .aligned .vXMLLargeTextField{width:unset}body.cms-admin a.skip-to-content-link,body.cms-admin-modal #header,body.cms-admin-sideframe #header{display:none}body.cms-admin-sideframe #container{padding-top:46px}body.cms-admin-sideframe #content>h1{display:none}body.cms-admin-modal .content{margin-top:36px}body.cms-admin-modal #nav-sidebar,body.cms-admin-modal #toggle-nav-sidebar,body.cms-admin-modal .breadcrumbs{display:none}body.cms-admin-sideframe.djangocms-simple-admin-style{margin-top:0}.djangocms-simple-admin-style .parler-language-tabs span.current{background-color:var(--primary);border-color:var(--primary);color:var(--dca-white)}.djangocms-simple-admin-style .parler-language-tabs span.available,.djangocms-simple-admin-style .parler-language-tabs span.current,.djangocms-simple-admin-style .parler-language-tabs span.empty{border-radius:3px 3px 0 0}.djangocms-simple-admin-style .parler-language-tabs{border-bottom-color:var(--primary)}.parler-language-tabs a:link,.parler-language-tabs a:visited{color:var(--body-fg)}#page_form_lang_tabs{border-bottom:2px solid var(--primary)}#page_form_lang_tabs input[type=button]{border-bottom:none;border-radius:3px 3px 0 0;margin-bottom:0;padding:5px 15px}.cms-btn-group{border:1px solid var(--dca-gray-lighter,#ddd);border-radius:0;line-height:15px;margin-left:-5px;margin-right:0;padding:10px 15px}.cms-btn,.cms-btn-group{background:var(--button-bg);color:var(--button-fg);display:inline-block}.cms-btn{border:1px solid var(--dca-gray-lighter,#ddd);border-radius:4px;margin-left:5px}a.cms-btn-group,a.cms-btn-group:hover,a.cms-btn-group:link{color:var(--button-fg)}.cms-btn-group:first-child{border-bottom-left-radius:4px;border-top-left-radius:4px;margin-left:5px}.cms-btn-group:last-child{border-bottom-right-radius:4px;border-top-right-radius:4px}.cms-btn-active{background-color:var(--dca-gray-lighter)}
+:root,body{--font-family-primary:Helvetica,Arial,sans-serif;--primary:var(--dca-primary);--secondary:var(--dca-white);--accent:var(--primary);--primary-fg:var(--dca-white);--body-fg:var(--dca-gray-darkest);--body-bg:var(--dca-white);--header-color:var(--dca-black);--header-branding-color:var(--accent);--header-bg:var(--secondary);--header-link-color:var(--body-fg);--breadcrumbs-fg:var(--dca-gray);--breadcrumbs-link-fg:var(--dca-primary);--breadcrumbs-bg:var(--dca-gray-lightest);--link-fg:var(--dca-primary);--darkened-bg:var(--dca-gray-lightest);--button-fg:var(--dca-gray-darker);--button-bg:var(--dca-white);--button-hover-bg:var(--dca-gray-lighter);--default-button-fg:var(--dca-white);--default-button-bg:var(--dca-primary);--object-tools-fg:var(--body-fg);--object-tools-bg:vaR(--dca-white);--object-tools-hover-bg:var(--dca-gray-lighter)}:root[data-color-scheme=light],:root[data-theme=light],html,html[data-color-scheme=light],html[data-theme=light],root{--dca-light-mode:1;--dca-dark-mode:0;--dca-white:#fff;--dca-black:#000;--dca-primary:#0bf;--dca-gray:#666;--dca-gray-lightest:#f2f2f2;--dca-gray-lighter:#ddd;--dca-gray-light:#999;--dca-gray-darker:#454545;--dca-gray-darkest:#333;--dca-gray-super-lightest:#f7f7f7;color-scheme:light}@media (prefers-color-scheme:dark){:root{--dca-light-mode:0;--dca-dark-mode:1;--dca-white:#2a2c2e;--dca-black:#fff;--dca-primary:#58d1fc;--dca-gray:#999;--dca-gray-lightest:#444;--dca-gray-lighter:#666;--dca-gray-light:#888;--dca-gray-darker:#aaa;--dca-gray-darkest:#eee;--dca-gray-super-lightest:#333;--active-brightness:2;--focus-brightness:1.5;color-scheme:dark}}:root[data-theme=dark],html[data-color-scheme=dark],html[data-theme=dark],root[data-color-scheme=dark]{--dca-light-mode:0;--dca-dark-mode:1;--dca-white:#2a2c2e;--dca-black:#fff;--dca-primary:#58d1fc;--dca-gray:#999;--dca-gray-lightest:#444;--dca-gray-lighter:#666;--dca-gray-light:#888;--dca-gray-darker:#aaa;--dca-gray-darkest:#eee;--dca-gray-super-lightest:#333;--active-brightness:2;--focus-brightness:1.5;color-scheme:dark}.dashboard #content{width:calc(100% - 340px)}h1{font-size:1.4rem}h2{font-size:1.25rem}h3{font-size:1rem}.inline-group h2,.module caption,h4,td,th{font-size:.875rem}.help,.small,div.help,div.help li,form div.help,form p.help,h5,p.help{font-size:.75rem}.mini{font-size:.6815rem}dd,dt,li{font-size:.875rem;line-height:1.4rem}.inline-group h2,.module caption,.module h2{background:var(--body-bg);color:var(--body-fg)}#nav-sidebar .module caption{background:var(--primary)}#nav-sidebar .current-app .section:link,#nav-sidebar .current-app .section:visited,#nav-sidebar .section:link,#nav-sidebar .section:visited{color:var(--dca-white)}#nav-sidebar a{color:var(--body-fg)}.submit-row{background:var(--dca-white,#fff)}.button.default,.submit-row a.deletelink,.submit-row input.default,input[type=submit].default{color:var(--dca-white,#fff)}.object-tools a{border:1px solid var(--dca-gray-lighter);border-radius:3px}.object-tools a.addlink{background-color:var(--default-button-bg);border-color:var(--default-button-fg);color:var(--default-button-fg)}.object-tools a.addlink:focus,.object-tools a.addlink:hover{background-color:var(--default-button-hover-bg)}th{font-weight:400}.inline-group h2,.module caption,.module h2{font-weight:600}.aligned label:not(.btn){color:var(--body-fg);float:unset;font-weight:600;width:unset}.aligned label.btn{display:inline-block}#user-tools #logout-form button,#user-tools a:link,#user-tools a:visited{color:var(--primary)}#logout-form button:active,#logout-form button:hover{margin-bottom:2px;padding-bottom:1px}.aligned .fieldBox>label:first-child,.flex-container,.form-row>div>label{display:block}.required label:not(.vCheckboxLabel):after,label.required:not(.vCheckboxLabel):after{color:var(--delete-button-bg);content:"*"}form .aligned div.help,form .aligned p.help{margin-left:0;padding-left:0}form button{background-color:var(--default-button-bg);border:1px solid var(--default-button-bg);border-radius:3px;color:var(--default-button-fg);font-family:var(--font-family-primary);font-size:.8125rem;font-weight:400;margin:2px 0;padding:5px 6px;vertical-align:middle}.aligned label+div.help,.aligned label+div.readonly,.aligned label+p,form .aligned input+div.help,form .aligned input+p.help,form .aligned select+div.help,form .aligned select+p.help,form .aligned textarea+div.help,form .aligned textarea+p.help{margin-left:0}.button,.submit-row input,a.btn,a.button,input[type=button],input[type=submit]{border:1px solid var(--dca-gray-lighter,#ddd)}a.btn{color:var(--body-fg)}.colM .aligned .vLargeTextField,.colM .aligned .vXMLLargeTextField,.flex-container textarea,.vLargeTextField,.vTextField,.vURLField,.vUUIDField,.vXMLLargeTextField,input[type=email],input[type=text],input[type=url]{width:calc(100% - 10px)}#changelist-search input[type=text]{width:unset}.form-row p,form .button,input,select,textarea{font-family:unset}div.form-row{display:flex;flex-wrap:wrap}.form-row>div{flex:1 0 0;min-width:463px;width:100%}fieldset.collapse.collapsed .form-row{display:none}.select2{width:calc(100% - 92px)!important}.flex-container .related-widget-wrapper,.flex-container .select2-container,.flex-container select{width:100%}select[multiple]{min-width:200px}.related-widget-wrappxer select{width:calc(100% - 92px)}.colMS .aligned .vLargeTextField,.colMS .aligned .vXMLLargeTextField{width:unset}body.cms-admin a.skip-to-content-link,body.cms-admin-modal #header,body.cms-admin-sideframe #header{display:none}body.cms-admin-sideframe #container{padding-top:46px}body.cms-admin-sideframe #content>h1{display:none}body.cms-admin-modal .content{margin-top:36px}body.cms-admin-modal #nav-sidebar,body.cms-admin-modal #toggle-nav-sidebar,body.cms-admin-modal .breadcrumbs{display:none}body.cms-admin-sideframe.djangocms-simple-admin-style{margin-top:0}.djangocms-simple-admin-style .parler-language-tabs span.current{background-color:var(--primary);border-color:var(--primary);color:var(--dca-white)}.djangocms-simple-admin-style .parler-language-tabs span.available,.djangocms-simple-admin-style .parler-language-tabs span.current,.djangocms-simple-admin-style .parler-language-tabs span.empty{border-radius:3px 3px 0 0}.djangocms-simple-admin-style .parler-language-tabs{border-bottom-color:var(--primary)}.parler-language-tabs a:link,.parler-language-tabs a:visited{color:var(--body-fg)}#page_form_lang_tabs{border-bottom:2px solid var(--primary)}#page_form_lang_tabs input[type=button]{border-bottom:none;border-radius:3px 3px 0 0;margin-bottom:0;padding:5px 15px}.djangocms-simple-admin-style #page_form_lang_tabs input[type=button].language_button.selected{background-color:var(--default-button-bg);border-color:var(--default-button-bg);color:var(--default-button-fg)}.cms-btn-group{border:1px solid var(--dca-gray-lighter,#ddd);border-radius:0;line-height:15px;margin-left:-5px;margin-right:0;padding:10px 15px}.cms-btn,.cms-btn-group{background:var(--button-bg);color:var(--button-fg);display:inline-block}.cms-btn{border:1px solid var(--dca-gray-lighter,#ddd);border-radius:4px;margin-left:5px}a.cms-btn-group,a.cms-btn-group:hover,a.cms-btn-group:link{color:var(--button-fg)}.cms-btn-group:first-child{border-bottom-left-radius:4px;border-top-left-radius:4px;margin-left:5px}.cms-btn-group:last-child{border-bottom-right-radius:4px;border-top-right-radius:4px}.cms-btn-active{background-color:var(--dca-gray-lighter)}.delete-confirmation form .cancel-link,.delete-confirmation form input[type=submit]{color:var(--dca-white)}
```

### Comparing `djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style/templates/admin/base_site.html` & `djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style/templates/admin/base_site.html`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/PKG-INFO` & `djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-simple-admin-style
-Version: 0.3.1
+Version: 0.4.0
 Summary: Adds pretty CSS styles for the django CMS admin interface.
 Home-page: https://github.com/fsbraun/djangocms-simple-admin-style
 Author: Fabian Braun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
@@ -89,15 +89,15 @@
 Contributions are highly welcome! Install the development environment by typing
 
 .. code-block::
 
     nvm use
     npm install
 
-Changes are made in the `private/djangocms-simple-admin.css` file. Minify the file using `. ./build` command.
+Changes are made in the `private/djangocms-simple-admin.css` file. Minify the file using `. ./minify-css` command.
 
 
 .. |pypi| image:: https://badge.fury.io/py/djangocms-simple-admin-style.svg
     :target: http://badge.fury.io/py/djangocms-simple-admin-style
 .. |django| image:: https://img.shields.io/badge/django-2.2%2B-blue.svg
     :target: https://www.djangoproject.com/
 .. |djangocms| image:: https://img.shields.io/badge/django%20CMS-3.6%2B-blue.svg
```

### Comparing `djangocms-simple-admin-style-0.3.1/djangocms_simple_admin_style.egg-info/SOURCES.txt` & `djangocms-simple-admin-style-0.4.0/djangocms_simple_admin_style.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.3.1/setup.cfg` & `djangocms-simple-admin-style-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangocms-simple-admin-style-0.3.1/setup.py` & `djangocms-simple-admin-style-0.4.0/setup.py`

 * *Files identical despite different names*

