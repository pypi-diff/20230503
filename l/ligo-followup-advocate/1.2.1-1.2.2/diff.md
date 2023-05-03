# Comparing `tmp/ligo-followup-advocate-1.2.1.tar.gz` & `tmp/ligo-followup-advocate-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ligo-followup-advocate-1.2.1.tar", last modified: Thu Apr 20 18:01:03 2023, max compression
+gzip compressed data, was "ligo-followup-advocate-1.2.2.tar", last modified: Wed May  3 17:51:18 2023, max compression
```

## Comparing `ligo-followup-advocate-1.2.1.tar` & `ligo-followup-advocate-1.2.2.tar`

### file list

```diff
@@ -1,152 +1,168 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.914352 ligo-followup-advocate-1.2.1/
--rw-rw-rw-   0 root         (0) root         (0)    17895 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/COPYING.md
--rw-rw-rw-   0 root         (0) root         (0)      110 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      880 2023-04-20 18:01:03.915351 ligo-followup-advocate-1.2.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.876350 ligo-followup-advocate-1.2.1/ligo/
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.916351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/
--rw-rw-rw-   0 root         (0) root         (0)    21231 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-04-20 18:01:03.916351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1244 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/jinja.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.880350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/
--rw-rw-rw-   0 root         (0) root         (0)     2855 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/RAVEN_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      944 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/RAVEN_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/authors.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      376 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/compare_skymaps.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      795 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/em_bright.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     2184 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/initial_body.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/initial_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     8572 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/macros.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      567 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1786 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1504 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      344 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      461 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/p_astro.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      419 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/retraction.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1122 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/skymap_info.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      310 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/subject.jinja2
--rw-rw-rw-   0 root         (0) root         (0)     1350 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/update_circular.jinja2
--rw-rw-rw-   0 root         (0) root         (0)      223 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/userguide_conclusion.jinja2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.880350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.874350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.881350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/
--rw-rw-rw-   0 root         (0) root         (0)     1880 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.881350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      987 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.882350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1133/
--rw-rw-rw-   0 root         (0) root         (0)     1883 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1133/event.json
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1133/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.882350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.882350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      515 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.883350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/
--rw-rw-rw-   0 root         (0) root         (0)     1881 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.883350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)     1086 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.884350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/
--rw-rw-rw-   0 root         (0) root         (0)     1876 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.884350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       34 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)      610 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.885351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/
--rw-rw-rw-   0 root         (0) root         (0)     1904 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.885351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/
--rw-rw-rw-   0 root         (0) root         (0)       57 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/distances_x.json
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
--rw-rw-rw-   0 root         (0) root         (0)      991 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.886350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/
--rw-rw-rw-   0 root         (0) root         (0)     1918 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.886350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/files/
--rw-rw-rw-   0 root         (0) root         (0)     5761 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/files/initial.data
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.886350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/
--rw-rw-rw-   0 root         (0) root         (0)     1931 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/event.json
--rw-rw-rw-   0 root         (0) root         (0)      633 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.886350 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/
--rw-rw-rw-   0 root         (0) root         (0)     3958 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.887351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/
--rw-rw-rw-   0 root         (0) root         (0)     3956 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/event.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.887351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/files/
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.887351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/
--rw-rw-rw-   0 root         (0) root         (0)     3957 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/event.json
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.887351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/event.json
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/files.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.888351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.894351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/
--rw-rw-rw-   0 root         (0) root         (0)     4675 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       89 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)     1824 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7997 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5870 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.894351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.895351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/
--rw-rw-rw-   0 root         (0) root         (0)     4476 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)      766 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files.json
--rw-rw-rw-   0 root         (0) root         (0)     4911 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     3382 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)      966 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/voevents.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.897351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.913351 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)     6731 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
--rw-rw-rw-   0 root         (0) root         (0)     6716 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)       80 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
--rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
--rw-rw-rw-   0 root         (0) root         (0)   777600 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
--rw-rw-rw-   0 root         (0) root         (0)       44 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/em_bright.json
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/p_astro.json
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
--rw-rw-rw-   0 root         (0) root         (0)     2260 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files.json
--rw-rw-rw-   0 root         (0) root         (0)     7678 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/logs.json
--rw-rw-rw-   0 root         (0) root         (0)     5616 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/superevent.json
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/voevents.json
--rw-rw-rw-   0 root         (0) root         (0)     4791 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/test_tool.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/ligo/followup_advocate/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-20 18:01:03.914352 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/
--rw-r--r--   0 root         (0) root         (0)      880 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6415 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-04-20 18:01:03.000000 ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1793 2023-04-20 18:01:03.916351 ligo-followup-advocate-1.2.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      539 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-04-20 18:00:51.000000 ligo-followup-advocate-1.2.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.610091 ligo-followup-advocate-1.2.2/
+-rw-rw-rw-   0 root         (0) root         (0)    17895 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/COPYING.md
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      880 2023-05-03 17:51:18.610091 ligo-followup-advocate-1.2.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.567091 ligo-followup-advocate-1.2.2/ligo/
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.611091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/
+-rw-rw-rw-   0 root         (0) root         (0)    24975 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-05-03 17:51:18.611091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/jinja.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.573091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     2855 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/RAVEN_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      944 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/RAVEN_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      634 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/authors.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      376 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/compare_skymaps.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1032 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/em_bright.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2596 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/initial_body.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/initial_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/llama_alert_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      436 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/llama_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     2303 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/llama_track_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     9941 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/macros.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      567 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1786 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1504 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      344 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      461 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/p_astro.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      419 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/retraction.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1122 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/skymap_info.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      310 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/subject.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)     1350 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/update_circular.jinja2
+-rw-rw-rw-   0 root         (0) root         (0)      223 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/userguide_conclusion.jinja2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.573091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.566091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.574091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1880 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.574091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      987 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.575091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1133/
+-rw-rw-rw-   0 root         (0) root         (0)     1877 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1133/event.json
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1133/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.575091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.576091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      515 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.576091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.577091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)     1086 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.577091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/
+-rw-rw-rw-   0 root         (0) root         (0)     1876 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.578091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)      714 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)      610 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.578091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/
+-rw-rw-rw-   0 root         (0) root         (0)     1904 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.579091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/distances_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/distances_x.json
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_pygrb.json
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files/false_alarm_probability_x.json
+-rw-rw-rw-   0 root         (0) root         (0)      991 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.580091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/
+-rw-rw-rw-   0 root         (0) root         (0)     1918 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.580091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)     5761 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/files/initial.data
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.580091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/
+-rw-rw-rw-   0 root         (0) root         (0)     1936 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      633 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.581091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.581091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1235/
+-rw-rw-rw-   0 root         (0) root         (0)     3982 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1235/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1235/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.581091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/
+-rw-rw-rw-   0 root         (0) root         (0)     3956 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.582091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.582091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/event.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.582091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/files/
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2469/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.583091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/
+-rw-rw-rw-   0 root         (0) root         (0)     3958 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/event.json
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.583091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.583091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5679/
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5679/event.json
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5679/files.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.584091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.590091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4609 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
+-rw-rw-rw-   0 root         (0) root         (0)     4599 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       89 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)     1937 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7997 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5897 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1612 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.591091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.593091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/
+-rw-rw-rw-   0 root         (0) root         (0)     4476 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)  1065600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)     4047 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     4911 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     3397 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)      966 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/voevents.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.594091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.608091 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)     6731 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6716 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)  1540117 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)       80 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/coincidence_far.json
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0
+-rw-rw-rw-   0 root         (0) root         (0)  2224415 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1
+-rw-rw-rw-   0 root         (0) root         (0)   777600 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/em_bright.json
+-rw-rw-rw-   0 root         (0) root         (0)       52 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/em_bright.json,0
+-rw-rw-rw-   0 root         (0) root         (0)      107 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/p_astro.json
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/p_astro.json,0
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files.json
+-rw-rw-rw-   0 root         (0) root         (0)     7678 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/logs.json
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/superevent.json
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/voevents.json
+-rw-rw-rw-   0 root         (0) root         (0)     5123 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/test_tool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2576 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/ligo/followup_advocate/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 17:51:18.609091 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      880 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7102 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       76 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       79 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-03 17:51:18.000000 ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1793 2023-05-03 17:51:18.611091 ligo-followup-advocate-1.2.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      539 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-03 17:51:05.000000 ligo-followup-advocate-1.2.2/versioneer.py
```

### Comparing `ligo-followup-advocate-1.2.1/COPYING.md` & `ligo-followup-advocate-1.2.2/COPYING.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/PKG-INFO` & `ligo-followup-advocate-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.1
+Version: 1.2.2
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.1/README.md` & `ligo-followup-advocate-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/__init__.py` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -24,46 +24,61 @@
 
 
 def authors(authors, service=rest.DEFAULT_SERVICE_URL):
     """Write GCN Circular author list"""
     return env.get_template('authors.jinja2').render(authors=authors).strip()
 
 
-def guess_skyloc_pipeline(comments):
-    skyloc_pipelines = ['cWB', 'BAYESTAR', 'Bilby', 'LIB', 'LALInference',
-                        'oLIB', 'MLy', 'UNKNOWN']
-    for skyloc_pipeline in skyloc_pipelines:
-        if skyloc_pipeline.upper() in comments.upper():
-            break
-    return skyloc_pipeline
+def guess_skyloc_pipeline(filename):
+    keys = ['cWB', 'BAYESTAR', 'Bilby', 'LIB', 'LALInference',
+            'oLIB', 'MLy', 'UNKNOWN']
+    skyloc_pipelines_dict = dict(zip([x.lower() for x in keys], keys))
+    skyloc_pipelines_dict['rapidpe_rift'] = 'RapidPE-RIFT'
+    try:
+        return skyloc_pipelines_dict[filename.split('.')[0].lower()]
+    except KeyError:
+        return filename.split('.')[0]
 
 
 def main_dict(gracedb_id, client):
     """Create general dictionary to pass to compose circular"""
 
     event = client.superevent(gracedb_id).json()
     preferred_event = event['preferred_event_data']
     preferred_pipeline = preferred_event['pipeline']
-    other_pipelines = []
+    early_warning_pipelines = []
+    pipelines = []
     gw_events = event['gw_events']
+    early_warning_alert = False
 
     for gw_event in gw_events:
-        pipeline = client.event(gw_event).json()['pipeline']
-        if pipeline not in other_pipelines and pipeline != preferred_pipeline:
-            other_pipelines.append(pipeline)
+        gw_event_dict = client.event(gw_event).json()
+        pipeline = gw_event_dict['pipeline']
+        search = gw_event_dict['search']
+        if pipeline not in pipelines:
+            pipelines.append(pipeline)
+        if pipeline not in early_warning_pipelines and \
+                search == 'EarlyWarning':
+            early_warning_pipelines.append(pipeline)
+    # Sort to get alphabetical order
+    pipelines.sort()
+    early_warning_pipelines.sort()
 
     voevents = client.voevents(gracedb_id).json()['voevents']
     if not voevents:
         raise ValueError(
             "{} has no VOEvent to generate circulars from.".format(
                 gracedb_id))
 
-    pipelines = [preferred_pipeline] + other_pipelines
     citation_index = {pipeline.lower(): pipelines.index(pipeline) + 1 for
                       pipeline in pipelines}
+    for pipeline in early_warning_pipelines:
+        if pipeline.lower() != 'mbta':
+            citation_index[pipeline.lower() + '_earlywarning'] = \
+                max(citation_index.values()) + 1
 
     gpstime = float(preferred_event['gpstime'])
     event_time = astropy.time.Time(gpstime, format='gps').utc
 
     # Grab latest p_astro and em_bright files
     superevent_files = client.files(gracedb_id).json()
     em_brightfilename = 'em_bright'
@@ -96,14 +111,17 @@
 
     skymaps = {}
     for voevent in voevents:
         voevent_text = client.files(gracedb_id, voevent['filename']).read()
         root = lxml.etree.fromstring(voevent_text)
         alert_type = root.find(
             './What/Param[@name="AlertType"]').attrib['value'].lower()
+        if alert_type == 'earlywarning':
+            # Add text for early warning detection if one early warning alert
+            early_warning_alert = True
         url = root.find('./What/Group/Param[@name="skymap_fits"]')
         if url is None:
             continue
         url = url.attrib['value']
         _, filename = os.path.split(url)
         skyloc_pipeline = guess_skyloc_pipeline(filename)
         issued_time = astropy.time.Time(root.find('./Who/Date').text).datetime
@@ -123,24 +141,26 @@
     kwargs = dict(
         subject='Identification',
         gracedb_id=gracedb_id,
         gracedb_service_url=urllib.parse.urlunsplit(
             (o.scheme, o.netloc, '/superevents/', '', '')),
         group=preferred_event['group'],
         pipeline=preferred_pipeline,
-        other_pipelines=other_pipelines,
         all_pipelines=pipelines,
+        early_warning_alert=early_warning_alert,
+        early_warning_pipelines=early_warning_pipelines,
         gpstime='{0:.03f}'.format(round(float(preferred_event['gpstime']), 3)),
         search=preferred_event.get('search', ''),
         far=preferred_event['far'],
         utctime=event_time.iso,
         instruments=preferred_event['instruments'].split(','),
         skymaps=skymaps,
         prob_has_ns=source_classification.get('HasNS'),
         prob_has_remnant=source_classification.get('HasRemnant'),
+        prob_has_massgap=source_classification.get('HasMassGap'),
         include_ellipse=None,
         classifications=classifications,
         citation_index=citation_index)
 
     if skymaps:
         preferred_skymap = skymaps[-1]['filename']
         cl = 90
@@ -211,14 +231,87 @@
         .strip())
     body = (
         env.get_template('RAVEN_circular.jinja2').render(**kwargs)
         .strip())
     return '{0}\n\n{1}'.format(subject, body)
 
 
+def compose_llama(
+        gracedb_id, authors=(), service=rest.DEFAULT_SERVICE_URL,
+        icecube_alert=None,
+        client=None):
+    """Compose GRB LLAMA GCN Circular draft.
+    Here, gracedb_id will be a GRB superevent ID in GraceDb."""
+
+    if client is None:
+        client = rest.GraceDb(service)
+
+    superevent = client.superevent(gracedb_id).json()
+
+    gpstime = float(superevent['t_0'])
+    tl, th = gpstime - 500, gpstime + 500
+    event_time = astropy.time.Time(gpstime, format='gps').utc
+    tl_datetime = str(astropy.time.Time(
+                      tl, format='gps').isot).replace('T', ' ')
+    th_datetime = str(astropy.time.Time(
+                      th, format='gps').isot).replace('T', ' ')
+
+    o = urllib.parse.urlparse(client.service_url)
+    kwargs = dict(
+        gracedb_service_url=urllib.parse.urlunsplit(
+            (o.scheme, o.netloc, '/events/', '', '')),
+        gracedb_id=gracedb_id,
+        llama=True,
+        icecube_alert=icecube_alert,
+        event_time=event_time,
+        tl_datetime=tl_datetime,
+        th_datetime=th_datetime,
+        authors=authors)
+
+    citation_index = {'llama': 1, 'llama_stat': 2}
+    kwargs.update(citation_index=citation_index)
+
+    files = client.files(gracedb_id).json()
+
+    llama_stat_filename = 'significance_subthreshold_lvc-i3.json'
+    if llama_stat_filename in files:
+        llama_stat_file = client.files(gracedb_id, llama_stat_filename).json()
+        llama_fap = llama_stat_file["p_value"]
+        neutrinos = llama_stat_file["inputs"]["neutrino_info"]
+        lines = []
+        for neutrino in neutrinos:
+            # Build aligned string
+            vals = []
+            dt = (event_time -
+                  astropy.time.Time(neutrino['mjd'],
+                                    format='mjd')).to(u.s).value
+            vals.append('{:.2f}'.format(dt))
+            vals.append('{:.2f}'.format(neutrino['ra']))
+            vals.append('{:.2f}'.format(neutrino['dec']))
+            vals.append('{:.2f}'.format(neutrino['sigma']))
+            vals.append('{:.4f}'.format(llama_fap))
+            lines.append(align_number_string(vals, [0, 11, 21, 40, 59]))
+
+        kwargs.update(llama_fap=llama_fap,
+                      neutrinos=lines)
+
+    subject = (
+        env.get_template('llama_subject.jinja2').render(**kwargs)
+        .strip())
+    if icecube_alert:
+        body = (
+            env.get_template('llama_alert_circular.jinja2').render(**kwargs)
+            .strip())
+    else:
+        body = (
+            env.get_template('llama_track_circular.jinja2').render(**kwargs)
+            .strip())
+    return '{0}\n\n{1}'.format(subject, body)
+
+
 def compose_grb_medium_latency(
         gracedb_id, authors=(), service=rest.DEFAULT_SERVICE_URL, client=None):
     """Compose GRB Medium Latency GCN Circular draft.
     Here, gracedb_id will be a GRB external trigger ID in GraceDb."""
 
     if client is None:
         client = rest.GraceDb(service)
@@ -384,14 +477,21 @@
             pass
 
 
 def read_map_from_path(path, client):
     return read_map_gracedb(*path.split('/'), client)[0]
 
 
+def align_number_string(nums, positions):
+    positions.append(len(nums[-1]))
+    gen = (val + ' ' * (positions[i+1]-positions[i]-len(val))
+           for i, val in enumerate(nums))
+    return ''.join(gen)
+
+
 def mask_cl(p, level=90):
     pflat = p.ravel()
     i = np.flipud(np.argsort(p))
     cs = np.cumsum(pflat[i])
     cls = np.empty_like(pflat)
     cls[i] = cs
     cls = cls.reshape(p.shape)
@@ -473,16 +573,17 @@
     other_ext_pipelines = \
         [*set(client.event(id).json()['pipeline'] for id
               in event['em_events'])]
     # Remove preferred pipeline
     other_ext_pipelines.remove(external_pipeline)
     # FIXME in GraceDb: Even SNEWS triggers have an extra attribute GRB.
     external_trigger_id = em_event['extra_attributes']['GRB']['trigger_id']
-    snews = (em_event['search'] == 'Supernova')
-    grb = em_event['search'] in ['GRB', 'SubGRB', 'SubGRBTargeted', 'MDC']
+    snews = (em_event['pipeline'] == 'SNEWS')
+    grb = (em_event['search'] in ['GRB', 'SubGRB', 'SubGRBTargeted', 'MDC']
+           and not snews)
     subthreshold = em_event['search'] in ['SubGRB', 'SubGRBTargeted']
     subthreshold_targeted = em_event['search'] == 'SubGRBTargeted'
     far_grb = em_event['far']
 
     o = urllib.parse.urlparse(client.service_url)
     kwargs.update(
         gracedb_service_url=urllib.parse.urlunsplit(
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/jinja.py` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/jinja.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/RAVEN_circular.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/RAVEN_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/RAVEN_subject.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/RAVEN_subject.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/em_bright.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/em_bright.jinja2`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 {% from 'macros.jinja2' import evidence_for, probability,
                                citeskymap_number %}
 {% filter rewrap %}
 {% if subject == 'Update' %}Based on posterior support from parameter
 estimation {{citeskymap_number(updated_skymap.pipeline, citation_index)}},
 under the assumption that the candidate {{gracedb_id}} is astrophysical in
 origin,{% else %}Assuming the candidate is astrophysical in origin, {% endif %}
-the probability that the lighter compact object has a mass
-< 3 solar masses (HasNS) is {{probability(prob_has_ns)}}.
-[{{citation_index['em_bright']}}] Using the
-masses and spins inferred from the signal, the probability of
-matter outside the final compact object (HasRemnant)
-is {{probability(prob_has_remnant)}}. [{{citation_index['em_bright']}}]
+the probability that the lighter compact object is consistent with a neutron star mass
+(HasNS) is {{probability(prob_has_ns)}}.
+[{{citation_index['em_bright']}}] Using the masses and spins inferred from the signal, the
+probability of matter outside the final compact object (HasRemnant) is
+{{probability(prob_has_remnant)}}. [{{citation_index['em_bright']}}]
+Both HasNS and HasRemnant consider the support of several neutron star
+equations of state. The probability that any one of the binary components
+lie between 3 to 5 solar mass (HasMassgap) is {{probability(prob_has_massgap)}}.
 
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/initial_body.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/initial_body.jinja2`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 {% from 'macros.jinja2' import oxford_commas, evidence_for, probability,
                             naturalinstruments, naturalfar,
-                            naturalclassifications, naturalotherpipelines,
+                            naturalclassifications, naturalpipelines,
+                            naturalearlywarningpipelines,
                             renamegroup, citeskymap %}
 {% filter rewrap %}
 We identified the {{renamegroup(group)}} candidate {{gracedb_id}} during real-time processing of data from
 {{naturalinstruments(instruments, )}} at {{utctime}} UTC (GPS time: {{gpstime}}).
