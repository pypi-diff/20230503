# Comparing `tmp/verstack-3.6.7.tar.gz` & `tmp/verstack-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verstack-3.6.7.tar", last modified: Tue Mar 28 10:32:07 2023, max compression
+gzip compressed data, was "verstack-3.7.0.tar", last modified: Wed May  3 13:12:39 2023, max compression
```

## Comparing `verstack-3.6.7.tar` & `verstack-3.7.0.tar`

### file list

```diff
@@ -1,536 +1,537 @@
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.716321 verstack-3.6.7/
--rw-r--r--   0 danil      (501) staff       (20)      174 2021-11-08 12:56:11.000000 verstack-3.6.7/.readthedocs.yaml
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.253320 verstack-3.6.7/.vscode/
--rw-r--r--   0 danil      (501) staff       (20)      121 2022-10-18 14:42:35.000000 verstack-3.6.7/.vscode/settings.json
--rw-r--r--   0 danil      (501) staff       (20)     1071 2020-09-18 21:03:44.000000 verstack-3.6.7/LICENSE.txt
--rw-r--r--   0 danil      (501) staff       (20)      106 2020-09-18 21:51:05.000000 verstack-3.6.7/MANIFEST
--rw-r--r--   0 danil      (501) staff       (20)     3361 2023-03-28 10:32:07.716483 verstack-3.6.7/PKG-INFO
--rw-r--r--   0 danil      (501) staff       (20)     2266 2023-03-28 10:23:26.000000 verstack-3.6.7/README.rst
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.253739 verstack-3.6.7/dist/
--rw-r--r--   0 danil      (501) staff       (20)     7308 2020-09-18 21:51:05.000000 verstack-3.6.7/dist/verstack-0.1.0.tar.gz
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.256458 verstack-3.6.7/docs/
--rw-r--r--   0 danil      (501) staff       (20)      692 2023-02-12 13:53:02.000000 verstack-3.6.7/docs/Doc_update_manual.txt
--rw-r--r--   0 danil      (501) staff       (20)      638 2020-09-20 09:39:03.000000 verstack-3.6.7/docs/Makefile
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.227591 verstack-3.6.7/docs/build/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.258880 verstack-3.6.7/docs/build/doctrees/
--rw-r--r--   0 danil      (501) staff       (20)    26942 2020-09-20 12:30:25.000000 verstack-3.6.7/docs/build/doctrees/README.doctree
--rw-r--r--   0 danil      (501) staff       (20)    30868 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/doctrees/environment.pickle
--rw-r--r--   0 danil      (501) staff       (20)   166536 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/doctrees/index.doctree
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.266723 verstack-3.6.7/docs/build/html/
--rw-r--r--   0 danil      (501) staff       (20)      230 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/.buildinfo
--rw-r--r--   0 danil      (501) staff       (20)        0 2020-09-20 11:46:51.000000 verstack-3.6.7/docs/build/html/.nojekyll
--rw-r--r--   0 danil      (501) staff       (20)    20042 2020-09-20 12:35:34.000000 verstack-3.6.7/docs/build/html/README.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.268789 verstack-3.6.7/docs/build/html/_sources/
--rw-r--r--   0 danil      (501) staff       (20)     6117 2020-09-19 13:46:17.000000 verstack-3.6.7/docs/build/html/_sources/README.md.txt
--rw-r--r--   0 danil      (501) staff       (20)     6298 2020-09-20 09:22:18.000000 verstack-3.6.7/docs/build/html/_sources/README.rst.txt
--rw-r--r--   0 danil      (501) staff       (20)    28954 2021-12-07 08:58:57.000000 verstack-3.6.7/docs/build/html/_sources/index.rst.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.309934 verstack-3.6.7/docs/build/html/_static/
--rw-r--r--   0 danil      (501) staff       (20)    11185 2020-09-20 11:40:14.000000 verstack-3.6.7/docs/build/html/_static/alabaster.css
--rw-r--r--   0 danil      (501) staff       (20)    14652 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/_static/basic.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.312318 verstack-3.6.7/docs/build/html/_static/css/
--rw-r--r--   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/css/bootstrap-theme.min.css
--rw-r--r--   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/css/bootstrap.min.css
--rw-r--r--   0 danil      (501) staff       (20)       42 2018-10-08 18:31:32.000000 verstack-3.6.7/docs/build/html/_static/custom.css
--rw-r--r--   0 danil      (501) staff       (20)     9592 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/build/html/_static/doctools.js
--rw-r--r--   0 danil      (501) staff       (20)      355 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 danil      (501) staff       (20)      286 2020-02-10 16:38:31.000000 verstack-3.6.7/docs/build/html/_static/file.png
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.398166 verstack-3.6.7/docs/build/html/_static/fonts/
--rw-r--r--   0 danil      (501) staff       (20)    18173 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.eot
--rw-r--r--   0 danil      (501) staff       (20)    47724 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.svg
--rw-r--r--   0 danil      (501) staff       (20)    31552 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.ttf
--rw-r--r--   0 danil      (501) staff       (20)    21624 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.woff
--rw-r--r--   0 danil      (501) staff       (20)    21280 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400.eot
--rw-r--r--   0 danil      (501) staff       (20)    76169 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400.svg
--rw-r--r--   0 danil      (501) staff       (20)    45116 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400.ttf
--rw-r--r--   0 danil      (501) staff       (20)    25740 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400.woff
--rw-r--r--   0 danil      (501) staff       (20)    18079 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400italic.eot
--rw-r--r--   0 danil      (501) staff       (20)    80212 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400italic.svg
--rw-r--r--   0 danil      (501) staff       (20)    34740 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400italic.ttf
--rw-r--r--   0 danil      (501) staff       (20)    20488 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400italic.woff
--rw-r--r--   0 danil      (501) staff       (20)    20859 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700.eot
--rw-r--r--   0 danil      (501) staff       (20)    76108 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700.svg
--rw-r--r--   0 danil      (501) staff       (20)    43948 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700.ttf
--rw-r--r--   0 danil      (501) staff       (20)    25232 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700.woff
--rw-r--r--   0 danil      (501) staff       (20)    18177 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700italic.eot
--rw-r--r--   0 danil      (501) staff       (20)    79742 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700italic.svg
--rw-r--r--   0 danil      (501) staff       (20)    34360 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700italic.ttf
--rw-r--r--   0 danil      (501) staff       (20)    20472 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700italic.woff
--rw-r--r--   0 danil      (501) staff       (20)    16639 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400.eot
--rw-r--r--   0 danil      (501) staff       (20)    58571 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400.svg
--rw-r--r--   0 danil      (501) staff       (20)    29288 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19216 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400.woff
--rw-r--r--   0 danil      (501) staff       (20)    15864 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400italic.eot
--rw-r--r--   0 danil      (501) staff       (20)    58853 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400italic.svg
--rw-r--r--   0 danil      (501) staff       (20)    26644 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400italic.ttf
--rw-r--r--   0 danil      (501) staff       (20)    18396 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400italic.woff
--rw-r--r--   0 danil      (501) staff       (20)    16716 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700.eot
--rw-r--r--   0 danil      (501) staff       (20)    57996 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700.svg
--rw-r--r--   0 danil      (501) staff       (20)    29704 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19332 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700.woff
--rw-r--r--   0 danil      (501) staff       (20)    16849 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700italic.eot
--rw-r--r--   0 danil      (501) staff       (20)    58214 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700italic.svg
--rw-r--r--   0 danil      (501) staff       (20)    28932 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700italic.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19444 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700italic.woff
--rw-r--r--   0 danil      (501) staff       (20)    24132 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400.eot
--rw-r--r--   0 danil      (501) staff       (20)    95257 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400.svg
--rw-r--r--   0 danil      (501) staff       (20)    42116 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400.ttf
--rw-r--r--   0 danil      (501) staff       (20)    26804 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400.woff
--rw-r--r--   0 danil      (501) staff       (20)    22002 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400italic.eot
--rw-r--r--   0 danil      (501) staff       (20)    70885 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400italic.svg
--rw-r--r--   0 danil      (501) staff       (20)    38736 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400italic.ttf
--rw-r--r--   0 danil      (501) staff       (20)    25372 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400italic.woff
--rw-r--r--   0 danil      (501) staff       (20)    27033 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700.eot
--rw-r--r--   0 danil      (501) staff       (20)    96461 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700.svg
--rw-r--r--   0 danil      (501) staff       (20)    47276 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700.ttf
--rw-r--r--   0 danil      (501) staff       (20)    30532 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700.woff
--rw-r--r--   0 danil      (501) staff       (20)    25348 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700italic.eot
--rw-r--r--   0 danil      (501) staff       (20)   107048 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700italic.svg
--rw-r--r--   0 danil      (501) staff       (20)    44008 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700italic.ttf
--rw-r--r--   0 danil      (501) staff       (20)    28060 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700italic.woff
--rw-r--r--   0 danil      (501) staff       (20)    14004 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_400.eot
--rw-r--r--   0 danil      (501) staff       (20)    61056 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_400.svg
--rw-r--r--   0 danil      (501) staff       (20)    27916 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_400.ttf
--rw-r--r--   0 danil      (501) staff       (20)    15640 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_400.woff
--rw-r--r--   0 danil      (501) staff       (20)    13750 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_700.eot
--rw-r--r--   0 danil      (501) staff       (20)    59518 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_700.svg
--rw-r--r--   0 danil      (501) staff       (20)    27696 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_700.ttf
--rw-r--r--   0 danil      (501) staff       (20)    15340 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_700.woff
--rw-r--r--   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.398902 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.439115 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/
--rw-r--r--   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/open-sans/stylesheet.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.444061 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.452496 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/
--rw-r--r--   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
--rw-r--r--   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
--rw-r--r--   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
--rw-r--r--   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
--rw-r--r--   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
--rw-r--r--   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
--rw-r--r--   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/LICENSE.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.460302 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/
--rw-r--r--   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
--rw-r--r--   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
--rw-r--r--   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
--rw-r--r--   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
--rw-r--r--   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
--rw-r--r--   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
--rw-r--r--   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/README.md
--rw-r--r--   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/ReadMe.html
--rw-r--r--   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.468248 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/
--rw-r--r--   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
--rw-r--r--   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
--rw-r--r--   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
--rw-r--r--   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
--rw-r--r--   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
--rw-r--r--   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.230913 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.472727 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/
--rw-r--r--   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.478766 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/
--rw-r--r--   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/bower.json
--rw-r--r--   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/source-serif-pro.css
--rw-r--r--   0 danil      (501) staff       (20)    18299 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/_static/guzzle.css
--rw-r--r--   0 danil      (501) staff       (20)     1912 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-example.png
--rw-r--r--   0 danil      (501) staff       (20)     1478 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-important.png
--rw-r--r--   0 danil      (501) staff       (20)     1234 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-javascript-example.png
--rw-r--r--   0 danil      (501) staff       (20)     1086 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-json-example.png
--rw-r--r--   0 danil      (501) staff       (20)     1526 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-lconf-example.png
--rw-r--r--   0 danil      (501) staff       (20)     2331 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-note.png
--rw-r--r--   0 danil      (501) staff       (20)      679 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-optional.png
--rw-r--r--   0 danil      (501) staff       (20)      759 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-python-example.png
--rw-r--r--   0 danil      (501) staff       (20)     1701 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-seealso.png
--rw-r--r--   0 danil      (501) staff       (20)     1082 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-shell-example.png
--rw-r--r--   0 danil      (501) staff       (20)     1912 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-text-example.png
--rw-r--r--   0 danil      (501) staff       (20)      587 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-tip.png
--rw-r--r--   0 danil      (501) staff       (20)     2271 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-todo.png
--rw-r--r--   0 danil      (501) staff       (20)     1962 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/icon-warning.png
--rw-r--r--   0 danil      (501) staff       (20)   280364 2020-02-10 16:38:31.000000 verstack-3.6.7/docs/build/html/_static/jquery-3.4.1.js
--rw-r--r--   0 danil      (501) staff       (20)   287630 2020-09-20 11:51:08.000000 verstack-3.6.7/docs/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 danil      (501) staff       (20)     3510 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/jquery.cookie.js
--rw-r--r--   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/jquery.js
--rw-r--r--   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/jquery.min.map
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.480146 verstack-3.6.7/docs/build/html/_static/js/
--rw-r--r--   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/js/bootstrap.js
--rw-r--r--   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/build/html/_static/js/bootstrap.min.js
--rw-r--r--   0 danil      (501) staff       (20)    10854 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/_static/language_data.js
--rw-r--r--   0 danil      (501) staff       (20)    14747 2020-09-20 11:42:10.000000 verstack-3.6.7/docs/build/html/_static/local_fonts.css
--rw-r--r--   0 danil      (501) staff       (20)       90 2020-02-10 16:38:31.000000 verstack-3.6.7/docs/build/html/_static/minus.png
--rw-r--r--   0 danil      (501) staff       (20)    27652 2020-09-20 11:45:40.000000 verstack-3.6.7/docs/build/html/_static/p_sphinx_theme.css
--rw-r--r--   0 danil      (501) staff       (20)    17752 2020-09-20 11:45:40.000000 verstack-3.6.7/docs/build/html/_static/p_sphinx_theme.js
--rw-r--r--   0 danil      (501) staff       (20)       90 2020-02-10 16:38:31.000000 verstack-3.6.7/docs/build/html/_static/plus.png
--rw-r--r--   0 danil      (501) staff       (20)     4846 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/_static/pygments.css
--rw-r--r--   0 danil      (501) staff       (20)    16578 2021-08-12 13:47:18.000000 verstack-3.6.7/docs/build/html/_static/searchtools.js
--rw-r--r--   0 danil      (501) staff       (20)    67692 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/build/html/_static/underscore-1.12.0.js
--rw-r--r--   0 danil      (501) staff       (20)    68420 2021-08-12 13:47:18.000000 verstack-3.6.7/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 danil      (501) staff       (20)    35168 2020-02-10 16:38:31.000000 verstack-3.6.7/docs/build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 danil      (501) staff       (20)    19358 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/build/html/_static/underscore.js
--rw-r--r--   0 danil      (501) staff       (20)     3419 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/genindex.html
--rw-r--r--   0 danil      (501) staff       (20)    72729 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/index.html
--rw-r--r--   0 danil      (501) staff       (20)      254 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/objects.inv
--rw-r--r--   0 danil      (501) staff       (20)     4531 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/search.html
--rw-r--r--   0 danil      (501) staff       (20)     4971 2021-12-07 08:59:04.000000 verstack-3.6.7/docs/build/html/searchindex.js
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.480696 verstack-3.6.7/docs/guzzle_sphinx_theme/
--rw-r--r--   0 danil      (501) staff       (20)     4856 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/__init__.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.481277 verstack-3.6.7/docs/guzzle_sphinx_theme/__pycache__/
--rw-r--r--   0 danil      (501) staff       (20)     5478 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/__pycache__/__init__.cpython-37.pyc
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.484962 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/
--rw-r--r--   0 danil      (501) staff       (20)      828 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/comments.html
--rw-r--r--   0 danil      (501) staff       (20)      323 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/globaltoc.html
--rw-r--r--   0 danil      (501) staff       (20)     5778 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/layout.html
--rw-r--r--   0 danil      (501) staff       (20)      206 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/localtoc.html
--rw-r--r--   0 danil      (501) staff       (20)       92 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/logo-text.html
--rw-r--r--   0 danil      (501) staff       (20)     1695 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/search.html
--rw-r--r--   0 danil      (501) staff       (20)      521 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/searchbox.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.487150 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.489110 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/
--rwxr-xr-x   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap-theme.min.css
--rwxr-xr-x   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap.min.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.492716 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/
--rwxr-xr-x   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.493386 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.524407 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/
--rwxr-xr-x   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
--rwxr-xr-x   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
--rwxr-xr-x   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
--rwxr-xr-x   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/stylesheet.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.529992 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.535855 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/
--rwxr-xr-x   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
--rwxr-xr-x   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
--rwxr-xr-x   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
--rwxr-xr-x   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
--rwxr-xr-x   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
--rwxr-xr-x   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
--rwxr-xr-x   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/LICENSE.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.543249 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/
--rwxr-xr-x   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
--rwxr-xr-x   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
--rwxr-xr-x   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
--rwxr-xr-x   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
--rwxr-xr-x   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
--rwxr-xr-x   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
--rwxr-xr-x   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/README.md
--rwxr-xr-x   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/ReadMe.html
--rwxr-xr-x   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/SourceSerifProReadMe.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.549712 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/
--rwxr-xr-x   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
--rwxr-xr-x   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.234761 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.555783 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/
--rwxr-xr-x   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.561007 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/
--rwxr-xr-x   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
--rwxr-xr-x   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/bower.json
--rwxr-xr-x   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/source-serif-pro.css
--rw-r--r--   0 danil      (501) staff       (20)    18300 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/guzzle.css_t
--rw-r--r--   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.js
--rwxr-xr-x   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.min.map
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.562653 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/
--rw-r--r--   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.js
--rwxr-xr-x   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.min.js
--rw-r--r--   0 danil      (501) staff       (20)      649 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/theme.conf
--rw-r--r--   0 danil      (501) staff       (20)      799 2020-09-20 09:39:03.000000 verstack-3.6.7/docs/make.bat
--rw-r--r--   0 danil      (501) staff       (20)       47 2021-11-08 12:54:50.000000 verstack-3.6.7/docs/requirements.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.563930 verstack-3.6.7/docs/source/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.235779 verstack-3.6.7/docs/source/_build/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.569286 verstack-3.6.7/docs/source/_build/html/
--rw-r--r--   0 danil      (501) staff       (20)      230 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/.buildinfo
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.570731 verstack-3.6.7/docs/source/_build/html/.doctrees/
--rw-r--r--   0 danil      (501) staff       (20)    34100 2022-02-10 20:51:19.000000 verstack-3.6.7/docs/source/_build/html/.doctrees/environment.pickle
--rw-r--r--   0 danil      (501) staff       (20)   233769 2022-02-10 20:51:19.000000 verstack-3.6.7/docs/source/_build/html/.doctrees/index.doctree
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.572376 verstack-3.6.7/docs/source/_build/html/_sources/
--rw-r--r--   0 danil      (501) staff       (20)    42285 2022-02-10 20:51:17.000000 verstack-3.6.7/docs/source/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.584418 verstack-3.6.7/docs/source/_build/html/_static/
--rw-r--r--   0 danil      (501) staff       (20)    14652 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/_static/basic.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.585575 verstack-3.6.7/docs/source/_build/html/_static/css/
--rw-r--r--   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/css/bootstrap-theme.min.css
--rw-r--r--   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/css/bootstrap.min.css
--rw-r--r--   0 danil      (501) staff       (20)     9592 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/source/_build/html/_static/doctools.js
--rw-r--r--   0 danil      (501) staff       (20)      355 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/_static/documentation_options.js
--rw-r--r--   0 danil      (501) staff       (20)      286 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/source/_build/html/_static/file.png
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.588649 verstack-3.6.7/docs/source/_build/html/_static/fonts/
--rw-r--r--   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.589113 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.632116 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/
--rw-r--r--   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
--rw-r--r--   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
--rw-r--r--   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
--rw-r--r--   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
--rw-r--r--   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/stylesheet.css
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.634942 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.642824 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/
--rw-r--r--   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
--rw-r--r--   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
--rw-r--r--   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
--rw-r--r--   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
--rw-r--r--   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
--rw-r--r--   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
--rw-r--r--   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/LICENSE.txt
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.649725 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/
--rw-r--r--   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
--rw-r--r--   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
--rw-r--r--   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
--rw-r--r--   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
--rw-r--r--   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
--rw-r--r--   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
--rw-r--r--   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/README.md
--rw-r--r--   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/ReadMe.html
--rw-r--r--   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.658616 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/
--rw-r--r--   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
--rw-r--r--   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
--rw-r--r--   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
--rw-r--r--   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
--rw-r--r--   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
--rw-r--r--   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.239159 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.664561 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/
--rw-r--r--   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
--rw-r--r--   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.669449 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/
--rw-r--r--   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
--rw-r--r--   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/bower.json
--rw-r--r--   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/source-serif-pro.css
--rw-r--r--   0 danil      (501) staff       (20)    18299 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/_static/guzzle.css
--rw-r--r--   0 danil      (501) staff       (20)   287630 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/source/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/jquery.js
--rw-r--r--   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/jquery.min.map
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.670613 verstack-3.6.7/docs/source/_build/html/_static/js/
--rw-r--r--   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/js/bootstrap.js
--rw-r--r--   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.6.7/docs/source/_build/html/_static/js/bootstrap.min.js
--rw-r--r--   0 danil      (501) staff       (20)    10854 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/_static/language_data.js
--rw-r--r--   0 danil      (501) staff       (20)       90 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/source/_build/html/_static/minus.png
--rw-r--r--   0 danil      (501) staff       (20)       90 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/source/_build/html/_static/plus.png
--rw-r--r--   0 danil      (501) staff       (20)     4846 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/_static/pygments.css
--rw-r--r--   0 danil      (501) staff       (20)    16578 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/source/_build/html/_static/searchtools.js
--rw-r--r--   0 danil      (501) staff       (20)    67692 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/source/_build/html/_static/underscore-1.12.0.js
--rw-r--r--   0 danil      (501) staff       (20)    19358 2021-05-11 23:58:54.000000 verstack-3.6.7/docs/source/_build/html/_static/underscore.js
--rw-r--r--   0 danil      (501) staff       (20)     3419 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/genindex.html
--rw-r--r--   0 danil      (501) staff       (20)   101829 2022-02-10 20:51:19.000000 verstack-3.6.7/docs/source/_build/html/index.html
--rw-r--r--   0 danil      (501) staff       (20)      254 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/objects.inv
--rw-r--r--   0 danil      (501) staff       (20)     4531 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/search.html
--rw-r--r--   0 danil      (501) staff       (20)     6846 2022-02-10 20:51:20.000000 verstack-3.6.7/docs/source/_build/html/searchindex.js
--rw-r--r--   0 danil      (501) staff       (20)     5223 2022-02-10 20:40:52.000000 verstack-3.6.7/docs/source/conf.py
--rw-r--r--   0 danil      (501) staff       (20)    70759 2023-03-28 10:23:26.000000 verstack-3.6.7/docs/source/index.rst
--rw-r--r--   0 danil      (501) staff       (20)      548 2023-02-12 13:52:00.000000 verstack-3.6.7/increment_version.py
--rw-r--r--   0 danil      (501) staff       (20)   253628 2023-02-12 13:48:06.000000 verstack-3.6.7/logo.png
--rw-r--r--   0 danil      (501) staff       (20)   200067 2023-02-12 13:48:04.000000 verstack-3.6.7/logo.pxd
--rw-r--r--   0 danil      (501) staff       (20)     1703 2023-02-12 13:53:15.000000 verstack-3.6.7/package_update_instructions.txt
--rw-r--r--   0 danil      (501) staff       (20)      310 2023-01-13 15:33:39.000000 verstack-3.6.7/requirements.txt
--rw-r--r--   0 danil      (501) staff       (20)       80 2023-03-28 10:32:07.717004 verstack-3.6.7/setup.cfg
--rw-r--r--   0 danil      (501) staff       (20)     2188 2023-03-28 10:24:47.000000 verstack-3.6.7/setup.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.679758 verstack-3.6.7/verstack/
--rw-r--r--   0 danil      (501) staff       (20)    39819 2023-01-16 10:00:49.000000 verstack-3.6.7/verstack/DateParser.py
--rw-r--r--   0 danil      (501) staff       (20)    24902 2022-06-21 13:31:01.000000 verstack-3.6.7/verstack/FeatureSelector.py
--rw-r--r--   0 danil      (501) staff       (20)     7756 2022-04-29 08:46:57.000000 verstack-3.6.7/verstack/Multicore.py
--rwxr-xr-x   0 danil      (501) staff       (20)    18447 2022-12-09 20:53:43.000000 verstack-3.6.7/verstack/NaNImputer.py
--rw-r--r--   0 danil      (501) staff       (20)    33143 2022-12-09 20:16:44.000000 verstack-3.6.7/verstack/NaNImputerLegacy.py
--rw-r--r--   0 danil      (501) staff       (20)    12408 2022-12-19 10:43:57.000000 verstack-3.6.7/verstack/PandasOptimizer.py
--rw-r--r--   0 danil      (501) staff       (20)     8816 2023-03-28 10:21:12.000000 verstack-3.6.7/verstack/ThreshTuner.py
--rw-r--r--   0 danil      (501) staff       (20)      980 2022-12-19 08:48:26.000000 verstack-3.6.7/verstack/__init__.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.684889 verstack-3.6.7/verstack/categoric_encoders/
--rw-r--r--   0 danil      (501) staff       (20)     5115 2022-04-29 12:08:27.000000 verstack-3.6.7/verstack/categoric_encoders/Factorizer.py
--rw-r--r--   0 danil      (501) staff       (20)     4669 2022-04-28 10:31:19.000000 verstack-3.6.7/verstack/categoric_encoders/FrequencyEncoder.py
--rw-r--r--   0 danil      (501) staff       (20)     7499 2023-01-11 14:23:40.000000 verstack-3.6.7/verstack/categoric_encoders/MeanTargetEncoder.py
--rw-r--r--   0 danil      (501) staff       (20)     6647 2022-04-28 09:22:13.000000 verstack-3.6.7/verstack/categoric_encoders/OneHotEncoder.py
--rw-r--r--   0 danil      (501) staff       (20)     7352 2022-04-28 09:22:53.000000 verstack-3.6.7/verstack/categoric_encoders/WeightOfEvidenceEncoder.py
--rw-r--r--   0 danil      (501) staff       (20)        0 2021-12-07 14:06:33.000000 verstack-3.6.7/verstack/categoric_encoders/__init__.py
--rw-r--r--   0 danil      (501) staff       (20)     2173 2021-12-06 19:04:49.000000 verstack-3.6.7/verstack/categoric_encoders/args_validators.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.687322 verstack-3.6.7/verstack/lgbm_optuna_tuning/
--rw-r--r--   0 danil      (501) staff       (20)    48712 2023-01-11 14:00:27.000000 verstack-3.6.7/verstack/lgbm_optuna_tuning/LGBMTuner.py
--rw-r--r--   0 danil      (501) staff       (20)        0 2021-12-22 20:41:08.000000 verstack-3.6.7/verstack/lgbm_optuna_tuning/__init__.py
--rw-r--r--   0 danil      (501) staff       (20)     2229 2021-12-24 13:13:34.000000 verstack-3.6.7/verstack/lgbm_optuna_tuning/args_validators.py
--rw-r--r--   0 danil      (501) staff       (20)    17600 2022-06-17 08:57:23.000000 verstack-3.6.7/verstack/lgbm_optuna_tuning/lgb_metrics.py
--rw-r--r--   0 danil      (501) staff       (20)      859 2021-12-21 19:02:16.000000 verstack-3.6.7/verstack/lgbm_optuna_tuning/optuna_tools.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.694525 verstack-3.6.7/verstack/stacking/
--rw-r--r--   0 danil      (501) staff       (20)    30222 2022-12-11 11:13:47.000000 verstack-3.6.7/verstack/stacking/Stacker.py
--rw-r--r--   0 danil      (501) staff       (20)        0 2022-04-04 06:15:43.000000 verstack-3.6.7/verstack/stacking/__init__.py
--rw-r--r--   0 danil      (501) staff       (20)     2371 2022-05-04 09:07:10.000000 verstack-3.6.7/verstack/stacking/args_validators.py
--rw-r--r--   0 danil      (501) staff       (20)     3627 2022-04-05 06:23:16.000000 verstack-3.6.7/verstack/stacking/generate_default_layers.py
--rw-r--r--   0 danil      (501) staff       (20)     5430 2022-03-31 15:35:58.000000 verstack-3.6.7/verstack/stacking/kerasModel.py
--rw-r--r--   0 danil      (501) staff       (20)     3033 2022-12-11 11:14:24.000000 verstack-3.6.7/verstack/stacking/load_stacker.py
--rw-r--r--   0 danil      (501) staff       (20)     7657 2022-04-28 09:37:07.000000 verstack-3.6.7/verstack/stacking/optimise_params.py
--rwxr-xr-x   0 danil      (501) staff       (20)     8946 2023-02-12 14:01:23.000000 verstack-3.6.7/verstack/stratified_continuous_split.py
--rw-r--r--   0 danil      (501) staff       (20)     3523 2022-06-09 19:16:34.000000 verstack-3.6.7/verstack/tools.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.715758 verstack-3.6.7/verstack/unittest/
--rw-r--r--   0 danil      (501) staff       (20)     2443 2023-01-16 10:07:03.000000 verstack-3.6.7/verstack/unittest/common.py
--rw-r--r--   0 danil      (501) staff       (20)      373 2023-01-16 10:07:50.000000 verstack-3.6.7/verstack/unittest/test_DateParser.py
--rw-r--r--   0 danil      (501) staff       (20)      939 2022-12-06 11:05:04.000000 verstack-3.6.7/verstack/unittest/test_Factorizer.py
--rw-r--r--   0 danil      (501) staff       (20)      984 2022-12-06 11:13:56.000000 verstack-3.6.7/verstack/unittest/test_FrequencyEncoder.py
--rw-r--r--   0 danil      (501) staff       (20)      654 2022-12-06 11:18:41.000000 verstack-3.6.7/verstack/unittest/test_LGBMTuner.py
--rw-r--r--   0 danil      (501) staff       (20)      791 2022-12-06 11:20:55.000000 verstack-3.6.7/verstack/unittest/test_MeanTargetEncoder.py
--rw-r--r--   0 danil      (501) staff       (20)      600 2022-12-06 11:33:00.000000 verstack-3.6.7/verstack/unittest/test_Multicore.py
--rw-r--r--   0 danil      (501) staff       (20)      393 2022-12-06 11:34:15.000000 verstack-3.6.7/verstack/unittest/test_NaNImputer.py
--rw-r--r--   0 danil      (501) staff       (20)      531 2022-12-06 11:35:42.000000 verstack-3.6.7/verstack/unittest/test_OneHotEncoder.py
--rw-r--r--   0 danil      (501) staff       (20)      414 2022-12-19 09:08:24.000000 verstack-3.6.7/verstack/unittest/test_PandasOptimizer.py
--rw-r--r--   0 danil      (501) staff       (20)      336 2022-12-06 11:37:18.000000 verstack-3.6.7/verstack/unittest/test_Printer.py
--rw-r--r--   0 danil      (501) staff       (20)     1726 2022-12-11 12:01:19.000000 verstack-3.6.7/verstack/unittest/test_Stacker.py
--rw-r--r--   0 danil      (501) staff       (20)      710 2022-12-13 07:01:40.000000 verstack-3.6.7/verstack/unittest/test_ThreshTuner.py
--rw-r--r--   0 danil      (501) staff       (20)      863 2022-12-06 14:19:28.000000 verstack-3.6.7/verstack/unittest/test_WeightOfEvidenceEncoder.py
--rw-r--r--   0 danil      (501) staff       (20)      604 2022-12-06 14:16:48.000000 verstack-3.6.7/verstack/unittest/test_stratified_continuous_split.py
--rw-r--r--   0 danil      (501) staff       (20)     1370 2022-12-06 14:58:08.000000 verstack-3.6.7/verstack/unittest/unittesting_manual.txt
--rw-r--r--   0 danil      (501) staff       (20)       21 2023-03-28 10:23:26.000000 verstack-3.6.7/verstack/version.py
-drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-03-28 10:32:07.681625 verstack-3.6.7/verstack.egg-info/
--rw-r--r--   0 danil      (501) staff       (20)     3361 2023-03-28 10:32:06.000000 verstack-3.6.7/verstack.egg-info/PKG-INFO
--rw-r--r--   0 danil      (501) staff       (20)    31402 2023-03-28 10:32:07.000000 verstack-3.6.7/verstack.egg-info/SOURCES.txt
--rw-r--r--   0 danil      (501) staff       (20)        1 2023-03-28 10:32:06.000000 verstack-3.6.7/verstack.egg-info/dependency_links.txt
--rw-r--r--   0 danil      (501) staff       (20)      271 2023-03-28 10:32:06.000000 verstack-3.6.7/verstack.egg-info/requires.txt
--rw-r--r--   0 danil      (501) staff       (20)        9 2023-03-28 10:32:06.000000 verstack-3.6.7/verstack.egg-info/top_level.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.079571 verstack-3.7.0/
+-rw-r--r--   0 danil      (501) staff       (20)      174 2021-11-08 12:56:11.000000 verstack-3.7.0/.readthedocs.yaml
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.376980 verstack-3.7.0/.vscode/
+-rw-r--r--   0 danil      (501) staff       (20)      121 2022-10-18 14:42:35.000000 verstack-3.7.0/.vscode/settings.json
+-rw-r--r--   0 danil      (501) staff       (20)     1071 2020-09-18 21:03:44.000000 verstack-3.7.0/LICENSE.txt
+-rw-r--r--   0 danil      (501) staff       (20)      106 2020-09-18 21:51:05.000000 verstack-3.7.0/MANIFEST
+-rw-r--r--   0 danil      (501) staff       (20)     3361 2023-05-03 13:12:39.079894 verstack-3.7.0/PKG-INFO
+-rw-r--r--   0 danil      (501) staff       (20)     2266 2023-05-03 13:09:53.000000 verstack-3.7.0/README.rst
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.377669 verstack-3.7.0/dist/
+-rw-r--r--   0 danil      (501) staff       (20)     7308 2020-09-18 21:51:05.000000 verstack-3.7.0/dist/verstack-0.1.0.tar.gz
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.381412 verstack-3.7.0/docs/
+-rw-r--r--   0 danil      (501) staff       (20)      692 2023-02-12 13:53:02.000000 verstack-3.7.0/docs/Doc_update_manual.txt
+-rw-r--r--   0 danil      (501) staff       (20)      638 2020-09-20 09:39:03.000000 verstack-3.7.0/docs/Makefile
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.346720 verstack-3.7.0/docs/build/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.385054 verstack-3.7.0/docs/build/doctrees/
+-rw-r--r--   0 danil      (501) staff       (20)    26942 2020-09-20 12:30:25.000000 verstack-3.7.0/docs/build/doctrees/README.doctree
+-rw-r--r--   0 danil      (501) staff       (20)    30868 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/doctrees/environment.pickle
+-rw-r--r--   0 danil      (501) staff       (20)   166536 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/doctrees/index.doctree
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.394826 verstack-3.7.0/docs/build/html/
+-rw-r--r--   0 danil      (501) staff       (20)      230 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/.buildinfo
+-rw-r--r--   0 danil      (501) staff       (20)        0 2020-09-20 11:46:51.000000 verstack-3.7.0/docs/build/html/.nojekyll
+-rw-r--r--   0 danil      (501) staff       (20)    20042 2020-09-20 12:35:34.000000 verstack-3.7.0/docs/build/html/README.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.397446 verstack-3.7.0/docs/build/html/_sources/
+-rw-r--r--   0 danil      (501) staff       (20)     6117 2020-09-19 13:46:17.000000 verstack-3.7.0/docs/build/html/_sources/README.md.txt
+-rw-r--r--   0 danil      (501) staff       (20)     6298 2020-09-20 09:22:18.000000 verstack-3.7.0/docs/build/html/_sources/README.rst.txt
+-rw-r--r--   0 danil      (501) staff       (20)    28954 2021-12-07 08:58:57.000000 verstack-3.7.0/docs/build/html/_sources/index.rst.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.443735 verstack-3.7.0/docs/build/html/_static/
+-rw-r--r--   0 danil      (501) staff       (20)    11185 2020-09-20 11:40:14.000000 verstack-3.7.0/docs/build/html/_static/alabaster.css
+-rw-r--r--   0 danil      (501) staff       (20)    14652 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/_static/basic.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.445791 verstack-3.7.0/docs/build/html/_static/css/
+-rw-r--r--   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/css/bootstrap-theme.min.css
+-rw-r--r--   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/css/bootstrap.min.css
+-rw-r--r--   0 danil      (501) staff       (20)       42 2018-10-08 18:31:32.000000 verstack-3.7.0/docs/build/html/_static/custom.css
+-rw-r--r--   0 danil      (501) staff       (20)     9592 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/build/html/_static/doctools.js
+-rw-r--r--   0 danil      (501) staff       (20)      355 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/_static/documentation_options.js
+-rw-r--r--   0 danil      (501) staff       (20)      286 2020-02-10 16:38:31.000000 verstack-3.7.0/docs/build/html/_static/file.png
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.543723 verstack-3.7.0/docs/build/html/_static/fonts/
+-rw-r--r--   0 danil      (501) staff       (20)    18173 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Droid_Sans_Mono_400.eot
+-rw-r--r--   0 danil      (501) staff       (20)    47724 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Droid_Sans_Mono_400.svg
+-rw-r--r--   0 danil      (501) staff       (20)    31552 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Droid_Sans_Mono_400.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    21624 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Droid_Sans_Mono_400.woff
+-rw-r--r--   0 danil      (501) staff       (20)    21280 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400.eot
+-rw-r--r--   0 danil      (501) staff       (20)    76169 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400.svg
+-rw-r--r--   0 danil      (501) staff       (20)    45116 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    25740 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400.woff
+-rw-r--r--   0 danil      (501) staff       (20)    18079 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400italic.eot
+-rw-r--r--   0 danil      (501) staff       (20)    80212 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400italic.svg
+-rw-r--r--   0 danil      (501) staff       (20)    34740 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400italic.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    20488 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400italic.woff
+-rw-r--r--   0 danil      (501) staff       (20)    20859 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700.eot
+-rw-r--r--   0 danil      (501) staff       (20)    76108 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700.svg
+-rw-r--r--   0 danil      (501) staff       (20)    43948 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    25232 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700.woff
+-rw-r--r--   0 danil      (501) staff       (20)    18177 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700italic.eot
+-rw-r--r--   0 danil      (501) staff       (20)    79742 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700italic.svg
+-rw-r--r--   0 danil      (501) staff       (20)    34360 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700italic.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    20472 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700italic.woff
+-rw-r--r--   0 danil      (501) staff       (20)    16639 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400.eot
+-rw-r--r--   0 danil      (501) staff       (20)    58571 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400.svg
+-rw-r--r--   0 danil      (501) staff       (20)    29288 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19216 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400.woff
+-rw-r--r--   0 danil      (501) staff       (20)    15864 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400italic.eot
+-rw-r--r--   0 danil      (501) staff       (20)    58853 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400italic.svg
+-rw-r--r--   0 danil      (501) staff       (20)    26644 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400italic.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    18396 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400italic.woff
+-rw-r--r--   0 danil      (501) staff       (20)    16716 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700.eot
+-rw-r--r--   0 danil      (501) staff       (20)    57996 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700.svg
+-rw-r--r--   0 danil      (501) staff       (20)    29704 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19332 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700.woff
+-rw-r--r--   0 danil      (501) staff       (20)    16849 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700italic.eot
+-rw-r--r--   0 danil      (501) staff       (20)    58214 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700italic.svg
+-rw-r--r--   0 danil      (501) staff       (20)    28932 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700italic.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19444 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700italic.woff
+-rw-r--r--   0 danil      (501) staff       (20)    24132 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400.eot
+-rw-r--r--   0 danil      (501) staff       (20)    95257 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400.svg
+-rw-r--r--   0 danil      (501) staff       (20)    42116 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    26804 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400.woff
+-rw-r--r--   0 danil      (501) staff       (20)    22002 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400italic.eot
+-rw-r--r--   0 danil      (501) staff       (20)    70885 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400italic.svg
+-rw-r--r--   0 danil      (501) staff       (20)    38736 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400italic.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    25372 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400italic.woff
+-rw-r--r--   0 danil      (501) staff       (20)    27033 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700.eot
+-rw-r--r--   0 danil      (501) staff       (20)    96461 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700.svg
+-rw-r--r--   0 danil      (501) staff       (20)    47276 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    30532 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700.woff
+-rw-r--r--   0 danil      (501) staff       (20)    25348 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700italic.eot
+-rw-r--r--   0 danil      (501) staff       (20)   107048 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700italic.svg
+-rw-r--r--   0 danil      (501) staff       (20)    44008 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700italic.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    28060 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700italic.woff
+-rw-r--r--   0 danil      (501) staff       (20)    14004 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_400.eot
+-rw-r--r--   0 danil      (501) staff       (20)    61056 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_400.svg
+-rw-r--r--   0 danil      (501) staff       (20)    27916 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_400.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    15640 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_400.woff
+-rw-r--r--   0 danil      (501) staff       (20)    13750 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_700.eot
+-rw-r--r--   0 danil      (501) staff       (20)    59518 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_700.svg
+-rw-r--r--   0 danil      (501) staff       (20)    27696 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_700.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    15340 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_700.woff
+-rw-r--r--   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.544979 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.605703 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/
+-rw-r--r--   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/open-sans/stylesheet.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.612423 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.625639 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/
+-rw-r--r--   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
+-rw-r--r--   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
+-rw-r--r--   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
+-rw-r--r--   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
+-rw-r--r--   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
+-rw-r--r--   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
+-rw-r--r--   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/LICENSE.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.638754 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/
+-rw-r--r--   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
+-rw-r--r--   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
+-rw-r--r--   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
+-rw-r--r--   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
+-rw-r--r--   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
+-rw-r--r--   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
+-rw-r--r--   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/README.md
+-rw-r--r--   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/ReadMe.html
+-rw-r--r--   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.651771 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/
+-rw-r--r--   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.350414 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.660062 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/
+-rw-r--r--   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.670317 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/
+-rw-r--r--   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/bower.json
+-rw-r--r--   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/source-serif-pro.css
+-rw-r--r--   0 danil      (501) staff       (20)    18299 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/_static/guzzle.css
+-rw-r--r--   0 danil      (501) staff       (20)     1912 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-example.png
+-rw-r--r--   0 danil      (501) staff       (20)     1478 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-important.png
+-rw-r--r--   0 danil      (501) staff       (20)     1234 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-javascript-example.png
+-rw-r--r--   0 danil      (501) staff       (20)     1086 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-json-example.png
+-rw-r--r--   0 danil      (501) staff       (20)     1526 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-lconf-example.png
+-rw-r--r--   0 danil      (501) staff       (20)     2331 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-note.png
+-rw-r--r--   0 danil      (501) staff       (20)      679 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-optional.png
+-rw-r--r--   0 danil      (501) staff       (20)      759 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-python-example.png
+-rw-r--r--   0 danil      (501) staff       (20)     1701 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-seealso.png
+-rw-r--r--   0 danil      (501) staff       (20)     1082 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-shell-example.png
+-rw-r--r--   0 danil      (501) staff       (20)     1912 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-text-example.png
+-rw-r--r--   0 danil      (501) staff       (20)      587 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-tip.png
+-rw-r--r--   0 danil      (501) staff       (20)     2271 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-todo.png
+-rw-r--r--   0 danil      (501) staff       (20)     1962 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/icon-warning.png
+-rw-r--r--   0 danil      (501) staff       (20)   280364 2020-02-10 16:38:31.000000 verstack-3.7.0/docs/build/html/_static/jquery-3.4.1.js
+-rw-r--r--   0 danil      (501) staff       (20)   287630 2020-09-20 11:51:08.000000 verstack-3.7.0/docs/build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 danil      (501) staff       (20)     3510 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/jquery.cookie.js
+-rw-r--r--   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/jquery.js
+-rw-r--r--   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/jquery.min.map
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.672760 verstack-3.7.0/docs/build/html/_static/js/
+-rw-r--r--   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/js/bootstrap.js
+-rw-r--r--   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/build/html/_static/js/bootstrap.min.js
+-rw-r--r--   0 danil      (501) staff       (20)    10854 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/_static/language_data.js
+-rw-r--r--   0 danil      (501) staff       (20)    14747 2020-09-20 11:42:10.000000 verstack-3.7.0/docs/build/html/_static/local_fonts.css
+-rw-r--r--   0 danil      (501) staff       (20)       90 2020-02-10 16:38:31.000000 verstack-3.7.0/docs/build/html/_static/minus.png
+-rw-r--r--   0 danil      (501) staff       (20)    27652 2020-09-20 11:45:40.000000 verstack-3.7.0/docs/build/html/_static/p_sphinx_theme.css
+-rw-r--r--   0 danil      (501) staff       (20)    17752 2020-09-20 11:45:40.000000 verstack-3.7.0/docs/build/html/_static/p_sphinx_theme.js
+-rw-r--r--   0 danil      (501) staff       (20)       90 2020-02-10 16:38:31.000000 verstack-3.7.0/docs/build/html/_static/plus.png
+-rw-r--r--   0 danil      (501) staff       (20)     4846 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/_static/pygments.css
+-rw-r--r--   0 danil      (501) staff       (20)    16578 2021-08-12 13:47:18.000000 verstack-3.7.0/docs/build/html/_static/searchtools.js
+-rw-r--r--   0 danil      (501) staff       (20)    67692 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/build/html/_static/underscore-1.12.0.js
+-rw-r--r--   0 danil      (501) staff       (20)    68420 2021-08-12 13:47:18.000000 verstack-3.7.0/docs/build/html/_static/underscore-1.13.1.js
+-rw-r--r--   0 danil      (501) staff       (20)    35168 2020-02-10 16:38:31.000000 verstack-3.7.0/docs/build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 danil      (501) staff       (20)    19358 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/build/html/_static/underscore.js
+-rw-r--r--   0 danil      (501) staff       (20)     3419 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/genindex.html
+-rw-r--r--   0 danil      (501) staff       (20)    72729 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/index.html
+-rw-r--r--   0 danil      (501) staff       (20)      254 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/objects.inv
+-rw-r--r--   0 danil      (501) staff       (20)     4531 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/search.html
+-rw-r--r--   0 danil      (501) staff       (20)     4971 2021-12-07 08:59:04.000000 verstack-3.7.0/docs/build/html/searchindex.js
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.673764 verstack-3.7.0/docs/guzzle_sphinx_theme/
+-rw-r--r--   0 danil      (501) staff       (20)     4856 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/__init__.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.674340 verstack-3.7.0/docs/guzzle_sphinx_theme/__pycache__/
+-rw-r--r--   0 danil      (501) staff       (20)     5478 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/__pycache__/__init__.cpython-37.pyc
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.683577 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/
+-rw-r--r--   0 danil      (501) staff       (20)      828 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/comments.html
+-rw-r--r--   0 danil      (501) staff       (20)      323 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/globaltoc.html
+-rw-r--r--   0 danil      (501) staff       (20)     5778 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/layout.html
+-rw-r--r--   0 danil      (501) staff       (20)      206 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/localtoc.html
+-rw-r--r--   0 danil      (501) staff       (20)       92 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/logo-text.html
+-rw-r--r--   0 danil      (501) staff       (20)     1695 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/search.html
+-rw-r--r--   0 danil      (501) staff       (20)      521 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/searchbox.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.687192 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.690197 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/
+-rwxr-xr-x   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap-theme.min.css
+-rwxr-xr-x   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap.min.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.696304 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/
+-rwxr-xr-x   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.697804 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.754908 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/
+-rwxr-xr-x   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
+-rwxr-xr-x   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/stylesheet.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.760605 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.794968 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/
+-rwxr-xr-x   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
+-rwxr-xr-x   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/LICENSE.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.814812 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/
+-rwxr-xr-x   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
+-rwxr-xr-x   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
+-rwxr-xr-x   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
+-rwxr-xr-x   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
+-rwxr-xr-x   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
+-rwxr-xr-x   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
+-rwxr-xr-x   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/README.md
+-rwxr-xr-x   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/ReadMe.html
+-rwxr-xr-x   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/SourceSerifProReadMe.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.827304 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/
+-rwxr-xr-x   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
+-rwxr-xr-x   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.355276 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.842668 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/
+-rwxr-xr-x   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.854754 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/
+-rwxr-xr-x   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
+-rwxr-xr-x   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/bower.json
+-rwxr-xr-x   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/source-serif-pro.css
+-rw-r--r--   0 danil      (501) staff       (20)    18300 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/guzzle.css_t
+-rw-r--r--   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.js
+-rwxr-xr-x   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.min.map
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.857967 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/
+-rw-r--r--   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.js
+-rwxr-xr-x   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.min.js
+-rw-r--r--   0 danil      (501) staff       (20)      649 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/theme.conf
+-rw-r--r--   0 danil      (501) staff       (20)      799 2020-09-20 09:39:03.000000 verstack-3.7.0/docs/make.bat
+-rw-r--r--   0 danil      (501) staff       (20)       47 2021-11-08 12:54:50.000000 verstack-3.7.0/docs/requirements.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.859727 verstack-3.7.0/docs/source/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.356341 verstack-3.7.0/docs/source/_build/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.867684 verstack-3.7.0/docs/source/_build/html/
+-rw-r--r--   0 danil      (501) staff       (20)      230 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/.buildinfo
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.870318 verstack-3.7.0/docs/source/_build/html/.doctrees/
+-rw-r--r--   0 danil      (501) staff       (20)    34100 2022-02-10 20:51:19.000000 verstack-3.7.0/docs/source/_build/html/.doctrees/environment.pickle
+-rw-r--r--   0 danil      (501) staff       (20)   233769 2022-02-10 20:51:19.000000 verstack-3.7.0/docs/source/_build/html/.doctrees/index.doctree
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.872966 verstack-3.7.0/docs/source/_build/html/_sources/
+-rw-r--r--   0 danil      (501) staff       (20)    42285 2022-02-10 20:51:17.000000 verstack-3.7.0/docs/source/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.893702 verstack-3.7.0/docs/source/_build/html/_static/
+-rw-r--r--   0 danil      (501) staff       (20)    14652 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/_static/basic.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.895630 verstack-3.7.0/docs/source/_build/html/_static/css/
+-rw-r--r--   0 danil      (501) staff       (20)    13353 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/css/bootstrap-theme.min.css
+-rw-r--r--   0 danil      (501) staff       (20)   102105 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/css/bootstrap.min.css
+-rw-r--r--   0 danil      (501) staff       (20)     9592 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/source/_build/html/_static/doctools.js
+-rw-r--r--   0 danil      (501) staff       (20)      355 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/_static/documentation_options.js
+-rw-r--r--   0 danil      (501) staff       (20)      286 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/source/_build/html/_static/file.png
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.903123 verstack-3.7.0/docs/source/_build/html/_static/fonts/
+-rw-r--r--   0 danil      (501) staff       (20)    20290 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 danil      (501) staff       (20)    62850 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 danil      (501) staff       (20)    41236 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    23292 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.904106 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.971586 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/
+-rw-r--r--   0 danil      (501) staff       (20)    30858 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    57401 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    30680 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19788 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    34166 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    60750 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    33960 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    21940 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    30602 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    58215 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    30404 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19972 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    33758 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    61071 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    33532 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    21824 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    34798 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    62096 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    34612 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    22416 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    29794 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    56447 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    29612 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19396 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    34578 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    62430 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    34368 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    22444 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    29934 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    58495 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    29744 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19624 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    30350 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    57560 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    30156 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    19736 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)    34866 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot
+-rw-r--r--   0 danil      (501) staff       (20)    62044 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg
+-rw-r--r--   0 danil      (501) staff       (20)    34644 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf
+-rw-r--r--   0 danil      (501) staff       (20)    22332 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff
+-rw-r--r--   0 danil      (501) staff       (20)     5151 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/stylesheet.css
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.978868 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.993008 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/
+-rw-r--r--   0 danil      (501) staff       (20)   111902 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot
+-rw-r--r--   0 danil      (501) staff       (20)   113630 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot
+-rw-r--r--   0 danil      (501) staff       (20)   112362 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot
+-rw-r--r--   0 danil      (501) staff       (20)   112866 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot
+-rw-r--r--   0 danil      (501) staff       (20)   112354 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot
+-rw-r--r--   0 danil      (501) staff       (20)   113510 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot
+-rw-r--r--   0 danil      (501) staff       (20)     4616 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/LICENSE.txt
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.005205 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/
+-rw-r--r--   0 danil      (501) staff       (20)    91216 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf
+-rw-r--r--   0 danil      (501) staff       (20)    92760 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf
+-rw-r--r--   0 danil      (501) staff       (20)    89720 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf
+-rw-r--r--   0 danil      (501) staff       (20)    91424 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf
+-rw-r--r--   0 danil      (501) staff       (20)    91276 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf
+-rw-r--r--   0 danil      (501) staff       (20)    93144 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf
+-rw-r--r--   0 danil      (501) staff       (20)     1081 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/README.md
+-rw-r--r--   0 danil      (501) staff       (20)     4402 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/ReadMe.html
+-rw-r--r--   0 danil      (501) staff       (20)    11781 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.018060 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/
+-rw-r--r--   0 danil      (501) staff       (20)   111572 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   113320 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   112004 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   112528 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   112048 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf
+-rw-r--r--   0 danil      (501) staff       (20)   113168 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:38.360100 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.026546 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/
+-rw-r--r--   0 danil      (501) staff       (20)    48788 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    51188 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    47136 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    49672 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    48972 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    51272 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.037181 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/
+-rw-r--r--   0 danil      (501) staff       (20)    49496 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    51924 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    48784 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    50792 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    49604 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)    51772 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff
+-rw-r--r--   0 danil      (501) staff       (20)      404 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/bower.json
+-rw-r--r--   0 danil      (501) staff       (20)     2429 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/source-serif-pro.css
+-rw-r--r--   0 danil      (501) staff       (20)    18299 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/_static/guzzle.css
+-rw-r--r--   0 danil      (501) staff       (20)   287630 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/source/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 danil      (501) staff       (20)    92634 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/jquery.js
+-rw-r--r--   0 danil      (501) staff       (20)   138746 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/jquery.min.map
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.039874 verstack-3.7.0/docs/source/_build/html/_static/js/
+-rw-r--r--   0 danil      (501) staff       (20)    55329 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/js/bootstrap.js
+-rw-r--r--   0 danil      (501) staff       (20)    29182 2020-09-20 11:50:32.000000 verstack-3.7.0/docs/source/_build/html/_static/js/bootstrap.min.js
+-rw-r--r--   0 danil      (501) staff       (20)    10854 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/_static/language_data.js
+-rw-r--r--   0 danil      (501) staff       (20)       90 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/source/_build/html/_static/minus.png
+-rw-r--r--   0 danil      (501) staff       (20)       90 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/source/_build/html/_static/plus.png
+-rw-r--r--   0 danil      (501) staff       (20)     4846 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/_static/pygments.css
+-rw-r--r--   0 danil      (501) staff       (20)    16578 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/source/_build/html/_static/searchtools.js
+-rw-r--r--   0 danil      (501) staff       (20)    67692 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/source/_build/html/_static/underscore-1.12.0.js
+-rw-r--r--   0 danil      (501) staff       (20)    19358 2021-05-11 23:58:54.000000 verstack-3.7.0/docs/source/_build/html/_static/underscore.js
+-rw-r--r--   0 danil      (501) staff       (20)     3419 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/genindex.html
+-rw-r--r--   0 danil      (501) staff       (20)   101829 2022-02-10 20:51:19.000000 verstack-3.7.0/docs/source/_build/html/index.html
+-rw-r--r--   0 danil      (501) staff       (20)      254 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/objects.inv
+-rw-r--r--   0 danil      (501) staff       (20)     4531 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/search.html
+-rw-r--r--   0 danil      (501) staff       (20)     6846 2022-02-10 20:51:20.000000 verstack-3.7.0/docs/source/_build/html/searchindex.js
+-rw-r--r--   0 danil      (501) staff       (20)     5223 2022-02-10 20:40:52.000000 verstack-3.7.0/docs/source/conf.py
+-rw-r--r--   0 danil      (501) staff       (20)    73120 2023-05-03 13:09:53.000000 verstack-3.7.0/docs/source/index.rst
+-rw-r--r--   0 danil      (501) staff       (20)      548 2023-02-12 13:52:00.000000 verstack-3.7.0/increment_version.py
+-rw-r--r--   0 danil      (501) staff       (20)   253628 2023-02-12 13:48:06.000000 verstack-3.7.0/logo.png
+-rw-r--r--   0 danil      (501) staff       (20)   200067 2023-02-12 13:48:04.000000 verstack-3.7.0/logo.pxd
+-rw-r--r--   0 danil      (501) staff       (20)     1703 2023-02-12 13:53:15.000000 verstack-3.7.0/package_update_instructions.txt
+-rw-r--r--   0 danil      (501) staff       (20)      310 2023-01-13 15:33:39.000000 verstack-3.7.0/requirements.txt
+-rw-r--r--   0 danil      (501) staff       (20)       80 2023-05-03 13:12:39.081237 verstack-3.7.0/setup.cfg
+-rw-r--r--   0 danil      (501) staff       (20)     2188 2023-05-03 13:12:15.000000 verstack-3.7.0/setup.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.050082 verstack-3.7.0/verstack/
+-rw-r--r--   0 danil      (501) staff       (20)    39819 2023-01-16 10:00:49.000000 verstack-3.7.0/verstack/DateParser.py
+-rw-r--r--   0 danil      (501) staff       (20)    24902 2022-06-21 13:31:01.000000 verstack-3.7.0/verstack/FeatureSelector.py
+-rw-r--r--   0 danil      (501) staff       (20)     7756 2022-04-29 08:46:57.000000 verstack-3.7.0/verstack/Multicore.py
+-rwxr-xr-x   0 danil      (501) staff       (20)    18447 2022-12-09 20:53:43.000000 verstack-3.7.0/verstack/NaNImputer.py
+-rw-r--r--   0 danil      (501) staff       (20)    33143 2022-12-09 20:16:44.000000 verstack-3.7.0/verstack/NaNImputerLegacy.py
+-rw-r--r--   0 danil      (501) staff       (20)    12408 2022-12-19 10:43:57.000000 verstack-3.7.0/verstack/PandasOptimizer.py
+-rw-r--r--   0 danil      (501) staff       (20)     8816 2023-03-28 10:21:12.000000 verstack-3.7.0/verstack/ThreshTuner.py
+-rw-r--r--   0 danil      (501) staff       (20)      980 2022-12-19 08:48:26.000000 verstack-3.7.0/verstack/__init__.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.058097 verstack-3.7.0/verstack/categoric_encoders/
+-rw-r--r--   0 danil      (501) staff       (20)     5115 2022-04-29 12:08:27.000000 verstack-3.7.0/verstack/categoric_encoders/Factorizer.py
+-rw-r--r--   0 danil      (501) staff       (20)     4669 2022-04-28 10:31:19.000000 verstack-3.7.0/verstack/categoric_encoders/FrequencyEncoder.py
+-rw-r--r--   0 danil      (501) staff       (20)     7499 2023-01-11 14:23:40.000000 verstack-3.7.0/verstack/categoric_encoders/MeanTargetEncoder.py
+-rw-r--r--   0 danil      (501) staff       (20)     6647 2022-04-28 09:22:13.000000 verstack-3.7.0/verstack/categoric_encoders/OneHotEncoder.py
+-rw-r--r--   0 danil      (501) staff       (20)     7352 2022-04-28 09:22:53.000000 verstack-3.7.0/verstack/categoric_encoders/WeightOfEvidenceEncoder.py
+-rw-r--r--   0 danil      (501) staff       (20)        0 2021-12-07 14:06:33.000000 verstack-3.7.0/verstack/categoric_encoders/__init__.py
+-rw-r--r--   0 danil      (501) staff       (20)     2173 2021-12-06 19:04:49.000000 verstack-3.7.0/verstack/categoric_encoders/args_validators.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.061124 verstack-3.7.0/verstack/lgbm_optuna_tuning/
+-rw-r--r--   0 danil      (501) staff       (20)    53225 2023-05-03 13:09:36.000000 verstack-3.7.0/verstack/lgbm_optuna_tuning/LGBMTuner.py
+-rw-r--r--   0 danil      (501) staff       (20)        0 2021-12-22 20:41:08.000000 verstack-3.7.0/verstack/lgbm_optuna_tuning/__init__.py
+-rw-r--r--   0 danil      (501) staff       (20)     2229 2021-12-24 13:13:34.000000 verstack-3.7.0/verstack/lgbm_optuna_tuning/args_validators.py
+-rw-r--r--   0 danil      (501) staff       (20)    17600 2022-06-17 08:57:23.000000 verstack-3.7.0/verstack/lgbm_optuna_tuning/lgb_metrics.py
+-rw-r--r--   0 danil      (501) staff       (20)      859 2021-12-21 19:02:16.000000 verstack-3.7.0/verstack/lgbm_optuna_tuning/optuna_tools.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.067695 verstack-3.7.0/verstack/stacking/
+-rw-r--r--   0 danil      (501) staff       (20)    30222 2022-12-11 11:13:47.000000 verstack-3.7.0/verstack/stacking/Stacker.py
+-rw-r--r--   0 danil      (501) staff       (20)        0 2022-04-04 06:15:43.000000 verstack-3.7.0/verstack/stacking/__init__.py
+-rw-r--r--   0 danil      (501) staff       (20)     2371 2022-05-04 09:07:10.000000 verstack-3.7.0/verstack/stacking/args_validators.py
+-rw-r--r--   0 danil      (501) staff       (20)     3627 2022-04-05 06:23:16.000000 verstack-3.7.0/verstack/stacking/generate_default_layers.py
+-rw-r--r--   0 danil      (501) staff       (20)     5430 2022-03-31 15:35:58.000000 verstack-3.7.0/verstack/stacking/kerasModel.py
+-rw-r--r--   0 danil      (501) staff       (20)     3033 2022-12-11 11:14:24.000000 verstack-3.7.0/verstack/stacking/load_stacker.py
+-rw-r--r--   0 danil      (501) staff       (20)     7657 2022-04-28 09:37:07.000000 verstack-3.7.0/verstack/stacking/optimise_params.py
+-rwxr-xr-x   0 danil      (501) staff       (20)     8946 2023-02-12 14:01:23.000000 verstack-3.7.0/verstack/stratified_continuous_split.py
+-rw-r--r--   0 danil      (501) staff       (20)     3523 2022-06-09 19:16:34.000000 verstack-3.7.0/verstack/tools.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.079118 verstack-3.7.0/verstack/unittest/
+-rw-r--r--   0 danil      (501) staff       (20)    25047 2023-05-03 13:08:18.000000 verstack-3.7.0/verstack/unittest/boston_train.parquet
+-rw-r--r--   0 danil      (501) staff       (20)     2443 2023-01-16 10:07:03.000000 verstack-3.7.0/verstack/unittest/common.py
+-rw-r--r--   0 danil      (501) staff       (20)      373 2023-01-16 10:07:50.000000 verstack-3.7.0/verstack/unittest/test_DateParser.py
+-rw-r--r--   0 danil      (501) staff       (20)      939 2022-12-06 11:05:04.000000 verstack-3.7.0/verstack/unittest/test_Factorizer.py
+-rw-r--r--   0 danil      (501) staff       (20)      984 2022-12-06 11:13:56.000000 verstack-3.7.0/verstack/unittest/test_FrequencyEncoder.py
+-rw-r--r--   0 danil      (501) staff       (20)      654 2022-12-06 11:18:41.000000 verstack-3.7.0/verstack/unittest/test_LGBMTuner.py
+-rw-r--r--   0 danil      (501) staff       (20)      791 2022-12-06 11:20:55.000000 verstack-3.7.0/verstack/unittest/test_MeanTargetEncoder.py
+-rw-r--r--   0 danil      (501) staff       (20)      600 2022-12-06 11:33:00.000000 verstack-3.7.0/verstack/unittest/test_Multicore.py
+-rw-r--r--   0 danil      (501) staff       (20)      393 2022-12-06 11:34:15.000000 verstack-3.7.0/verstack/unittest/test_NaNImputer.py
+-rw-r--r--   0 danil      (501) staff       (20)      531 2022-12-06 11:35:42.000000 verstack-3.7.0/verstack/unittest/test_OneHotEncoder.py
+-rw-r--r--   0 danil      (501) staff       (20)      414 2022-12-19 09:08:24.000000 verstack-3.7.0/verstack/unittest/test_PandasOptimizer.py
+-rw-r--r--   0 danil      (501) staff       (20)      336 2022-12-06 11:37:18.000000 verstack-3.7.0/verstack/unittest/test_Printer.py
+-rw-r--r--   0 danil      (501) staff       (20)     1726 2022-12-11 12:01:19.000000 verstack-3.7.0/verstack/unittest/test_Stacker.py
+-rw-r--r--   0 danil      (501) staff       (20)      710 2022-12-13 07:01:40.000000 verstack-3.7.0/verstack/unittest/test_ThreshTuner.py
+-rw-r--r--   0 danil      (501) staff       (20)      863 2022-12-06 14:19:28.000000 verstack-3.7.0/verstack/unittest/test_WeightOfEvidenceEncoder.py
+-rw-r--r--   0 danil      (501) staff       (20)      501 2023-05-03 13:08:40.000000 verstack-3.7.0/verstack/unittest/test_stratified_continuous_split.py
+-rw-r--r--   0 danil      (501) staff       (20)     1370 2022-12-06 14:58:08.000000 verstack-3.7.0/verstack/unittest/unittesting_manual.txt
+-rw-r--r--   0 danil      (501) staff       (20)       21 2023-05-03 13:09:53.000000 verstack-3.7.0/verstack/version.py
+drwxr-xr-x   0 danil      (501) staff       (20)        0 2023-05-03 13:12:39.053774 verstack-3.7.0/verstack.egg-info/
+-rw-r--r--   0 danil      (501) staff       (20)     3361 2023-05-03 13:12:38.000000 verstack-3.7.0/verstack.egg-info/PKG-INFO
+-rw-r--r--   0 danil      (501) staff       (20)    31441 2023-05-03 13:12:38.000000 verstack-3.7.0/verstack.egg-info/SOURCES.txt
+-rw-r--r--   0 danil      (501) staff       (20)        1 2023-05-03 13:12:38.000000 verstack-3.7.0/verstack.egg-info/dependency_links.txt
+-rw-r--r--   0 danil      (501) staff       (20)      271 2023-05-03 13:12:38.000000 verstack-3.7.0/verstack.egg-info/requires.txt
+-rw-r--r--   0 danil      (501) staff       (20)        9 2023-05-03 13:12:38.000000 verstack-3.7.0/verstack.egg-info/top_level.txt
```

### Comparing `verstack-3.6.7/LICENSE.txt` & `verstack-3.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/PKG-INFO` & `verstack-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: verstack
-Version: 3.6.7
+Version: 3.7.0
 Summary: Machine learning tools to make a Data Scientist's work more efficient
 Home-page: https://github.com/DanilZherebtsov/verstack
