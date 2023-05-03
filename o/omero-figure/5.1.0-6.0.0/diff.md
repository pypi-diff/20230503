# Comparing `tmp/omero-figure-5.1.0.tar.gz` & `tmp/omero-figure-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-figure-5.1.0.tar", last modified: Wed Nov 30 14:18:09 2022, max compression
+gzip compressed data, was "omero-figure-6.0.0.tar", last modified: Wed May  3 13:29:57 2023, max compression
```

## Comparing `omero-figure-5.1.0.tar` & `omero-figure-6.0.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (122)    34520 2022-11-30 14:17:52.000000 omero-figure-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       68 2022-11-30 14:17:52.000000 omero-figure-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     8550 2022-11-30 14:18:09.340944 omero-figure-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     7402 2022-11-30 14:17:52.000000 omero-figure-5.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/
--rw-r--r--   0 runner    (1001) docker     (122)       57 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (122)      235 2022-11-30 14:17:57.000000 omero-figure-5.1.0/omero_figure/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      864 2022-11-30 14:17:57.000000 omero-figure-5.1.0/omero_figure/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 runner    (1001) docker     (122)      972 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     1561 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/omeroutils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.328944 omero-figure-5.1.0/omero_figure/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.328944 omero-figure-5.1.0/omero_figure/scripts/omero/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/scripts/omero/figure_scripts/
--rw-r--r--   0 runner    (1001) docker     (122)    92749 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1073 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.328944 omero-figure-5.1.0/omero_figure/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/static/figure/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (122)    59497 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/backbone-1.0.0.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/
--rwxr-xr-x   0 runner    (1001) docker     (122)      769 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md
--rwxr-xr-x   0 runner    (1001) docker     (122)     2032 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.328944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/
--rw-r--r--   0 runner    (1001) docker     (122)   119892 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (122)    97339 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (122)    14079 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot
--rwxr-xr-x   0 runner    (1001) docker     (122)    63157 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg
--rwxr-xr-x   0 runner    (1001) docker     (122)    29512 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf
--rwxr-xr-x   0 runner    (1001) docker     (122)    16448 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/
--rw-r--r--   0 runner    (1001) docker     (122)    58458 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (122)    27427 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.328944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/
--rwxr-xr-x   0 runner    (1001) docker     (122)     4143 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css
--rwxr-xr-x   0 runner    (1001) docker     (122)     3487 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.328944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/
--rwxr-xr-x   0 runner    (1001) docker     (122)     3635 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png
--rwxr-xr-x   0 runner    (1001) docker     (122)     3271 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png
--rwxr-xr-x   0 runner    (1001) docker     (122)     2837 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png
--rwxr-xr-x   0 runner    (1001) docker     (122)     2972 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png
--rwxr-xr-x   0 runner    (1001) docker     (122)     8817 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/
--rw-r--r--   0 runner    (1001) docker     (122)    40582 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js
--rw-r--r--   0 runner    (1001) docker     (122)    17189 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/
--rw-r--r--   0 runner    (1001) docker     (122)    95786 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/
--rw-r--r--   0 runner    (1001) docker     (122)      819 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css
--rw-r--r--   0 runner    (1001) docker     (122)     1313 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css
--rw-r--r--   0 runner    (1001) docker     (122)   228478 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js
--rw-r--r--   0 runner    (1001) docker     (122)    17348 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/json2.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/
--rw-r--r--   0 runner    (1001) docker     (122)    53802 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js
--rw-r--r--   0 runner    (1001) docker     (122)    16798 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/
--rwxr-xr-x   0 runner    (1001) docker     (122)     4695 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js
--rw-r--r--   0 runner    (1001) docker     (122)     3570 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/ome.csrf.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)    91476 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js
--rw-r--r--   0 runner    (1001) docker     (122)   299677 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js
--rw-r--r--   0 runner    (1001) docker     (122)     3213 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    74385 2022-11-30 14:18:05.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js
--rw-r--r--   0 runner    (1001) docker     (122)    19530 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/css/
--rw-r--r--   0 runner    (1001) docker     (122)    22385 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/css/figure.css
--rw-r--r--   0 runner    (1001) docker     (122)   371780 2022-11-30 14:18:08.000000 omero-figure-5.1.0/omero_figure/static/figure/figure.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/static/figure/images/
--rw-r--r--   0 runner    (1001) docker     (122)     2878 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/arrow-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (122)     3274 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/button-down-grey.png
--rw-r--r--   0 runner    (1001) docker     (122)     1879 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/button-down.png
--rw-r--r--   0 runner    (1001) docker     (122)     2827 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/button-flat.png
--rw-r--r--   0 runner    (1001) docker     (122)     2111 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/button-up.png
--rw-r--r--   0 runner    (1001) docker     (122)     3022 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/crop20.png
--rw-r--r--   0 runner    (1001) docker     (122)      245 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/cursor-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (122)     3020 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/ellipse-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (122)     3405 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/gradient.png
--rw-r--r--   0 runner    (1001) docker     (122)     2865 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/line-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (122)    18556 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/luts_10.png
--rw-r--r--   0 runner    (1001) docker     (122)     3116 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/markdown_dark32x20.png
--rw-r--r--   0 runner    (1001) docker     (122)     3089 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/markdown_light32x20.png
--rw-r--r--   0 runner    (1001) docker     (122)     2880 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/polygon-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (122)     2874 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/polyline-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (122)     3585 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/projection20.png
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/static/figure/images/square-outline-icon-16.png
--rw-r--r--   0 runner    (1001) docker     (122)    64904 2022-11-30 14:18:08.000000 omero-figure-5.1.0/omero_figure/static/figure/templates.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.328944 omero-figure-5.1.0/omero_figure/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.340944 omero-figure-5.1.0/omero_figure/templates/figure/
--rw-r--r--   0 runner    (1001) docker     (122)    61917 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/templates/figure/index.html
--rw-r--r--   0 runner    (1001) docker     (122)     3487 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      981 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    24215 2022-11-30 14:17:52.000000 omero-figure-5.1.0/omero_figure/views.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-30 14:18:09.336944 omero-figure-5.1.0/omero_figure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     8550 2022-11-30 14:18:09.000000 omero-figure-5.1.0/omero_figure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4259 2022-11-30 14:18:09.000000 omero-figure-5.1.0/omero_figure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 14:18:09.000000 omero-figure-5.1.0/omero_figure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-30 14:18:09.000000 omero-figure-5.1.0/omero_figure.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-30 14:18:09.000000 omero-figure-5.1.0/omero_figure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2022-11-30 14:18:09.000000 omero-figure-5.1.0/omero_figure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       80 2022-11-30 14:18:09.344945 omero-figure-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     6148 2022-11-30 14:17:52.000000 omero-figure-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.493957 omero-figure-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34520 2023-05-03 13:29:42.000000 omero-figure-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 13:29:42.000000 omero-figure-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-03 13:29:57.493957 omero-figure-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-05-03 13:29:42.000000 omero-figure-6.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 13:29:46.000000 omero-figure-6.0.0/omero_figure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 13:29:46.000000 omero-figure-6.0.0/omero_figure/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/omeroutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/scripts/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/scripts/omero/figure_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)    93011 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    59497 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone-1.0.0.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      769 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2032 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   119892 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)    97339 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14079 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    63157 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29512 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16448 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    58458 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27427 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4143 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3487 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3271 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2837 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2972 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8817 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    40582 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17189 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    95786 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css
+-rw-r--r--   0 runner    (1001) docker     (123)   228478 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17348 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/json2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/
+-rw-r--r--   0 runner    (1001) docker     (123)    53802 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16798 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4695 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/ome.csrf.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    91476 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)   299677 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    74385 2023-05-03 13:29:53.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    19530 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.489957 omero-figure-6.0.0/omero_figure/static/figure/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    22795 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/css/figure.css
+-rw-r--r--   0 runner    (1001) docker     (123)   372938 2023-05-03 13:29:55.000000 omero-figure-6.0.0/omero_figure/static/figure/figure.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.493957 omero-figure-6.0.0/omero_figure/static/figure/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/arrow-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/button-down-grey.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/button-down.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/button-flat.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/button-up.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/crop20.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/cursor-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/ellipse-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/gradient.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/line-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18556 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/luts_10.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/markdown_dark32x20.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/markdown_light32x20.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/polygon-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/polyline-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/projection20.png
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/static/figure/images/square-outline-icon-16.png
+-rw-r--r--   0 runner    (1001) docker     (123)    66715 2023-05-03 13:29:55.000000 omero-figure-6.0.0/omero_figure/static/figure/templates.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.481956 omero-figure-6.0.0/omero_figure/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.493957 omero-figure-6.0.0/omero_figure/templates/figure/
+-rw-r--r--   0 runner    (1001) docker     (123)    61917 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/templates/figure/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24215 2023-05-03 13:29:42.000000 omero-figure-6.0.0/omero_figure/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 13:29:57.485957 omero-figure-6.0.0/omero_figure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 13:29:57.000000 omero-figure-6.0.0/omero_figure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-03 13:29:57.493957 omero-figure-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-03 13:29:42.000000 omero-figure-6.0.0/setup.py
```

### Comparing `omero-figure-5.1.0/LICENSE` & `omero-figure-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/PKG-INFO` & `omero-figure-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: omero-figure
-Version: 5.1.0
+Version: 6.0.0
 Summary: OMERO figure creation app
 Home-page: https://github.com/ome/omero-figure