-The candidate was found by the {{naturalotherpipelines(pipeline, other_pipelines, citation_index)}}
-analysis pipeline{% if ([pipeline] + other_pipelines)|length > 1 %}s{% endif %}.
+The candidate was found by the {{naturalpipelines(all_pipelines, citation_index)}}
+analysis pipeline{% if all_pipelines|length > 1 %}s{% endif %}.
+{% if early_warning_alert and early_warning_pipelines %}
+An early-warning alert was issued for this candidate, with {% if early_warning_pipelines|length > 1 %}detections{% else %} a detection{% endif %} from the {{naturalearlywarningpipelines(early_warning_pipelines, citation_index)}} early-warning pipeline{% if early_warning_pipelines|length > 1 %}s{% endif %}.
+{% endif %}
 
 {% if change_significance_statement %}
 Based on the analysis of gravitational-wave data alone, this candidate does not meet our criteria for a high-significance public alert.
 However, a search performed by the RAVEN pipeline found a significant coincidence between this candidate and {{external_trigger}}.
 {% else %}
 {{gracedb_id}} is an event of interest because its false alarm rate, as
 estimated by the online analysis, is {{naturalfar(far)}}.
 {% endif %}
 The event's properties can be found at this URL:
+
 {{ gracedb_service_url }}{{ gracedb_id }}
 
 {% if not update_alert %}
 {% if classifications|length > 0 %}
 {%- include 'p_astro.jinja2' -%}
 {% endif %}
 {% if prob_has_ns is not none %}
 {%- include 'em_bright.jinja2' -%}
 {% endif %}
 {% if skymaps|length == 0 %}
 No{% else %}{{ skymaps|length|apnumber|capitalize }}{% endif %} {% if combined_skymap is not defined %}sky map{% else %}GW-only sky map{% endif %}{% if skymaps|length == 1 %} is{% else %}s are{% endif %} available at this time{% if skymaps|length > 0 %} and can be retrieved from the GraceDB event page:{% else %}.{% endif %}
 
 {% for skymap in skymaps %}