-Download-URL: https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.6.7.tar.gz
+Download-URL: https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.7.0.tar.gz
 Author: Danil Zherebtsov
 Author-email: danil.com@me.com
 License: MIT
 Keywords: impute,missing,values,stratify,nan,continuous,multiprocessing,concurrent,timer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 .. image:: logo.png
 
-**verstack 3.6.7** is a set of Machine learning tools to make a Data Scientist's work efficient.
+**verstack 3.7.0** is a set of Machine learning tools to make a Data Scientist's work efficient.
 
 The package contains multiple tools for: training & tuning machine learning models, creating ensembles, working with datetime objects, data transformation & wrangling, imputing missing values, concurrency work and many more.
 
 Please refer to the `official documentation <https://verstack.readthedocs.io>`_ for more information.
 
 The project was created by Danil Zherebtsov in 2020.
```

### Comparing `verstack-3.6.7/README.rst` & `verstack-3.7.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 .. image:: logo.png
 
-**verstack 3.6.7** is a set of Machine learning tools to make a Data Scientist's work efficient.
+**verstack 3.7.0** is a set of Machine learning tools to make a Data Scientist's work efficient.
 
 The package contains multiple tools for: training & tuning machine learning models, creating ensembles, working with datetime objects, data transformation & wrangling, imputing missing values, concurrency work and many more.
 
 Please refer to the `official documentation <https://verstack.readthedocs.io>`_ for more information.
 
 The project was created by Danil Zherebtsov in 2020.