-Download-URL: https://github.com/ome/omero-figure/archive/v5.1.0.tar.gz
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
+Download-URL: https://github.com/ome/omero-figure/archive/v6.0.0.tar.gz
 Keywords: OMERO.web,figure
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -246,7 +247,9 @@
 
 OMERO.figure is released under the AGPL.
 
 Copyright
 ---------
 
 2016-2022, The Open Microscopy Environment
+
+
```

### Comparing `omero-figure-5.1.0/README.rst` & `omero-figure-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/apps.py` & `omero-figure-6.0.0/omero_figure/apps.py`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/omeroutils.py` & `omero-figure-6.0.0/omero_figure/omeroutils.py`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py` & `omero-figure-6.0.0/omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py`

 * *Files 0% similar despite different names*

```diff
@@ -897,15 +897,15 @@
 
         index = page if page is not None else 1
         if fext == "tiff" and self.page_count > 1:
             full_name = "%s_page_%02d.%s" % (name, index, fext)
         if self.zip_folder_name is not None:
             full_name = os.path.join(self.zip_folder_name, full_name)
 
-        while(os.path.exists(full_name)):
+        while os.path.exists(full_name):
             index += 1
             full_name = "%s_page_%02d.%s" % (name, index, fext)
             if self.zip_folder_name is not None:
                 full_name = os.path.join(self.zip_folder_name, full_name)
 
         # Handy to know what the last created file is:
         self.figure_file_name = full_name
@@ -1430,27 +1430,28 @@
         red = int(color[0:2], 16)
         green = int(color[2:4], 16)
         blue = int(color[4:6], 16)
 
         position = 'position' in sb and sb['position'] or 'bottomright'
         align = 'left'
 
+        half_height = sb.get('height', 3) // 2
         if position == 'topleft':
             lx = x + spacer
-            ly = y + spacer
+            ly = y + spacer + half_height
         elif position == 'topright':
             lx = x + width - spacer
-            ly = y + spacer
+            ly = y + spacer + half_height
             align = "right"
         elif position == 'bottomleft':
             lx = x + spacer
-            ly = y + height - spacer
+            ly = y + height - spacer - half_height
         elif position == 'bottomright':
             lx = x + width - spacer
-            ly = y + height - spacer
+            ly = y + height - spacer - half_height
             align = "right"
 
         pixel_size_x = panel['pixel_size_x']
 
         # If we previously calculated the zoom scale for big image rendering
         # Use this again here to scale the pixel size
         if 'zoom_level_scale' in panel:
@@ -1472,15 +1473,16 @@
 
         canvas_length = int(round(canvas_length))
         if align == 'left':
             lx_end = lx + canvas_length
         else:
             lx_end = lx - canvas_length
 