- * {{skymap.filename}}, an {% if skymap.alert_type in ['preliminary','initial'] %}initial{% else %}updated{% endif %} localization generated by {{citeskymap(skymap.pipeline, citation_index)}}, distributed via GCN notice about {{skymap.latency|naturaldelta}} after the candidate event time.
+ * {{skymap.filename}}, an {% if skymap.alert_type in ['earlywarning','preliminary','initial'] %}initial{% else %}updated{% endif %} localization generated by {{citeskymap(skymap.pipeline, citation_index)}}, distributed via GCN notice about {{skymap.latency|naturaldelta}} after the candidate event time.
 {% endfor %}
 
 {% if skymaps|length != 0 %}{%- include 'skymap_info.jinja2' -%}{% endif %}
 {% endif %}
 {% endfilter %}
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/macros.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/macros.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -94,27 +94,40 @@
 
 {% macro citeskymap_number(skymappipeline, citation_index) %}
 {% if skymappipeline|lower in citations %}[{{ citation_index[skymappipeline|lower] }}]
 {%- endif -%}
 {%- endmacro %}
 
 
-Macro to transform a list of other GW analysis pipelines like ['gstlal', 'mbtaonline', 'pycbc']
+Macro to transform a list of other GW analysis pipelines like ['gstlal', 'mbta', 'pycbc']
 to a natural-language list like "gstlal [2], mbtaonline [3], and pycbc [4]".
 