```

### Comparing `verstack-3.6.7/dist/verstack-0.1.0.tar.gz` & `verstack-3.7.0/dist/verstack-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/Doc_update_manual.txt` & `verstack-3.7.0/docs/Doc_update_manual.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/Makefile` & `verstack-3.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/doctrees/README.doctree` & `verstack-3.7.0/docs/build/doctrees/README.doctree`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/doctrees/environment.pickle` & `verstack-3.7.0/docs/build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/doctrees/index.doctree` & `verstack-3.7.0/docs/build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/README.html` & `verstack-3.7.0/docs/build/html/README.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_sources/README.md.txt` & `verstack-3.7.0/docs/build/html/_sources/README.md.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_sources/README.rst.txt` & `verstack-3.7.0/docs/build/html/_sources/README.rst.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_sources/index.rst.txt` & `verstack-3.7.0/docs/build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/alabaster.css` & `verstack-3.7.0/docs/build/html/_static/alabaster.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/basic.css` & `verstack-3.7.0/docs/build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/css/bootstrap-theme.min.css` & `verstack-3.7.0/docs/build/html/_static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/css/bootstrap.min.css` & `verstack-3.7.0/docs/build/html/_static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/doctools.js` & `verstack-3.7.0/docs/build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Droid_Sans_Mono_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Droid_Sans_Mono_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Droid_Sans_Mono_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Droid_Sans_Mono_400.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Droid_Sans_Mono_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400italic.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400italic.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400italic.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_400italic.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_400italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700italic.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700italic.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700italic.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noticia_Text_700italic.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noticia_Text_700italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400italic.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400italic.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400italic.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_400italic.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_400italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700italic.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700italic.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700italic.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Sans_700italic.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Sans_700italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400italic.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400italic.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400italic.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_400italic.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_400italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700italic.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700italic.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700italic.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700italic.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700italic.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700italic.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Noto_Serif_700italic.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Noto_Serif_700italic.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_400.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_400.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_400.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_400.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_400.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_400.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_400.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_400.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_700.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_700.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_700.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_700.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_700.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_700.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/Source_Code_Pro_700.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/Source_Code_Pro_700.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/glyphicons-halflings-regular.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/open-sans/stylesheet.css` & `verstack-3.7.0/docs/build/html/_static/fonts/open-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/LICENSE.txt` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/README.md` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/README.md`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/ReadMe.html` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/ReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/fonts/source-serif-pro/source-serif-pro.css` & `verstack-3.7.0/docs/build/html/_static/fonts/source-serif-pro/source-serif-pro.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/guzzle.css` & `verstack-3.7.0/docs/build/html/_static/guzzle.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-example.png` & `verstack-3.7.0/docs/build/html/_static/icon-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-important.png` & `verstack-3.7.0/docs/build/html/_static/icon-important.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-javascript-example.png` & `verstack-3.7.0/docs/build/html/_static/icon-javascript-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-json-example.png` & `verstack-3.7.0/docs/build/html/_static/icon-json-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-lconf-example.png` & `verstack-3.7.0/docs/build/html/_static/icon-lconf-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-note.png` & `verstack-3.7.0/docs/build/html/_static/icon-note.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-optional.png` & `verstack-3.7.0/docs/build/html/_static/icon-optional.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-python-example.png` & `verstack-3.7.0/docs/build/html/_static/icon-python-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-seealso.png` & `verstack-3.7.0/docs/build/html/_static/icon-seealso.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-shell-example.png` & `verstack-3.7.0/docs/build/html/_static/icon-shell-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-text-example.png` & `verstack-3.7.0/docs/build/html/_static/icon-text-example.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-tip.png` & `verstack-3.7.0/docs/build/html/_static/icon-tip.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-todo.png` & `verstack-3.7.0/docs/build/html/_static/icon-todo.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/icon-warning.png` & `verstack-3.7.0/docs/build/html/_static/icon-warning.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/jquery-3.4.1.js` & `verstack-3.7.0/docs/build/html/_static/jquery-3.4.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/jquery-3.5.1.js` & `verstack-3.7.0/docs/build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/jquery.cookie.js` & `verstack-3.7.0/docs/build/html/_static/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/jquery.js` & `verstack-3.7.0/docs/build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/jquery.min.map` & `verstack-3.7.0/docs/build/html/_static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/js/bootstrap.js` & `verstack-3.7.0/docs/build/html/_static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/js/bootstrap.min.js` & `verstack-3.7.0/docs/build/html/_static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/language_data.js` & `verstack-3.7.0/docs/build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/local_fonts.css` & `verstack-3.7.0/docs/build/html/_static/local_fonts.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/p_sphinx_theme.css` & `verstack-3.7.0/docs/build/html/_static/p_sphinx_theme.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/p_sphinx_theme.js` & `verstack-3.7.0/docs/build/html/_static/p_sphinx_theme.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/pygments.css` & `verstack-3.7.0/docs/build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/searchtools.js` & `verstack-3.7.0/docs/build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/underscore-1.12.0.js` & `verstack-3.7.0/docs/build/html/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/underscore-1.13.1.js` & `verstack-3.7.0/docs/build/html/_static/underscore-1.13.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/underscore-1.3.1.js` & `verstack-3.7.0/docs/build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/_static/underscore.js` & `verstack-3.7.0/docs/build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/genindex.html` & `verstack-3.7.0/docs/build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/index.html` & `verstack-3.7.0/docs/build/html/index.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/search.html` & `verstack-3.7.0/docs/build/html/search.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/build/html/searchindex.js` & `verstack-3.7.0/docs/build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/__init__.py` & `verstack-3.7.0/docs/guzzle_sphinx_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/__pycache__/__init__.cpython-37.pyc` & `verstack-3.7.0/docs/guzzle_sphinx_theme/__pycache__/__init__.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/comments.html` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/comments.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/layout.html` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/layout.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/search.html` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/search.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/searchbox.html` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap-theme.min.css` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap.min.css` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/stylesheet.css` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/open-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/LICENSE.txt` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/README.md` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/README.md`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/ReadMe.html` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/ReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/SourceSerifProReadMe.html` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/SourceSerifProReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/source-serif-pro.css` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/fonts/source-serif-pro/source-serif-pro.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/guzzle.css_t` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/guzzle.css_t`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.js` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.min.map` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.js` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.min.js` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/theme.conf` & `verstack-3.7.0/docs/guzzle_sphinx_theme/guzzle_sphinx_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/make.bat` & `verstack-3.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/.doctrees/environment.pickle` & `verstack-3.7.0/docs/source/_build/html/.doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/.doctrees/index.doctree` & `verstack-3.7.0/docs/source/_build/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_sources/index.rst.txt` & `verstack-3.7.0/docs/source/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/basic.css` & `verstack-3.7.0/docs/source/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/css/bootstrap-theme.min.css` & `verstack-3.7.0/docs/source/_build/html/_static/css/bootstrap-theme.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/css/bootstrap.min.css` & `verstack-3.7.0/docs/source/_build/html/_static/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/doctools.js` & `verstack-3.7.0/docs/source/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-BoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-ExtraBoldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Italic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Light-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-LightItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-Semibold-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.svg`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/fonts/OpenSans-SemiboldItalic-webfont.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/open-sans/stylesheet.css` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/open-sans/stylesheet.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Black.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Bold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-ExtraLight.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Light.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Regular.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/EOT/SourceSerifPro-Semibold.eot`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/LICENSE.txt` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Black.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Bold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-ExtraLight.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Light.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Regular.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/OTF/SourceSerifPro-Semibold.otf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/README.md` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/README.md`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/ReadMe.html` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/ReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/SourceSerifProReadMe.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Black.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Bold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Light.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/TTF/SourceSerifPro-Semibold.ttf`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Black.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Bold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-ExtraLight.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Light.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Regular.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/OTF/SourceSerifPro-Semibold.otf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Black.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Bold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-ExtraLight.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Light.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Regular.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/WOFF/TTF/SourceSerifPro-Semibold.ttf.woff`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/fonts/source-serif-pro/source-serif-pro.css` & `verstack-3.7.0/docs/source/_build/html/_static/fonts/source-serif-pro/source-serif-pro.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/guzzle.css` & `verstack-3.7.0/docs/source/_build/html/_static/guzzle.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/jquery-3.5.1.js` & `verstack-3.7.0/docs/source/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/jquery.js` & `verstack-3.7.0/docs/source/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/jquery.min.map` & `verstack-3.7.0/docs/source/_build/html/_static/jquery.min.map`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/js/bootstrap.js` & `verstack-3.7.0/docs/source/_build/html/_static/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/js/bootstrap.min.js` & `verstack-3.7.0/docs/source/_build/html/_static/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/language_data.js` & `verstack-3.7.0/docs/source/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/pygments.css` & `verstack-3.7.0/docs/source/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/searchtools.js` & `verstack-3.7.0/docs/source/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/underscore-1.12.0.js` & `verstack-3.7.0/docs/source/_build/html/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/_static/underscore.js` & `verstack-3.7.0/docs/source/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/genindex.html` & `verstack-3.7.0/docs/source/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/index.html` & `verstack-3.7.0/docs/source/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/search.html` & `verstack-3.7.0/docs/source/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/_build/html/searchindex.js` & `verstack-3.7.0/docs/source/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/conf.py` & `verstack-3.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/docs/source/index.rst` & `verstack-3.7.0/docs/source/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ############################
-verstack 3.6.7 Documentation
+verstack 3.7.0 Documentation
 ############################
 Machine learning tools to make a Data Scientist's work efficient
 
 veratack package contains the following tools:
 
 * **PandasOptimizer** oad a pandas.DataFrame with optimized datatypes (reduce RAM usage)
 * **Stacker** automated stacking ensemble configuration/train/features creation in train/test sets