-        self.draw_scalebar_line(lx, ly, lx_end, ly, 3, (red, green, blue))
+        self.draw_scalebar_line(lx, ly, lx_end, ly, sb.get("height", 3),
+                                (red, green, blue))
 
         if 'show_label' in sb and sb['show_label']:
             symbol = u"\u00B5m"
             if 'pixel_size_x_symbol' in panel:
                 symbol = panel['pixel_size_x_symbol']
             if scalebar_unit and scalebar_unit in unit_symbols:
                 symbol = unit_symbols[scalebar_unit]['symbol']
@@ -1488,21 +1490,25 @@
             font_size = 10
             try:
                 font_size = int(sb.get('font_size'))
             except Exception:
                 pass
 
             # For 'bottom' scalebar, put label above
+            # 5 is an empirically determined offset that "works"
             if 'bottom' in position:
-                ly = ly - font_size
+                ly = ly - font_size - 5
             else:
                 ly = ly + 5
 
             self.draw_text(
-                label, (lx + lx_end)/2, ly, font_size, (red, green, blue),
+                label, (lx + lx_end)/2,
+                ly + ((-1 if position in ["bottomleft", "bottomright"]
+                       else 1) * half_height),
+                font_size, (red, green, blue),
                 align="center")
 
     def is_big_image(self, image):
         """Return True if this is a 'big' tiled image."""
         max_w, max_h = self.conn.getMaxPlaneSize()
         return image.getSizeX() * image.getSizeY() > max_w * max_h
 
@@ -2209,18 +2215,16 @@
 
         x = scale_to_export_dpi(x)
         y = scale_to_export_dpi(y)
         x2 = scale_to_export_dpi(x2)
         y2 = scale_to_export_dpi(y2)
         width = scale_to_export_dpi(width)
 