-{% macro naturalotherpipelines(preferred_pipeline, other_pipelines, citation_index, conjunction='and') %}
-{% for pipeline in [preferred_pipeline] + other_pipelines %}
+{% macro naturalpipelines(pipelines, citation_index, conjunction='and') %}
+{% for pipeline in pipelines %}
 {% if 'pycbc' == pipeline|lower %}PyCBC Live{% elif 'gstlal' == pipeline|lower %}GstLAL{% elif 'spiir' == pipeline|lower %}SPIIR{% else %}{{pipeline}}{% endif %} [{{citation_index[pipeline|lower]}}]
 {%- if loop.length > 2 and not loop.last %},{% endif %}
 {%- if loop.length > 1 and not loop.last %} {% endif %}
 {%- if loop.length > 1 and loop.revindex == 2 %}{{conjunction}} {% endif %}
 {% endfor %}
 {%- endmacro %}
 
 
+Macro to transform a list of GW analysis early warning pipelines like ['gstlal', 'mbta', 'pycbc']
+to a natural-language list like "gstlal [2], mbtaonline [3], and pycbc [4]".
+
+{% macro naturalearlywarningpipelines(early_warning_pipelines, citation_index, conjunction='and') %}
+{% for pipeline in early_warning_pipelines %}
+{% if 'pycbc' == pipeline|lower %}PyCBC Live{% elif 'gstlal' == pipeline|lower %}GstLAL{% elif 'spiir' == pipeline|lower %}SPIIR{% else %}{{pipeline}}{% endif %} {% if 'mbta' == pipeline|lower %}[{{citation_index[pipeline|lower]}}]{% else %}[{{citation_index[(pipeline+'_earlywarning')|lower]}}]{% endif %}
+{%- if loop.length > 2 and not loop.last %},{% endif %}
+{%- if loop.length > 1 and not loop.last %} {% endif %}
+{%- if loop.length > 1 and loop.revindex == 2 %}{{conjunction}} {% endif %}
+{% endfor %}
+{%- endmacro %}
+
+
 Macro to enumerate and cite all GW analysis pipelines involved for the superevent; including the
 skymap pipelines.
 
 {%- macro citenumberedpipelines(citation_index) -%}
 {% for key in citation_index %}
  [{{ citation_index[key|lower] }}] {{citations[key|lower]}}
 {% endfor %}