@@ -790,26 +790,38 @@
 LGBMTuner selects optimal hyperparameters based on executed trials (configurable), optimizes n_estimators and fits the final model to the whole train set.
 Feature importances are available in numeric format, as a static plot, and as an interactive plot (html).
 Optimization history and parameters importance in static and interactive formats are alse accesable by built in methods.
 
 Logic
 ================================================================
 
-The only required user inputs are the X (features), y (labels) and evaluation metric name, LGBMTuner will handle the rest 
+The only required user inputs are the X (features), y (labels) and evaluation metric name, LGBMTuner will handle the rest.
 
+By default LGBMTuner will:
+1. Configure various LGBM model hyperparameters for regression or classification based on input data
  - lgbm model type (regression/classification) is inferred from the labels and evaluation metric (passed by user)
  - optimization metric may be different from the evaluation metric (passed by user). LGBMTuner at hyperparameters search stage imploys the error reduction strategy, thus:
    - most regression task type metrics are supported for optimization, if not, MSE is selected for optimization
    - for classification task types hyperparameters are tuned by optimizing log_loss, n_estimators are tuned with evaluation_metric
  - early stopping is engaged at each stage of LGBMTuner optimizations
- - for every trial (iteration) a random train_test_split is performed (stratified for classification)
+ - for every trial (iteration) a random train_test_split is performed (stratified for classification) eliminating the need for cross-validation
  - lgbm model initial parameters!=defaults and are inferred from the data stats and built in logic
  - optimization parameters and their search space are inferred from the data stats and built in logic
  - LGBMTuner class instance (after optimization) can be used for making predictions with conventional syntaxis (predict/predict_proba)
  - verbosity is controlled and by default outputs only the necessary optimization process/results information