-        for l in range(width):
-            draw.line([(x, y), (x2, y2)], fill=rgb)
-            y += 1
-            y2 += 1
+        for l in range(-width // 2, width // 2):
+            draw.line([(x, y+l), (x2, y2+l)], fill=rgb)
 
     def draw_temp_label(self, text, fontsize, rgb):
         """Returns a new PIL image with text. Handles html."""
         tokens = self.parse_html(text)
 
         widths = []
         heights = []
@@ -2291,15 +2295,14 @@
                 i += 1
         tokens.append({'text': token, 'bold': in_bold, 'italics': in_italics})
         return tokens
 
     def draw_text(self, text, x, y, fontsize, rgb, align="center"):
         """ Add text to the current figure page """
         x = scale_to_export_dpi(x)
-        y = y - 5       # seems to help, but would be nice to fix this!
         y = scale_to_export_dpi(y)
         fontsize = scale_to_export_dpi(fontsize)
 
         if markdown_imported:
             # convert markdown to html
             text = markdown.markdown(text)
```

### Comparing `omero-figure-5.1.0/omero_figure/settings.py` & `omero-figure-6.0.0/omero_figure/settings.py`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/backbone-1.0.0.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone-1.0.0.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/README.md`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/backbone.mousetrap/backbone.mousetrap.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.css`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/css/bootstrap-colorpicker.min.css`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha-horizontal.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/alpha.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue-horizontal.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/hue.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/img/bootstrap-colorpicker/saturation.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/bootstrap-colorpicker/js/bootstrap-colorpicker.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-1.11.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.base.css`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/css/jquery.ui.slider.css`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/jquery-ui-1.10.4/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/json2.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/json2.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/markdown-browser-0.6.0-beta1/markdown.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/mousetrap-1.5.3/mousetrap.min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/ome.csrf.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/ome.csrf.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael-min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/raphael.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/raphael-2.1.2/scaleraphael.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/shape-editor-4.0.0/shape-editor.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js` & `omero-figure-6.0.0/omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/css/figure.css` & `omero-figure-6.0.0/omero_figure/static/figure/css/figure.css`

 * *Files 2% similar despite different names*

```diff
@@ -271,20 +271,43 @@
 
     .new-label-form .input-group {
         width:160px;
         margin-right: 4px;
     }
 
     .scalebar_form .input-group {
-        width:50px;
+        width:80px;
         margin-right: 4px;
     }
 
+    .scalebar_form .form-group {
+        margin-bottom: 0;
+    }
+
+    .scalebar_form .row {
+        align-items: center;
+        display: flex;
+        gap: 3px;
+        margin-top: 3px;
+    }
+
+    .scalebar_form .scalebar_length {
+        padding-right: 0;
+    }
+
+    .scalebar_form .scalebar_text {
+        padding-right: 0;
+    }
+
+    .scalebar_form .scalebar_unit {
+        padding-left: 0;
+        padding-right: 10px;
+    }
+
     .scalebar {
-        height: 3px;
         position: absolute;
         margin: 5% !important;
     }
 
     .scalebar-label {
         position: absolute;
         left: -100%;
```

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/figure.js` & `omero-figure-6.0.0/omero_figure/static/figure/figure.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2,15 +2,15 @@
 
 //!  DO NOT EDIT THIS FILE! - Edit under static/figure/js/
 //!  figure.js created by $ grunt concat
 
 
 // Version of the json file we're saving.
 // This only needs to increment when we make breaking changes (not linked to release versions.)
-var VERSION = 6;
+var VERSION = 7;
 
 
 // ------------------------- Figure Model -----------------------------------
 // Has a PanelList as well as other attributes of the Figure
 var FigureModel = Backbone.Model.extend({
 
     defaults: {
@@ -262,14 +262,24 @@
                         label["text"] = "[time." + label["time"] + "]";
                         delete label.time;
                     }
                 }
             });
         }
 
+        if (v < 7) {
+            console.log("Transforming to VERSION 7");
+            // Adding the height parameter to the JSON
+            _.each(json.panels, function(p) {
+                // rename lineWidth to strokeWidth
+                if (p.scalebar && !p.scalebar.height) {
+                    p.scalebar.height = 3;
+                }
+            });
+        }
         return json;
     },
 
     figure_toJSON: function() {
         // Turn panels into json
         var p_json = [],
             self = this;
@@ -566,17 +576,24 @@
         if (coords.y !== undefined) {
             offset.y = coords.y % yspacing;
         }
         return offset;
     },
 
     getDefaultFigureName: function() {
+        const padL = (nr) => `${nr}`.padStart(2, '0');
         var d = new Date(),
-            dt = d.getFullYear() + "-" + (d.getMonth() + 1) + "-" + d.getDate(),
-            tm = d.getHours() + ":" + d.getMinutes() + ":" + d.getSeconds();
+            dt = [d.getFullYear(),
+                padL(d.getMonth() + 1),
+                padL(d.getDate())
+            ].join('-'),
+            tm = [padL(d.getHours()),
+                padL(d.getMinutes()),
+                padL(d.getSeconds())
+            ].join('-');
         return "Figure_" + dt + "_" + tm;
     },
 
     nudge_right: function() {
         this.nudge('x', 10);
     },
 
@@ -6787,18 +6804,18 @@
         }
         var sb = this.model.get('scalebar');
         if (sb && sb.show) {
             var sb_json = {};
             sb_json.position = sb.position;
             sb_json.color = sb.color;
             sb_json.length = sb.length;
+            sb_json.height = sb.height;
             sb_json.font_size = sb.font_size;
             sb_json.show_label = sb.show_label;
             sb_json.symbol = sb.units;
-
             // Use global LENGTH_UNITS to get symbol for unit.
             if (window.LENGTH_UNITS && window.LENGTH_UNITS[sb.units]) {
                 sb_json.symbol = window.LENGTH_UNITS[sb.units].symbol;
             }
 
             var sb_html = this.scalebar_template(sb_json);
             this.$el.append(sb_html);
@@ -9337,14 +9354,22 @@
         "submit .scalebar_form": "update_scalebar",
         "click .scalebar_label": "update_scalebar",
         "change .btn": "dropdown_btn_changed",
         "click .hide_scalebar": "hide_scalebar",
         "click .pixel_size_display": "edit_pixel_size",
         "keypress .pixel_size_input": "enter_pixel_size",
         "blur .pixel_size_input": "save_pixel_size",
+        "keyup input[type='text']": "handle_keyup",
+    },
+
+    handle_keyup: function(event) {
+        // If Enter key - submit form...
+        if (event.which == 13) {
+            this.update_scalebar();
+        }
     },
 
     // simply show / hide editing field
     edit_pixel_size: function() {
         $('.pixel_size_display', this.$el).hide();
         $(".pixel_size_input", this.$el).css('display', 'inline-block').focus();
     },
@@ -9384,22 +9409,23 @@
             m.hide_scalebar();
         });
     },
 
     // called when form changes
     update_scalebar: function(event) {
 
-        var $form = $('#scalebar_form form');
+        var $form = $('.scalebar_form ');
 
         var length = $('.scalebar-length', $form).val(),
             units = $('.scalebar-units span:first', $form).attr('data-unit'),
             position = $('.label-position span:first', $form).attr('data-position'),
             color = $('.label-color span:first', $form).attr('data-color'),
             show_label = $('.scalebar_label', $form).prop('checked'),
-            font_size = $('.scalebar_font_size span:first', $form).text().trim();
+            font_size = $('.scalebar_font_size span:first', $form).text().trim(),
+            height = parseInt($('.scalebar-height', $form).val());
 
         this.models.forEach(function(m) {
             var old_sb = m.get('scalebar');
             var sb = {
                 show: true
             };
             if (length != '-') sb.length = parseFloat(length, 10);
@@ -9416,14 +9442,15 @@
                     sb.units = "MICROMETER";
                 }
             }
             if (position != '-') sb.position = position;
             if (color != '-') sb.color = color;
             sb.show_label = show_label;
             if (font_size != '-') sb.font_size = font_size;
+            if (height != '-') sb.height = height;
 
             m.save_scalebar(sb);
         });
         return false;
     },
 
     render: function() {
@@ -9479,22 +9506,24 @@
                 if (!json.length) {
                     json.length = sb.length;
                     json.units = sb.units;
                     json.position = sb.position;
                     json.color = sb.color;
                     json.show_label = sb.show_label;
                     json.font_size = sb.font_size;
+                    json.height = sb.height;
                 } else {
                     // combine attributes. Use '-' if different values found
                     if (json.length != sb.length) json.length = '-';
                     if (json.units != sb.units) json.units = '-';
                     if (json.position != sb.position) json.position = '-';
                     if (json.color != sb.color) json.color = '-';
                     if (!sb.show_label) json.show_label = false;
                     if (json.font_size != sb.font_size) json.font_size = '-';
+                    if (json.height != sb.height) json.height = '-';
                 }
             }
             // if any panels don't have scalebar - we allow to add
             if (!sb || !sb.show) hidden = true;
         });
 
         if (this.models.length === 0 || hidden) {
@@ -9508,22 +9537,25 @@
             // find the symbol e.g. 'mm' from units 'MILLIMETER'
             json.units_symbol = LENGTH_UNITS[json.units].symbol;
         }
         json.position = json.position || 'bottomright';
         json.color = json.color || 'FFFFFF';
         json.font_size = json.font_size || 10;
         json.pixel_size_symbol = json.pixel_size_symbol || '-';
+        json.height = json.height || 3;
 
         var html = this.template(json);
         this.$el.html(html);
+        this.$el.find("[title]").tooltip();
 
         return this;
     }
 });
 
+
 // -------------- Selection Overlay Views ----------------------
 
 
 // SvgView uses ProxyRectModel to manage Svg Rects (raphael)
 // This converts between zoomed coordiantes of the html DOM panels
 // and the unzoomed SVG overlay.
 // Attributes of this model apply to the SVG canvas and are updated from
```

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/arrow-icon-16.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/arrow-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/button-down-grey.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/button-down-grey.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/button-down.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/button-down.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/button-flat.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/button-flat.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/button-up.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/button-up.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/crop20.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/crop20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/ellipse-icon-16.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/ellipse-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/gradient.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/gradient.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/line-icon-16.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/line-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/luts_10.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/luts_10.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/markdown_dark32x20.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/markdown_dark32x20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/markdown_light32x20.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/markdown_light32x20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/polygon-icon-16.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/polygon-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/polyline-icon-16.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/polyline-icon-16.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/images/projection20.png` & `omero-figure-6.0.0/omero_figure/static/figure/images/projection20.png`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/static/figure/templates.js` & `omero-figure-6.0.0/omero_figure/static/figure/templates.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,12 @@
 this["JST"] = this["JST"] || {};
 
 this["JST"]["src/templates/channel_slider_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n <div class="clearfix" style="position: relative; padding-bottom: 4px">\n\n\n    <div class="btn-group">\n            <button type="button"\n            title="' +
@@ -79,29 +78,27 @@
 
     }
     return __p
 };
 
 this["JST"]["src/templates/figure_panel_template.html"] = function(obj) {
     obj || (obj = {});
-    var __t, __p = '',
-        __e = _.escape;
+    var __t, __p = '';
     with(obj) {
         __p += '    <!-- The content of <div class=\'imagePanel\'> for each panel -->\n    <div class="imgContainer">\n        <div class="glyphicon glyphicon-refresh"></div>\n        <img class="img_panel" />\n        <div id="' +
             ((__t = (randomId)) == null ? '' : __t) +
             '" class="panel_canvas"></div>\n    </div>\n';
 
     }
     return __p
 };
 
 this["JST"]["src/templates/image_display_options_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <div class="btn-group image-display-options rotation-controls">\n        <button type="button" class="btn btn-default btn-sm show-rotation" title="Rotate image">\n            <span class="glyphicon glyphicon-repeat"></span>\n            <span class="rotation_value">' +
@@ -127,15 +124,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/info_panel_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <p>';
@@ -178,15 +174,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/labels_form_inner_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <div class="input-group pull-left">\n        <input type="text" class="label-text form-control input-sm" \n                placeholder="Label" value="';
@@ -230,15 +225,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/labels_form_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n        <div class="">\n\n            ';
@@ -259,47 +253,45 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/lut_picker.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
-        __p += '\n\n<div class="btn-group-vertical col-xs-6" role="group">\n\n\t';
+        __p += '\n\n<div class="btn-group-vertical col-xs-6" role="group">\n\n	';
         _.each(luts, function(lut, i) {
             ;
-            __p += '\n\n\t\t<button type="button" class="btn btn-default lutOption" data-lut="' +
+            __p += '\n\n		<button type="button" class="btn btn-default lutOption" data-lut="' +
                 ((__t = (lut.name)) == null ? '' : __t) +
-                '">\n\t\t\t<span class="lutBg" style="background-position: ' +
+                '">\n			<span class="lutBg" style="background-position: ' +
                 ((__t = (lut.bgPos)) == null ? '' : __t) +
-                '">&nbsp</span>\n\t\t\t' +
+                '">&nbsp</span>\n			' +
                 ((__t = (lut.displayName)) == null ? '' : __t) +
-                ' </button>\n\n\t\t';
+                ' </button>\n\n		';
             if (i === parseInt(luts.length / 2)) {
                 ;
-                __p += '\n\t\t\t</div>\n\t\t\t<div class="btn-group-vertical col-xs-6" role="group">\n\t\t';
+                __p += '\n			</div>\n			<div class="btn-group-vertical col-xs-6" role="group">\n		';
             };
-            __p += '\n\n\t';
+            __p += '\n\n	';
         });
         __p += '\n</div>\n';
 
     }
     return __p
 };
 
 this["JST"]["src/templates/rois_form_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n\n<h5>ROIs\n    ';
@@ -363,15 +355,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/scalebar_form_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <div class="pixel_size_form" style="position:relative">\n        <div class="pixel_size_div">\n            Pixel Size:\n            <input class="input-sm form-control pixel_size_input" placeholder="Pixel Size (' +
@@ -382,105 +373,113 @@
         if (!pixel_size_x) {
             print('<span style="color:red">NOT SET</span>')
         } else if (typeof pixel_size_x === 'number') {
             print(pixel_size_x.toFixed(3) + " " + pixel_size_symbol)
         } else {
             print(pixel_size_x + " " + pixel_size_symbol)
         };
-        __p += '\n            </span>\n        </div>\n\n    </div>\n\n    <form class="scalebar_form form-inline">\n\n    <div class="input-group pull-left">\n        <input type="text" class="scalebar-length form-control input-sm" \n                placeholder="Length" value="' +
+        __p += '\n            </span>\n        </div>\n    </div>\n    <form class="scalebar_form" style="position: relative">\n        <div style="position: absolute; right: 0;">\n            ';
+        if (show) {
+            ;
+            __p += '\n                <button type="submit" class="show_scalebar btn btn-sm btn-success pull-right">Show</button>\n            ';
+        } else {
+            ;
+            __p += '\n                <button type="button" class="hide_scalebar btn btn-default btn-sm pull-right">Hide</button>\n            ';
+        };
+        __p += '\n        </div>\n\n        <div class="row">\n            <div class="form-group col-sm-2 scalebar_text">\n                Length\n            </div>\n            <div class="form-group col-sm-2 scalebar_length">\n                <input type="text" class="scalebar-length form-control input-sm" \n                            placeholder="Length" value="' +
             ((__t = (length)) == null ? '' : __t) +
-            '" />\n    </div>\n\n    <!-- units -->\n    <div class="btn-group">\n        <button type="button" class="scalebar-units btn btn-default btn-sm dropdown-toggle"\n                title="Units" data-toggle="dropdown">\n            <span data-unit="' +
+            '" />\n            </div>\n            <div class="form-group col-sm-1 btn-group scalebar_unit">\n                <button type="button" class="scalebar-units btn btn-default btn-sm dropdown-toggle"\n                        title="Units" data-toggle="dropdown">\n                    <span data-unit="' +
             ((__t = (units)) == null ? '' : __t) +
             '">' +
             ((__t = (units_symbol)) == null ? '' : __t) +
-            '</span>\n            <span class="caret"></span>\n        </button>\n        <ul class="dropdown-menu" role="menu">\n            ';
+            '</span>\n                    <span class="caret"></span>\n                </button>\n                <ul class="dropdown-menu" role="menu">\n                    ';
         _.each(unit_symbols, function(u) {
             ;
-            __p += '\n                <li><a href=\'#\'>' +
+            __p += '\n                        <li><a href=\'#\'>' +
                 ((__t = (u.unit)) == null ? '' : __t) +
                 ' (<span data-unit="' +
                 ((__t = (u.unit)) == null ? '' : __t) +
                 '">' +
                 ((__t = (u.symbol)) == null ? '' : __t) +
-                '</span>)</a></li>\n            ';
+                '</span>)</a></li>\n                    ';
         });;
-        __p += '\n        </ul>\n    </div>\n\n    <div class="btn-group">\n        <button type="button" class="label-position btn btn-default btn-sm dropdown-toggle" \n                title="Position" data-toggle="dropdown">\n            <span data-position="' +
+        __p += '\n                </ul>\n            </div>\n            <div class="col-sm-1" />\n            <div class="form-group col-sm-auto btn-group">\n                <button type="button" class="label-position btn btn-default btn-sm dropdown-toggle" \n                        title="Position" data-toggle="dropdown">\n                    <span data-position="' +
             ((__t = (position)) == null ? '' : __t) +
             '" class="labelicon-' +
             ((__t = (position)) == null ? '' : __t) +
-            ' glyphicon \n                ';
+            ' glyphicon \n                        ';
         if (_.contains(['top', 'bottom', 'left', 'right'], position)) print('glyphicon-log-out');
         else {
             print('glyphicon-new-window')
         };
-        __p += '"></span>\n            <span class="caret"></span>\n        </button>\n        <ul class="dropdown-menu" role="menu">\n            <li role="presentation" class="dropdown-header">Inside Corners</li>\n            <li><a href="#">\n                <span data-position="topleft" class="labelicon-topleft glyphicon glyphicon-new-window"></span>\n                Top Left</a>\n            </li>\n            <li><a href="#">\n                <span data-position="topright" class="labelicon-topright glyphicon glyphicon-new-window"></span>\n                Top Right</a>\n            </li>\n            <li><a href="#">\n                <span data-position="bottomleft" class="labelicon-bottomleft glyphicon glyphicon-new-window"></span>\n                Bottom Left</a>\n            </li>\n            <li><a href="#">\n                <span data-position="bottomright" class="labelicon-bottomright glyphicon glyphicon-new-window"></span>\n                Bottom Right</a>\n            </li>\n        </ul>\n    </div>\n\n    <div class="btn-group">\n        <button type="button" class="label-color btn btn-default btn-sm dropdown-toggle" title="Label Color"\n            data-toggle="dropdown">\n            <span data-color="' +
+        __p += '"></span>\n                    <span class="caret"></span>\n                </button>\n                <ul class="dropdown-menu" role="menu">\n                    <li role="presentation" class="dropdown-header">Inside Corners</li>\n                    <li><a href="#">\n                        <span data-position="topleft" class="labelicon-topleft glyphicon glyphicon-new-window"></span>\n                        Top Left</a>\n                    </li>\n                    <li><a href="#">\n                        <span data-position="topright" class="labelicon-topright glyphicon glyphicon-new-window"></span>\n                        Top Right</a>\n                    </li>\n                    <li><a href="#">\n                        <span data-position="bottomleft" class="labelicon-bottomleft glyphicon glyphicon-new-window"></span>\n                        Bottom Left</a>\n                    </li>\n                    <li><a href="#">\n                        <span data-position="bottomright" class="labelicon-bottomright glyphicon glyphicon-new-window"></span>\n                        Bottom Right</a>\n                    </li>\n                </ul>\n            </div>\n            <div class="form-group col-sm-auto btn-group">\n                <button type="button" class="label-color btn btn-default btn-sm dropdown-toggle" title="Label Color"\n                    data-toggle="dropdown">\n                    <span data-color="' +
             ((__t = (color)) == null ? '' : __t) +
             '" style="background-color:#' +
             ((__t = (color)) == null ? '' : __t) +
-            '">&nbsp &nbsp &nbsp</span>\n            <span class="caret"></span>\n        </button>\n        <ul class="dropdown-menu colorpicker" role="menu">\n            <li><a href="#">\n                <span data-color="000000" style="background-color:#000">&nbsp &nbsp &nbsp</span>&nbsp Black\n            </a></li>\n            <li><a href="#">\n                <span data-color="0000FF" style="background-color:#00f">&nbsp &nbsp &nbsp</span>&nbsp Blue\n            </a></li>\n            <li><a href="#">\n                <span data-color="00FF00" style="background-color:#0f0">&nbsp &nbsp &nbsp</span>&nbsp Green\n            </a></li>\n            <li><a href="#">\n                <span data-color="FF0000" style="background-color:#f00">&nbsp &nbsp &nbsp</span>&nbsp Red\n            </a></li>\n            <li><a href="#">\n                <span data-color="FFFF00" style="background-color:#ff0">&nbsp &nbsp &nbsp</span>&nbsp Yellow\n            </a></li>\n            <li><a href="#">\n                <span data-color="FFFFFF" style="background-color:#fff">&nbsp &nbsp &nbsp</span>&nbsp White\n            </a></li>\n            <li><a href="#">\n                <span data-color="FF00FF" style="background-color:#f0f">&nbsp &nbsp &nbsp</span>&nbsp Magenta\n            </a></li>\n        </ul>\n    </div>\n\n    <div class="checkbox">\n        <label>\n            <input type="checkbox" class="scalebar_label" ';
+            '">&nbsp &nbsp &nbsp</span>\n                    <span class="caret"></span>\n                </button>\n                <ul class="dropdown-menu colorpicker" role="menu">\n                    <li><a href="#">\n                        <span data-color="000000" style="background-color:#000">&nbsp &nbsp &nbsp</span>&nbsp Black\n                    </a></li>\n                    <li><a href="#">\n                        <span data-color="0000FF" style="background-color:#00f">&nbsp &nbsp &nbsp</span>&nbsp Blue\n                    </a></li>\n                    <li><a href="#">\n                        <span data-color="00FF00" style="background-color:#0f0">&nbsp &nbsp &nbsp</span>&nbsp Green\n                    </a></li>\n                    <li><a href="#">\n                        <span data-color="FF0000" style="background-color:#f00">&nbsp &nbsp &nbsp</span>&nbsp Red\n                    </a></li>\n                    <li><a href="#">\n                        <span data-color="FFFF00" style="background-color:#ff0">&nbsp &nbsp &nbsp</span>&nbsp Yellow\n                    </a></li>\n                    <li><a href="#">\n                        <span data-color="FFFFFF" style="background-color:#fff">&nbsp &nbsp &nbsp</span>&nbsp White\n                    </a></li>\n                    <li><a href="#">\n                        <span data-color="FF00FF" style="background-color:#f0f">&nbsp &nbsp &nbsp</span>&nbsp Magenta\n                    </a></li>\n                </ul>\n            </div>\n        </div>\n\n        <div class="row">\n            <div class="form-group col-sm-2 scalebar_text">\n                Height\n            </div>\n            <div class="form-group col-sm-2 scalebar_length">\n                <input type="text" class="scalebar-height form-control input-sm" \n                placeholder="Height" value="' +
+            ((__t = (height)) == null ? '' : __t) +
+            '" />\n            </div>\n            <div class="form-group col-sm-1 scalebar_text" style="padding-left: 2px;">\n                px\n            </div>\n\n            <div class="form-group col-sm-auto scalebar_text">\n                Label\n            </div>\n            <div class="form-group col-sm-auto" style="margin: 2px">\n                <input type="checkbox" class="scalebar_label" ';
         if (show_label) print("checked");
-        __p += ' > Label\n        </label>\n    </div>\n\n    <div class="btn-group">\n        <button type="button" class="scalebar_font_size btn btn-default btn-sm dropdown-toggle" title="Label Size"\n            data-toggle="dropdown" style="width:33px; ';
+        __p += ' /> \n            </div>\n            <div class="form-group col-sm-1 btn-group" style="padding: 0;">\n                <button type="button" class="scalebar_font_size btn btn-default btn-sm dropdown-toggle" title="Font Size"\n                data-toggle="dropdown" style="width:33px; ';
         if (!show_label) print("display:none");
-        __p += '">\n            <span>' +
+        __p += '">\n                    <span>' +
             ((__t = (font_size)) == null ? '' : __t) +
-            '</span>\n            <span class="caret"></span>\n        </button>\n        <ul class="dropdown-menu" role="menu">\n        ';
+            '</span>\n                    <span class="caret"></span>\n                </button>\n                <ul class="dropdown-menu" role="menu">\n                ';
         _.each([6, 8, 10, 12, 14, 18, 21, 24, 36, 48], function(p) {
             print("<li><a href='#'><span>" + p + "</span></a></li>")
         });;
-        __p += '\n        </ul>\n    </div>\n\n    ';
-        if (show) {
-            ;
-            __p += '\n        <button type="submit" class="show_scalebar btn btn-sm btn-success pull-right">Show</button>\n    ';
-        } else {
-            ;
-            __p += '\n        <button type="button" class="hide_scalebar btn btn-sm btn-default pull-right">Hide</button>\n    ';
-        };
-        __p += '\n    </form>\n';
+        __p += '\n                </ul>\n            </div>\n            <div class="form-group col-sm-1 scalebar_text" style="padding-left: 2px;">\n                ';
+        if (show_label) print("pt");
+        __p += '\n            </div>\n        </div>\n    </form>';
 
     }
     return __p
 };
 
 this["JST"]["src/templates/scalebar_panel_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <div class="scalebar label_' +
             ((__t = (position)) == null ? '' : __t) +
             '" style="background-color: #' +
             ((__t = (color)) == null ? '' : __t) +
-            '">\n        ';
+            '; height: ' +
+            ((__t = (height)) == null ? '' : __t) +
+            'px">\n        ';
         if (show_label) {
             ;
             __p += '\n            <div class=\'scalebar-label\' style=\'color: #' +
                 ((__t = (color)) == null ? '' : __t) +
                 '; font-size: ' +
                 ((__t = (font_size)) == null ? '' : __t) +
-                'px\'>\n                ' +
+                'px;\n            ';
+            if (position === "bottomleft" || position === "bottomright") print("margin-bottom:" + height);;
+            __p += 'px;\n            ';
+            if (position === "topleft" || position === "topright") print("margin-top:" + height);;
+            __p += 'px;\'>\n                ' +
                 ((__t = (length)) == null ? '' : __t) +
                 ' ' +
                 ((__t = (symbol)) == null ? '' : __t) +
                 '\n            </div>\n        ';
         };
         __p += '\n    </div>\n';
 
     }
     return __p
 };
 
 this["JST"]["src/templates/viewport_inner_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    ';
@@ -517,16 +516,15 @@
 
     }
     return __p
 };
 
 this["JST"]["src/templates/viewport_template.html"] = function(obj) {
     obj || (obj = {});
-    var __t, __p = '',
-        __e = _.escape;
+    var __t, __p = '';
     with(obj) {
         __p += '\n        <div id="vp_z_label">Z</div>\n        <div id="vp_z_value"></div>\n        <div id="vp_t_label">T</div>\n        <div id="vp_t_value"></div>\n        <div id="vp_deltaT"></div>\n        <div class="vp_frame" style="width:' +
             ((__t = (frame_w)) == null ? '' : __t) +
             'px; height:' +
             ((__t = (frame_h)) == null ? '' : __t) +
             'px">\n            ' +
             ((__t = (inner_template({
@@ -538,15 +536,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/xywh_panel_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n\n\n    <table id="xywh_table" class="table">\n        <tbody>\n            <tr><td>\n                Panel\n\n                <form class="form-inline pull-right">\n                    <div class="checkbox">\n                        ' +
@@ -576,15 +573,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/zoom_crop_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n<h5 style="margin-top:6px">\n    View\n    <span style="font-weight:normal; float:right">\n        x: <span style="color: #aaa">' +
@@ -650,15 +646,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/labels/label_table_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <!-- Alternative label_template - uses table to valign middle for \'left\' & \'right\' labels -->\n    <div class="label_layout label_middle label_' +
@@ -679,15 +674,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/labels/label_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n\n    <!-- One of these added to each position \'top\', \'topleft\' etc within Panel $el -->\n    <div class="label_layout label_' +
@@ -708,15 +702,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/labels/label_vertical_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <div class="label_layout left_vlabels">\n        <div>\n            ';
@@ -735,15 +728,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/modal_dialogs/crop_modal_roi.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n<tr class="roiPickMe">\n    <td>\n        <div class="roi_wrapper" style="position: relative; overflow: hidden; margin: 5px; height: ' +
@@ -803,15 +795,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/modal_dialogs/paper_setup_modal_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <div class="col-sm-12">\n        <div class="form-horizontal">\n            <div class="form-group col-sm-6" style="margin-bottom: 15px;">\n                <label>Page Color</label>\n                <input class="pageColor form-control"\n                    value="#' +
@@ -986,15 +977,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/modal_dialogs/roi_modal_roi.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n<tr>\n    <th></th>\n    <th></th>\n    <th>Z</th>\n    <th>T</th>\n    <th></th>\n</tr>\n';
@@ -1057,15 +1047,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/modal_dialogs/roi_modal_shape.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n\n';
@@ -1124,15 +1113,14 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/modal_dialogs/roi_zt_buttons.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n<span class="label label-default" style="font-size: 12px">Z: ' +
@@ -1158,41 +1146,39 @@
     }
     return __p
 };
 
 this["JST"]["src/templates/shapes/shape_item_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n    <div ';
         if (selected) print("style='background:#ddf'");
-        __p += ' >\n\n    \t' +
+        __p += ' >\n\n    	' +
             ((__t = (type)) == null ? '' : __t) +
-            '\n\n    \t';
+            '\n\n    	';
         if (type === 'RECT') print("x:" + x + " y:" + y + " width:" + width + " height:" + height);
-        __p += '\n\n    \t';
+        __p += '\n\n    	';
         if (type === 'LINE' || type === 'ARROW') print("x1:" + (x1 >> 0) + " y1:" + (y1 >> 0) + " x2:" + (x2 >> 0) + " y2:" + (y2 >> 0));
-        __p += '\n\n    \t';
+        __p += '\n\n    	';
         if (type === 'ELLIPSE') print("x:" + (cx >> 0) + " y:" + (cy >> 0) + " rx:" + (rx >> 0) + " ry:" + (ry >> 0));
         __p += '\n\n    </div>\n';
 
     }
     return __p
 };
 
 this["JST"]["src/templates/shapes/shape_toolbar_template.html"] = function(obj) {
     obj || (obj = {});
     var __t, __p = '',
-        __e = _.escape,
         __j = Array.prototype.join;
 
     function print() {
         __p += __j.call(arguments, '')
     }
     with(obj) {
         __p += '\n\n<div class="btn-group shape-option" role="group" aria-label="...">\n    <button type="button" data-state="SELECT"\n        class="btn btn-default';
```

### Comparing `omero-figure-5.1.0/omero_figure/templates/figure/index.html` & `omero-figure-6.0.0/omero_figure/templates/figure/index.html`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/urls.py` & `omero-figure-6.0.0/omero_figure/urls.py`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure/utils.py` & `omero-figure-6.0.0/omero_figure/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 
 import json
 import os
 
-__version__ = "5.1.0"
+__version__ = "6.0.0"
 
 
 def read_file(fname, content_type=None):
     p = os.path.abspath(fname)
     with open(p) as f:
         if content_type in ('json',):
             data = json.load(f)
```

### Comparing `omero-figure-5.1.0/omero_figure/views.py` & `omero-figure-6.0.0/omero_figure/views.py`

 * *Files identical despite different names*

### Comparing `omero-figure-5.1.0/omero_figure.egg-info/PKG-INFO` & `omero-figure-6.0.0/omero_figure.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: omero-figure
-Version: 5.1.0
+Version: 6.0.0
 Summary: OMERO figure creation app
 Home-page: https://github.com/ome/omero-figure
-Download-URL: https://github.com/ome/omero-figure/archive/v5.1.0.tar.gz
 Author: The Open Microscopy Team
 Author-email: ome-devel@lists.openmicroscopy.org.uk
 License: AGPL-3.0
+Download-URL: https://github.com/ome/omero-figure/archive/v6.0.0.tar.gz
 Keywords: OMERO.web,figure
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
@@ -246,7 +247,9 @@
 
 OMERO.figure is released under the AGPL.
 
 Copyright
 ---------
 
 2016-2022, The Open Microscopy Environment
+
+
```

### Comparing `omero-figure-5.1.0/omero_figure.egg-info/SOURCES.txt` & `omero-figure-6.0.0/omero_figure.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 omero_figure/views.py
 omero_figure.egg-info/PKG-INFO
 omero_figure.egg-info/SOURCES.txt
 omero_figure.egg-info/dependency_links.txt
 omero_figure.egg-info/not-zip-safe
 omero_figure.egg-info/requires.txt
 omero_figure.egg-info/top_level.txt
-omero_figure/__pycache__/__init__.cpython-311.pyc
-omero_figure/__pycache__/utils.cpython-311.pyc
+omero_figure/__pycache__/__init__.cpython-310.pyc
+omero_figure/__pycache__/utils.cpython-310.pyc
 omero_figure/scripts/omero/figure_scripts/Figure_To_Pdf.py
 omero_figure/static/figure/figure.js
 omero_figure/static/figure/templates.js
 omero_figure/static/figure/3rdparty/backbone-1.0.0.js
 omero_figure/static/figure/3rdparty/json2.js
 omero_figure/static/figure/3rdparty/ome.csrf.js
 omero_figure/static/figure/3rdparty/underscore-1.13.1-umd-min.js
```

### Comparing `omero-figure-5.1.0/setup.py` & `omero-figure-6.0.0/setup.py`

 * *Files identical despite different names*