@@ -230,19 +243,25 @@
 {%- endif -%}
 {%- endmacro -%}
 
 
 Dictionary of common citations.
 
 {% set citations = {'pycbc': 'Dal Canton et al. ApJ 923, 254 (2021)',
-                    'mbta': 'Adams et al. CQG 33, 175012 (2016)',
-                    'gstlal': 'Messick et al. PRD 95, 042001 (2017)',
+                    'mbta': 'Aubin et al. CQG 38, 095004 (2021)',
+                    'gstlal': 'Tsukada et al. LIGO-DCC P2300116 (2023) and Ewing et al. LIGO-DCC P2300124 (2023)',
                     'spiir': 'Qi Chu, PhD Thesis, The University of Western Australia (2017)',
+                    'pycbc_earlywarning': 'Nitz A. H., Schäfer M., Dal Canton T. ApJL 902, 2 (2020)',
+                    'gstlal_earlywarning': 'Sachdev et al. ApJL 905, 2 (2020)',
+                    'spiir_earlywarning': 'Kovalam et al. ApJL 927, 1 (2022)',
                     'cwb': 'Klimenko et al. PRD 93, 042004 (2016)',
                     'olib': 'Lynch et al. PRD 95, 104046 (2017)',
                     'mly': 'Skliris et al. arXiv:2009.14611 (2020)',
                     'em_bright': 'Chatterjee et al. The Astrophysical Journal 896, 1 (2020)',
                     'pygrb': 'Williamson et al. PRD 90, 122004 (2014)',
                     'xpipeline': 'Was et al. PRD 86, 022003 (2012)',
+                    'llama': 'Baret et al., Astroparticle Physics 35, 1 (2011)',
+                    'llama_stat': 'Bartos et al. arXiv:1810.11467 (2018) and Countryman et al.\n arXiv:1901.05486 (2019)',
                     'bayestar': 'Singer & Price PRD 93, 024013 (2016)',
                     'bilby': 'Ashton et al. ApJS 241, 27 (2019)',
-                    'lalinference': 'Veitch et al. PRD 91, 042003 (2015)'} %}
+                    'lalinference': 'Veitch et al. PRD 91, 042003 (2015)',
+                    'rapidpe_rift': 'Rose et al. arXiv:2201.05263 (2022)'} %}
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/skymap_info.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/skymap_info.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/templates/update_circular.jinja2` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/templates/update_circular.jinja2`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1122/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1133/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1133/event.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'search'": "'MDC'"}*

```diff
@@ -35,11 +35,11 @@
         "neighbors": "https://gracedb-pcdev1.ligo.org/api/events/E1133/neighbors/",
         "self": "https://gracedb-pcdev1.ligo.org/api/events/E1133",
         "tags": "https://gracedb-pcdev1.ligo.org/api/events/E1133/tag/"
     },
     "nevents": null,
     "offline": false,
     "pipeline": "SNEWS",
-    "search": "Supernova",
+    "search": "MDC",
     "submitter": "emfollow",
     "superevent": "S1234"
 }
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1134/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1134/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files/initial.data` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1234/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files/initial.data` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E1235/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E1235/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E2244/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E2244/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/E5678/files/initial.data` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/E5678/files/initial.data`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/event.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9705882352941176%*

 * *Differences: {"'gpstime'": '1366915853.2760432'}*

```diff
@@ -19,15 +19,15 @@
             "snr": 5.91607978309962,
             "start_time": 1227349206,
             "start_time_ns": 726600000
         }
     },
     "far": 7.80319e-08,
     "far_is_upper_limit": false,
-    "gpstime": 1214190501.74,
+    "gpstime": 1366915853.2760432,
     "graceid": "M1122",
     "group": "Burst",
     "instruments": "H1,L1,V1",
     "labels": [],
     "likelihood": 35.0,
     "links": {
         "emobservations": "https://gracedb-playground.ligo.org/api/events/M1122/emobservation/",
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1122/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1122/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M1234/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M1234/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/event.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M2468/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M2468/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/event.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9411764705882353%*

 * *Differences: {"'group'": "'CBC'", "'pipeline'": "'MBTA'"}*

```diff
@@ -83,27 +83,27 @@
             }
         ]
     },
     "far": 9.1106993648613e-07,
     "far_is_upper_limit": false,
     "gpstime": 1214190502.740928,
     "graceid": "M5678",
-    "group": "Burst",
+    "group": "CBC",
     "instruments": "H1,L1",
     "labels": [],
     "likelihood": 2.69725974901838e+25,
     "links": {
         "emobservations": "https://gracedb-dev1.ligo.org/api/events/M5678/emobservation/",
         "files": "https://gracedb-dev1.ligo.org/api/events/M5678/files/",
         "labels": "https://gracedb-dev1.ligo.org/api/events/M5678/labels/",
         "log": "https://gracedb-dev1.ligo.org/api/events/M5678/log/",
         "neighbors": "https://gracedb-dev1.ligo.org/api/events/M5678/neighbors/",
         "self": "https://gracedb-dev1.ligo.org/api/events/M5678",
         "tags": "https://gracedb-dev1.ligo.org/api/events/M5678/tag/"
     },
     "nevents": 2,
     "offline": false,
-    "pipeline": "oLIB",
+    "pipeline": "MBTA",
     "search": "MDC",
     "submitter": "leo.singer@LIGO.ORG",
     "superevent": "S180628g"
 }
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5566/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/event.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5566/event.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9117647058823529%*

 * *Differences: {"'gpstime'": '1366915853.2860432', "'group'": "'Burst'", "'pipeline'": "'oLIB'"}*

```diff
@@ -81,29 +81,29 @@
                 "template_duration": 94.5259213794174,
                 "ttotal": 94.521187
             }
         ]
     },
     "far": 9.1106993648613e-07,
     "far_is_upper_limit": false,