+2. Optimize the follwoing parameters within the defined ranges:
+ - 'feature_fraction' : {'low': 0.5, 'high': 1}
+ - 'num_leaves' : {'low' : 16, 'high': 255}
+ - 'bagging_fraction' : {'low' : 0.5, 'high' : 1.0}
+ - 'min_sum_hessian_in_leaf' : {'low' : 1e-3, 'high' " 10.0}
+ - 'lambda_l1' : {'low' " 1e-8, 'high' : 10.0}
+ - 'lambda_l2' : {'low' " 1e-8, 'high' : 10.0}
+
+.. note:: 
+  User may define other parameters and their respective grids for optimization by changing the LGBM.grid dictionary after the class is initialized.
 
 **Initialize LGBMTuner**
 
 .. code-block:: python
 
   from verstack import LGBMTuner
   
@@ -1059,14 +1071,18 @@
 
   learned optimized parameters
 
 * ``eval_results``
 
   dictionary with evaluation results per each of non-pruned trials measured by a function derived from the ``metric`` argument
 
+* ``grid``
+
+  dictionary with all the supported and currently selected optimization parameters
+
 Examples
 ================================================================
 
 Using LGBMTuner with all default parameters
 
 .. code-block:: python
 
@@ -1086,14 +1102,51 @@
 
   imputer = LGBMTuner(metric = 'auc', trials = 300, verbosity = 3, visualization = False)
   tuner.fit(X, y)
   tuner.plot_importances(legend = True)
   tuner.plot_intermediate_values(interactive = True)
   tuner.predict(test, threshold = 0.3)
 
+LGBMTuner with custom optimization parameters
+
+.. code-block:: python
+
+  tuner = LGBMTuner(metric = 'auc', trials = 300)
+  # show the supported parameters for optimization
+  tuner.grid
+  #--->{'boosting_type': None,
+  #--->'num_iterations': None,
+  #--->'learning_rate': None,
+  #--->'num_leaves': {'low': 16, 'high': 255},                  <--- default setting
+  #--->'max_depth': None,
+  #--->'min_data_in_leaf': None,
+  #--->'min_sum_hessian_in_leaf': {'low': 0.001, 'high': 10.0}, <--- default setting
+  #--->'bagging_fraction': {'low': 0.5, 'high': 1.0},           <--- default setting
+  #--->'feature_fraction': {'low': 0.5, 'high': 1.0},           <--- default setting
+  #--->'max_delta_step': None,
+  #--->'lambda_l1': {'low': 1e-08, 'high': 10.0},               <--- default setting
+  #--->'lambda_l2': {'low': 1e-08, 'high': 10.0},               <--- default setting
+  #--->'linear_lambda': None,
+  #--->'min_gain_to_split': None,
+  #--->'drop_rate': None,
+  #--->'top_rate': None,
+  #--->'min_data_per_group': None,
+  #--->'max_cat_threshold': None}
+
+  # change optimization parameters
+  # parameters can be passed by any of the following ways: 
+  # - list (will be used for a random search)
+  # - tuple (will be used to define the uniform grid range between the min(tuple), max(tuple))
+  # - dict with keywords 'choice'/'low'/'high'
+  tuner.grid['boosting_type'] = ['gbdt', 'rf'] 
+  tuner.grid['max_data_in_leaf'] = {'choice' : ['gbdt', 'rf']}
+  tuner.grid['learning_rate'] = (0.001, 0.1)
+  tuner.grid['lambda_l1'] = {'low': 0.1, 'high': 5}
+  tuner.fit(X, y)
+
 ******************
 NaNImputer
 ******************
 
 Impute all missing values in a pandas dataframe by xgboost models in multiprocessing mode using a single line of code.
 
 .. note::
```

### Comparing `verstack-3.6.7/increment_version.py` & `verstack-3.7.0/increment_version.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/logo.png` & `verstack-3.7.0/logo.png`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/logo.pxd` & `verstack-3.7.0/logo.pxd`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/package_update_instructions.txt` & `verstack-3.7.0/package_update_instructions.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/setup.py` & `verstack-3.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
   license='MIT',
   description = "Machine learning tools to make a Data Scientist's work more efficient",
   long_description=long_description,
   long_description_content_type="text/markdown",
   author = 'Danil Zherebtsov',
   author_email = 'danil.com@me.com',
   url = 'https://github.com/DanilZherebtsov/verstack',
-  download_url = 'https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.6.7.tar.gz',
+  download_url = 'https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.7.0.tar.gz',
   keywords = ['impute', 'missing', 'values', 'stratify', 'nan', 'continuous', 'multiprocessing', 'concurrent', 'timer'],
   install_requires=dependencies,
   classifiers=[
   'Development Status :: 4 - Beta',
   'Intended Audience :: Developers',
   'Topic :: Software Development :: Build Tools',
   'License :: OSI Approved :: MIT License',
```

### Comparing `verstack-3.6.7/verstack/DateParser.py` & `verstack-3.7.0/verstack/DateParser.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/FeatureSelector.py` & `verstack-3.7.0/verstack/FeatureSelector.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/Multicore.py` & `verstack-3.7.0/verstack/Multicore.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/NaNImputer.py` & `verstack-3.7.0/verstack/NaNImputer.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/NaNImputerLegacy.py` & `verstack-3.7.0/verstack/NaNImputerLegacy.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/PandasOptimizer.py` & `verstack-3.7.0/verstack/PandasOptimizer.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/ThreshTuner.py` & `verstack-3.7.0/verstack/ThreshTuner.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/__init__.py` & `verstack-3.7.0/verstack/__init__.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/categoric_encoders/Factorizer.py` & `verstack-3.7.0/verstack/categoric_encoders/Factorizer.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/categoric_encoders/FrequencyEncoder.py` & `verstack-3.7.0/verstack/categoric_encoders/FrequencyEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/categoric_encoders/MeanTargetEncoder.py` & `verstack-3.7.0/verstack/categoric_encoders/MeanTargetEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/categoric_encoders/OneHotEncoder.py` & `verstack-3.7.0/verstack/categoric_encoders/OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/categoric_encoders/WeightOfEvidenceEncoder.py` & `verstack-3.7.0/verstack/categoric_encoders/WeightOfEvidenceEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/categoric_encoders/args_validators.py` & `verstack-3.7.0/verstack/categoric_encoders/args_validators.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/lgbm_optuna_tuning/LGBMTuner.py` & `verstack-3.7.0/verstack/lgbm_optuna_tuning/LGBMTuner.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,24 @@
 from verstack.lgbm_optuna_tuning.lgb_metrics import get_pruning_metric, get_optimization_metric_func, define_objective, classification_metrics, regression_metrics, get_eval_score, print_lower_greater_better, supported_metrics, get_n_rounds_optimization_metric
 from verstack.lgbm_optuna_tuning.args_validators import *
 from verstack.lgbm_optuna_tuning.optuna_tools import Distribution, OPTUNA_DISTRIBUTIONS_MAP, SearchSpace
 # BACKLOG: add option to pass different init params on class __init__
 # BACKLOG: add option to pass different param_grid for optimization
 # OPTIONAL TODO - add factorization to targets and inverse_transform predictions for classification (E.g. Ghosts, prudential)
 
+supported_gridsearch_params = [
+    'boosting_type', 'num_iterations', 'learning_rate', 'num_leaves', 'max_depth', 
+    'min_data_in_leaf', 'min_sum_hessian_in_leaf', 'bagging_fraction', 'feature_fraction',
+    'max_delta_step', 'lambda_l1', 'lambda_l2', 'linear_lambda', 'min_gain_to_split',
+    'drop_rate', 'top_rate', 'min_data_per_group', 'max_cat_threshold'
+    ]
+
 class LGBMTuner:
 
-    __version__ = '0.1.2'
+    __version__ = '1.0.0'
 
     def __init__(self, **kwargs):
         '''
         Class to automatically tune LGBM model with optuna.
         
         Model type (regressor/classifier) is inferred based on target variable & metric.
         Init parameters and search space are inferred by built in logic.
@@ -47,14 +54,46 @@
         seed : int
             random_state.
         device_type : str
             cpu/gpu/cuda/cuda_exp.
         eval_results_callback : func
             callback function to be applied on the eval_results dictionary that is being populated
             with evaluation metric score upon completion of each training trial.
+        grid: dict
+            Parameters search space for optimization. 
+            
+            A default search space is populated at fit, depending on number of trials:
+            "feature_fraction" = (Distribution.UNIFORM, low=0.5, high=1.0) 
+            "num_leaves" = (Distribution.INTUNIFORM, low=16, high=255)
+            if self.trials > 30:
+                "bagging_fraction" = (Distribution.UNIFORM, low=0.5, high=1.0) 
+                "min_sum_hessian_in_leaf" = (Distribution.LOGUNIFORM, low=1e-3, high=10.0)
+            if self.trials > 100:
+                "lambda_l1" = (Distribution.LOGUNIFORM, low=1e-8, high=10.0)
+                "lambda_l2" = (Distribution.LOGUNIFORM, low=1e-8, high=10.0)
+
+            Grid can be modified with the following parameters to be included in the Search Space:
+                boosting_type : 'gbdt', 'dart', 'rf' 
+                num_iterations : >= 0
+                learning_rate : > 0.0
+                num_leaves : 1 < num_leaves <= 131072
+                max_depth : 
+                min_data_in_leaf : >= 0
+                min_sum_hessian_in_leaf : >= 0.0
+                bagging_fraction : 0.0 < bagging_fraction <= 1.0
+                feature_fraction : 0.0 < feature_fraction <= 1.0
+                max_delta_step : 
+                lambda_l1 : >=0
+                lambda_l2 : >=0
+                linear_lambda : >=0
+                min_gain_to_split : >=0.0
+                drop_rate : 0.0 <= drop_rate <= 1.0
+                top_rate : 0.0 <= top_rate <= 1.0
+                min_data_per_group : > 0
+                max_cat_threshold : > 0
 
         Returns
         -------
         None.
 
         '''
         self.verbosity = kwargs.get('verbosity', 1)
@@ -70,23 +109,39 @@
         self._feature_importances = None
         self._study = None # save optuna study for plotting
         self.target_classes = None
         self._init_params = None
         self._best_params = None
         self.eval_results = {} # evaluation metric results per each trial storage
         self.eval_results_callback = kwargs.get('eval_results_callback', None)
+        self.search_space = self._get_default_search_space()
+        self.grid = self._get_all_available_and_defined_grids()
+
+        # get user defined grid
+
+    def _get_all_available_and_defined_grids(self):
+        all_grids = {}
+        for param in supported_gridsearch_params:
+            if param in self.search_space:
+                all_grids[param] = self.search_space[param].params
+            else:
+                all_grids[param] = None
+        return all_grids
+        
 
     # print init parameters when calling the class instance
     def __repr__(self):
         return f'LGBMTuner(Evaluation metric: {self._metric}\
             \n          trials: {self.trials}\
             \n          refit: {self.refit}\
             \n          verbosity: {self.verbosity}\
             \n          visualization: {self.visualization})\
-            \n          device_type: {self.device_type})'
+            \n          device_type: {self.device_type})\
+            \n          grid: {self.grid})'
+    
 
     # Validate init arguments
     # =========================================================================
     # define cmmon functions for setters
     def _is_bool(self, val):
         return type(val) == bool
 
@@ -224,36 +279,36 @@
         '''
         # TODO: use number of features
         
         # default lgbm parameters - basis for minor changes based on dataset length
         default_params_classification = {"task": "train",
                                         "learning_rate": 0.05,
                                         "num_leaves": 128,
-                                        "colsample_bytree": 0.7,
-                                        "subsample": 0.7,
+                                        "feature_fraction": 0.7,
+                                        "bagging_fraction": 0.7,
                                         "bagging_freq": 1,
                                         "max_depth": -1,
                                         "verbosity": -1,
-                                        "reg_alpha": 1,
-                                        "reg_lambda": 0.0,
+                                        "lambda_l1": 1,
+                                        "lambda_l2": 0.0,
                                         "min_split_gain": 0.0,
                                         "zero_as_missing": False,
                                         "max_bin": 255,
                                         "min_data_in_bin": 3,
-                                        "n_estimators": 3000,
+                                        "num_iterations": 3000,
                                         "early_stopping_rounds": 100,
                                         "random_state": 42,
                                         "device_type": self.device_type}
 
         default_params_regression = {"learning_rate": 0.05,
                                     "num_leaves": 32,
-                                    "colsample_bytree": 0.9,
-                                    "subsample": 0.9,
+                                    "feature_fraction": 0.9,
+                                    "bagging_fraction": 0.9,
                                     "verbosity": -1,
-                                    "n_estimators": 3000,
+                                    "num_iterations": 3000,
                                     "early_stopping_rounds": 100,
                                     "random_state": 42,
                                     "device_type": self.device_type}
 
 
         task = define_objective(self.metric, y)
         
@@ -300,35 +355,35 @@
 
         if rows_num > 300000:
             self._init_params["num_leaves"] = 128 if task == "regression" else 244
         elif rows_num > 100000:
             self._init_params["num_leaves"] = 64 if task == "regression" else 128
         elif rows_num > 50000:
             self._init_params["num_leaves"] = 32 if task == "regression" else 64
-            # params['reg_alpha'] = 1 if task == 'reg' else 0.5
+            # params['lambda_l1'] = 1 if task == 'reg' else 0.5
         elif rows_num > 20000:
             self._init_params["num_leaves"] = 32 if task == "regression" else 32
-            self._init_params["reg_alpha"] = 0.5 if task == "regression" else 0.0
+            self._init_params["lambda_l1"] = 0.5 if task == "regression" else 0.0
         elif rows_num > 10000:
             self._init_params["num_leaves"] = 32 if task == "regression" else 64
-            self._init_params["reg_alpha"] = 0.5 if task == "regression" else 0.2
+            self._init_params["lambda_l1"] = 0.5 if task == "regression" else 0.2
         elif rows_num > 5000:
             self._init_params["num_leaves"] = 24 if task == "regression" else 32
-            self._init_params["reg_alpha"] = 0.5 if task == "regression" else 0.5
+            self._init_params["lambda_l1"] = 0.5 if task == "regression" else 0.5
         else:
             self._init_params["num_leaves"] = 16 if task == "regression" else 16
-            self._init_params["reg_alpha"] = 1 if task == "regression" else 1
+            self._init_params["lambda_l1"] = 1 if task == "regression" else 1
 
         self._init_params["learning_rate"] = init_lr
-        self._init_params["n_estimators"] = ntrees
+        self._init_params["num_iterations"] = ntrees
         self._init_params["early_stopping_rounds"] = es
     # -----------------------------------------------------------------------------
 
-    def _get_default_search_space(self, estimated_n_trials):
-        '''Sample hyperparameters from suggested.
+    def _get_default_search_space(self):
+        '''Sample hyperparameters from suggested
 
         Parameters
         ----------
         estimated_n_trials : int
             number of optuna trails.
 
         Returns
@@ -336,71 +391,69 @@
         search_space : dict
             optimization search space grid and type of distribution for each parameter.
 
         '''
         # TODO: create addditional options based on bigger estimated_n_trials
         search_space = {}
 
-        search_space["colsample_bytree"] = SearchSpace(Distribution.UNIFORM, low=0.5, high=1.0) 
+        search_space["feature_fraction"] = SearchSpace(Distribution.UNIFORM, low=0.5, high=1.0) 
         search_space["num_leaves"] = SearchSpace(Distribution.INTUNIFORM, low=16, high=255)
 
-        if estimated_n_trials > 30:
-            search_space["subsample"] = SearchSpace(Distribution.UNIFORM, low=0.5, high=1.0) 
+        if self.trials > 30:
+            search_space["bagging_fraction"] = SearchSpace(Distribution.UNIFORM, low=0.5, high=1.0) 
             search_space["min_sum_hessian_in_leaf"] = SearchSpace(Distribution.LOGUNIFORM, low=1e-3, high=10.0)
 
-        if estimated_n_trials > 100:
-            search_space["reg_alpha"] = SearchSpace(Distribution.LOGUNIFORM, low=1e-8, high=10.0)
-            search_space["reg_lambda"] = SearchSpace(Distribution.LOGUNIFORM, low=1e-8, high=10.0)
+        if self.trials > 100:
+            search_space["lambda_l1"] = SearchSpace(Distribution.LOGUNIFORM, low=1e-8, high=10.0)
+            search_space["lambda_l2"] = SearchSpace(Distribution.LOGUNIFORM, low=1e-8, high=10.0)
 
         return search_space
     # -----------------------------------------------------------------------------
 
-    def _sample_from_search_space(self, optimization_search_space, trial):
+    def _sample_from_search_space(self, trial):
         '''
         Get params for a trial.
 
         Parameters
         ----------
-        optimization_search_space : dict
-            grid for selecting parameters.
         trial : optuna.Trial
             trial object.
         suggested_params : dict
             init params on input.
 
         Raises
         ------
         ValueError
             Optuna distribution error.
 
         Returns
         -------
         trial_values : dict
-            trial parameters consisting from suggested_params modified by optimization_search_space.
+            trial parameters consisting from suggested_params modified by grid.
 
         '''
         trial_values = copy(self._init_params)
-        for parameter, SearchSpace in optimization_search_space.items():
+        for parameter, SearchSpace in self.search_space.items():
             if SearchSpace.distribution_type in OPTUNA_DISTRIBUTIONS_MAP:
                 trial_values[parameter] = getattr(trial, OPTUNA_DISTRIBUTIONS_MAP[SearchSpace.distribution_type])(
                     name=parameter, **SearchSpace.params)
             else:
-                for key, value in optimization_search_space.items():
+                for key, value in self.search_space.items():
                     print(key)
                     print(value.distribution_type)
                 raise ValueError(f"Optuna does not support distribution {SearchSpace.distribution_type}")
         return trial_values
     # -----------------------------------------------------------------------------
 
     def _get_dtrain_dvalid_objects(self, X, y, metric, seed = None, return_raw_valid = False):
         '''
         Create lgbm.Datasets for training and validation.
         
         By default splits without defined random_state in order to replicate CV (sort of).
-        Seed is used for optimize_n_estimators.
+        Seed is used for optimize_num_iterations.
 
         Parameters
         ----------
         X : pd.DataFrame
             train features.
         y : pd.Series
             train labels.
@@ -427,18 +480,17 @@
         dvalid = lgb.Dataset(valid_x, label=valid_y)
         if return_raw_valid:
             return dtrain, dvalid, valid_x, valid_y
         else:
             return dtrain, dvalid
     # -----------------------------------------------------------------------------
 
-    def optimize_n_estimators(self, X, y, params, verbose_eval = 100):
+    def optimize_num_iterations(self, X, y, params, verbose_eval = 100):
         '''
-        Optimize n_estimators for lgb model.
-        
+        Optimize num_iterations for lgb model.
         Here (after all the tuning) the actual eval_metric is used for early stopping.
         get_n_rounds_optimization_metric(self.metric) returns the feval function 
         from lgb_metrics in an acceptable format.
 
         Parameters
         ----------
         X : np.array
@@ -447,25 +499,25 @@
             train target.
         params : dict
             model parameters.
 
         Returns
         -------
         int
-            best_iteration for further n_estimators param.
+            best_iteration for further num_iterations param.
         best_score : float
             validation score from best_iteration
 
         '''
         validate_numpy_ndarray_arguments(X)
         validate_numpy_ndarray_arguments(y)
         validate_params_argument(params)
         validate_verbose_eval_argument(verbose_eval)
 
-        self.printer.print('Tune n_estimators with early_stopping', order=2)
+        self.printer.print('Tune num_iterations with early_stopping', order=2)
         if self.verbosity>0:
             verbose_eval_rounds = verbose_eval
         else:
             verbose_eval_rounds = None
 
         # temporarily change the params['metric'] for the best performance on the eval_metric
         n_rounds_optimization_params = params.copy()
@@ -617,16 +669,20 @@
         -------
         result : float
             optimization metric validation result.
 
         '''
         optimization_metric_func = get_optimization_metric_func(self.metric)
         dtrain, dvalid, valid_x, valid_y = self._get_dtrain_dvalid_objects(X, y, self.metric, return_raw_valid = True)
-        optimization_search_space = self._get_default_search_space(estimated_n_trials = 200)    
-        params = self._sample_from_search_space(optimization_search_space, trial)
+        # get default grid
+
+
+
+
+        params = self._sample_from_search_space(trial)
         # Add a callback for pruning.
         pruning_callback = optuna.integration.LightGBMPruningCallback(trial, get_pruning_metric(self.metric, self.target_classes))
         result = self._get_validation_score(trial, dtrain, dvalid, valid_x, valid_y, optimization_metric_func, params, pruning_callback)
 
         return result 
     # ------------------------------------------------------------------------------------------
     def _check_refit_status(self, method):
@@ -704,22 +760,22 @@
             raise TypeError('predict_proba() is applicable for classification problems only')
         pred = self._fitted_model.predict(test.values, num_threads = self._init_params['num_threads'])
         return pred
     # ------------------------------------------------------------------------------------------
     
     def _populate_best_params_to_init_params(self, best_params):
         '''Populate the learned params into the suggested params'''
-        # output params are temporary, because n_estimators tuning will follow
+        # output params are temporary, because num_iterations tuning will follow
         temp_params = copy(self._init_params)
         for key, val in best_params.items():
             temp_params[key] = val
-        # remove early_stopping & n_estimators from params (used during optuna optimization).
+        # remove early_stopping & num_iterations from params (used during optuna optimization).
         # final early stopping will be trained during final_estimators_tuning
         del temp_params['early_stopping_rounds']
-        del temp_params['n_estimators']
+        del temp_params['num_iterations']
         
         return temp_params
     # ------------------------------------------------------------------------------------------
 
     def _save_feature_importances(self, train_features):
         '''Save feature importances in class instance as a pd.Series'''
         feat_importances = pd.Series(self._fitted_model.feature_importance(), index = train_features)
@@ -1047,15 +1103,49 @@
                                           1 : 'CRITICAL',
                                           2 : 'ERROR',
                                           3 : 'WARNING',
                                           4 : 'INFO',
                                           5 : 'DEBUG'}
         optuna.logging.set_verbosity(getattr(optuna.logging, value_to_optuna_verbosity_dict[value]))
     # ------------------------------------------------------------------------------------------
-        
+
+    def _contains_float(self, iterable):
+        '''Check if float any floats are in iterable'''
+        return float in [type(x) for x in iterable]
+
+    def _all_ints(self, iterable):
+        '''Check if iterable contains only ints'''
+        return np.all([type(x)==int for x in iterable])
+
+    def _align_grid_and_search_space(self):
+        '''Redefine self.search_space for optuna based on self.grid which could be amended by user'''
+        unsupported_params = []
+        for param_name, param_grid in self.grid.items():
+            if param_name not in supported_gridsearch_params:
+                unsupported_params.append(param_name)
+                continue
+            if isinstance(param_grid, list):
+                self.search_space[param_name] = SearchSpace(Distribution.CHOICE, choices = param_grid)
+            elif isinstance(param_grid, tuple):
+                if self._contains_float(param_grid):
+                    self.search_space[param_name] = SearchSpace(Distribution.UNIFORM, low = min(param_grid), high = max(param_grid))
+                elif self._all_ints(param_grid):
+                    self.search_space[param_name] = SearchSpace(Distribution.INTUNIFORM, low = min(param_grid), high = max(param_grid))
+            elif isinstance(param_grid, dict):
+                if 'choices' in param_grid:
+                    self.search_space[param_name] = SearchSpace(Distribution.CHOICE, choices = param_grid['choices'])
+                elif 'low' in param_grid:
+                    if self._contains_float(param_grid.values()):
+                        self.search_space[param_name] = SearchSpace(Distribution.UNIFORM, low = param_grid['low'], high = param_grid['high'])
+                    elif self._all_ints(param_grid.values()):
+                        self.search_space[param_name] = SearchSpace(Distribution.INTUNIFORM, low = param_grid['low'], high = param_grid['high'])
+        if unsupported_params:
+            self.printer.print(f'Following changed parameters are not supported for tuning: {unsupported_params}', order = 'error', trailing_blank_paragraph=True)
+        self.grid = {key: value for key, value in self.grid.items() if key not in unsupported_params}
+    
     @timer
     def fit(self, X, y):
         '''
         Find optimized parameters for LightGBM model based on training data and 
         metric (defined by user at __init__).
         
         Considering the lower-better strategy:
@@ -1096,14 +1186,15 @@
         self.printer.print(f'Evaluation metric: {self.metric} ', order=4)
         self.printer.print(f'Study direction: minimize {optimization_metric_func.__name__}', order=4)#{get_study_direction(metric)} {optimization_metric_func.__name__})
         print()
             
         self.target_classes = y.unique().tolist()
         self._get_target_minimum(y)
         self._init_params_on_input(len(X), y)
+        self._align_grid_and_search_space()
         self._set_optuna_verbosity(self.verbosity)
         
         sampler = optuna.samplers.TPESampler(seed=self.seed)
         study = optuna.create_study(pruner=optuna.pruners.MedianPruner(n_warmup_steps=5), 
                                     sampler=sampler, 
                                     direction = 'minimize')#get_study_direction(metric))
 
@@ -1111,17 +1202,17 @@
 
         study.optimize(optimization_function, n_trials = self.trials)
 
 
         # populate the learned params into the suggested params
         temp_params = self._populate_best_params_to_init_params(study.best_params)
 
-        # tune n_estimators    
-        iteration, best_score = self.optimize_n_estimators(X.values, y.values, temp_params)
-        temp_params['n_estimators'] = iteration
+        # tune num_iterations    
+        iteration, best_score = self.optimize_num_iterations(X.values, y.values, temp_params)
+        temp_params['num_iterations'] = iteration
         self._best_params = temp_params        
         if self.refit:
             self.fit_optimized(X.values, y.values)
             self._save_feature_importances(X.columns)
         self._study = study
 
         if self.visualization:
@@ -1138,9 +1229,9 @@
         # clean up
         self.eval_results_callback = None
         # --------------------------------
         break_symbol = '|'
         print()
         self.printer.print(f"Optuna hyperparameters optimization finished", order=3)
         self.printer.print(f"Best trial number:{study.best_trial.number:>2}{break_symbol:>5}     {optimization_metric_func.__name__}:{study.best_trial.value:>29}", order=4, breakline='-')
-        self.printer.print(f'n_estimators optimization finished', order=3)
+        self.printer.print(f'num_iterations optimization finished', order=3)
         self.printer.print(f'best iteration:{iteration:>5}{break_symbol:>4}     {n_rounds_eval_metric}:{best_score:>29}', order=4, breakline='=')
```

### Comparing `verstack-3.6.7/verstack/lgbm_optuna_tuning/args_validators.py` & `verstack-3.7.0/verstack/lgbm_optuna_tuning/args_validators.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/lgbm_optuna_tuning/lgb_metrics.py` & `verstack-3.7.0/verstack/lgbm_optuna_tuning/lgb_metrics.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/lgbm_optuna_tuning/optuna_tools.py` & `verstack-3.7.0/verstack/lgbm_optuna_tuning/optuna_tools.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/stacking/Stacker.py` & `verstack-3.7.0/verstack/stacking/Stacker.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/stacking/args_validators.py` & `verstack-3.7.0/verstack/stacking/args_validators.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/stacking/generate_default_layers.py` & `verstack-3.7.0/verstack/stacking/generate_default_layers.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/stacking/kerasModel.py` & `verstack-3.7.0/verstack/stacking/kerasModel.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/stacking/load_stacker.py` & `verstack-3.7.0/verstack/stacking/load_stacker.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/stacking/optimise_params.py` & `verstack-3.7.0/verstack/stacking/optimise_params.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/stratified_continuous_split.py` & `verstack-3.7.0/verstack/stratified_continuous_split.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/tools.py` & `verstack-3.7.0/verstack/tools.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/common.py` & `verstack-3.7.0/verstack/unittest/common.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_Factorizer.py` & `verstack-3.7.0/verstack/unittest/test_Factorizer.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_FrequencyEncoder.py` & `verstack-3.7.0/verstack/unittest/test_FrequencyEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_LGBMTuner.py` & `verstack-3.7.0/verstack/unittest/test_LGBMTuner.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_MeanTargetEncoder.py` & `verstack-3.7.0/verstack/unittest/test_MeanTargetEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_Multicore.py` & `verstack-3.7.0/verstack/unittest/test_Multicore.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_OneHotEncoder.py` & `verstack-3.7.0/verstack/unittest/test_OneHotEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_Stacker.py` & `verstack-3.7.0/verstack/unittest/test_Stacker.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_ThreshTuner.py` & `verstack-3.7.0/verstack/unittest/test_ThreshTuner.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/test_WeightOfEvidenceEncoder.py` & `verstack-3.7.0/verstack/unittest/test_WeightOfEvidenceEncoder.py`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack/unittest/unittesting_manual.txt` & `verstack-3.7.0/verstack/unittest/unittesting_manual.txt`

 * *Files identical despite different names*

### Comparing `verstack-3.6.7/verstack.egg-info/PKG-INFO` & `verstack-3.7.0/verstack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: verstack
-Version: 3.6.7
+Version: 3.7.0
 Summary: Machine learning tools to make a Data Scientist's work more efficient
 Home-page: https://github.com/DanilZherebtsov/verstack
-Download-URL: https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.6.7.tar.gz
+Download-URL: https://github.com/DanilZherebtsov/verstack/archive/refs/tags/3.7.0.tar.gz
 Author: Danil Zherebtsov
 Author-email: danil.com@me.com
 License: MIT
 Keywords: impute,missing,values,stratify,nan,continuous,multiprocessing,concurrent,timer
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 .. image:: logo.png
 
-**verstack 3.6.7** is a set of Machine learning tools to make a Data Scientist's work efficient.
+**verstack 3.7.0** is a set of Machine learning tools to make a Data Scientist's work efficient.
 
 The package contains multiple tools for: training & tuning machine learning models, creating ensembles, working with datetime objects, data transformation & wrangling, imputing missing values, concurrency work and many more.
 
 Please refer to the `official documentation <https://verstack.readthedocs.io>`_ for more information.
 
 The project was created by Danil Zherebtsov in 2020.
```

### Comparing `verstack-3.6.7/verstack.egg-info/SOURCES.txt` & `verstack-3.7.0/verstack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -452,14 +452,15 @@
 verstack/stacking/Stacker.py
 verstack/stacking/__init__.py
 verstack/stacking/args_validators.py
 verstack/stacking/generate_default_layers.py
 verstack/stacking/kerasModel.py
 verstack/stacking/load_stacker.py
 verstack/stacking/optimise_params.py
+verstack/unittest/boston_train.parquet
 verstack/unittest/common.py
 verstack/unittest/test_DateParser.py
 verstack/unittest/test_Factorizer.py
 verstack/unittest/test_FrequencyEncoder.py
 verstack/unittest/test_LGBMTuner.py
 verstack/unittest/test_MeanTargetEncoder.py
 verstack/unittest/test_Multicore.py
```

