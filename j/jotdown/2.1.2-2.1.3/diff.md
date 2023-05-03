# Comparing `tmp/jotdown-2.1.2.tar.gz` & `tmp/jotdown-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jotdown-2.1.2.tar", last modified: Wed May  3 06:13:50 2023, max compression
+gzip compressed data, was "jotdown-2.1.3.tar", last modified: Wed May  3 06:21:32 2023, max compression
```

## Comparing `jotdown-2.1.2.tar` & `jotdown-2.1.3.tar`

### file list

```diff
@@ -1,26 +1,133 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1073 2023-05-02 20:41:15.000000 jotdown-2.1.2/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      121 2023-05-02 20:41:15.000000 jotdown-2.1.2/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-03 06:13:50.709586 jotdown-2.1.2/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3512 2023-05-02 20:41:15.000000 jotdown-2.1.2/README.md
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/include/jotdown/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1371 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/api.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19857 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/compiler.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      327 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/error.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1821 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/interfaces.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    33928 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/object.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    35119 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/parser.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26971 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/query.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2080 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/utils.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/jotdown.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-03 06:13:50.000000 jotdown-2.1.2/jotdown.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      471 2023-05-03 06:13:50.000000 jotdown-2.1.2/jotdown.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-03 06:13:50.000000 jotdown-2.1.2/jotdown.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-02 23:27:10.000000 jotdown-2.1.2/jotdown.egg-info/not-zip-safe
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-03 06:13:50.000000 jotdown-2.1.2/jotdown.egg-info/top_level.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      129 2023-05-03 00:21:08.000000 jotdown-2.1.2/pyproject.toml
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-03 06:13:50.709586 jotdown-2.1.2/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1498 2023-05-03 06:11:30.000000 jotdown-2.1.2/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/src/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19488 2023-05-02 20:41:15.000000 jotdown-2.1.2/src/jotdown.cpp
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.928892 jotdown-2.1.3/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1073 2023-05-02 20:41:15.000000 jotdown-2.1.3/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       85 2023-05-03 06:21:12.000000 jotdown-2.1.3/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-03 06:21:32.928892 jotdown-2.1.3/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3512 2023-05-02 20:41:15.000000 jotdown-2.1.3/README.md
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/moonlight/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/moonlight/deps/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/moonlight/deps/date/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/moonlight/deps/date/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.922226 jotdown-2.1.3/deps/moonlight/deps/date/include/date/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1467 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/chrono_io.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)   237524 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/date.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1609 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/ios.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    71119 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/islamic.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    43138 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/iso_week.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    71984 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/julian.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    27217 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/ptz.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    78728 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/solar_hijri.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    84615 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/tz.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10690 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/include/date/tz_private.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/moonlight/deps/date/test/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.922226 jotdown-2.1.3/deps/moonlight/deps/date/test/tz_test/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2602 2023-05-03 06:00:59.000000 jotdown-2.1.3/deps/moonlight/deps/date/test/tz_test/OffsetZone.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.922226 jotdown-2.1.3/deps/moonlight/deps/tinyformat/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    49197 2023-05-03 06:00:58.000000 jotdown-2.1.3/deps/moonlight/deps/tinyformat/tinyformat.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/moonlight/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.922226 jotdown-2.1.3/deps/moonlight/include/moonlight/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5894 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/ansi.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      812 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/as.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    12062 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/automata.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3878 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/classify.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7342 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/cli.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3614 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/collect.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5575 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/color.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      513 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/constants.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7476 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/curses.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26982 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/date.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    12925 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/debug.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4250 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/exceptions.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5833 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/file.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1489 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/finally.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    23071 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/generator.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      535 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/hash.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.925559 jotdown-2.1.3/deps/moonlight/include/moonlight/json/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4257 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/json/array.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6918 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/json/core.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5703 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/json/mapping.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6580 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/json/object.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11194 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/json/parser.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3780 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/json/serializer.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5160 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/json.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    17790 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/lex.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9257 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/linked_map.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      473 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/make.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1655 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/maps.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      648 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/meta.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2265 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/mmap.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1456 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/nanoid.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      819 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/posix.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1448 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/rx.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      689 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/sdl2.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6621 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/shlex.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1683 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/slice.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7645 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/string.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1597 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/system.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6729 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/test.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5179 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/time.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4166 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/traits.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7265 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/tty.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1830 2023-05-03 06:00:53.000000 jotdown-2.1.3/deps/moonlight/include/moonlight/variadic.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/pybind11/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/deps/pybind11/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.925559 jotdown-2.1.3/deps/pybind11/include/pybind11/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    23959 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7069 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    65942 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8458 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      120 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/common.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2096 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.925559 jotdown-2.1.3/deps/pybind11/include/pybind11/detail/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    28518 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    53288 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5962 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    17859 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    28221 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    42659 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1625 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/detail/typeid.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.925559 jotdown-2.1.3/deps/pybind11/include/pybind11/eigen/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    31450 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/eigen/matrix.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    18140 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/eigen/tensor.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      316 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13459 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4731 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5002 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8262 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8862 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    79416 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9103 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2734 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/options.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)   126420 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    94641 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.925559 jotdown-2.1.3/deps/pybind11/include/pybind11/stl/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4185 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    15399 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    29824 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.925559 jotdown-2.1.3/deps/pybind11/tests/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11736 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2847 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/tests/local_bindings.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5743 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/tests/object.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2685 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      399 2023-05-03 06:00:57.000000 jotdown-2.1.3/deps/pybind11/tests/test_exceptions.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.918892 jotdown-2.1.3/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.928892 jotdown-2.1.3/include/jotdown/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1371 2023-05-02 20:41:15.000000 jotdown-2.1.3/include/jotdown/api.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19857 2023-05-02 20:41:15.000000 jotdown-2.1.3/include/jotdown/compiler.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      327 2023-05-02 20:41:15.000000 jotdown-2.1.3/include/jotdown/error.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1821 2023-05-02 20:41:15.000000 jotdown-2.1.3/include/jotdown/interfaces.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    33928 2023-05-02 20:41:15.000000 jotdown-2.1.3/include/jotdown/object.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    35119 2023-05-02 20:41:15.000000 jotdown-2.1.3/include/jotdown/parser.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26971 2023-05-02 20:41:15.000000 jotdown-2.1.3/include/jotdown/query.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2080 2023-05-02 20:41:15.000000 jotdown-2.1.3/include/jotdown/utils.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.928892 jotdown-2.1.3/jotdown.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-03 06:21:32.000000 jotdown-2.1.3/jotdown.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4236 2023-05-03 06:21:32.000000 jotdown-2.1.3/jotdown.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-03 06:21:32.000000 jotdown-2.1.3/jotdown.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-02 23:27:10.000000 jotdown-2.1.3/jotdown.egg-info/not-zip-safe
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-03 06:21:32.000000 jotdown-2.1.3/jotdown.egg-info/top_level.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      129 2023-05-03 00:21:08.000000 jotdown-2.1.3/pyproject.toml
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-03 06:21:32.928892 jotdown-2.1.3/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1498 2023-05-03 06:21:22.000000 jotdown-2.1.3/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:21:32.928892 jotdown-2.1.3/src/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19488 2023-05-02 20:41:15.000000 jotdown-2.1.3/src/jotdown.cpp
```

### Comparing `jotdown-2.1.2/LICENSE` & `jotdown-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/PKG-INFO` & `jotdown-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jotdown
-Version: 2.1.2
+Version: 2.1.3
 Summary: Jotdown structrured document language, C++ to python wrapper module.
 Home-page: https://github.com/lainproliant/jotdown
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: document structure parser query language
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jotdown-2.1.2/README.md` & `jotdown-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/include/jotdown/api.h` & `jotdown-2.1.3/include/jotdown/api.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/include/jotdown/compiler.h` & `jotdown-2.1.3/include/jotdown/compiler.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/include/jotdown/interfaces.h` & `jotdown-2.1.3/include/jotdown/interfaces.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/include/jotdown/object.h` & `jotdown-2.1.3/include/jotdown/object.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/include/jotdown/parser.h` & `jotdown-2.1.3/include/jotdown/parser.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/include/jotdown/query.h` & `jotdown-2.1.3/include/jotdown/query.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/include/jotdown/utils.h` & `jotdown-2.1.3/include/jotdown/utils.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.2/jotdown.egg-info/PKG-INFO` & `jotdown-2.1.3/jotdown.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jotdown
-Version: 2.1.2
+Version: 2.1.3
 Summary: Jotdown structrured document language, C++ to python wrapper module.
 Home-page: https://github.com/lainproliant/jotdown
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: document structure parser query language
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jotdown-2.1.2/setup.py` & `jotdown-2.1.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 # Get the long description from the README file
 with open(Path("README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="jotdown",
-    version="2.1.2",
+    version="2.1.3",
     description="Jotdown structrured document language, C++ to python wrapper module.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/jotdown",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

### Comparing `jotdown-2.1.2/src/jotdown.cpp` & `jotdown-2.1.3/src/jotdown.cpp`

 * *Files identical despite different names*