-    "gpstime": 1214190502.740928,
+    "gpstime": 1366915853.2860432,
     "graceid": "M5678",
-    "group": "CBC",
+    "group": "Burst",
     "instruments": "H1,L1",
     "labels": [],
     "likelihood": 2.69725974901838e+25,
     "links": {
         "emobservations": "https://gracedb-dev1.ligo.org/api/events/M5678/emobservation/",
         "files": "https://gracedb-dev1.ligo.org/api/events/M5678/files/",
         "labels": "https://gracedb-dev1.ligo.org/api/events/M5678/labels/",
         "log": "https://gracedb-dev1.ligo.org/api/events/M5678/log/",
         "neighbors": "https://gracedb-dev1.ligo.org/api/events/M5678/neighbors/",
         "self": "https://gracedb-dev1.ligo.org/api/events/M5678",
         "tags": "https://gracedb-dev1.ligo.org/api/events/M5678/tag/"
     },
     "nevents": 2,
     "offline": false,
-    "pipeline": "MBTA",
+    "pipeline": "oLIB",
     "search": "MDC",
     "submitter": "leo.singer@LIGO.ORG",
     "superevent": "S180628g"
 }
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/M5678/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/M5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml`

 * *Files 2% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml`

```diff
@@ -1,24 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
-<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-1-Initial">
+<voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S1234-1-EarlyWarning">
   <Who>
-    <Date>2018-06-28T13:42:02</Date>
+    <Date>2018-06-28T13:36:02</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
     </Param>
     <Param name="Pkt_Ser_Num" dataType="string" value="1"/>
     <Param name="SupereventID" dataType="string" value="S1234" ucd="meta.id">
       <Description>Identifier in GraceDB</Description>
     </Param>
-    <Param name="AlertType" dataType="string" value="Initial" ucd="meta.version" unit="">
+    <Param name="AlertType" dataType="string" value="EarlyWarning" ucd="meta.version" unit="">
       <Description>VOEvent alert type</Description>
     </Param>
     <Param name="Retraction" dataType="string" value="false" ucd="meta.code" unit="">
       <Description>Set to true if the event is retracted.</Description>
     </Param>
     <Param name="HardwareInj" dataType="int" value="0" ucd="meta.number" unit="">
       <Description>Indicates that this event is a hardware injection if 1, no if 0</Description>
@@ -48,15 +48,14 @@
       <Description>Specific low-latency search</Description>
     </Param>
     <Param dataType="int" name="Significant" ucd="meta.number" value="1">
       <Description>Indicates that this event is a significant alert if 1, no if 0</Description>
     </Param>
     <Group type="GW_SKYMAP" name="BAYESTAR">
       <Param name="skymap_fits" dataType="string" value="https://gracedb-playground.ligo.org/apibasic/superevents/S1234/files/bayestar.fits.gz" ucd="meta.ref.url" unit="">
-        <Description>Sky Map FITS basic auth protected</Description>
         <Description>Sky Map FITS</Description>
       </Param>
     </Group>
   </What>
   <WhereWhen>
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/files.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7619047619047619%*

 * *Differences: {"'S1234-1-EarlyWarning.xml'": "'https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-1-EarlyWarning.xml'",*

 * * "'S1234-2-Initial.xml'": "'https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-2-Initial.xml'",*

 * * "'S1234-3-Update.xml'": "'https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-3-Update.xml'",*

 * * 'delete': "['S1234-1-Initial.xml', 'S1234-2-Update.xml']"}*

```diff
@@ -1,10 +1,11 @@
 {
-    "S1234-1-Initial.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-1-Initial.xml",
-    "S1234-2-Update.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-2-Update.xml",
+    "S1234-1-EarlyWarning.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-1-EarlyWarning.xml",
+    "S1234-2-Initial.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-2-Initial.xml",
+    "S1234-3-Update.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/S1234-3-Update.xml",
     "bayestar-ext.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar-ext.fits.gz",
     "bayestar.fits.gz": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.fits.gz",
     "bayestar.fits.gz,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.fits.gz,0",
     "bayestar.multiorder.fits": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.multiorder.fits",
     "bayestar.multiorder.fits,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/bayestar.multiorder.fits,0",
     "coinc.xml": "https://gracedb-dev1.ligo.org/api/events/S1234/files/coinc.xml",
     "coinc.xml,0": "https://gracedb-dev1.ligo.org/api/events/S1234/files/coinc.xml,0",
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/logs.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/superevent.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S1234/superevent.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.984375%*

 * *Differences: {"'gw_events'": "{insert: [(1, 'M1235'), (3, 'M5679'), (5, 'M2469')]}"}*

```diff
@@ -5,16 +5,19 @@
         "E1234",
         "E2244",
         "E1235"
     ],
     "em_type": "E1234",
     "gw_events": [
         "M1234",
+        "M1235",
         "M5678",
-        "M2468"
+        "M5679",
+        "M2468",
+        "M2469"
     ],
     "labels": [
         "EM_COINC",
         "EM_SelectedConfident"
     ],
     "links": {
         "emobservations": "https://gracedb-dev1.ligo.org/api/superevents/S1234/emobservations/",
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S1234/voevents.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/voevents.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9201388888888888%*

 * *Differences: {"'links'": "{'self': 'https://gracedb-playground.ligo.org/api/superevents/S2468/voevents/', "*

 * *            "'first': 'https://gracedb-playground.ligo.org/api/superevents/S2468/voevents/', "*

 * *            "'last': 'https://gracedb-playground.ligo.org/api/superevents/S2468/voevents/'}",*

 * * "'voevents'": "{0: {'ivorn': 'ivo://gwnet/gcn_sender#S2468-1-Initial', 'filename': "*

 * *               "'S2468-1-Initial.xml', 'links': {'self': "*

 * *               "'https://gracedb-playground.ligo.org/api/superevents/S2468/voevents […]*

```diff
@@ -1,27 +1,27 @@
 {
     "links": {
-        "first": "https://gracedb-playground.ligo.org/api/superevents/S1234/voevents/",
-        "last": "https://gracedb-playground.ligo.org/api/superevents/S1234/voevents/",
-        "self": "https://gracedb-playground.ligo.org/api/superevents/S1234/voevents/"
+        "first": "https://gracedb-playground.ligo.org/api/superevents/S2468/voevents/",
+        "last": "https://gracedb-playground.ligo.org/api/superevents/S2468/voevents/",
+        "self": "https://gracedb-playground.ligo.org/api/superevents/S2468/voevents/"
     },
     "numRows": 1,
     "start": 0,
     "voevents": [
         {
             "N": 1,
             "created": "2018-06-28 13:42:02 UTC",
             "file_version": 0,
-            "filename": "S1234-1-Initial.xml",
+            "filename": "S2468-1-Initial.xml",
             "issuer": "emfollow",
-            "ivorn": "ivo://gwnet/gcn_sender#S1234-1-Initial",
+            "ivorn": "ivo://gwnet/gcn_sender#S2468-1-Initial",
             "links": {
                 "file": [
-                    "https://gracedb-playground.ligo.org/api/superevents/S1234/files/S1234-1-Initial.xml,0"
+                    "https://gracedb-playground.ligo.org/api/superevents/S2468/files/S2468-1-Initial.xml,0"
                 ],
-                "self": "https://gracedb-playground.ligo.org/api/superevents/S1234/voevents/1/"
+                "self": "https://gracedb-playground.ligo.org/api/superevents/S2468/voevents/1/"
             },
             "text": "voevent text",
             "voevent_type": "IN"
         }
     ]
 }
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

 * *Files 2% similar despite different names*

#### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml`

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <voe:VOEvent xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:voe="http://www.ivoa.net/xml/VOEvent/v2.0" xsi:schemaLocation="http://www.ivoa.net/xml/VOEvent/v2.0 http://www.ivoa.net/xml/VOEvent/VOEvent-v2.0.xsd" version="2.0" role="test" ivorn="ivo://gwnet/gcn_sender#S2468-1-Initial">
   <Who>
-    <Date>2018-06-28T13:42:02</Date>
+    <Date>2023-04-30T18:55:35</Date>
     <Author>
       <contactName>LIGO Scientific Collaboration and Virgo Collaboration</contactName>
     </Author>
   </Who>
   <What>
     <Param name="internal" dataType="int" value="1">
       <Description>Indicates whether this event should be distributed to LSC/Virgo members only</Description>
@@ -58,15 +58,15 @@
     <ObsDataLocation>
       <ObservatoryLocation id="LIGO Virgo"/>
       <ObservationLocation>
         <AstroCoordSystem id="UTC-FK5-GEO"/>
         <AstroCoords coord_system_id="UTC-FK5-GEO">
           <Time>
             <TimeInstant>
-              <ISOTime>2018-06-28T13:35:16.911085</ISOTime>
+              <ISOTime>2023-04-30T18:50:35.276956</ISOTime>
             </TimeInstant>
           </Time>
         </AstroCoords>
       </ObservationLocation>
     </ObsDataLocation>
   </WhereWhen>
   <How>
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/files.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.875%*

 * *Differences: {"'significance_subthreshold_lvc-i3.json'": "'https://gracedb-dev1.ligo.org/api/events/S2468/files/significance_subthreshold_lvc-i3.json'"}*

```diff
@@ -1,9 +1,10 @@
 {
     "S2468-1-Initial.xml": "https://gracedb-dev1.ligo.org/api/events/S2468/files/S2468-1-Initial.xml",
     "cwb.multiorder.fits": "https://gracedb-playground.ligo.org/api/events/S2468/files/cwb.multiorder.fits",
     "cwb.multiorder.fits,0": "https://gracedb-playground.ligo.org/api/events/S2468/files/cwb.multiorder.fits",
     "event.log": "https://gracedb-playground.ligo.org/api/events/S2468/files/event.log",
     "event.log,0": "https://gracedb-playground.ligo.org/api/events/S2468/files/event.log,0",
+    "significance_subthreshold_lvc-i3.json": "https://gracedb-dev1.ligo.org/api/events/S2468/files/significance_subthreshold_lvc-i3.json",
     "trigger_1227349206.7390.txt": "https://gracedb-playground.ligo.org/api/events/S2468/files/trigger_1227349206.7390.txt",
     "trigger_1227349206.7390.txt,0": "https://gracedb-playground.ligo.org/api/events/S2468/files/trigger_1227349206.7390.txt,0"
 }
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/logs.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S2468/superevent.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S2468/superevent.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8928571428571429%*

 * *Differences: {"'t_0'": '1366915853.2760432', "'t_end'": '1366915854.2760432', "'t_start'": '1366915852.2760432'}*

```diff
@@ -77,11 +77,11 @@
         "pipeline": "CWB",
         "search": "AllSky",
         "submitter": "waveburst",
         "superevent": "S2468"
     },
     "submitter": "leo.singer@LIGO.ORG",
     "superevent_id": "S2468",
