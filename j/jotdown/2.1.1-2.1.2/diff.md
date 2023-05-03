# Comparing `tmp/jotdown-2.1.1.tar.gz` & `tmp/jotdown-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jotdown-2.1.1.tar", last modified: Tue May  2 23:43:17 2023, max compression
+gzip compressed data, was "jotdown-2.1.2.tar", last modified: Wed May  3 06:13:50 2023, max compression
```

## Comparing `jotdown-2.1.1.tar` & `jotdown-2.1.2.tar`

### file list

```diff
@@ -1,122 +1,26 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.442318 jotdown-2.1.1/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1073 2023-05-02 20:41:15.000000 jotdown-2.1.1/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      121 2023-05-02 20:41:15.000000 jotdown-2.1.1/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-02 23:43:17.442318 jotdown-2.1.1/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3512 2023-05-02 20:41:15.000000 jotdown-2.1.1/README.md
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.432318 jotdown-2.1.1/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.435651 jotdown-2.1.1/include/jotdown/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1371 2023-05-02 20:41:15.000000 jotdown-2.1.1/include/jotdown/api.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19857 2023-05-02 20:41:15.000000 jotdown-2.1.1/include/jotdown/compiler.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      327 2023-05-02 20:41:15.000000 jotdown-2.1.1/include/jotdown/error.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1821 2023-05-02 20:41:15.000000 jotdown-2.1.1/include/jotdown/interfaces.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    33928 2023-05-02 20:41:15.000000 jotdown-2.1.1/include/jotdown/object.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    35119 2023-05-02 20:41:15.000000 jotdown-2.1.1/include/jotdown/parser.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26971 2023-05-02 20:41:15.000000 jotdown-2.1.1/include/jotdown/query.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2080 2023-05-02 20:41:15.000000 jotdown-2.1.1/include/jotdown/utils.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.435651 jotdown-2.1.1/jotdown.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-02 23:43:17.000000 jotdown-2.1.1/jotdown.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3488 2023-05-02 23:43:17.000000 jotdown-2.1.1/jotdown.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-02 23:43:17.000000 jotdown-2.1.1/jotdown.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-02 23:27:10.000000 jotdown-2.1.1/jotdown.egg-info/not-zip-safe
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-02 23:43:17.000000 jotdown-2.1.1/jotdown.egg-info/top_level.txt
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.432318 jotdown-2.1.1/moonlight/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.432318 jotdown-2.1.1/moonlight/deps/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.432318 jotdown-2.1.1/moonlight/deps/date/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.432318 jotdown-2.1.1/moonlight/deps/date/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.438984 jotdown-2.1.1/moonlight/deps/date/include/date/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1467 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/chrono_io.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)   235920 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/date.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1617 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/ios.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    71119 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/islamic.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    43034 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/iso_week.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    71992 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/julian.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    24012 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/ptz.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    78738 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/solar_hijri.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    84617 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/tz.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10690 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/include/date/tz_private.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.432318 jotdown-2.1.1/moonlight/deps/date/test/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.438984 jotdown-2.1.1/moonlight/deps/date/test/tz_test/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2602 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/date/test/tz_test/OffsetZone.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.438984 jotdown-2.1.1/moonlight/deps/tinyformat/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    49197 2023-05-02 20:57:39.000000 jotdown-2.1.1/moonlight/deps/tinyformat/tinyformat.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.435651 jotdown-2.1.1/moonlight/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.438984 jotdown-2.1.1/moonlight/include/moonlight/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7148 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/ansi.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    12260 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/automata.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3944 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/classify.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7672 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/cli.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3614 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/collect.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6235 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/color.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      513 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/constants.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8598 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/curses.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26982 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/date.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    12915 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/debug.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4250 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/exceptions.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5833 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/file.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1489 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/finally.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    22082 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/generator.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      601 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/hash.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.442318 jotdown-2.1.1/moonlight/include/moonlight/json/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4257 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/json/array.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6890 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/json/core.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5703 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/json/mapping.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6580 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/json/object.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11194 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/json/parser.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3780 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/json/serializer.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5160 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/json.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10383 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/lex.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9257 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/linked_map.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      473 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/make.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1655 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/maps.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      648 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/meta.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2595 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/mmap.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1456 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/nanoid.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      819 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/posix.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      689 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/sdl2.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6627 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/shlex.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1683 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/slice.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7645 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/string.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1597 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/system.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6131 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/test.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5179 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/time.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4166 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/traits.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7265 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/tty.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1830 2023-05-02 20:57:37.000000 jotdown-2.1.1/moonlight/include/moonlight/variadic.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.435651 jotdown-2.1.1/pybind11/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.435651 jotdown-2.1.1/pybind11/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.442318 jotdown-2.1.1/pybind11/include/pybind11/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    20266 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/attr.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4823 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    92922 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/cast.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7701 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      120 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/common.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2001 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.442318 jotdown-2.1.1/pybind11/include/pybind11/detail/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25371 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    38852 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3566 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    16322 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    15964 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1450 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    29043 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7849 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/embed.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3865 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/eval.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3599 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/functional.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5655 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    67870 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9049 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/operators.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2031 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/options.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    99932 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    58683 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    14029 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/stl.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    23239 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.442318 jotdown-2.1.1/pybind11/tests/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11157 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/tests/constructor_stats.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2126 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/tests/local_bindings.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5389 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/tests/object.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2151 2023-05-02 20:57:39.000000 jotdown-2.1.1/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      114 2023-05-02 23:43:10.000000 jotdown-2.1.1/pyproject.toml
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-02 23:43:17.442318 jotdown-2.1.1/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1454 2023-05-02 23:42:06.000000 jotdown-2.1.1/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 23:43:17.442318 jotdown-2.1.1/src/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19488 2023-05-02 20:41:15.000000 jotdown-2.1.1/src/jotdown.cpp
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1073 2023-05-02 20:41:15.000000 jotdown-2.1.2/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      121 2023-05-02 20:41:15.000000 jotdown-2.1.2/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-03 06:13:50.709586 jotdown-2.1.2/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3512 2023-05-02 20:41:15.000000 jotdown-2.1.2/README.md
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/include/jotdown/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1371 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/api.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19857 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/compiler.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      327 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/error.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1821 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/interfaces.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    33928 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/object.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    35119 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/parser.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26971 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/query.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2080 2023-05-02 20:41:15.000000 jotdown-2.1.2/include/jotdown/utils.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/jotdown.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-03 06:13:50.000000 jotdown-2.1.2/jotdown.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      471 2023-05-03 06:13:50.000000 jotdown-2.1.2/jotdown.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-03 06:13:50.000000 jotdown-2.1.2/jotdown.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-02 23:27:10.000000 jotdown-2.1.2/jotdown.egg-info/not-zip-safe
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-03 06:13:50.000000 jotdown-2.1.2/jotdown.egg-info/top_level.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      129 2023-05-03 00:21:08.000000 jotdown-2.1.2/pyproject.toml
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-03 06:13:50.709586 jotdown-2.1.2/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1498 2023-05-03 06:11:30.000000 jotdown-2.1.2/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-03 06:13:50.709586 jotdown-2.1.2/src/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19488 2023-05-02 20:41:15.000000 jotdown-2.1.2/src/jotdown.cpp
```

### Comparing `jotdown-2.1.1/LICENSE` & `jotdown-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/PKG-INFO` & `jotdown-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jotdown
-Version: 2.1.1
+Version: 2.1.2
 Summary: Jotdown structrured document language, C++ to python wrapper module.
 Home-page: https://github.com/lainproliant/jotdown
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: document structure parser query language
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jotdown-2.1.1/README.md` & `jotdown-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/include/jotdown/api.h` & `jotdown-2.1.2/include/jotdown/api.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/include/jotdown/compiler.h` & `jotdown-2.1.2/include/jotdown/compiler.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/include/jotdown/interfaces.h` & `jotdown-2.1.2/include/jotdown/interfaces.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/include/jotdown/object.h` & `jotdown-2.1.2/include/jotdown/object.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/include/jotdown/parser.h` & `jotdown-2.1.2/include/jotdown/parser.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/include/jotdown/query.h` & `jotdown-2.1.2/include/jotdown/query.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/include/jotdown/utils.h` & `jotdown-2.1.2/include/jotdown/utils.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.1.1/jotdown.egg-info/PKG-INFO` & `jotdown-2.1.2/jotdown.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jotdown
-Version: 2.1.1
+Version: 2.1.2
 Summary: Jotdown structrured document language, C++ to python wrapper module.
 Home-page: https://github.com/lainproliant/jotdown
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
 Keywords: document structure parser query language
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `jotdown-2.1.1/setup.py` & `jotdown-2.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from pathlib import Path
 from setuptools import setup
 from pybind11.setup_helpers import Pybind11Extension, build_ext
+from xeno.shell import check
 
 ext_modules = [
     Pybind11Extension(
         name="jotdown",
         include_dirs=[
             "include",
-            "moonlight/deps",
-            "moonlight/include",
-            "pybind11/include",
+            "deps/moonlight/deps",
+            "deps/moonlight/include",
+            "deps/pybind11/include",
         ],
         sources=[str(src) for src in Path.cwd().glob("src/*.cpp")],
         extra_compile_args=["-O3", "-shared", "-std=c++2a", "-fPIC", "-fpermissive"],
     )
 ]
 
 # Get the long description from the README file
 with open(Path("README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="jotdown",
-    version="2.1.1",
+    version="2.1.2",
     description="Jotdown structrured document language, C++ to python wrapper module.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/jotdown",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

### Comparing `jotdown-2.1.1/src/jotdown.cpp` & `jotdown-2.1.2/src/jotdown.cpp`

 * *Files identical despite different names*