-    "t_0": 1214190502.74,
-    "t_end": 1214190503.74,
-    "t_start": 1214190501.74
+    "t_0": 1366915853.2760432,
+    "t_end": 1366915854.2760432,
+    "t_start": 1366915852.2760432
 }
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/bilby.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,0`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.fits.gz,1`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files/combined-ext.multiorder.fits`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/files.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/files.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/logs.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/logs.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/superevent.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/superevent.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/data/S5678/voevents.json` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/data/S5678/voevents.json`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/test/test_tool.py` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/test/test_tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,25 @@
 
 
 def test_medium_latency_cbc_burst_exclusion(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/',
           'compose_grb_medium_latency', 'E2244'])
 
 
+def test_llama_neutrino_track(mock_gracedb):
+    main(['--service', 'https://gracedb.invalid/api/',
+          'compose_llama', 'S2468'])
+
+
+def test_llama_icecube_alert(mock_gracedb):
+    main(['--service', 'https://gracedb.invalid/api/',
+          'compose_llama', 'S2468',
+          '--icecube_alert', 'IceCubeCascade-230430a'])
+
+
 def test_retraction(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/', 'compose_retraction',
           'S1234'])
 
 
 def test_retraction_early_warning(mock_gracedb):
     main(['--service', 'https://gracedb.invalid/api/', 'compose_retraction',
```

### Comparing `ligo-followup-advocate-1.2.1/ligo/followup_advocate/tool.py` & `ligo-followup-advocate-1.2.2/ligo/followup_advocate/tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -32,14 +32,20 @@
     cmd.add_argument('gracedb_id', metavar='S123456',
                      help='GraceDB ID of superevent')
 
     cmd = add_command(followup_advocate.compose_raven, parents=[authors])
     cmd.add_argument('gracedb_id', metavar='S123456',
                      help='GraceDB ID of superevent')
 
+    cmd = add_command(followup_advocate.compose_llama, parents=[authors])
+    cmd.add_argument('gracedb_id', metavar='S123456', help='GraceDB ID')
+    cmd.add_argument('--icecube_alert', metavar='IceCube-230501',
+                     required=False,
+                     default=None, help='IceCube alert ID')
+
     cmd = add_command(followup_advocate.compose_grb_medium_latency,
                       parents=[authors])
     cmd.add_argument('gracedb_id', metavar='E123456', help='GraceDB ID of GRB')
 
     cmd = add_command(followup_advocate.compose_update, parents=[authors])
     cmd.add_argument('gracedb_id', metavar='S123456', help='GraceDB ID')
     cmd.add_argument('update_types', metavar='[sky_localization]',
```

### Comparing `ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/PKG-INFO` & `ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ligo-followup-advocate
-Version: 1.2.1
+Version: 1.2.2
 Summary: LIGO/Virgo/KAGRA Follow-up Advocate Tools
 Home-page: https://git.ligo.org/emfollow/ligo-followup-advocate
 Author: Leo Singer
 Author-email: leo.singer@ligo.org
 Maintainer: Brandon Piotrzkowski
 Maintainer-email: brandon.piotrzkowski@ligo.org
 License: GPL-2+
```

### Comparing `ligo-followup-advocate-1.2.1/ligo_followup_advocate.egg-info/SOURCES.txt` & `ligo-followup-advocate-1.2.2/ligo_followup_advocate.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 ligo/followup_advocate/templates/RAVEN_subject.jinja2
 ligo/followup_advocate/templates/__init__.py
 ligo/followup_advocate/templates/authors.jinja2
 ligo/followup_advocate/templates/compare_skymaps.jinja2
 ligo/followup_advocate/templates/em_bright.jinja2
 ligo/followup_advocate/templates/initial_body.jinja2
 ligo/followup_advocate/templates/initial_circular.jinja2
+ligo/followup_advocate/templates/llama_alert_circular.jinja2
+ligo/followup_advocate/templates/llama_subject.jinja2
+ligo/followup_advocate/templates/llama_track_circular.jinja2
 ligo/followup_advocate/templates/macros.jinja2
 ligo/followup_advocate/templates/medium_latency_grb_circular.jinja2
 ligo/followup_advocate/templates/medium_latency_grb_detection_circular.jinja2
 ligo/followup_advocate/templates/medium_latency_grb_exclusion_circular.jinja2
 ligo/followup_advocate/templates/medium_latency_grb_subject.jinja2
 ligo/followup_advocate/templates/numbered_pipeline_citations.jinja2
 ligo/followup_advocate/templates/p_astro.jinja2
@@ -65,38 +68,47 @@
 ligo/followup_advocate/test/data/E5678/event.json
 ligo/followup_advocate/test/data/E5678/files.json
 ligo/followup_advocate/test/data/E5678/files/initial.data
 ligo/followup_advocate/test/data/M1122/event.json
 ligo/followup_advocate/test/data/M1122/files.json
 ligo/followup_advocate/test/data/M1234/event.json
 ligo/followup_advocate/test/data/M1234/files.json
+ligo/followup_advocate/test/data/M1235/event.json
+ligo/followup_advocate/test/data/M1235/files.json
 ligo/followup_advocate/test/data/M2468/event.json
 ligo/followup_advocate/test/data/M2468/files.json
 ligo/followup_advocate/test/data/M2468/files/p_astro.json
+ligo/followup_advocate/test/data/M2469/event.json
+ligo/followup_advocate/test/data/M2469/files.json
+ligo/followup_advocate/test/data/M2469/files/p_astro.json
 ligo/followup_advocate/test/data/M5566/event.json
 ligo/followup_advocate/test/data/M5566/files.json
 ligo/followup_advocate/test/data/M5678/event.json
 ligo/followup_advocate/test/data/M5678/files.json
+ligo/followup_advocate/test/data/M5679/event.json
+ligo/followup_advocate/test/data/M5679/files.json
 ligo/followup_advocate/test/data/S1234/files.json
 ligo/followup_advocate/test/data/S1234/logs.json
 ligo/followup_advocate/test/data/S1234/superevent.json
 ligo/followup_advocate/test/data/S1234/voevents.json
-ligo/followup_advocate/test/data/S1234/files/S1234-1-Initial.xml
+ligo/followup_advocate/test/data/S1234/files/S1234-1-EarlyWarning.xml
+ligo/followup_advocate/test/data/S1234/files/S1234-2-Initial.xml
 ligo/followup_advocate/test/data/S1234/files/bayestar-ext.fits.gz
 ligo/followup_advocate/test/data/S1234/files/bayestar.fits.gz
 ligo/followup_advocate/test/data/S1234/files/bayestar.multiorder.fits
 ligo/followup_advocate/test/data/S1234/files/coincidence_far.json
 ligo/followup_advocate/test/data/S1234/files/em_bright.json
 ligo/followup_advocate/test/data/S1234/files/p_astro.json
 ligo/followup_advocate/test/data/S2468/files.json
 ligo/followup_advocate/test/data/S2468/logs.json
 ligo/followup_advocate/test/data/S2468/superevent.json
 ligo/followup_advocate/test/data/S2468/voevents.json
 ligo/followup_advocate/test/data/S2468/files/S2468-1-Initial.xml
 ligo/followup_advocate/test/data/S2468/files/cwb.multiorder.fits
+ligo/followup_advocate/test/data/S2468/files/significance_subthreshold_lvc-i3.json
 ligo/followup_advocate/test/data/S5678/files.json
 ligo/followup_advocate/test/data/S5678/logs.json
 ligo/followup_advocate/test/data/S5678/superevent.json
 ligo/followup_advocate/test/data/S5678/voevents.json
 ligo/followup_advocate/test/data/S5678/files/LALInference.fits.gz,0
 ligo/followup_advocate/test/data/S5678/files/S5678-1-Initial.xml
 ligo/followup_advocate/test/data/S5678/files/S5678-2-Update.xml
```

### Comparing `ligo-followup-advocate-1.2.1/setup.cfg` & `ligo-followup-advocate-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/setup.py` & `ligo-followup-advocate-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `ligo-followup-advocate-1.2.1/versioneer.py` & `ligo-followup-advocate-1.2.2/versioneer.py`

 * *Files identical despite different names*

