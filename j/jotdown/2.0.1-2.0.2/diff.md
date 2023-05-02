# Comparing `tmp/jotdown-2.0.1.tar.gz` & `tmp/jotdown-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jotdown-2.0.1.tar", last modified: Tue Jan 26 00:36:36 2021, max compression
+gzip compressed data, was "jotdown-2.0.2.tar", last modified: Tue May  2 22:05:31 2023, max compression
```

## Comparing `jotdown-2.0.1.tar` & `jotdown-2.0.2.tar`

### file list

```diff
@@ -1,224 +1,121 @@
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.114206 jotdown-2.0.1/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       73 2021-01-20 00:59:54.000000 jotdown-2.0.1/.gitignore
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      173 2021-01-20 00:59:54.000000 jotdown-2.0.1/.gitmodules
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1322 2021-01-24 12:16:39.000000 jotdown-2.0.1/.ycm_extra_conf.py
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    12636 2021-01-20 00:59:54.000000 jotdown-2.0.1/DOCUMENTATION.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1073 2021-01-20 00:59:54.000000 jotdown-2.0.1/LICENSE
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      121 2021-01-20 00:59:54.000000 jotdown-2.0.1/MANIFEST.in
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4792 2021-01-26 00:36:36.114206 jotdown-2.0.1/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3512 2021-01-24 12:16:39.000000 jotdown-2.0.1/README.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       42 2021-01-24 12:16:39.000000 jotdown-2.0.1/TODO
--rwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)     6566 2021-01-24 12:16:39.000000 jotdown-2.0.1/build.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.084206 jotdown-2.0.1/demo/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      703 2021-01-20 00:59:54.000000 jotdown-2.0.1/demo/demo.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      984 2021-01-20 00:59:54.000000 jotdown-2.0.1/demo/jd-json.cpp
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2132 2021-01-20 00:59:54.000000 jotdown-2.0.1/demo/jd-query.cpp
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      943 2021-01-24 12:16:39.000000 jotdown-2.0.1/demo/jd-roundtrip.cpp
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1120 2021-01-20 00:59:54.000000 jotdown-2.0.1/demo/jd-tokenize.cpp
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.077539 jotdown-2.0.1/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.087539 jotdown-2.0.1/include/jotdown/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1368 2021-01-24 11:26:41.000000 jotdown-2.0.1/include/jotdown/api.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19806 2021-01-24 12:16:39.000000 jotdown-2.0.1/include/jotdown/compiler.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      460 2021-01-20 00:59:54.000000 jotdown-2.0.1/include/jotdown/error.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1808 2021-01-20 00:59:54.000000 jotdown-2.0.1/include/jotdown/interfaces.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    31738 2021-01-24 12:16:39.000000 jotdown-2.0.1/include/jotdown/object.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    35031 2021-01-24 12:16:39.000000 jotdown-2.0.1/include/jotdown/parser.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26230 2021-01-24 11:54:02.000000 jotdown-2.0.1/include/jotdown/query.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5078 2021-01-24 12:16:39.000000 jotdown-2.0.1/include/jotdown/utils.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.087539 jotdown-2.0.1/jotdown.egg-info/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4792 2021-01-26 00:36:35.000000 jotdown-2.0.1/jotdown.egg-info/PKG-INFO
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9097 2021-01-26 00:36:35.000000 jotdown-2.0.1/jotdown.egg-info/SOURCES.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2021-01-26 00:36:35.000000 jotdown-2.0.1/jotdown.egg-info/dependency_links.txt
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2021-01-24 12:16:56.000000 jotdown-2.0.1/jotdown.egg-info/not-zip-safe
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2021-01-26 00:36:35.000000 jotdown-2.0.1/jotdown.egg-info/top_level.txt
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/deps/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/deps/date/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/deps/date/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.090873 jotdown-2.0.1/moonlight/deps/date/include/date/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1467 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/chrono_io.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)   230423 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/date.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1617 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/ios.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    71119 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/islamic.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    43034 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/iso_week.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    71643 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/julian.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    18346 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/ptz.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    78234 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/solar_hijri.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    84515 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/tz.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10686 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/include/date/tz_private.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/deps/date/test/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.090873 jotdown-2.0.1/moonlight/deps/date/test/tz_test/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2602 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/deps/date/test/tz_test/OffsetZone.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.094206 jotdown-2.0.1/moonlight/include/moonlight/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4578 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/ansi.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    12213 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/automata.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7264 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/cli.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3771 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/collect.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      881 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/core.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8691 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/curses.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1011 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/debug.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5557 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/exceptions.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5906 2021-01-22 23:18:49.000000 jotdown-2.0.1/moonlight/include/moonlight/file.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7013 2021-01-22 23:13:49.000000 jotdown-2.0.1/moonlight/include/moonlight/generator.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      533 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/hash.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13110 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/json.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5332 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/linked_map.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      472 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/make.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2029 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/maps.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2591 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/mmap.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      819 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/posix.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      689 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/sdl2.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1830 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/slice.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5186 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/string.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      625 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/system.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5929 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/test.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5179 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/time.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1834 2021-01-20 01:10:02.000000 jotdown-2.0.1/moonlight/include/moonlight/variadic.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.094206 jotdown-2.0.1/moonlight/include/picojson/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    33087 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/include/picojson/picojson.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.094206 jotdown-2.0.1/moonlight/include/picojson/picotest/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1519 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/include/picojson/picotest/picotest.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.094206 jotdown-2.0.1/moonlight/include/tinyformat/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    43125 2021-01-20 01:10:07.000000 jotdown-2.0.1/moonlight/include/tinyformat/tinyformat.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.084206 jotdown-2.0.1/moonlight/inifile-cpp/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/inifile-cpp/dep/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.080873 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.107539 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5044 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_approx.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2714 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_assertionhandler.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      910 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_assertioninfo.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1800 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_assertionresult.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3762 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_capture_matchers.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1275 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_clara.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      582 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_commandline.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3023 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_common.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    13682 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_compiler_capabilities.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1797 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_console_colour.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1627 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_context.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      461 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_debug_console.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1469 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_debugger.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9742 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_decomposer.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1552 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_enforce.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1057 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_enum_values_registry.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      502 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_errno_guard.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1011 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_exception_translator_registry.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      752 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_external_interfaces.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1509 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_fatal_condition.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3631 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_capture.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2661 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_config.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1454 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_enum_values_registry.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3122 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_exception.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1273 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_generatortracker.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2216 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_registry_hub.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9286 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_reporter.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      552 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_runner.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      881 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_tag_alias_registry.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1277 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_interfaces_testcase.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      465 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_leak_detector.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      967 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_list.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5678 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_matchers.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1652 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_matchers_floating.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3169 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_matchers_string.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6810 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_matchers_vector.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2892 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_message.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3335 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_output_redirect.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      822 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_platform.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      571 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_random_number_generator.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      594 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_reenable_warnings.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1086 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_reporter_registry.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1634 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_result_type.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5644 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_run_context.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1587 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_section.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1156 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_section_info.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1692 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_session.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      813 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_startup_exception_registry.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1194 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_stream.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1460 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_string_manip.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4209 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_stringref.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1019 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_suppress_warnings.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      655 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_tag_alias.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      895 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_tag_alias_autoregistrar.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1019 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_tag_alias_registry.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2502 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_test_case_info.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2415 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_test_case_registry_impl.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4474 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_test_case_tracker.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    27527 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_test_registry.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2665 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_test_spec.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2665 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_test_spec_parser.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      475 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_text.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      885 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_timer.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    20435 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_tostring.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1063 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_totals.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      511 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_uncaught_exceptions.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      596 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_user_interfaces.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1234 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_version.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1141 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_wildcard_pattern.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      966 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_windows_h_proxy.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2892 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/internal/catch_xmlwriter.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.107539 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/reporters/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1155 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/reporters/catch_reporter_compact.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3036 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/reporters/catch_reporter_console.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1949 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/reporters/catch_reporter_junit.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2418 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/reporters/catch_reporter_listening.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2123 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/include/reporters/catch_reporter_xml.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.084206 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/projects/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.084206 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/projects/XCode/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.084206 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/projects/XCode/OCTest/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.107539 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/projects/XCode/OCTest/OCTest/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      581 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/projects/XCode/OCTest/OCTest/CatchOCTestCase.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      581 2021-01-22 23:38:59.000000 jotdown-2.0.1/moonlight/inifile-cpp/dep/Catch2/projects/XCode/OCTest/OCTest/TestObj.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.107539 jotdown-2.0.1/moonlight/inifile-cpp/include/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    15872 2021-01-22 23:38:56.000000 jotdown-2.0.1/moonlight/inifile-cpp/include/inicpp.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.084206 jotdown-2.0.1/pybind11/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.084206 jotdown-2.0.1/pybind11/include/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.110873 jotdown-2.0.1/pybind11/include/pybind11/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    20266 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/attr.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4823 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    92922 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/cast.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7701 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      120 2021-01-20 01:10:07.000000 jotdown-2.0.1/pybind11/include/pybind11/common.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2001 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.110873 jotdown-2.0.1/pybind11/include/pybind11/detail/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25371 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    38852 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3566 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    16322 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    15964 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1450 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    29043 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7849 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/embed.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3865 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/eval.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3599 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/functional.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5655 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    67870 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9049 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/operators.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2031 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/options.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    99932 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    58683 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/pytypes.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    14029 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/stl.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    23239 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.114206 jotdown-2.0.1/pybind11/tests/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11157 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/tests/constructor_stats.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2126 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/tests/local_bindings.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5389 2021-01-20 01:10:07.000000 jotdown-2.0.1/pybind11/tests/object.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2151 2021-01-24 12:09:00.000000 jotdown-2.0.1/pybind11/tests/pybind11_tests.h
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2114 2021-01-20 00:59:54.000000 jotdown-2.0.1/select-notes.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       63 2021-01-20 00:59:54.000000 jotdown-2.0.1/select-test.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2021-01-26 00:36:36.114206 jotdown-2.0.1/setup.cfg
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1309 2021-01-26 00:36:00.000000 jotdown-2.0.1/setup.py
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.114206 jotdown-2.0.1/src/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    20809 2021-01-26 00:35:07.000000 jotdown-2.0.1/src/jotdown.cpp
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.114206 jotdown-2.0.1/test/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.084206 jotdown-2.0.1/test/data/
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.114206 jotdown-2.0.1/test/data/front-matter/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      123 2021-01-20 00:59:54.000000 jotdown-2.0.1/test/data/front-matter/front-matter-json.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      108 2021-01-20 00:59:54.000000 jotdown-2.0.1/test/data/front-matter/front-matter-no-langspec.md
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.114206 jotdown-2.0.1/test/data/links/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      180 2021-01-24 12:16:39.000000 jotdown-2.0.1/test/data/links/links.md
-drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2021-01-26 00:36:36.114206 jotdown-2.0.1/test/data/query/
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       73 2021-01-20 00:59:54.000000 jotdown-2.0.1/test/data/query/children.md
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1339 2021-01-20 00:59:54.000000 jotdown-2.0.1/test/front-matter.cpp
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      626 2021-01-24 12:16:39.000000 jotdown-2.0.1/test/links.cpp
--rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3341 2021-01-20 00:59:54.000000 jotdown-2.0.1/test/query.cpp
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.573832 jotdown-2.0.2/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1073 2023-05-02 20:41:15.000000 jotdown-2.0.2/LICENSE
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      121 2023-05-02 20:41:15.000000 jotdown-2.0.2/MANIFEST.in
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-02 22:05:31.573832 jotdown-2.0.2/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3512 2023-05-02 20:41:15.000000 jotdown-2.0.2/README.md
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.567165 jotdown-2.0.2/include/jotdown/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1371 2023-05-02 20:41:15.000000 jotdown-2.0.2/include/jotdown/api.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19857 2023-05-02 20:41:15.000000 jotdown-2.0.2/include/jotdown/compiler.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      327 2023-05-02 20:41:15.000000 jotdown-2.0.2/include/jotdown/error.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1821 2023-05-02 20:41:15.000000 jotdown-2.0.2/include/jotdown/interfaces.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    33928 2023-05-02 20:41:15.000000 jotdown-2.0.2/include/jotdown/object.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    35119 2023-05-02 20:41:15.000000 jotdown-2.0.2/include/jotdown/parser.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26971 2023-05-02 20:41:15.000000 jotdown-2.0.2/include/jotdown/query.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2080 2023-05-02 20:41:15.000000 jotdown-2.0.2/include/jotdown/utils.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.567165 jotdown-2.0.2/jotdown.egg-info/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4175 2023-05-02 22:05:31.000000 jotdown-2.0.2/jotdown.egg-info/PKG-INFO
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3473 2023-05-02 22:05:31.000000 jotdown-2.0.2/jotdown.egg-info/SOURCES.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-02 22:05:31.000000 jotdown-2.0.2/jotdown.egg-info/dependency_links.txt
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        1 2023-05-02 22:05:31.000000 jotdown-2.0.2/jotdown.egg-info/not-zip-safe
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)        8 2023-05-02 22:05:31.000000 jotdown-2.0.2/jotdown.egg-info/top_level.txt
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/moonlight/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/moonlight/deps/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/moonlight/deps/date/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/moonlight/deps/date/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.567165 jotdown-2.0.2/moonlight/deps/date/include/date/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1467 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/chrono_io.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)   235920 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/date.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1617 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/ios.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    71119 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/islamic.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    43034 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/iso_week.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    71992 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/julian.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    24012 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/ptz.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    78738 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/solar_hijri.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    84617 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/tz.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10690 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/include/date/tz_private.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/moonlight/deps/date/test/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.567165 jotdown-2.0.2/moonlight/deps/date/test/tz_test/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2602 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/date/test/tz_test/OffsetZone.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.567165 jotdown-2.0.2/moonlight/deps/tinyformat/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    49197 2023-05-02 20:57:39.000000 jotdown-2.0.2/moonlight/deps/tinyformat/tinyformat.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/moonlight/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.570499 jotdown-2.0.2/moonlight/include/moonlight/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7148 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/ansi.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    12260 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/automata.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3944 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/classify.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7672 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/cli.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3614 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/collect.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6235 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/color.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      513 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/constants.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     8598 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/curses.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    26982 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/date.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    12915 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/debug.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4250 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/exceptions.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5833 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/file.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1489 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/finally.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    22082 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/generator.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      601 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/hash.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.570499 jotdown-2.0.2/moonlight/include/moonlight/json/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4257 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/json/array.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6890 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/json/core.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5703 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/json/mapping.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6580 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/json/object.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11194 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/json/parser.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3780 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/json/serializer.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5160 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/json.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    10383 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/lex.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9257 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/linked_map.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      473 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/make.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1655 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/maps.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      648 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/meta.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2595 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/mmap.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1456 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/nanoid.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      819 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/posix.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      689 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/sdl2.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6627 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/shlex.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1683 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/slice.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7645 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/string.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1597 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/system.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     6131 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/test.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5179 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/time.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4166 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/traits.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7265 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/tty.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1830 2023-05-02 20:57:37.000000 jotdown-2.0.2/moonlight/include/moonlight/variadic.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/pybind11/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.563832 jotdown-2.0.2/pybind11/include/
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.570499 jotdown-2.0.2/pybind11/include/pybind11/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    20266 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     4823 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    92922 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7701 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)      120 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/common.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2001 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.573832 jotdown-2.0.2/pybind11/include/pybind11/detail/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    25371 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    38852 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3566 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    16322 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    15964 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1450 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    29043 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     7849 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3865 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     3599 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5655 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    67870 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     9049 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2031 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/options.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    99932 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    58683 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/pytypes.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    14029 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    23239 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.573832 jotdown-2.0.2/pybind11/tests/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    11157 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/tests/constructor_stats.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2126 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/tests/local_bindings.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     5389 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/tests/object.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     2151 2023-05-02 20:57:39.000000 jotdown-2.0.2/pybind11/tests/pybind11_tests.h
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)       38 2023-05-02 22:05:31.573832 jotdown-2.0.2/setup.cfg
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)     1309 2023-05-02 22:05:23.000000 jotdown-2.0.2/setup.py
+drwxr-xr-x   0 lainproliant  (1000) lainproliant  (1000)        0 2023-05-02 22:05:31.573832 jotdown-2.0.2/src/
+-rw-r--r--   0 lainproliant  (1000) lainproliant  (1000)    19488 2023-05-02 20:41:15.000000 jotdown-2.0.2/src/jotdown.cpp
```

### Comparing `jotdown-2.0.1/LICENSE` & `jotdown-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/PKG-INFO` & `jotdown-2.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 Metadata-Version: 2.1
 Name: jotdown
-Version: 2.0.1
+Version: 2.0.2
 Summary: Jotdown structrured document language, C++ to python wrapper module.
 Home-page: https://github.com/lainproliant/jotdown
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
-Description: # Jotdown
-        Jotdown is a structured document language.  It is an opinionated, augmented
-        subset of Markdown with features inspired by plain-text organizational tools
-        like org-mode.  The main purpose of Jotdown is to centralize personal and
-        project organization into a set of plain-text documents that can be easily
-        edited, parsed, and manipulated both by scripts and humans alike.
-        
-        Jotdown is offered simultaneously as a header-only C++ library and a compiled
-        Python module sharing the same code.  The Python bindings are enabled via
-        pybind11.  It is released under an MIT license, see LICENSE for more info.
-        
-        See [DOCUMENTATION.md] for a detailed explanation of the language and its
-        features.
-        
-        See [API_CXX.md] for documentation regarding the header-only C++ library.
-        
-        See [API_PY.md] for documentation regarding the Python module, including how to
-        build and install it.
-        
-        ## Goals
-        These are the primary goals of the Jotdown language and project:
-        
-        - Support the creation, analysis, and modification of plain-text structured
-            documents.
-        - Support the hypertext linkage of documents within a document-set, and to
-            outside resources on the web or elsewhere.
-        - First-class support for loading, querying, modifying, saving, and creating
-            documents in C++ and Python.
-        
-        ## Q/A
-        ### Why not just use Markdown for this?
-        While Markdown is great as a text formatting language, it doesn't work as an
-        easily parsable structured document language.  It's main focus has always been 
-        generating HTML, and as such many of the existing parsers don't even bother
-        creating an intermediate AST.  I also feel that Markdown, though it is formally
-        defined in the CommonMark and Github Flavored Markdown specs, has hugely complex
-        rules for parsing to support features that aren't often used or don't need to
-        exist.
-        
-        ### Why is Jotdown offered in C++ and Python?
-        I wanted to be able to support the runtime power and expressiveness of C++ while
-        also extending support into Python where scripts and plugins can be easily built
-        around Jotdown document structures.
-        
-        ### Why is my language not supported?
-        I'm sorry!  I'm really happy you're interested in Jotdown though.  Feel free to
-        submit an issue to add support for your language.  I can't guarantee I'll ever
-        get around to writing bindings myself, but someone in the community might step
-        up and help out!
-        
-        ### What are you planning to do with Jotdown in the future?
-        Some things I'm planning on building around Jotdown include:
-        
-        - A Vim plugin which will support advanced editing features and highlighting.
-        - Command line productivity tools built around the concept of a Jotdown document set.
-        - A web wiki built around the concept of a Jotdown document set.
-        
-        # Change Log
-        ### 01/24/2021: v2.0.0
-        - Removed support for custom '@' style links, replaced with Markdown style
-          links and link indexes.
-        
-        ### 07/24/2020: v1.3.0
-        - Added support for document front-matter.
-        - New features for the Python interface:
-          - Collections are now callable.  With no arguments, calling them will return
-            their contents as a list.  With arguments, they will return themselves with
-            all of the arguments being added in sequence.
-          - Section can now be constructed with a string or a TextContent for the header.
-          - TextContent can now be initialized with a string.
-        
-        ### 07/17/2020: v1.2.0
-        - Refactored `objects.h` to do runtime validation of insertion types rather than
-          limiting via the C++ type system to reduce code duplication.
-        - Added `Container::insert_before` and `Container::insert_after`.
-        
-        
 Keywords: document structure parser query language
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Jotdown
+Jotdown is a structured document language.  It is an opinionated, augmented
+subset of Markdown with features inspired by plain-text organizational tools
+like org-mode.  The main purpose of Jotdown is to centralize personal and
+project organization into a set of plain-text documents that can be easily
+edited, parsed, and manipulated both by scripts and humans alike.
+
+Jotdown is offered simultaneously as a header-only C++ library and a compiled
+Python module sharing the same code.  The Python bindings are enabled via
+pybind11.  It is released under an MIT license, see LICENSE for more info.
+
+See [DOCUMENTATION.md] for a detailed explanation of the language and its
+features.
+
+See [API_CXX.md] for documentation regarding the header-only C++ library.
+
+See [API_PY.md] for documentation regarding the Python module, including how to
+build and install it.
+
+## Goals
+These are the primary goals of the Jotdown language and project:
+
+- Support the creation, analysis, and modification of plain-text structured
+    documents.
+- Support the hypertext linkage of documents within a document-set, and to
+    outside resources on the web or elsewhere.
+- First-class support for loading, querying, modifying, saving, and creating
+    documents in C++ and Python.
+
+## Q/A
+### Why not just use Markdown for this?
+While Markdown is great as a text formatting language, it doesn't work as an
+easily parsable structured document language.  It's main focus has always been 
+generating HTML, and as such many of the existing parsers don't even bother
+creating an intermediate AST.  I also feel that Markdown, though it is formally
+defined in the CommonMark and Github Flavored Markdown specs, has hugely complex
+rules for parsing to support features that aren't often used or don't need to
+exist.
+
+### Why is Jotdown offered in C++ and Python?
+I wanted to be able to support the runtime power and expressiveness of C++ while
+also extending support into Python where scripts and plugins can be easily built
+around Jotdown document structures.
+
+### Why is my language not supported?
+I'm sorry!  I'm really happy you're interested in Jotdown though.  Feel free to
+submit an issue to add support for your language.  I can't guarantee I'll ever
+get around to writing bindings myself, but someone in the community might step
+up and help out!
+
+### What are you planning to do with Jotdown in the future?
+Some things I'm planning on building around Jotdown include:
+
+- A Vim plugin which will support advanced editing features and highlighting.
+- Command line productivity tools built around the concept of a Jotdown document set.
+- A web wiki built around the concept of a Jotdown document set.
+
+# Change Log
+### 01/24/2021: v2.0.0
+- Removed support for custom '@' style links, replaced with Markdown style
+  links and link indexes.
+
+### 07/24/2020: v1.3.0
+- Added support for document front-matter.
+- New features for the Python interface:
+  - Collections are now callable.  With no arguments, calling them will return
+    their contents as a list.  With arguments, they will return themselves with
+    all of the arguments being added in sequence.
+  - Section can now be constructed with a string or a TextContent for the header.
+  - TextContent can now be initialized with a string.
+
+### 07/17/2020: v1.2.0
+- Refactored `objects.h` to do runtime validation of insertion types rather than
+  limiting via the C++ type system to reduce code duplication.
+- Added `Container::insert_before` and `Container::insert_after`.
+
```

### Comparing `jotdown-2.0.1/README.md` & `jotdown-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/demo/jd-query.cpp` & `jotdown-2.0.2/include/jotdown/api.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,73 +1,52 @@
 /*
- * parse.cpp
+ * api.h
  *
  * Author: Lain Musgrove (lain.proliant@gmail.com)
- * Date: Wednesday May 27, 2020
+ * Date: Thursday June 11, 2020
  *
  * Distributed under terms of the MIT license.
  */
 
-#include <iostream>
+#ifndef __JOTDOWN_API_H
+#define __JOTDOWN_API_H
+
+#include "jotdown/object.h"
 #include "jotdown/parser.h"
 #include "jotdown/compiler.h"
-#include "jotdown/object.h"
 #include "jotdown/query.h"
-#include "jotdown/utils.h"
-#include "moonlight/core.h"
-#include "moonlight/cli.h"
-
-void query_repl(std::shared_ptr<jotdown::object::Document> doc) {
-    for (;;) {
-        std::string str;
-        std::cout << "jdq> ";
-        std::cout.flush();
-        std::cin >> str;
-
-        if (str == "exit" || str == "quit") {
-            break;
-        }
-
-        auto tokens = jotdown::query::tokenize(str);
-        std::cout << moonlight::str::join(moonlight::collect::map<std::string>(tokens, [](auto token) -> std::string { return tfm::format("\"%s\"", jotdown::strliteral(token)); }), ",") << std::endl;
-        jotdown::query::Query query;
-        try {
-            query = jotdown::query::parse(str);
-        } catch (const std::exception& e) {
-            std::cout << "ERROR: " << e.what() << std::endl;
-            continue;
-        }
-        std::cout << query.repr() << std::endl;
-        auto results = query.select({doc});
-        for (auto result : results) {
-            std::cout << result->repr() << std::endl;
-        }
-    }
-}
-
-std::shared_ptr<jotdown::object::Document> load(std::istream& input, const std::string& name = "<input>") {
-    jotdown::parser::Parser parser(input, name);
-    jotdown::compiler::Compiler compiler;
+
+namespace jotdown {
+
+inline std::shared_ptr<Document> load(std::istream& infile, const std::string& filename = "<in>") {
+    parser::Parser parser(infile, filename);
+    Compiler compiler;
     return compiler.compile(parser.begin(), parser.end());
 }
 
-int main(int argc, char** argv) {
-    try {
-        auto cmd = moonlight::cli::parse(argc, argv);
-        std::shared_ptr<jotdown::object::Document> doc;
-
-        if (cmd.args().size() != 1) {
-            throw moonlight::core::Exception("Missing required argument.");
-
-        } else {
-            auto infile = moonlight::file::open_r(cmd.args()[0]);
-            doc = load(infile);
-        }
-
-        query_repl(doc);
-
-    } catch(const std::exception& e) {
-        std::cout << "ERROR: " << e.what() << std::endl;
-    }
+inline std::shared_ptr<Document> load(const std::string& filename) {
+    auto infile = moonlight::file::open_r(filename);
+    return load(infile, filename);
+}
+
+inline void save(std::shared_ptr<const Document> doc, const std::string& filename) {
+    auto outfile = moonlight::file::open_w(filename);
+    outfile << doc->to_jotdown();
+}
 
-    return 0;
+inline q::Query query(const std::string& query_str) {
+    return q::parse(query_str);
 }
+
+inline std::vector<obj_t> query(const std::vector<obj_t>& objects,
+                                const std::string& query_str) {
+    return q::parse(query_str).select(objects);
+}
+
+inline std::vector<obj_t> query(obj_t obj,
+                                const std::string& query_str) {
+    return query(std::vector<obj_t>{obj}, query_str);
+}
+
+}
+
+#endif /* !__JOTDOWN_API_H */
```

### Comparing `jotdown-2.0.1/include/jotdown/compiler.h` & `jotdown-2.0.2/include/jotdown/compiler.h`

 * *Files 4% similar despite different names*

```diff
@@ -14,25 +14,23 @@
 #include "jotdown/parser.h"
 #include "jotdown/interfaces.h"
 #include "jotdown/object.h"
 #include "tinyformat/tinyformat.h"
 #include "moonlight/json.h"
 
 namespace jotdown {
-namespace compiler {
 
-using namespace object;
 using jotdown::parser::Token;
 using jotdown::parser::token_t;
 
 //-------------------------------------------------------------------
 class CompilerError : public JotdownError {
 public:
-    CompilerError(const std::string& message, const Location& location)
-    : JotdownError(format_message(message, location)),
+    CompilerError(const std::string& message, const Location& location, const moonlight::debug::Source& where = {})
+    : JotdownError(format_message(message, location), where, moonlight::type_name<CompilerError>()),
     _location(location) { }
 
     const Location& location() const {
         return _location;
     }
 
 private:
@@ -105,20 +103,22 @@
     std::shared_ptr<Document> doc;
     BufferedTokens tokens;
 };
 
 //-------------------------------------------------------------------
 class CompileState : public moonlight::automata::State<Context> {
 protected:
-    CompilerError unexpected_token(token_t tk, const std::string& doing) {
+    CompilerError unexpected_token(token_t tk, const std::string& doing,
+                                   const moonlight::debug::Source& where = {}) {
         return CompilerError(
             tfm::format("Unexpected '%s' token: %s.",
                         tk->type_name(tk->type()),
                         doing),
-            tk->begin());
+            tk->begin(),
+            where);
     }
 };
 
 //-------------------------------------------------------------------
 class CompileTextContent : public CompileState {
 public:
     CompileTextContent(std::shared_ptr<TextContent> text_content,
@@ -135,41 +135,41 @@
         if (_text_content->range().begin == NOWHERE) {
             _text_content->range().begin = tk->begin();
         }
 
         switch (tk->type()) {
         case Token::Type::TEXT:
             context().tokens.advance();
-            _text_content->add(std::make_shared<Text>(tk->content()))->range(tk->range());
+            _text_content->add(Text::create(tk->content()))->range(tk->range());
             break;
         case Token::Type::HASHTAG:
             context().tokens.advance();
-            _text_content->add(std::make_shared<Hashtag>(tk->content()))->range(tk->range());
+            _text_content->add(Hashtag::create(tk->content()))->range(tk->range());
             break;
         case Token::Type::CODE:
             context().tokens.advance();
-            _text_content->add(std::make_shared<Code>(tk->content()))->range(tk->range());
+            _text_content->add(Code::create(tk->content()))->range(tk->range());
             break;
         case Token::Type::ANCHOR:
             context().tokens.advance();
-            _text_content->add(std::make_shared<Anchor>(tk->content()))->range(tk->range());
+            _text_content->add(Anchor::create(tk->content()))->range(tk->range());
             break;
         case Token::Type::REF:
             context().tokens.advance();
             ingest_ref_token(tk);
             break;
         case Token::Type::INDEX:
             context().tokens.advance();
             ingest_index_token(tk);
             break;
 
         default:
             if (tk->type() != _terminal_type && _terminal_type != Token::Type::NONE) {
                 throw unexpected_token(
-                    tk, "expecting " + tk->type_name(_terminal_type));
+                    tk, "expecting " + tk->type_name(_terminal_type), LOCATION);
 
             } else if (tk->type() == _terminal_type) {
                 context().tokens.advance();
                 _text_content->range().end = tk->end();
 
             } else {
                 _text_content->range().end = tk->begin();
@@ -183,29 +183,29 @@
     void ingest_ref_token(token_t tk) {
         obj_t obj;
         std::shared_ptr<parser::RefToken> ref_tk = (
             dynamic_pointer_cast<parser::RefToken>(tk));
 
         if (! ref_tk->index_name().empty()) {
             obj = _text_content->add(
-                std::make_shared<IndexedRef>(ref_tk->text(), ref_tk->index_name()));
+                IndexedRef::create(ref_tk->text(), ref_tk->index_name()));
 
         } else {
             obj = _text_content->add(
-                std::make_shared<Ref>(ref_tk->link(), ref_tk->text()));
+                Ref::create(ref_tk->link(), ref_tk->text()));
         }
 
         obj->range(tk->range());
     }
 
     void ingest_index_token(token_t tk) {
         std::shared_ptr<parser::IndexToken> index_tk = (
             dynamic_pointer_cast<parser::IndexToken>(tk));
         auto obj = _text_content->add(
-            std::make_shared<RefIndex>(index_tk->name(), index_tk->link()));
+            RefIndex::create(index_tk->name(), index_tk->link()));
         obj->range(tk->range());
     }
 
     std::shared_ptr<TextContent> _text_content;
     Token::Type _terminal_type;
 };
 
@@ -241,21 +241,21 @@
     }
 
 protected:
     virtual void _process_list_item(std::shared_ptr<parser::ListItemToken> tk) = 0;
 
     void _process_sub_list(std::shared_ptr<parser::ListItemToken> tk) {
         if (tk->type() == Token::Type::OL_ITEM) {
-            auto new_list = std::make_shared<OrderedList>();
+            auto new_list = OrderedList::create();
             last_item->add(new_list);
             new_list->range().begin = tk->begin();
             push<CompileOrderedList>(new_list, level + 1);
 
         } else if (tk->type() == Token::Type::UL_ITEM) {
-            auto new_list = std::make_shared<UnorderedList>();
+            auto new_list = UnorderedList::create();
             new_list->range().begin = tk->begin();
             last_item->add(new_list);
             push<CompileUnorderedList>(new_list, level + 1);
         }
     }
 
     std::shared_ptr<List> list;
@@ -272,15 +272,15 @@
 
     const char* tracer_name() const {
         return "OrderedList";
     }
 
     void _process_list_item(std::shared_ptr<parser::ListItemToken> li_tk) {
         if (li_tk->type() != Token::Type::OL_ITEM) {
-            throw unexpected_token(li_tk, "compiling ordered list at the same level");
+            throw unexpected_token(li_tk, "compiling ordered list at the same level", LOCATION);
         }
         std::shared_ptr<parser::OrderedListItemToken> oli_tk = (
             std::dynamic_pointer_cast<parser::OrderedListItemToken>(li_tk));
 
         auto oli = OrderedListItem::create(oli_tk->ordinal());
         oli->level(level);
         oli->range(oli_tk->range());
@@ -305,15 +305,15 @@
 
     const char* tracer_name() const {
         return "UnorderedList";
     }
 
     void _process_list_item(std::shared_ptr<parser::ListItemToken> li_tk) {
         if (li_tk->type() != Token::Type::UL_ITEM) {
-            throw unexpected_token(li_tk, "compiling unordered list at the same level");
+            throw unexpected_token(li_tk, "compiling unordered list at the same level", LOCATION);
         }
         auto uli = UnorderedListItem::create();
         uli->level(level);
         uli->range(li_tk->range());
         _list->add(uli);
         last_item = uli;
         last_token = li_tk;
@@ -336,25 +336,25 @@
         return "TopLevelList";
     }
 
     void run() {
         auto tk = context().tokens.peek();
 
         if (tk->type() == Token::Type::OL_ITEM) {
-            auto ordered_list = _parent->add(std::make_shared<OrderedList>());
+            auto ordered_list = _parent->add(OrderedList::create());
             ordered_list->range().begin = tk->begin();
             transition<CompileOrderedList>(ordered_list);
 
         } else if (tk->type() == Token::Type::UL_ITEM) {
-            auto unordered_list = _parent->add(std::make_shared<UnorderedList>());
+            auto unordered_list = _parent->add(UnorderedList::create());
             unordered_list->range().begin = tk->begin();
             transition<CompileUnorderedList>(unordered_list);
 
         } else {
-            throw unexpected_token(tk, "parsing top-level list");
+            throw unexpected_token(tk, "parsing top-level list", LOCATION);
         }
     }
 
 private:
     std::shared_ptr<Section> _parent;
 };
 
@@ -364,22 +364,22 @@
     const char* tracer_name() const {
         return "CompileFrontMatter";
     }
 
     void run() {
         auto tk = context().tokens.get();
         if (tk == nullptr || tk->type() != Token::Type::FRONT_MATTER) {
-            throw unexpected_token(tk, "compiling front matter, expected FRONT_MATTER");
+            throw unexpected_token(tk, "compiling front matter, expected FRONT_MATTER", LOCATION);
         }
 
         std::shared_ptr<parser::EmbeddedDocumentToken> front_matter_tk = (
             std::dynamic_pointer_cast<parser::EmbeddedDocumentToken>(tk)
         );
 
-        auto obj = std::make_shared<FrontMatter>(front_matter_tk->content(), front_matter_tk->langspec());
+        auto obj = FrontMatter::create(front_matter_tk->content(), front_matter_tk->langspec());
         context().doc->front_matter(obj);
         pop();
     }
 };
 
 //-------------------------------------------------------------------
 class CompileCodeBlock : public CompileState {
@@ -389,22 +389,22 @@
     const char* tracer_name() const {
         return "CodeBlock";
     }
 
     void run() {
         auto tk = context().tokens.get();
         if (tk == nullptr || tk->type() != Token::Type::CODE_BLOCK) {
-            throw unexpected_token(tk, "compiling code block, expected CODE_BLOCK");
+            throw unexpected_token(tk, "compiling code block, expected CODE_BLOCK", LOCATION);
         }
         std::shared_ptr<parser::EmbeddedDocumentToken> code_tk = (
             std::dynamic_pointer_cast<parser::EmbeddedDocumentToken>(tk)
         );
 
         auto obj = _section->add(
-            std::make_shared<CodeBlock>(code_tk->content(), code_tk->langspec()));
+            CodeBlock::create(code_tk->content(), code_tk->langspec()));
         obj->range(tk->range());
         pop();
     }
 
 private:
     std::shared_ptr<Section> _section;
 };
@@ -450,36 +450,36 @@
         case Token::Type::OL_ITEM:
         case Token::Type::UL_ITEM:
             push<CompileTopLevelList>(_section);
             break;
 
         case Token::Type::NEWLINE:
             context().tokens.advance();
-            _section->add(std::make_shared<LineBreak>())->range(tk->range());
+            _section->add(LineBreak::create())->range(tk->range());
             break;
 
         case Token::Type::END:
             _section->range().end = tk->end();
             pop();
             break;
 
         default:
-            throw unexpected_token(tk, "parsing section");
+            throw unexpected_token(tk, "parsing section", LOCATION);
         }
     }
 
 private:
     bool is_subsection(token_t tk) {
         std::shared_ptr<parser::HeaderStartToken> header_tk = (
             dynamic_pointer_cast<parser::HeaderStartToken>(tk));
         return header_tk->level() > _section->level();
     }
 
     void init_text_content() {
-        auto text_content = _section->add(std::make_shared<TextContent>());
+        auto text_content = _section->add(TextContent::create());
         push<CompileTextContent>(text_content);
     }
 
     std::shared_ptr<Section> _section;
 };
 
 //-------------------------------------------------------------------
@@ -587,15 +587,15 @@
 public:
     template<class T>
     std::shared_ptr<Document> compile(T true_begin, T true_end) {
         auto begin = moonlight::gen::wrap(true_begin, true_end);
         auto end = moonlight::gen::end<typename T::value_type>();
 
         Context ctx {
-            .doc = std::make_shared<Document>(),
+            .doc = Document::create(),
             .tokens = BufferedTokens(begin, end)
         };
 
 
         auto machine = CompileState::Machine::init<CompileBegin>(ctx);
 #ifdef MOONLIGHT_AUTOMATA_DEBUG
         machine.add_tracer([](CompileState::Machine::TraceEvent event,
@@ -630,10 +630,9 @@
         machine.run_until_complete();
 
         return ctx.doc;
     }
 };
 
 }
-}
 
 #endif /* !__JOTDOWN_COMPILER_H */
```

### Comparing `jotdown-2.0.1/include/jotdown/interfaces.h` & `jotdown-2.0.2/include/jotdown/interfaces.h`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #define __JOTDOWN_INTERFACES_H
 
 #include <string>
 #include "moonlight/json.h"
 
 namespace jotdown {
 
-using JSON = moonlight::json::Wrapper;
+namespace json = moonlight::json;
 
 // ------------------------------------------------------------------
 struct Location {
     std::string filename;
     int line, col;
 
     static const Location& nowhere() {
@@ -37,38 +37,38 @@
         );
     }
 
     bool operator!=(const Location& other) const {
         return ! operator==(other);
     }
 
-    JSON to_json() const {
-        JSON json;
+    json::Object to_json() const {
+        json::Object json;
         json.set<std::string>("filename", filename);
         json.set<float>("line", line);
         json.set<float>("col", col);
         return json;
     }
 };
 
 const struct Location NOWHERE = {"<none>", -1, -1};
 
 //-------------------------------------------------------------------
 struct Range {
     Location begin;
     Location end;
 
-    JSON to_json() const {
-        JSON json, begin_json, end_json;
+    json::Object to_json() const {
+        json::Object json, begin_json, end_json;
         begin_json.set<float>("line", begin.line);
         begin_json.set<float>("col", begin.col);
         end_json.set<float>("line", end.line);
         end_json.set<float>("col", end.col);
-        json.set_object("begin", begin_json);
-        json.set_object("end", end_json);
+        json.set("begin", begin_json);
+        json.set("end", end_json);
         return json;
     }
 
     bool operator==(const Range& other) const {
         return begin == other.begin && end == other.end;
     }
 };
```

### Comparing `jotdown-2.0.1/include/jotdown/object.h` & `jotdown-2.0.2/include/jotdown/object.h`

 * *Files 5% similar despite different names*

```diff
@@ -14,42 +14,46 @@
 #include "jotdown/interfaces.h"
 #include "tinyformat/tinyformat.h"
 #include "moonlight/json.h"
 
 #include <memory>
 
 namespace jotdown {
-namespace object {
+
+class Object;
+class Container;
+class TextContent;
+
+typedef std::shared_ptr<Object> obj_t;
+typedef std::shared_ptr<const Object> cobj_t;
+typedef std::shared_ptr<Container> container_t;
+typedef std::shared_ptr<const Container> ccontainer_t;
+typedef std::shared_ptr<TextContent> text_t;
+typedef std::shared_ptr<const TextContent> ctext_t;
+
+typedef std::shared_ptr<Object> obj_t;
+typedef std::shared_ptr<const Object> cobj_t;
+typedef std::shared_ptr<Container> container_t;
+typedef std::shared_ptr<const Container> ccontainer_t;
+typedef std::shared_ptr<TextContent> text_t;
+typedef std::shared_ptr<const TextContent> ctext_t;
 
 using jotdown::NOWHERE;
 
-typedef moonlight::json::Wrapper JSON;
+namespace json = moonlight::json;
 
 //-------------------------------------------------------------------
 struct Config {
     int list_indent;
 };
 
 //-------------------------------------------------------------------
-class ObjectError : public moonlight::core::Exception {
-public:
-    using Exception::Exception;
-};
+EXCEPTION_TYPE(ObjectError)
 
 //-------------------------------------------------------------------
-class Object;
-class Container;
-class TextContent;
-typedef std::shared_ptr<Object> obj_t;
-typedef std::shared_ptr<const Object> cobj_t;
-typedef std::shared_ptr<Container> container_t;
-typedef std::shared_ptr<const Container> ccontainer_t;
-typedef std::shared_ptr<TextContent> text_t;
-typedef std::shared_ptr<const TextContent> ctext_t;
-
 class Object : public std::enable_shared_from_this<Object> {
 public:
     enum class Type {
         NONE,
         ANCHOR,
         CODE,
         CODE_BLOCK,
@@ -149,19 +153,19 @@
     static Config& config() {
         static Config config {
             .list_indent = 2
         };
         return config;
     }
 
-    virtual JSON to_json() const {
-        JSON json;
+    virtual json::Object to_json() const {
+        json::Object json;
         json.set<std::string>("type", type_name(type()));
         if (range().begin != NOWHERE && range().end != NOWHERE) {
-            json.set_object("range", range().to_json());
+            json.set("range", range().to_json());
         }
         return json;
     }
 
     virtual obj_t clone() const = 0;
     virtual std::string to_jotdown() const = 0;
     virtual std::string to_search_string() const = 0;
@@ -206,26 +210,26 @@
     }
 
     template<class T>
     std::shared_ptr<T> insert_before(cobj_t pivot, std::shared_ptr<T> obj) {
         _check_can_contain(obj);
         auto iter = std::find(_contents.begin(), _contents.end(), pivot);
         if (iter == _contents.end()) {
-            throw ObjectError("Pivot object does not exist in container.");
+            THROW(ObjectError, "Pivot object does not exist in container.");
         }
         _contents.insert(iter, obj);
         return obj;
     }
 
     template<class T>
     std::shared_ptr<T> insert_after(cobj_t pivot, std::shared_ptr<T> obj) {
         _check_can_contain(obj);
         auto iter = std::find(_contents.begin(), _contents.end(), pivot);
         if (iter == _contents.end()) {
-            throw ObjectError("Pivot object does not exist in container.");
+            THROW(ObjectError, "Pivot object does not exist in container.");
         }
         _contents.insert(std::next(iter), obj);
         return obj;
     }
 
     iterator begin() {
         return _contents.begin();
@@ -246,37 +250,49 @@
     const std::vector<obj_t>& contents() const {
         return _contents;
     }
 
     void shift_up(cobj_t obj) {
         auto iter = std::find(_contents.begin(), _contents.end(), obj);
         if (iter == _contents.end()) {
-            throw ObjectError("Object does not exist in this container.");
+            THROW(ObjectError, "Object does not exist in this container.");
         }
         if (iter == _contents.begin()) {
-            throw ObjectError("Object is already the first in the container.");
+            THROW(ObjectError, "Object is already the first in the container.");
         }
         std::iter_swap(std::prev(iter), iter);
     }
 
+    void shift_first(cobj_t obj) {
+        try {
+            for (;;) shift_up(obj);
+        } catch (...) { }
+    }
+
     void shift_down(cobj_t obj) {
         auto iter = std::find(_contents.begin(), _contents.end(), obj);
         if (iter == _contents.end()) {
-            throw ObjectError("Object does not exist in this container.");
+            THROW(ObjectError, "Object does not exist in this container.");
         }
         if (std::next(iter) == _contents.end()) {
-            throw ObjectError("Object is already the last in the container.");
+            THROW(ObjectError, "Object is already the last in the container.");
         }
         std::iter_swap(std::next(iter), iter);
     }
 
+    void shift_last(cobj_t obj) {
+        try {
+            for (;;) shift_up(obj);
+        } catch (...) { }
+    }
+
     void remove(obj_t obj) {
         auto iter = std::find(_contents.begin(), _contents.end(), obj);
         if (iter == _contents.end()) {
-            throw ObjectError("Object is not in the container.");
+            THROW(ObjectError, "Object is not in the container.");
         }
         _contents.erase(iter);
         if ((*iter)->has_parent() && (*iter)->parent() == shared_from_this()) {
             (*iter)->parent(nullptr);
         }
     }
 
@@ -285,21 +301,21 @@
             if (obj->has_parent() && obj->parent() == shared_from_this()) {
                 obj->parent(nullptr);
             }
         }
         _contents.clear();
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
-        std::vector<JSON> json_contents;
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
+        std::vector<json::Object> json_contents;
         for (auto& obj : contents()) {
             json_contents.push_back(obj->to_json());
         }
-        json.set_object_array("contents", json_contents);
+        json.set("contents", json::Array(json_contents));
         return json;
     }
 
     std::string to_search_string() const {
         std::ostringstream sb;
         for (auto obj : contents()) {
             sb << obj->to_search_string();
@@ -323,38 +339,42 @@
         for (auto& obj : other->contents()) {
             add(obj->clone());
         }
     }
 
     void _check_can_contain(cobj_t obj) const {
         if (! can_contain(obj)) {
-            throw ObjectError(tfm::format("%s cannot contain %s.",
+            THROW(ObjectError, tfm::format("%s cannot contain %s.",
                                           type_name(type()),
                                           obj->type_name(obj->type())));
         }
     }
 };
 
 //-------------------------------------------------------------------
 class Anchor : public Object {
 public:
     Anchor(const std::string& name) : Object(Type::ANCHOR), _name(name) { }
 
+    static std::shared_ptr<Anchor> create(const std::string& name) {
+        return std::make_shared<Anchor>(name);
+    }
+
     const std::string& name() const {
         return _name;
     }
 
     obj_t clone() const {
-        auto obj = std::make_shared<Anchor>(name());
+        auto obj = create(name());
         obj->range(range());
         return obj;
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
         json.set<std::string>("name", name());
         return json;
     }
 
     std::string to_jotdown() const {
         return tfm::format("&%s", name());
     }
@@ -372,26 +392,30 @@
 };
 
 //-------------------------------------------------------------------
 class Text : public Object {
 public:
     Text(const std::string& text = "") : Object(Type::TEXT), _text(text) { }
 
+    static std::shared_ptr<Text> create(const std::string& text) {
+        return std::make_shared<Text>(text);
+    }
+
     const std::string& text() const {
         return _text;
     }
 
     obj_t clone() const {
-        auto obj = std::make_shared<Text>(text());
+        auto obj = create(text());
         obj->range(range());
         return obj;
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
         json.set<std::string>("text", text());
         return json;
     }
 
     std::string to_jotdown() const {
         return _text;
     }
@@ -409,26 +433,30 @@
 };
 
 //-------------------------------------------------------------------
 class Hashtag : public Object {
 public:
     Hashtag(const std::string& tag) : Object(Type::HASHTAG), _tag(tag) { }
 
+    static std::shared_ptr<Hashtag> create(const std::string& tag) {
+        return std::make_shared<Hashtag>(tag);
+    }
+
     const std::string& tag() const {
         return _tag;
     }
 
     obj_t clone() const {
-        auto obj = std::make_shared<Hashtag>(tag());
+        auto obj = create(tag());
         obj->range(range());
         return obj;
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
         json.set<std::string>("tag", tag());
         return json;
     }
 
     std::string to_jotdown() const {
         return tfm::format("#%s", tag());
     }
@@ -446,16 +474,20 @@
 };
 
 //-------------------------------------------------------------------
 class LineBreak : public Object {
 public:
     LineBreak() : Object(Type::LINE_BREAK) { }
 
+    static std::shared_ptr<LineBreak> create() {
+        return std::make_shared<LineBreak>();
+    }
+
     obj_t clone() const {
-        auto obj = std::make_shared<LineBreak>();
+        auto obj = create();
         obj->range(range());
         return obj;
     }
 
     std::string to_jotdown() const {
         return "\n";
     }
@@ -466,26 +498,30 @@
 };
 
 //-------------------------------------------------------------------
 class Code : public Object {
 public:
     Code(const std::string& code) : Object(Type::CODE), _code(code) { }
 
+    static std::shared_ptr<Code> create(const std::string& code) {
+        return std::make_shared<Code>(code);
+    }
+
     const std::string& code() const {
         return _code;
     }
 
     obj_t clone() const {
-        auto obj = std::make_shared<Code>(code());
+        auto obj = create(code());
         obj->range(range());
         return obj;
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
         json.set<std::string>("code", code());
         return json;
     }
 
     std::string to_jotdown() const {
         return tfm::format("`%s`",
                            strescape(code(), "`"));
@@ -506,30 +542,34 @@
 
 //-------------------------------------------------------------------
 class Ref : public Object {
 public:
     Ref(const std::string& link, const std::string& text = "")
     : Object(Type::REF), _link(link), _text(text) { }
 
+    static std::shared_ptr<Ref> create(const std::string& link, const std::string& text = "") {
+        return std::make_shared<Ref>(link, text);
+    }
+
     const std::string& link() const {
         return _link;
     }
 
     const std::string& text() const {
         return _text;
     }
 
     obj_t clone() const {
-        auto obj = std::make_shared<Ref>(link(), text());
+        auto obj = create(link(), text());
         obj->range(range());
         return obj;
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
         json.set<std::string>("link", link());
         if (text() != link()) {
             json.set<std::string>("text", text());
         }
         return json;
     }
 
@@ -563,14 +603,18 @@
 };
 
 //-------------------------------------------------------------------
 class IndexedRef : public Object {
 public:
     IndexedRef(const std::string& text, const std::string& index_name) : Object(Type::REF), _text(text), _index_name(index_name) { }
 
+    static std::shared_ptr<IndexedRef> create(const std::string& text, const std::string& index_name) {
+        return std::make_shared<IndexedRef>(text, index_name);
+    }
+
     void link(const std::string& link) {
         _link = link;
     }
 
     const std::string& link() const {
         return _link;
     }
@@ -579,23 +623,23 @@
         return _text;
     }
 
     const std::string& index_name() const {
         return _index_name;
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
         json.set<std::string>("text", text());
         json.set<std::string>("index_name", index_name());
         return json;
     }
 
     obj_t clone() const {
-        auto obj = std::make_shared<IndexedRef>(text(), index_name());
+        auto obj = create(text(), index_name());
         obj->link(link());
         obj->range(range());
         return obj;
     }
 
     std::string to_jotdown() const {
         return tfm::format("[%s][%s]",
@@ -618,30 +662,34 @@
 };
 
 //-------------------------------------------------------------------
 class RefIndex : public Object {
 public:
     RefIndex(const std::string& name, const std::string& link) : Object(Type::REF_INDEX), _name(name), _link(link) { }
 
+    static std::shared_ptr<RefIndex> create(const std::string& name, const std::string& link) {
+        return std::make_shared<RefIndex>(name, link);
+    }
+
     const std::string& name() const {
         return _name;
     }
 
     const std::string& link() const {
         return _link;
     }
 
     obj_t clone() const {
-        auto obj = std::make_shared<RefIndex>(name(), link());
+        auto obj = create(name(), link());
         obj->range(range());
         return obj;
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
         json.set<std::string>("name", name());
         json.set<std::string>("link", link());
         return json;
     }
 
     std::string to_jotdown() const {
         return tfm::format("[%s]: %s",
@@ -666,28 +714,32 @@
 class TextContent : public Container {
 public:
     friend class Section;
     friend class OrderedListItem;
     friend class UnorderedListItem;
     TextContent() : Container(Type::TEXT_CONTENT) { }
 
+    static std::shared_ptr<TextContent> create() {
+        return std::make_shared<TextContent>();
+    }
+
     bool can_contain(cobj_t obj) const {
         static const std::vector<Type> cont = {
             Type::ANCHOR,
             Type::CODE,
             Type::HASHTAG,
             Type::REF,
             Type::REF_INDEX,
             Type::TEXT
         };
         return std::find(cont.begin(), cont.end(), obj->type()) != cont.end();
     }
 
     obj_t clone() const {
-        auto textblock = std::make_shared<TextContent>();
+        auto textblock = create();
         textblock->_copy_from(std::static_pointer_cast<const Container>(shared_from_this()));
         textblock->range(range());
         return textblock;
     }
 
     std::string to_jotdown() const {
         std::ostringstream sb;
@@ -785,17 +837,17 @@
         return _status;
     }
 
     void status(const std::string& status) {
         _status = status;
     }
 
-    virtual JSON to_json() const {
-        JSON json = Container::to_json();
-        json.set_object("text", ctext()->to_json());
+    virtual json::Object to_json() const {
+        json::Object json = Container::to_json();
+        json.set("text", ctext()->to_json());
         if (status().size() > 0) {
             json.set<std::string>("status", status());
         }
         return json;
     }
 
     std::string to_jotdown() const {
@@ -901,16 +953,16 @@
         oli->_copy_from(std::static_pointer_cast<const ListItem>(shared_from_this()));
         oli->range(range());
         oli->text()->_copy_from(std::static_pointer_cast<const Container>(ctext()));
         oli->text()->range(ctext()->range());
         return oli;
     }
 
-    JSON to_json() const {
-        JSON json = ListItem::to_json();
+    json::Object to_json() const {
+        json::Object json = ListItem::to_json();
         json.set<std::string>("ordinal", ordinal());
         return json;
     }
 
 private:
     OrderedListItem(const std::string& ordinal)
     : ListItem(Type::ORDERED_LIST_ITEM), _ordinal(ordinal) { }
@@ -945,37 +997,45 @@
 };
 
 //-------------------------------------------------------------------
 class OrderedList : public List {
 public:
     OrderedList() : List(Type::ORDERED_LIST) { }
 
+    static std::shared_ptr<OrderedList> create() {
+        return std::make_shared<OrderedList>();
+    }
+
     bool can_contain(cobj_t obj) const {
         return obj->type() == Type::ORDERED_LIST_ITEM;
     }
 
     obj_t clone() const {
-        auto ol = std::make_shared<OrderedList>();
+        auto ol = create();
         ol->_copy_from(std::static_pointer_cast<const List>(shared_from_this()));
         ol->range(range());
         return ol;
     }
 };
 
 //-------------------------------------------------------------------
 class UnorderedList : public List {
 public:
     UnorderedList() : List(Type::UNORDERED_LIST) { }
 
+    static std::shared_ptr<UnorderedList> create() {
+        return std::make_shared<UnorderedList>();
+    }
+
     bool can_contain(cobj_t obj) const {
         return obj->type() == Type::UNORDERED_LIST_ITEM;
     }
 
     obj_t clone() const {
-        auto ul = std::make_shared<UnorderedList>();
+        auto ul = create();
         ul->_copy_from(std::static_pointer_cast<const List>(shared_from_this()));
         ul->range(range());
         return ul;
     }
 };
 
 //-------------------------------------------------------------------
@@ -988,16 +1048,16 @@
         return _code;
     }
 
     const std::string& language() const {
         return _language;
     }
 
-    JSON to_json() const {
-        JSON json = Object::to_json();
+    json::Object to_json() const {
+        json::Object json = Object::to_json();
         json.set<std::string>("code", code());
         if (_language.size() != 0) {
             json.set<std::string>("language", language());
         }
         return json;
     }
 
@@ -1036,19 +1096,23 @@
     std::string _code;
     std::string _language;
 };
 
 //-------------------------------------------------------------------
 class CodeBlock : public EmbeddedDocument {
 public:
-    CodeBlock(const std::string& code, const std::string& language)
+    CodeBlock(const std::string& code, const std::string& language = "")
     : EmbeddedDocument(Type::CODE_BLOCK, code, language) { }
 
+    static std::shared_ptr<CodeBlock> create(const std::string& code, const std::string& language = "") {
+        return std::make_shared<CodeBlock>(code, language);
+    }
+
     obj_t clone() const {
-        auto obj = std::make_shared<CodeBlock>(code(), language());
+        auto obj = create(code(), language());
         obj->range(range());
         return obj;
     }
 
     const std::string& delimiter() const {
         static const std::string delim = "```";
         return delim;
@@ -1058,19 +1122,23 @@
     std::string _code;
     std::string _language;
 };
 
 //-------------------------------------------------------------------
 class FrontMatter : public EmbeddedDocument {
 public:
-    FrontMatter(const std::string& code, const std::string& language)
+    FrontMatter(const std::string& code, const std::string& language = "")
     : EmbeddedDocument(Type::FRONT_MATTER, code, language) { }
 
+    static std::shared_ptr<FrontMatter> create(const std::string& code, const std::string& language = "") {
+        return std::make_shared<FrontMatter>(code, language);
+    }
+
     obj_t clone() const {
-        auto obj = std::make_shared<FrontMatter>(code(), language());
+        auto obj = create(code(), language());
         obj->range(range());
         return obj;
     }
 
     const std::string& delimiter() const {
         static const std::string delim = "---";
         return delim;
@@ -1123,26 +1191,26 @@
             Type::TEXT_CONTENT,
             Type::UNORDERED_LIST
         };
         return std::find(cont.begin(), cont.end(), obj->type()) != cont.end();
     }
 
     obj_t clone() const {
-        auto section = Section::create(level());
+        auto section = create(level());
         section->_copy_from(std::static_pointer_cast<const Section>(shared_from_this()));
         section->range(range());
         section->header()->_copy_from(std::static_pointer_cast<const Container>(cheader()));
         section->header()->range(cheader()->range());
         return section;
     }
 
-    JSON to_json() const {
-        JSON json = Container::to_json();
+    json::Object to_json() const {
+        json::Object json = Container::to_json();
         json.set<double>("level", level());
-        json.set_object("header", cheader()->to_json());
+        json.set("header", cheader()->to_json());
         return json;
     }
 
     std::string to_jotdown() const {
         std::stringstream sb;
         sb << std::string(level(), '#') << " ";
         sb << cheader()->to_jotdown();
@@ -1169,28 +1237,32 @@
 };
 
 //-------------------------------------------------------------------
 class Document : public Container {
 public:
     Document() : Container(Type::DOCUMENT) { }
 
+    static std::shared_ptr<Document> create() {
+        return std::make_shared<Document>();
+    }
+
     bool can_contain(cobj_t obj) const {
         return obj->type() == Type::SECTION;
     }
 
     std::shared_ptr<FrontMatter> front_matter() const {
         return _front_matter;
     }
 
     void front_matter(std::shared_ptr<FrontMatter> front_matter) {
         _front_matter = front_matter;
     }
 
     obj_t clone() const {
-        auto doc = std::make_shared<Document>();
+        auto doc = create();
         if (front_matter() != nullptr) {
             doc->front_matter(std::static_pointer_cast<FrontMatter>(front_matter()->clone()));
         }
         doc->_copy_from(std::static_pointer_cast<const Container>(shared_from_this()));
         doc->range(range());
         return doc;
     }
@@ -1207,10 +1279,9 @@
     }
 
 private:
     std::shared_ptr<FrontMatter> _front_matter;
 };
 
 }
-}
 
 #endif /* !__JOTDOWN_OBJECT_H */
```

### Comparing `jotdown-2.0.1/include/jotdown/parser.h` & `jotdown-2.0.2/include/jotdown/parser.h`

 * *Files 0% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 
 namespace jotdown {
 namespace parser {
 
 // ------------------------------------------------------------------
 class ParserError : public JotdownError {
 public:
-    ParserError(const std::string& message, const Location& location)
-    : JotdownError(format_message(message, location)),
+    ParserError(const std::string& message, const Location& location, const moonlight::debug::Source& where = {})
+    : JotdownError(format_message(message, location), where, moonlight::type_name<ParserError>()),
     _location(location) { }
 
     const Location& location() const {
         return _location;
     }
 
 private:
```

### Comparing `jotdown-2.0.1/include/jotdown/query.h` & `jotdown-2.0.2/include/jotdown/query.h`

 * *Files 10% similar despite different names*

```diff
@@ -7,35 +7,30 @@
  * Distributed under terms of the MIT license.
  */
 
 #ifndef __JOTDOWN_QUERY_H
 #define __JOTDOWN_QUERY_H
 
 #include "moonlight/slice.h"
+#include "moonlight/classify.h"
 #include "jotdown/error.h"
 #include "jotdown/interfaces.h"
 #include "jotdown/object.h"
 #include "jotdown/utils.h"
 #include "tinyformat/tinyformat.h"
 
 #include <regex>
 #include <vector>
 #include <set>
 
 namespace jotdown {
-namespace query {
 
-using Object = object::Object;
-using ObjectType = object::Object::Type;
-using obj_t = object::obj_t;
+EXCEPTION_TYPE(QueryError);
 
-// ------------------------------------------------------------------
-class QueryError : public moonlight::core::Exception {
-    using Exception::Exception;
-};
+namespace q {
 
 // ------------------------------------------------------------------
 class Selector {
 public:
     virtual ~Selector() { }
 
     virtual Selector* clone() const  = 0;
@@ -89,14 +84,18 @@
                 break;
             }
             results = query->select(results);
         }
         return results;
     }
 
+    std::vector<obj_t> select(obj_t object) const {
+        return select(std::vector<obj_t>{object});
+    }
+
     std::string repr() const {
         std::vector<std::string> seq_reprs;
         for (auto& query : sequence) {
             seq_reprs.push_back(query->repr());
         }
         return tfm::format("Query(%d)<%s>", sequence.size(), moonlight::str::join(seq_reprs, " "));
     }
@@ -108,42 +107,42 @@
         return q;
     }
 
     std::vector<std::unique_ptr<const Selector>> sequence;
 };
 
 // ------------------------------------------------------------------
-class Type : public Selector {
+class TypeSelect : public Selector {
 public:
-    Type(ObjectType type) : type(type) { }
+    TypeSelect(Object::Type type) : type(type) { }
 
     Selector* clone() const {
-        return new Type(type);
+        return new TypeSelect(type);
     }
 
     bool choose(obj_t obj) const {
         return obj->type() == type;
     }
 
     std::string repr() const {
         return tfm::format("Type<\"%s\">", Object::type_name(type));
     }
 
 private:
-    ObjectType type;
+    Object::Type type;
 };
 
 // ------------------------------------------------------------------
-class Slice : public Selector {
+class SliceSelect : public Selector {
 public:
-    Slice(const std::optional<int>& begin, const std::optional<int>& end)
+    SliceSelect(const std::optional<int>& begin, const std::optional<int>& end)
     : begin(begin), end(end) { }
 
     Selector* clone() const {
-        return new Slice(begin, end);
+        return new SliceSelect(begin, end);
     }
 
     std::vector<obj_t> select(const std::vector<obj_t>& objects) const {
         return moonlight::slice(objects, begin, end);
     }
 
     std::string repr() const {
@@ -162,43 +161,43 @@
     }
 
 private:
     std::optional<int> begin, end;
 };
 
 // ------------------------------------------------------------------
-class Offset : public Selector {
+class OffsetSelector : public Selector {
 public:
-    Offset(int offset) : offset(offset) { }
+    OffsetSelector(int offset) : offset(offset) { }
 
     std::vector<obj_t> select(const std::vector<obj_t>& objects) const {
         try {
             return {moonlight::slice(objects, offset)};
 
-        } catch (const moonlight::SliceError& e) {
+        } catch (const moonlight::core::IndexError& e) {
             return {};
         }
     }
 
     Selector* clone() const {
-        return new Offset(offset);
+        return new OffsetSelector(offset);
     }
 
     std::string repr() const {
         return tfm::format("Offset<%d>", offset);
     }
 
 private:
     int offset;
 };
 
 // ------------------------------------------------------------------
-class Label : public Selector {
+class LabelSelector : public Selector {
     Selector* clone() const {
-        return new Label();
+        return new LabelSelector();
     }
 
     std::vector<obj_t> select(const std::vector<obj_t>& objects) const {
         std::vector<obj_t> results;
 
         for (auto obj : objects) {
             if (obj->has_label()) {
@@ -212,17 +211,17 @@
 
     std::string repr() const {
         return "Label";
     }
 };
 
 // ------------------------------------------------------------------
-class Parents : public Selector {
+class ParentSelector : public Selector {
     Selector* clone() const {
-        return new Parents();
+        return new ParentSelector();
     }
 
     std::vector<obj_t> select(const std::vector<obj_t>& objects) const {
         std::vector<obj_t> intermediate_results;
         std::vector<obj_t> final_results;
         std::set<obj_t> final_result_set;
 
@@ -244,32 +243,32 @@
 
     std::string repr() const {
         return "Parents";
     }
 };
 
 // ------------------------------------------------------------------
-class Children : public Selector {
+class ChildrenSelector : public Selector {
 public:
-    Children(bool include_labels = false) : include_labels(include_labels) { }
+    ChildrenSelector(bool include_labels = false) : include_labels(include_labels) { }
 
     Selector* clone() const {
-        return new Children(include_labels);
+        return new ChildrenSelector(include_labels);
     }
 
     std::vector<obj_t> select(const std::vector<obj_t>& objects) const {
         std::vector<obj_t> results;
 
         for (auto obj : objects) {
             if (include_labels && obj->has_label()) {
                 auto sub_results = select({obj->label()});
                 std::copy(sub_results.begin(), sub_results.end(), std::back_inserter(results));
             }
             if (obj->is_container()) {
-                auto container = std::static_pointer_cast<object::Container>(obj);
+                auto container = std::static_pointer_cast<Container>(obj);
                 auto& contents = container->contents();
                 std::copy(contents.begin(), contents.end(), std::back_inserter(results));
             }
         }
 
         return results;
     }
@@ -283,32 +282,32 @@
     }
 
 private:
     bool include_labels;
 };
 
 // ------------------------------------------------------------------
-class Descendants : public Selector {
+class DescendantsSelector : public Selector {
 public:
-    Descendants(bool include_labels = false) : include_labels(include_labels) { }
+    DescendantsSelector(bool include_labels = false) : include_labels(include_labels) { }
 
     Selector* clone() const {
-        return new Descendants(include_labels);
+        return new DescendantsSelector(include_labels);
     }
 
     std::vector<obj_t> select(const std::vector<obj_t>& objects) const {
         std::vector<obj_t> results;
 
         for (auto obj : objects) {
             if (include_labels && obj->has_label()) {
                 auto sub_results = select({obj->label()});
                 std::copy(sub_results.begin(), sub_results.end(), std::back_inserter(results));
             }
             if (obj->is_container()) {
-                auto container = std::static_pointer_cast<object::Container>(obj);
+                auto container = std::static_pointer_cast<Container>(obj);
                 auto& contents = container->contents();
                 std::copy(contents.begin(), contents.end(), std::back_inserter(results));
                 auto sub_results = select(contents);
                 std::copy(sub_results.begin(), sub_results.end(), std::back_inserter(results));
             }
         }
 
@@ -324,18 +323,18 @@
     }
 
 private:
     bool include_labels = false;
 };
 
 // ------------------------------------------------------------------
-class Antecedents : public Selector {
+class AntecedentsSelector : public Selector {
 public:
     Selector* clone() const {
-        return new Antecedents();
+        return new AntecedentsSelector();
     }
 
     std::vector<obj_t> select(const std::vector<obj_t>& objects) const {
         std::vector<obj_t> results;
         std::vector<obj_t> final_results;
         std::set<obj_t> sieve;
         for (auto obj : objects) {
@@ -359,30 +358,30 @@
 
     std::string repr() const {
         return "Antecedents";
     }
 };
 
 // ------------------------------------------------------------------
-class Level : public Selector {
+class LevelSelector : public Selector {
 public:
-    Level(int level) : level(level) { }
+    LevelSelector(int level) : level(level) { }
 
     Selector* clone() const {
-        return new Level(level);
+        return new LevelSelector(level);
     }
 
     bool choose(obj_t obj) const {
-        if (obj->type() == ObjectType::ORDERED_LIST_ITEM ||
-            obj->type() == ObjectType::UNORDERED_LIST_ITEM) {
-            auto list_item = std::static_pointer_cast<object::ListItem>(obj);
+        if (obj->type() == Object::Type::ORDERED_LIST_ITEM ||
+            obj->type() == Object::Type::UNORDERED_LIST_ITEM) {
+            auto list_item = std::static_pointer_cast<ListItem>(obj);
             return list_item->level() == level;
 
-        } else if (obj->type() == ObjectType::SECTION) {
-            auto section = std::static_pointer_cast<object::Section>(obj);
+        } else if (obj->type() == Object::Type::SECTION) {
+            auto section = std::static_pointer_cast<Section>(obj);
             return section->level() == level;
         }
 
         return false;
     }
 
     std::string repr() const {
@@ -390,20 +389,20 @@
     }
 
 private:
     int level;
 };
 
 // ------------------------------------------------------------------
-class Search : public Selector {
+class RegexSelector : public Selector {
 public:
-    Search(const std::string& rx) : str_rx(rx), rx(rx) { }
+    RegexSelector(const std::string& rx) : str_rx(rx), rx(rx) { }
 
     Selector* clone() const {
-        return new Search(str_rx, rx);
+        return new RegexSelector(str_rx, rx);
     }
 
     bool choose(obj_t obj) const {
         if (obj->has_label()) {
             return std::regex_search(obj->label()->to_search_string(), rx);
         } else {
             return std::regex_search(obj->to_search_string(), rx);
@@ -411,119 +410,119 @@
     }
 
     std::string repr() const {
         return tfm::format("Search<\"%s\">", strliteral(str_rx));
     }
 
 private:
-    Search(const std::string& str_rx, const std::regex& rx) : str_rx(str_rx), rx(rx) { }
+    RegexSelector(const std::string& str_rx, const std::regex& rx) : str_rx(str_rx), rx(rx) { }
 
     std::string str_rx;
     std::regex rx;
 };
 
 // ------------------------------------------------------------------
-class Hashtag : public Selector {
+class HashtagSelector : public Selector {
 public:
-    Hashtag(const std::string& tag) : tag(tag) { }
+    HashtagSelector(const std::string& tag) : tag(tag) { }
 
     Selector* clone() const {
-        return new Hashtag(tag);
+        return new HashtagSelector(tag);
     }
 
     bool choose(obj_t obj) const {
-        if (obj->type() == ObjectType::HASHTAG) {
-            auto hashtag = std::static_pointer_cast<object::Hashtag>(obj);
+        if (obj->type() == Object::Type::HASHTAG) {
+            auto hashtag = std::static_pointer_cast<Hashtag>(obj);
             return tag == "" || moonlight::str::to_lower(hashtag->tag()) == moonlight::str::to_lower(tag);
         }
         return false;
     }
 
     std::string repr() const {
-        return tfm::format("Hashtag<\"%s\">", tag);
+        return tfm::format("HashtagSelector<\"%s\">", tag);
     }
 
 private:
     std::string tag;
 };
 
 // ------------------------------------------------------------------
-class List : public Selector {
+class ListSelector : public Selector {
 public:
-    List() : type(ObjectType::NONE) { }
+    ListSelector() : type(Object::Type::NONE) { }
 
     static Query Ordered() {
-        return Query().by(List(ObjectType::ORDERED_LIST));
+        return Query().by(ListSelector(Object::Type::ORDERED_LIST));
     }
 
     static Query Unordered() {
-        return Query().by(List(ObjectType::UNORDERED_LIST));
+        return Query().by(ListSelector(Object::Type::UNORDERED_LIST));
     }
 
     Selector* clone() const {
-        return new List(type);
+        return new ListSelector(type);
     }
 
     bool choose(obj_t obj) const {
-        if (type == ObjectType::NONE) {
-            return obj->type() == ObjectType::ORDERED_LIST || obj->type() == ObjectType::UNORDERED_LIST;
+        if (type == Object::Type::NONE) {
+            return obj->type() == Object::Type::ORDERED_LIST || obj->type() == Object::Type::UNORDERED_LIST;
 
         } else {
             return obj->type() == type;
         }
     }
 
     std::string repr() const {
-        if (type == ObjectType::NONE) {
-            return "List";
+        if (type == Object::Type::NONE) {
+            return "ListSelector";
         } else {
             return Object::type_name(type);
         }
     }
 
 private:
-    List(ObjectType type) : type(type) { }
-    ObjectType type;
+    ListSelector(Object::Type type) : type(type) { }
+    Object::Type type;
 };
 
 // ------------------------------------------------------------------
-class Item : public Selector {
+class ListItemSelector : public Selector {
 public:
-    Item() : type(ObjectType::NONE) { }
+    ListItemSelector() : type(Object::Type::NONE) { }
 
     static Query Ordered(const std::string& ordinal = "") {
-        return Query().by(Item(ObjectType::ORDERED_LIST_ITEM, ordinal));
+        return Query().by(ListItemSelector(Object::Type::ORDERED_LIST_ITEM, ordinal));
     }
 
     static Query Unordered() {
-        return Query().by(Item(ObjectType::UNORDERED_LIST_ITEM));
+        return Query().by(ListItemSelector(Object::Type::UNORDERED_LIST_ITEM));
     }
 
     static Query Checklist(const std::string& status = "") {
-        return Query().by(Item(ObjectType::NONE, "", true, status));
+        return Query().by(ListItemSelector(Object::Type::NONE, "", true, status));
     }
 
     Selector* clone() const {
-        return new Item(type, ordinal, checklist_item, status);
+        return new ListItemSelector(type, ordinal, checklist_item, status);
     }
 
     bool choose(obj_t obj) const {
         if (! is_correct_type(obj)) {
             return false;
         }
 
-        if (type == ObjectType::ORDERED_LIST_ITEM && ordinal.size() > 0) {
-            auto oli = std::static_pointer_cast<object::OrderedListItem>(obj);
+        if (type == Object::Type::ORDERED_LIST_ITEM && ordinal.size() > 0) {
+            auto oli = std::static_pointer_cast<OrderedListItem>(obj);
             if (oli->ordinal() != ordinal) {
                 return false;
             }
         }
 
         if (checklist_item) {
-            auto item = std::static_pointer_cast<object::ListItem>(obj);
+            auto item = std::static_pointer_cast<ListItem>(obj);
             return item->status() != "" && (status == "" || item->status() == status);
         }
 
         return true;
     }
 
     std::string repr() const {
@@ -531,90 +530,90 @@
             if (status != "") {
                 return tfm::format("ChecklistItem<\"%s\">", status);
             } else {
                 return "ChecklistItem";
             }
         }
 
-        if (type == ObjectType::UNORDERED_LIST_ITEM) {
+        if (type == Object::Type::UNORDERED_LIST_ITEM) {
             return "UnorderedListItem";
         }
 
-        if (type == ObjectType::ORDERED_LIST_ITEM) {
+        if (type == Object::Type::ORDERED_LIST_ITEM) {
             if (ordinal != "") {
                 return "OrderedListItem";
             } else {
                 return tfm::format("OrderedListItem<\"%s\">", ordinal);
             }
         }
 
         return "ListItem";
     }
 
 private:
     bool is_correct_type(obj_t obj) const {
-        if (type == ObjectType::NONE) {
-            return obj->type() == ObjectType::ORDERED_LIST_ITEM || obj->type() == ObjectType::UNORDERED_LIST_ITEM;
+        if (type == Object::Type::NONE) {
+            return obj->type() == Object::Type::ORDERED_LIST_ITEM || obj->type() == Object::Type::UNORDERED_LIST_ITEM;
 
         } else {
             return obj->type() == type;
         }
     }
 
-    Item(ObjectType type, const std::string& ordinal = "", bool checklist_item = false, const std::string& status = "")
+    ListItemSelector(Object::Type type, const std::string& ordinal = "", bool checklist_item = false, const std::string& status = "")
     : type(type), ordinal(ordinal), checklist_item(checklist_item), status(status) { }
 
-    ObjectType type;
+    Object::Type type;
     std::string ordinal;
     bool checklist_item = false;
     std::string status;
 };
 
 // ------------------------------------------------------------------
-class Anchor : public Selector {
+class AnchorSelector : public Selector {
 public:
-    Anchor(const std::string& name) : name(name) { }
+    AnchorSelector(const std::string& name) : name(name) { }
 
     Selector* clone() const {
-        return new Anchor(name);
+        return new AnchorSelector(name);
     }
 
     bool choose(obj_t obj) const {
-        if (obj->type() == ObjectType::HASHTAG) {
-            auto anchor = std::static_pointer_cast<object::Anchor>(obj);
+        if (obj->type() == Object::Type::HASHTAG) {
+            auto anchor = std::static_pointer_cast<Anchor>(obj);
             return name == "" || anchor->name() == name;
         }
         return false;
     }
 
     std::string repr() const {
         if (name != "") {
-            return tfm::format("Anchor<\"%s\">", name);
+            return tfm::format("AnchorSelector<\"%s\">", name);
 
         } else {
-            return "Anchor";
+            return "AnchorSelector";
         }
     }
 
 private:
     std::string name;
 };
 
 // ------------------------------------------------------------------
-class Reference : public Selector {
+class ReferenceSelector : public Selector {
 public:
-    Reference(const std::string& ref_search) : ref_search(ref_search) { }
+    ReferenceSelector(const std::string& ref_search) : ref_search(ref_search) { }
 
     Selector* clone() const {
-        return new Reference(ref_search);
+        return new ReferenceSelector(ref_search);
     }
 
     bool choose(obj_t obj) const {
-        if (obj->type() == ObjectType::REF) {
-            auto ref = std::static_pointer_cast<object::Ref>(obj);
+        if (obj->type() == Object::Type::REF) {
+            auto ref = std::static_pointer_cast<Ref>(obj);
             auto& link = ref->link();
             return ref_search == "" || link.find(ref_search) != std::string::npos;
         }
         return false;
     }
 
     std::string repr() const {
@@ -626,20 +625,20 @@
     }
 
 private:
     std::string ref_search;
 };
 
 // ------------------------------------------------------------------
-class Not : public Selector {
+class LogicalNot : public Selector {
 public:
-    Not(const Query& query) : query(query.clone()) { }
+    LogicalNot(const Query& query) : query(query.clone()) { }
 
     Selector* clone() const {
-        return new Not(query.get());
+        return new LogicalNot(query.get());
     }
 
     std::vector<obj_t> select(const std::vector<obj_t>& objects) const {
         auto results = query->select(objects);
         std::set<obj_t> results_set;
         results_set.insert(results.begin(), results.end());
         results.clear();
@@ -650,46 +649,48 @@
     }
 
     std::string repr() const {
         return tfm::format("Not<%s>", query->repr());
     }
 
 private:
-    Not(const Selector* selector) : query(selector->clone()) { }
+    LogicalNot(const Selector* selector) : query(selector->clone()) { }
     std::unique_ptr<Selector> query;
 };
 
 // ------------------------------------------------------------------
 class Contains : public Selector {
 public:
     Contains(const Query& query) : query(query.clone()) { }
 
     Selector* clone() const {
         return new Contains(query.get());
     }
 
     bool choose(obj_t obj) const {
         if (obj->is_container()) {
-            auto container = std::static_pointer_cast<object::Container>(obj);
+            auto container = std::static_pointer_cast<Container>(obj);
             return query->select(container->contents()).size() > 0;
         }
         return false;
     }
 
     std::string repr() const {
         return tfm::format("Contains<%s>", query->repr());
     }
 
 private:
     Contains(const Selector* selector) : query(selector->clone()) { }
     std::unique_ptr<Selector> query;
 };
 
+namespace _private {
+
 // ------------------------------------------------------------------
-inline std::vector<std::string> tokenize(const std::string& query) {
+inline std::vector<std::string> tokenize_query(const std::string& query) {
     std::istringstream sinput(query);
     moonlight::file::BufferedInput input(sinput);
     std::vector<std::string> tokens;
     std::string token;
 
     for (;;) {
         int c = input.getc();
@@ -752,34 +753,34 @@
         }
     }
 
     return tokens;
 }
 
 // ------------------------------------------------------------------
-inline Search build_search_query(std::vector<std::string>& tokens) {
+inline RegexSelector build_search_query(std::vector<std::string>& tokens) {
     if (tokens.size() == 0) {
         throw QueryError("/search query requires an argument.");
     }
 
     auto rx = tokens.back();
     tokens.pop_back();
-    return Search(rx);
+    return RegexSelector(rx);
 }
 
 // ------------------------------------------------------------------
-inline Level build_level_query(std::vector<std::string>& tokens) {
+inline LevelSelector build_level_query(std::vector<std::string>& tokens) {
     if (tokens.size() == 0) {
         throw QueryError("/level query requires an argument.");
     }
 
     try {
         auto level = std::stoi(tokens.back());
         tokens.pop_back();
-        return Level(level);
+        return LevelSelector(level);
 
     } catch (const std::exception& e) {
         throw QueryError("Failed to parse /level query parameter as integer.");
     }
 }
 
 // ------------------------------------------------------------------
@@ -787,121 +788,130 @@
     if (tokens.size() == 0) {
         throw QueryError("/ordinal query requires an argument.");
     }
 
     auto ordinal = tokens.back();
     tokens.pop_back();
 
-    return Item::Ordered(ordinal);
+    return ListItemSelector::Ordered(ordinal);
 }
 
 // ------------------------------------------------------------------
 inline Query build_status_list_item_query(std::vector<std::string>& tokens) {
     if (tokens.size() == 0) {
         throw QueryError("/status query requires an argument.");
     }
 
     auto status = tokens.back();
     tokens.pop_back();
 
-    return Item::Checklist(status);
+    return ListItemSelector::Checklist(status);
 }
 
 // ------------------------------------------------------------------
 inline bool scan_offset_or_slice(Query& result, const std::string& token) {
     auto parts = moonlight::str::split(token, ":");
     switch(parts.size()) {
     case 2:
         try {
             result = Query().by(
-                Slice(parts[0] == "" ? std::optional<int>() : std::stoi(parts[0]),
+                SliceSelect(parts[0] == "" ? std::optional<int>() : std::stoi(parts[0]),
                       parts[1] == "" ? std::optional<int>() : std::stoi(parts[1])));
             return true;
         } catch (...) {
             return false;
         }
 
     case 1:
         try {
-            result = Query().by(Offset(std::stoi(parts[0])));
+            result = Query().by(OffsetSelector(std::stoi(parts[0])));
             return true;
 
         } catch (...) {
             return false;
         }
 
     default:
         return false;
     }
 }
 
 // ------------------------------------------------------------------
-inline Query _parse(std::vector<std::string>& tokens, int depth = -1) {
+inline Query parse(std::vector<std::string>& tokens, int depth = -1) {
     Query query;
     Query sub_result;
-    Classifier<std::string> classify;
+    moonlight::Classifier<std::string> classify;
     int cycles = 0;
 
     auto startswith = [](const std::string& s) {
         return [=](const std::string& x) {
             return x.starts_with(s);
         };
     };
 
-    classify("*") = [&]() { query.by(Children(true)); };
-    classify("**") = [&]() { query.by(Descendants(true)); };
-    classify(">") = [&]() { query.by(Children(false)); };
-    classify(">>") = [&]() { query.by(Descendants(false)); };
-    classify("<") = [&]() { query.by(Parents()); };
-    classify("<<") = [&]() { query.by(Antecedents()); };
-    classify("label") = [&]() { query.by(Label()); };
-    classify("contains") = [&]() { query.by(Contains(_parse(tokens))); };
-    classify("not", "!") = [&]() { query.by(Not(_parse(tokens, 1))); };
+    classify("*") = [&]() { query.by(ChildrenSelector(true)); };
+    classify("**") = [&]() { query.by(DescendantsSelector(true)); };
+    classify(">") = [&]() { query.by(ChildrenSelector(false)); };
+    classify(">>") = [&]() { query.by(DescendantsSelector(false)); };
+    classify("<") = [&]() { query.by(ParentSelector()); };
+    classify("<<") = [&]() { query.by(AntecedentsSelector()); };
+    classify("label") = [&]() { query.by(LabelSelector()); };
+    classify("contains") = [&]() { query.by(Contains(parse(tokens))); };
+    classify("not", "!") = [&]() { query.by(LogicalNot(parse(tokens, 1))); };
     classify("search") = [&]() { query.by(build_search_query(tokens)); };
     classify("level") = [&]() { query.by(build_level_query(tokens)); };
-    classify("line_break", "br") = [&]() { query.by(Type(ObjectType::LINE_BREAK)); };
-    classify("text", "t") = [&]() { query.by(Type(ObjectType::TEXT)); };
-    classify("content") = [&]() { query.by(Type(ObjectType::TEXT_CONTENT)); };
-    classify("list") = [&]() { query.by(List()); };
-    classify("ordered_list", "ol") = [&]() { query.by(List::Ordered()); };
-    classify("unordered_list", "ul") = [&]() { query.by(List::Unordered()); };
-    classify("check_list", "task_list") = [&]() { query.by(Contains(Item::Checklist())); };
+    classify("line_break", "br") = [&]() { query.by(TypeSelect(Object::Type::LINE_BREAK)); };
+    classify("text", "t") = [&]() { query.by(TypeSelect(Object::Type::TEXT)); };
+    classify("content") = [&]() { query.by(TypeSelect(Object::Type::TEXT_CONTENT)); };
+    classify("list") = [&]() { query.by(ListSelector()); };
+    classify("ordered_list", "ol") = [&]() { query.by(ListSelector::Ordered()); };
+    classify("unordered_list", "ul") = [&]() { query.by(ListSelector::Unordered()); };
+    classify("check_list", "task_list") = [&]() { query.by(Contains(ListItemSelector::Checklist())); };
     classify("status") = [&]() { query.by(build_status_list_item_query(tokens)); };
-    classify("item", "list_item", "li") = [&]() { query.by(Item()); };
+    classify("item", "list_item", "li") = [&]() { query.by(ListItemSelector()); };
     classify("ordinal", "ord") = [&]() { query.by(build_ordinal_list_item_query(tokens)); };
-    classify("ordered_list_item", "oli") = [&]() { query.by(Item::Ordered()); };
-    classify("unordered_list_item", "uli") = [&]() { query.by(Item::Unordered()); };
-    classify("section", "s") = [&]() { query.by(Type(ObjectType::SECTION)); };
-    classify("task", "check_item", "task_item") = [&]() { query.by(Item::Checklist()); };
+    classify("ordered_list_item", "oli") = [&]() { query.by(ListItemSelector::Ordered()); };
+    classify("unordered_list_item", "uli") = [&]() { query.by(ListItemSelector::Unordered()); };
+    classify("section", "s") = [&]() { query.by(TypeSelect(Object::Type::SECTION)); };
+    classify("task", "check_item", "task_item") = [&]() { query.by(ListItemSelector::Checklist()); };
     classify(startswith("(")) = [&](const std::string& token) {
-        auto subquery_tokens = tokenize(moonlight::slice(token, 1, -1));
-        query.by(Query(_parse(subquery_tokens)));
+        auto subquery_tokens = tokenize_query(moonlight::slice(token, 1, -1));
+        query.by(Query(parse(subquery_tokens)));
     };
-    classify(startswith("~")) = [&](const std::string& token) { query.by(Search(moonlight::slice(token, 1, {}))); };
-    classify(startswith("#")) = [&](const std::string& token) { query.by(Hashtag(moonlight::slice(token, 1, {}))); };
-    classify(startswith("@")) = [&](const std::string& token) { query.by(Reference(moonlight::slice(token, 1, {}))); };
+    classify(startswith("~")) = [&](const std::string& token) { query.by(RegexSelector(moonlight::slice(token, 1, {}))); };
+    classify(startswith("#")) = [&](const std::string& token) { query.by(HashtagSelector(moonlight::slice(token, 1, {}))); };
+    classify(startswith("@")) = [&](const std::string& token) { query.by(ReferenceSelector(moonlight::slice(token, 1, {}))); };
     classify(([&](const std::string& token) { return scan_offset_or_slice(sub_result, token); })) = [&]() { query.by(sub_result); };
     classify.otherwise() = [](const std::string& token) {
         throw QueryError(tfm::format("Unrecognized query token: \"%s\"", strliteral(token)));
     };
 
     while (tokens.size() > 0 && (depth == -1 || cycles < depth)) {
         cycles++;
         auto token = tokens.back();
         tokens.pop_back();
-        classify.match(token);
+        classify.apply(token);
     }
 
     return query;
 }
 
+}
+
+}
+
+namespace q {
+
 // ------------------------------------------------------------------
 inline Query parse(const std::string& str) {
-    auto tokens = tokenize(str);
+    auto tokens = _private::tokenize_query(str);
     std::reverse(tokens.begin(), tokens.end());
-    return _parse(tokens);
+    return _private::parse(tokens);
 }
 
 }
+
+typedef q::Query Query;
+
 }
 
 #endif /* !__JOTDOWN_QUERY_H */
```

### Comparing `jotdown-2.0.1/include/jotdown/utils.h` & `jotdown-2.0.2/moonlight/include/moonlight/classify.h`

 * *Files 23% similar despite different names*

```diff
@@ -1,117 +1,59 @@
 /*
- * utils.h
+ * classify.h
  *
  * Author: Lain Musgrove (lain.proliant@gmail.com)
- * Date: Wednesday May 27, 2020
+ * Date: Wednesday June 23, 2021
  *
  * Distributed under terms of the MIT license.
  */
 
-#ifndef __JOTDOWN_UTILS_H
-#define __JOTDOWN_UTILS_H
+#ifndef __MOONLIGHT_CLASSIFY_H
+#define __MOONLIGHT_CLASSIFY_H
 
-#include <string>
-#include <vector>
-#include <map>
-#include <sstream>
-#include <memory>
-
-#include "tinyformat/tinyformat.h"
-
-namespace jotdown {
-
-// ------------------------------------------------------------------
-inline std::string make_search_string(const std::string& src) {
-    std::string str;
-
-    for (char c : src) {
-        if (isspace(c)) {
-            if (str.size() == 0 || !isspace(str.back())) {
-                str.push_back(' ');
-            }
-        } else {
-            str.push_back(c);
-        }
-    }
-
-    return str;
-}
-
-// ------------------------------------------------------------------
-inline std::string strescape(const std::string& str, const std::string& escapes) {
-    std::ostringstream sb;
-    for (auto c : str) {
-        if (c == '\\' || escapes.find(c) != std::string::npos) {
-            sb << '\\';
-        }
-        sb << c;
-    }
-    return sb.str();
-}
-
-// ------------------------------------------------------------------
-inline std::string strliteral(const std::string& str) {
-    static const std::map<char, std::string> ESCAPE_SEQUENCES = {
-        {'\a', "\\a"},
-        {'\b', "\\b"},
-        {'\e', "\\e"},
-        {'\f', "\\f"},
-        {'\n', "\\n"},
-        {'\r', "\\r"},
-        {'\t', "\\t"},
-        {'\v', "\\v"},
-        {'\\', "\\\\"},
-        {'"', "\\\""}
-    };
+#include <functional>
+#include <optional>
+#include "moonlight/exceptions.h"
 
-    std::stringstream sb;
+namespace moonlight {
 
-    for (size_t x = 0; str[x] != '\0'; x++) {
-        char c = str[x];
-        std::string repr = "";
+namespace _private {
 
-        auto iter = ESCAPE_SEQUENCES.find(c);
-        if (iter != ESCAPE_SEQUENCES.end()) {
-            repr = iter->second;
-        }
-
-        if (repr == "" && !isprint(c)) {
-            repr = tfm::format("\\x%x", c);
-        }
+template <typename RT> struct ClassifierTraits {
+    typedef std::optional<RT> Result;
+};
 
-        if (repr != "") {
-            sb << repr;
-        } else {
-            sb << c;
-        }
-    }
+template<> struct ClassifierTraits<void> {
+    typedef void Result;
+};
 
-    return sb.str();
 }
 
-// ------------------------------------------------------------------
-template<class T>
+/** -----------------------------------------------------------------
+ */
+template<class T, class R = void>
 class Classifier {
 public:
     typedef std::function<bool(const T&)> MatchFunction;
-    typedef std::function<void()> NullaryAction;
-    typedef std::function<void(const T&)> UnaryAction;
+    typedef std::function<R()> NullaryAction;
+    typedef std::function<R(const T&)> UnaryAction;
+
+    typedef _private::ClassifierTraits<R> Traits;
 
     class Action {
     public:
         Action(NullaryAction action) : _nullary(action), _unary({}) { }
         Action(UnaryAction action) : _nullary({}), _unary(action) { }
 
-        void nullary() const {
-            _nullary.value()();
+        typename Traits::Result nullary() const {
+            return _nullary.value()();
         }
 
-        void unary(const T& value) const {
-            _unary.value()(value);
+        typename Traits::Result unary(const T& value) const {
+            return _unary.value()(value);
         }
 
         bool is_unary() const {
             return _unary.has_value();
         }
 
     private:
@@ -120,24 +62,24 @@
     };
 
     class Case {
     public:
         template<class ActionImpl>
         Case(MatchFunction match, ActionImpl action) : _match(match), _action(Action(action)) { }
 
-        bool match(const T& value) const {
-            if (_match(value)) {
-                if (_action.is_unary()) {
-                    _action.unary(value);
-                } else {
-                    _action.nullary();
-                }
-                return true;
+        typename Traits::Result apply(const T& value) const {
+            if (_action.is_unary()) {
+                return _action.unary(value);
+            } else {
+                return _action.nullary();
             }
-            return false;
+        }
+
+        bool match(const T& value) const {
+            return _match(value);
         }
 
     private:
         MatchFunction _match;
         Action _action;
     };
 
@@ -160,21 +102,30 @@
         return CaseAssigner(*this, f_or_join(matches...));
     }
 
     CaseAssigner otherwise() {
         return CaseAssigner(*this, [](const T& value) { (void)value; return true; });
     }
 
-    bool match(const T& value) const {
+    std::optional<Case> match(const T& value) const {
         for (auto case_ : _cases) {
             if (case_.match(value)) {
-                return true;
+                return case_;
             }
         }
-        return false;
+        return {};
+    }
+
+    typename Traits::Result apply(const T& value) const {
+        auto case_ = match(value);
+        if (case_.has_value()) {
+            return case_->apply(value);
+        } else {
+            return typename Traits::Result();
+        }
     }
 
 private:
     static MatchFunction f_eq(const T& value) {
         return [=](const T& x) {
             return x == value;
         };
@@ -205,8 +156,9 @@
     }
 
     std::vector<Case> _cases;
 };
 
 }
 
-#endif /* !__JOTDOWN_UTILS_H */
+
+#endif /* !__MOONLIGHT_CLASSIFY_H */
```

### Comparing `jotdown-2.0.1/jotdown.egg-info/PKG-INFO` & `jotdown-2.0.2/jotdown.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,93 +1,93 @@
 Metadata-Version: 2.1
 Name: jotdown
-Version: 2.0.1
+Version: 2.0.2
 Summary: Jotdown structrured document language, C++ to python wrapper module.
 Home-page: https://github.com/lainproliant/jotdown
 Author: Lain Musgrove (lainproliant)
 Author-email: lainproliant@gmail.com
 License: BSD
-Description: # Jotdown
-        Jotdown is a structured document language.  It is an opinionated, augmented
-        subset of Markdown with features inspired by plain-text organizational tools
-        like org-mode.  The main purpose of Jotdown is to centralize personal and
-        project organization into a set of plain-text documents that can be easily
-        edited, parsed, and manipulated both by scripts and humans alike.
-        
-        Jotdown is offered simultaneously as a header-only C++ library and a compiled
-        Python module sharing the same code.  The Python bindings are enabled via
-        pybind11.  It is released under an MIT license, see LICENSE for more info.
-        
-        See [DOCUMENTATION.md] for a detailed explanation of the language and its
-        features.
-        
-        See [API_CXX.md] for documentation regarding the header-only C++ library.
-        
-        See [API_PY.md] for documentation regarding the Python module, including how to
-        build and install it.
-        
-        ## Goals
-        These are the primary goals of the Jotdown language and project:
-        
-        - Support the creation, analysis, and modification of plain-text structured
-            documents.
-        - Support the hypertext linkage of documents within a document-set, and to
-            outside resources on the web or elsewhere.
-        - First-class support for loading, querying, modifying, saving, and creating
-            documents in C++ and Python.
-        
-        ## Q/A
-        ### Why not just use Markdown for this?
-        While Markdown is great as a text formatting language, it doesn't work as an
-        easily parsable structured document language.  It's main focus has always been 
-        generating HTML, and as such many of the existing parsers don't even bother
-        creating an intermediate AST.  I also feel that Markdown, though it is formally
-        defined in the CommonMark and Github Flavored Markdown specs, has hugely complex
-        rules for parsing to support features that aren't often used or don't need to
-        exist.
-        
-        ### Why is Jotdown offered in C++ and Python?
-        I wanted to be able to support the runtime power and expressiveness of C++ while
-        also extending support into Python where scripts and plugins can be easily built
-        around Jotdown document structures.
-        
-        ### Why is my language not supported?
-        I'm sorry!  I'm really happy you're interested in Jotdown though.  Feel free to
-        submit an issue to add support for your language.  I can't guarantee I'll ever
-        get around to writing bindings myself, but someone in the community might step
-        up and help out!
-        
-        ### What are you planning to do with Jotdown in the future?
-        Some things I'm planning on building around Jotdown include:
-        
-        - A Vim plugin which will support advanced editing features and highlighting.
-        - Command line productivity tools built around the concept of a Jotdown document set.
-        - A web wiki built around the concept of a Jotdown document set.
-        
-        # Change Log
-        ### 01/24/2021: v2.0.0
-        - Removed support for custom '@' style links, replaced with Markdown style
-          links and link indexes.
-        
-        ### 07/24/2020: v1.3.0
-        - Added support for document front-matter.
-        - New features for the Python interface:
-          - Collections are now callable.  With no arguments, calling them will return
-            their contents as a list.  With arguments, they will return themselves with
-            all of the arguments being added in sequence.
-          - Section can now be constructed with a string or a TextContent for the header.
-          - TextContent can now be initialized with a string.
-        
-        ### 07/17/2020: v1.2.0
-        - Refactored `objects.h` to do runtime validation of insertion types rather than
-          limiting via the C++ type system to reduce code duplication.
-        - Added `Container::insert_before` and `Container::insert_after`.
-        
-        
 Keywords: document structure parser query language
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Jotdown
+Jotdown is a structured document language.  It is an opinionated, augmented
+subset of Markdown with features inspired by plain-text organizational tools
+like org-mode.  The main purpose of Jotdown is to centralize personal and
+project organization into a set of plain-text documents that can be easily
+edited, parsed, and manipulated both by scripts and humans alike.
+
+Jotdown is offered simultaneously as a header-only C++ library and a compiled
+Python module sharing the same code.  The Python bindings are enabled via
+pybind11.  It is released under an MIT license, see LICENSE for more info.
+
+See [DOCUMENTATION.md] for a detailed explanation of the language and its
+features.
+
+See [API_CXX.md] for documentation regarding the header-only C++ library.
+
+See [API_PY.md] for documentation regarding the Python module, including how to
+build and install it.
+
+## Goals
+These are the primary goals of the Jotdown language and project:
+
+- Support the creation, analysis, and modification of plain-text structured
+    documents.
+- Support the hypertext linkage of documents within a document-set, and to
+    outside resources on the web or elsewhere.
+- First-class support for loading, querying, modifying, saving, and creating
+    documents in C++ and Python.
+
+## Q/A
+### Why not just use Markdown for this?
+While Markdown is great as a text formatting language, it doesn't work as an
+easily parsable structured document language.  It's main focus has always been 
+generating HTML, and as such many of the existing parsers don't even bother
+creating an intermediate AST.  I also feel that Markdown, though it is formally
+defined in the CommonMark and Github Flavored Markdown specs, has hugely complex
+rules for parsing to support features that aren't often used or don't need to
+exist.
+
+### Why is Jotdown offered in C++ and Python?
+I wanted to be able to support the runtime power and expressiveness of C++ while
+also extending support into Python where scripts and plugins can be easily built
+around Jotdown document structures.
+
+### Why is my language not supported?
+I'm sorry!  I'm really happy you're interested in Jotdown though.  Feel free to
+submit an issue to add support for your language.  I can't guarantee I'll ever
+get around to writing bindings myself, but someone in the community might step
+up and help out!
+
+### What are you planning to do with Jotdown in the future?
+Some things I'm planning on building around Jotdown include:
+
+- A Vim plugin which will support advanced editing features and highlighting.
+- Command line productivity tools built around the concept of a Jotdown document set.
+- A web wiki built around the concept of a Jotdown document set.
+
+# Change Log
+### 01/24/2021: v2.0.0
+- Removed support for custom '@' style links, replaced with Markdown style
+  links and link indexes.
+
+### 07/24/2020: v1.3.0
+- Added support for document front-matter.
+- New features for the Python interface:
+  - Collections are now callable.  With no arguments, calling them will return
+    their contents as a list.  With arguments, they will return themselves with
+    all of the arguments being added in sequence.
+  - Section can now be constructed with a string or a TextContent for the header.
+  - TextContent can now be initialized with a string.
+
+### 07/17/2020: v1.2.0
+- Refactored `objects.h` to do runtime validation of insertion types rather than
+  limiting via the C++ type system to reduce code duplication.
+- Added `Container::insert_before` and `Container::insert_after`.
+
```

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/chrono_io.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/chrono_io.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/date.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/date.h`

 * *Files 1% similar despite different names*

```diff
@@ -41,17 +41,15 @@
 #endif  // HAS_STRING_VIEW
 
 #include <cassert>
 #include <algorithm>
 #include <cctype>
 #include <chrono>
 #include <climits>
-#if !(__cplusplus >= 201402)
-#  include <cmath>
-#endif
+#include <cmath>
 #include <cstddef>
 #include <cstdint>
 #include <cstdlib>
 #include <ctime>
 #include <ios>
 #include <istream>
 #include <iterator>
@@ -134,15 +132,15 @@
 #  define CONSTDATA constexpr const
 #  define CONSTCD11 constexpr
 #  define CONSTCD14
 #  define NOEXCEPT noexcept
 #endif
 
 #ifndef HAS_UNCAUGHT_EXCEPTIONS
-#  if __cplusplus > 201703 || (defined(_MSVC_LANG) && _MSVC_LANG > 201703L)
+#  if __cplusplus >= 201703 || (defined(_MSVC_LANG) && _MSVC_LANG >= 201703L)
 #    define HAS_UNCAUGHT_EXCEPTIONS 1
 #  else
 #    define HAS_UNCAUGHT_EXCEPTIONS 0
 #  endif
 #endif  // HAS_UNCAUGHT_EXCEPTIONS
 
 #ifndef HAS_VOID_T
@@ -1018,35 +1016,38 @@
 template<class CharT, class Traits = std::char_traits<CharT>>
 class save_istream
 {
 protected:
     std::basic_ios<CharT, Traits>& is_;
     CharT fill_;
     std::ios::fmtflags flags_;
+    std::streamsize precision_;
     std::streamsize width_;
     std::basic_ostream<CharT, Traits>* tie_;
     std::locale loc_;
 
 public:
     ~save_istream()
     {
         is_.fill(fill_);
         is_.flags(flags_);
+        is_.precision(precision_);
         is_.width(width_);
         is_.imbue(loc_);
         is_.tie(tie_);
     }
 
     save_istream(const save_istream&) = delete;
     save_istream& operator=(const save_istream&) = delete;
 
     explicit save_istream(std::basic_ios<CharT, Traits>& is)
         : is_(is)
         , fill_(is.fill())
         , flags_(is.flags())
+        , precision_(is.precision())
         , width_(is.width(0))
         , tie_(is.tie(nullptr))
         , loc_(is.getloc())
         {
             if (tie_ != nullptr)
                 tie_->flush();
         }
@@ -1162,15 +1163,19 @@
 private:
     static const std::intmax_t gcd_n1_n2 = static_gcd<R1::num, R2::num>::value;
     static const std::intmax_t gcd_d1_d2 = static_gcd<R1::den, R2::den>::value;
     static const std::intmax_t n1 = R1::num / gcd_n1_n2;
     static const std::intmax_t d1 = R1::den / gcd_d1_d2;
     static const std::intmax_t n2 = R2::num / gcd_n1_n2;
     static const std::intmax_t d2 = R2::den / gcd_d1_d2;
+#ifdef __cpp_constexpr
     static const std::intmax_t max = std::numeric_limits<std::intmax_t>::max();
+#else
+    static const std::intmax_t max = LLONG_MAX;
+#endif
 
     template <std::intmax_t Xp, std::intmax_t Yp, bool overflow>
     struct mul    // overflow == false
     {
         static const std::intmax_t value = Xp * Yp;
     };
 
@@ -1350,14 +1355,55 @@
 using std::chrono::floor;
 using std::chrono::ceil;
 using std::chrono::round;
 using std::chrono::abs;
 
 #endif  // HAS_CHRONO_ROUNDING
 
+namespace detail
+{
+
+template <class To, class Rep, class Period>
+CONSTCD14
+inline
+typename std::enable_if
+<
+    !std::chrono::treat_as_floating_point<typename To::rep>::value,
+    To
+>::type
+round_i(const std::chrono::duration<Rep, Period>& d)
+{
+    return round<To>(d);
+}
+
+template <class To, class Rep, class Period>
+CONSTCD14
+inline
+typename std::enable_if
+<
+    std::chrono::treat_as_floating_point<typename To::rep>::value,
+    To
+>::type
+round_i(const std::chrono::duration<Rep, Period>& d)
+{
+    return d;
+}
+
+template <class To, class Clock, class FromDuration>
+CONSTCD11
+inline
+std::chrono::time_point<Clock, To>
+round_i(const std::chrono::time_point<Clock, FromDuration>& tp)
+{
+    using std::chrono::time_point;
+    return time_point<Clock, To>{round_i<To>(tp.time_since_epoch())};
+}
+
+}  // detail
+
 // trunc towards zero
 template <class To, class Clock, class FromDuration>
 CONSTCD11
 inline
 std::chrono::time_point<Clock, To>
 trunc(const std::chrono::time_point<Clock, FromDuration>& tp)
 {
@@ -1454,24 +1500,37 @@
 inline
 day
 operator-(const day& x, const days& y) NOEXCEPT
 {
     return x + -y;
 }
 
+namespace detail
+{
+
 template<class CharT, class Traits>
-inline
 std::basic_ostream<CharT, Traits>&
-operator<<(std::basic_ostream<CharT, Traits>& os, const day& d)
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const day& d)
 {
     detail::save_ostream<CharT, Traits> _(os);
     os.fill('0');
     os.flags(std::ios::dec | std::ios::right);
     os.width(2);
     os << static_cast<unsigned>(d);
+    return os;
+}
+
+}  // namespace detail
+
+template<class CharT, class Traits>
+inline
+std::basic_ostream<CharT, Traits>&
+operator<<(std::basic_ostream<CharT, Traits>& os, const day& d)
+{
+    detail::low_level_fmt(os, d);
     if (!d.ok())
         os << " is not a valid day";
     return os;
 }
 
 // month
 
@@ -1581,26 +1640,41 @@
 inline
 month
 operator-(const month& x, const months& y) NOEXCEPT
 {
     return x + -y;
 }
 
+namespace detail
+{
+
 template<class CharT, class Traits>
-inline
 std::basic_ostream<CharT, Traits>&
-operator<<(std::basic_ostream<CharT, Traits>& os, const month& m)
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const month& m)
 {
     if (m.ok())
     {
         CharT fmt[] = {'%', 'b', 0};
         os << format(os.getloc(), fmt, m);
     }
     else
-        os << static_cast<unsigned>(m) << " is not a valid month";
+        os << static_cast<unsigned>(m);
+    return os;
+}
+
+}  // namespace detail
+
+template<class CharT, class Traits>
+inline
+std::basic_ostream<CharT, Traits>&
+operator<<(std::basic_ostream<CharT, Traits>& os, const month& m)
+{
+    detail::low_level_fmt(os, m);
+    if (!m.ok())
+        os << " is not a valid month";
     return os;
 }
 
 // year
 
 CONSTCD11 inline year::year(int y) NOEXCEPT : y_(static_cast<decltype(y_)>(y)) {}
 CONSTCD14 inline year& year::operator++() NOEXCEPT {++y_; return *this;}
@@ -1706,25 +1780,38 @@
 inline
 year
 operator-(const year& x, const years& y) NOEXCEPT
 {
     return year{static_cast<int>(x) - y.count()};
 }
 
+namespace detail
+{
+
 template<class CharT, class Traits>
-inline
 std::basic_ostream<CharT, Traits>&
-operator<<(std::basic_ostream<CharT, Traits>& os, const year& y)
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const year& y)
 {
     detail::save_ostream<CharT, Traits> _(os);
     os.fill('0');
     os.flags(std::ios::dec | std::ios::internal);
     os.width(4 + (y < year{0}));
     os.imbue(std::locale::classic());
     os << static_cast<int>(y);
+    return os;
+}
+
+}  // namespace detail
+
+template<class CharT, class Traits>
+inline
+std::basic_ostream<CharT, Traits>&
+operator<<(std::basic_ostream<CharT, Traits>& os, const year& y)
+{
+    detail::low_level_fmt(os, y);
     if (!y.ok())
         os << " is not a valid year";
     return os;
 }
 
 // weekday
 
@@ -1842,26 +1929,41 @@
 inline
 weekday
 operator-(const weekday& x, const days& y) NOEXCEPT
 {
     return x + -y;
 }
 
+namespace detail
+{
+
 template<class CharT, class Traits>
-inline
 std::basic_ostream<CharT, Traits>&
-operator<<(std::basic_ostream<CharT, Traits>& os, const weekday& wd)
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const weekday& wd)
 {
     if (wd.ok())
     {
         CharT fmt[] = {'%', 'a', 0};
         os << format(fmt, wd);
     }
     else
-        os << static_cast<unsigned>(wd.wd_) << " is not a valid weekday";
+        os << wd.c_encoding();
+    return os;
+}
+
+}  // namespace detail
+
+template<class CharT, class Traits>
+inline
+std::basic_ostream<CharT, Traits>&
+operator<<(std::basic_ostream<CharT, Traits>& os, const weekday& wd)
+{
+    detail::low_level_fmt(os, wd);
+    if (!wd.ok())
+        os << " is not a valid weekday";
     return os;
 }
 
 #if !defined(_MSC_VER) || (_MSC_VER >= 1900)
 inline namespace literals
 {
 
@@ -1962,23 +2064,34 @@
     , index_(static_cast<decltype(index_)>(index))
     {}
 
 #ifdef __GNUC__
 #  pragma GCC diagnostic pop
 #endif  // __GNUC__
 
+namespace detail
+{
+
+template<class CharT, class Traits>
+std::basic_ostream<CharT, Traits>&
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const weekday_indexed& wdi)
+{
+    return low_level_fmt(os, wdi.weekday()) << '[' << wdi.index() << ']';
+}
+
+}  // namespace detail
+
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const weekday_indexed& wdi)
 {
-    os << wdi.weekday() << '[' << wdi.index();
-    if (!(1 <= wdi.index() && wdi.index() <= 5))
-        os << " is not a valid index";
-    os << ']';
+    detail::low_level_fmt(os, wdi);
+    if (!wdi.ok())
+        os << " is not a valid weekday_indexed";
     return os;
 }
 
 CONSTCD11
 inline
 weekday_indexed
 weekday::operator[](unsigned index) const NOEXCEPT
@@ -2020,20 +2133,35 @@
 inline
 bool
 operator!=(const weekday_last& x, const weekday_last& y) NOEXCEPT
 {
     return !(x == y);
 }
 
+namespace detail
+{
+
+template<class CharT, class Traits>
+std::basic_ostream<CharT, Traits>&
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const weekday_last& wdl)
+{
+    return low_level_fmt(os, wdl.weekday()) << "[last]";
+}
+
+}  // namespace detail
+
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const weekday_last& wdl)
 {
-    return os << wdl.weekday() << "[last]";
+    detail::low_level_fmt(os, wdl);
+    if (!wdl.ok())
+        os << " is not a valid weekday_last";
+    return os;
 }
 
 CONSTCD11
 inline
 weekday_last
 weekday::operator[](last_spec) const NOEXCEPT
 {
@@ -2200,20 +2328,36 @@
 inline
 year_month
 operator-(const year_month& ym, const years& dy) NOEXCEPT
 {
     return ym + -dy;
 }
 
+namespace detail
+{
+
+template<class CharT, class Traits>
+std::basic_ostream<CharT, Traits>&
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const year_month& ym)
+{
+    low_level_fmt(os, ym.year()) << '/';
+    return low_level_fmt(os, ym.month());
+}
+
+}  // namespace detail
+
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const year_month& ym)
 {
-    return os << ym.year() << '/' << ym.month();
+    detail::low_level_fmt(os, ym);
+    if (!ym.ok())
+        os << " is not a valid year_month";
+    return os;
 }
 
 // month_day
 
 CONSTCD11
 inline
 month_day::month_day(const date::month& m, const date::day& d) NOEXCEPT
@@ -2285,20 +2429,36 @@
 inline
 bool
 operator>=(const month_day& x, const month_day& y) NOEXCEPT
 {
     return !(x < y);
 }
 
+namespace detail
+{
+
+template<class CharT, class Traits>
+std::basic_ostream<CharT, Traits>&
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const month_day& md)
+{
+    low_level_fmt(os, md.month()) << '/';
+    return low_level_fmt(os, md.day());
+}
+
+}  // namespace detail
+
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const month_day& md)
 {
-    return os << md.month() << '/' << md.day();
+    detail::low_level_fmt(os, md);
+    if (!md.ok())
+        os << " is not a valid month_day";
+    return os;
 }
 
 // month_day_last
 
 CONSTCD11 inline month month_day_last::month() const NOEXCEPT {return m_;}
 CONSTCD11 inline bool month_day_last::ok() const NOEXCEPT {return m_.ok();}
 CONSTCD11 inline month_day_last::month_day_last(const date::month& m) NOEXCEPT : m_(m) {}
@@ -2347,20 +2507,35 @@
 inline
 bool
 operator>=(const month_day_last& x, const month_day_last& y) NOEXCEPT
 {
     return !(x < y);
 }
 
+namespace detail
+{
+
+template<class CharT, class Traits>
+std::basic_ostream<CharT, Traits>&
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const month_day_last& mdl)
+{
+    return low_level_fmt(os, mdl.month()) << "/last";
+}
+
+}  // namespace detail
+
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const month_day_last& mdl)
 {
-    return os << mdl.month() << "/last";
+    detail::low_level_fmt(os, mdl);
+    if (!mdl.ok())
+        os << " is not a valid month_day_last";
+    return os;
 }
 
 // month_weekday
 
 CONSTCD11
 inline
 month_weekday::month_weekday(const date::month& m,
@@ -2399,20 +2574,36 @@
 inline
 bool
 operator!=(const month_weekday& x, const month_weekday& y) NOEXCEPT
 {
     return !(x == y);
 }
 
+namespace detail
+{
+
+template<class CharT, class Traits>
+std::basic_ostream<CharT, Traits>&
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const month_weekday& mwd)
+{
+    low_level_fmt(os, mwd.month()) << '/';
+    return low_level_fmt(os, mwd.weekday_indexed());
+}
+
+}  // namespace detail
+
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const month_weekday& mwd)
 {
-    return os << mwd.month() << '/' << mwd.weekday_indexed();
+    detail::low_level_fmt(os, mwd);
+    if (!mwd.ok())
+        os << " is not a valid month_weekday";
+    return os;
 }
 
 // month_weekday_last
 
 CONSTCD11
 inline
 month_weekday_last::month_weekday_last(const date::month& m,
@@ -2451,20 +2642,36 @@
 inline
 bool
 operator!=(const month_weekday_last& x, const month_weekday_last& y) NOEXCEPT
 {
     return !(x == y);
 }
 
+namespace detail
+{
+
+template<class CharT, class Traits>
+std::basic_ostream<CharT, Traits>&
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const month_weekday_last& mwdl)
+{
+    low_level_fmt(os, mwdl.month()) << '/';
+    return low_level_fmt(os, mwdl.weekday_last());
+}
+
+}  // namespace detail
+
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const month_weekday_last& mwdl)
 {
-    return os << mwdl.month() << '/' << mwdl.weekday_last();
+    detail::low_level_fmt(os, mwdl);
+    if (!mwdl.ok())
+        os << " is not a valid month_weekday_last";
+    return os;
 }
 
 // year_month_day_last
 
 CONSTCD11
 inline
 year_month_day_last::year_month_day_last(const date::year& y,
@@ -2606,20 +2813,36 @@
 inline
 bool
 operator>=(const year_month_day_last& x, const year_month_day_last& y) NOEXCEPT
 {
     return !(x < y);
 }
 
+namespace detail
+{
+
+template<class CharT, class Traits>
+std::basic_ostream<CharT, Traits>&
+low_level_fmt(std::basic_ostream<CharT, Traits>& os, const year_month_day_last& ymdl)
+{
+    low_level_fmt(os, ymdl.year()) << '/';
+    return low_level_fmt(os, ymdl.month_day_last());
+}
+
+}  // namespace detail
+
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const year_month_day_last& ymdl)
 {
-    return os << ymdl.year() << '/' << ymdl.month_day_last();
+    detail::low_level_fmt(os, ymdl);
+    if (!ymdl.ok())
+        os << " is not a valid year_month_day_last";
+    return os;
 }
 
 template<class>
 CONSTCD14
 inline
 year_month_day_last
 operator+(const year_month_day_last& ymdl, const months& dm) NOEXCEPT
@@ -2842,20 +3065,21 @@
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const year_month_day& ymd)
 {
     detail::save_ostream<CharT, Traits> _(os);
     os.fill('0');
     os.flags(std::ios::dec | std::ios::right);
     os.imbue(std::locale::classic());
-    os << ymd.year() << '-';
+    os << static_cast<int>(ymd.year()) << '-';
     os.width(2);
     os << static_cast<unsigned>(ymd.month()) << '-';
-    os << ymd.day();
+    os.width(2);
+    os << static_cast<unsigned>(ymd.day());
     if (!ymd.ok())
-        os << " is not a valid date";
+        os << " is not a valid year_month_day";
     return os;
 }
 
 CONSTCD14
 inline
 year_month_day
 year_month_day::from_days(days dp) NOEXCEPT
@@ -3083,16 +3307,20 @@
 }
 
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const year_month_weekday& ymwdi)
 {
-    return os << ymwdi.year() << '/' << ymwdi.month()
-              << '/' << ymwdi.weekday_indexed();
+    detail::low_level_fmt(os, ymwdi.year()) << '/';
+    detail::low_level_fmt(os, ymwdi.month()) << '/';
+    detail::low_level_fmt(os, ymwdi.weekday_indexed());
+    if (!ymwdi.ok())
+        os << " is not a valid year_month_weekday";
+    return os;
 }
 
 template<class>
 CONSTCD14
 inline
 year_month_weekday
 operator+(const year_month_weekday& ymwd, const months& dm) NOEXCEPT
@@ -3260,15 +3488,20 @@
 }
 
 template<class CharT, class Traits>
 inline
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const year_month_weekday_last& ymwdl)
 {
-    return os << ymwdl.year() << '/' << ymwdl.month() << '/' << ymwdl.weekday_last();
+    detail::low_level_fmt(os, ymwdl.year()) << '/';
+    detail::low_level_fmt(os, ymwdl.month()) << '/';
+    detail::low_level_fmt(os, ymwdl.weekday_last());
+    if (!ymwdl.ok())
+        os << " is not a valid year_month_weekday_last";
+    return os;
 }
 
 template<class>
 CONSTCD14
 inline
 year_month_weekday_last
 operator+(const year_month_weekday_last& ymwdl, const months& dm) NOEXCEPT
@@ -3677,19 +3910,20 @@
 // If 1/n takes more than 18 fractional decimal digits,
 //   the result is truncated to 19.
 // Example:  width<2>::value    ==  1
 // Example:  width<3>::value    == 19
 // Example:  width<4>::value    ==  2
 // Example:  width<10>::value   ==  1
 // Example:  width<1000>::value ==  3
-template <std::uint64_t n, std::uint64_t d = 10, unsigned w = 0,
-          bool should_continue = !(n < 2) && d != 0 && (w < 19)>
+template <std::uint64_t n, std::uint64_t d, unsigned w = 0,
+          bool should_continue = n%d != 0 && (w < 19)>
 struct width
 {
-    static CONSTDATA unsigned value = 1 + width<n, d%n*10, w+1>::value;
+    static_assert(d > 0, "width called with zero denominator");
+    static CONSTDATA unsigned value = 1 + width<n%d*10, d, w+1>::value;
 };
 
 template <std::uint64_t n, std::uint64_t d, unsigned w>
 struct width<n, d, w, false>
 {
     static CONSTDATA unsigned value = 0;
 };
@@ -3710,17 +3944,18 @@
 };
 
 template <class Duration>
 class decimal_format_seconds
 {
     using CT = typename std::common_type<Duration, std::chrono::seconds>::type;
     using rep = typename CT::rep;
+    static unsigned CONSTDATA trial_width =
+        detail::width<CT::period::num, CT::period::den>::value;
 public:
-    static unsigned constexpr width = detail::width<CT::period::den>::value < 19 ?
-                                      detail::width<CT::period::den>::value : 6u;
+    static unsigned CONSTDATA width = trial_width < 19 ? trial_width : 6u;
     using precision = std::chrono::duration<rep,
                                             std::ratio<1, static_pow10<width>::value>>;
 
 private:
     std::chrono::seconds s_;
     precision            sub_s_;
 
@@ -3761,14 +3996,15 @@
     std::basic_ostream<CharT, Traits>&
     print(std::basic_ostream<CharT, Traits>& os, std::true_type) const
     {
         date::detail::save_ostream<CharT, Traits> _(os);
         std::chrono::duration<rep> d = s_ + sub_s_;
         if (d < std::chrono::seconds{10})
             os << '0';
+        os.precision(width+6);
         os << std::fixed << d.count();
         return os;
     }
 
     template <class CharT, class Traits>
     std::basic_ostream<CharT, Traits>&
     print(std::basic_ostream<CharT, Traits>& os, std::false_type) const
@@ -3951,31 +4187,28 @@
         h = hours{0};
     return h;
 }
 
 template <class Duration>
 using time_of_day = hh_mm_ss<Duration>;
 
-template <class Rep, class Period,
-          class = typename std::enable_if
-              <!std::chrono::treat_as_floating_point<Rep>::value>::type>
+template <class Rep, class Period>
 CONSTCD11
 inline
 hh_mm_ss<std::chrono::duration<Rep, Period>>
 make_time(const std::chrono::duration<Rep, Period>& d)
 {
     return hh_mm_ss<std::chrono::duration<Rep, Period>>(d);
 }
 
 template <class CharT, class Traits, class Duration>
 inline
 typename std::enable_if
 <
-    !std::chrono::treat_as_floating_point<typename Duration::rep>::value &&
-        std::ratio_less<typename Duration::period, days::period>::value
+    std::ratio_less<typename Duration::period, days::period>::value
     , std::basic_ostream<CharT, Traits>&
 >::type
 operator<<(std::basic_ostream<CharT, Traits>& os, const sys_time<Duration>& tp)
 {
     auto const dp = date::floor<days>(tp);
     return os << year_month_day(dp) << ' ' << make_time(tp-dp);
 }
@@ -4144,18 +4377,18 @@
     return x;
 }
 
 #if __cplusplus >= 201402  && (!defined(__EDG_VERSION__) || __EDG_VERSION__ > 411) \
                            && (!defined(__SUNPRO_CC) || __SUNPRO_CC > 0x5150)
 
 template <class CharT,
-          class = std::enable_if_t<std::is_same<CharT, char>{} ||
-                                   std::is_same<CharT, wchar_t>{} ||
-                                   std::is_same<CharT, char16_t>{} ||
-                                   std::is_same<CharT, char32_t>{}>>
+          class = std::enable_if_t<std::is_same<CharT, char>::value ||
+                                   std::is_same<CharT, wchar_t>::value ||
+                                   std::is_same<CharT, char16_t>::value ||
+                                   std::is_same<CharT, char32_t>::value>>
 CONSTCD14
 inline
 string_literal<CharT, 2>
 msl(CharT c) NOEXCEPT
 {
     return string_literal<CharT, 2>{c};
 }
@@ -4730,28 +4963,28 @@
         // Peek at the next CharT but don't consume it
         auto ic = is.peek();
         if (ic == EOF)
         {
             is.setstate(std::ios::eofbit);
             break;
         }
-        auto c = static_cast<char>(toupper(ic));
+        auto c = static_cast<char>(toupper(static_cast<unsigned char>(ic)));
         bool consume = false;
         // For each keyword which might match, see if the indx character is c
         // If a match if found, consume c
         // If a match is found, and that is the last character in the keyword,
         //    then that keyword matches.
         // If the keyword doesn't match this character, then change the keyword
         //    to doesn't match
         st = status;
         for (auto ky = kb; ky != ke; ++ky, ++st)
         {
             if (*st == might_match)
             {
-                if (c == static_cast<char>(toupper((*ky)[indx])))
+                if (c == static_cast<char>(toupper(static_cast<unsigned char>((*ky)[indx]))))
                 {
                     consume = true;
                     if (ky->size() == indx+1)
                     {
                         *st = does_match;
                         --n_might_match;
                         ++n_does_match;
@@ -6118,45 +6351,59 @@
 }
 
 template <class CharT, class Traits>
 long double
 read_long_double(std::basic_istream<CharT, Traits>& is, unsigned m = 1, unsigned M = 10)
 {
     unsigned count = 0;
+    unsigned fcount = 0;
+    unsigned long long i = 0;
+    unsigned long long f = 0;
+    bool parsing_fraction = false;
+#if ONLY_C_LOCALE
+    typename Traits::int_type decimal_point = '.';
+#else
     auto decimal_point = Traits::to_int_type(
         std::use_facet<std::numpunct<CharT>>(is.getloc()).decimal_point());
-    std::string buf;
+#endif
     while (true)
     {
         auto ic = is.peek();
         if (Traits::eq_int_type(ic, Traits::eof()))
             break;
         if (Traits::eq_int_type(ic, decimal_point))
         {
-            buf += '.';
             decimal_point = Traits::eof();
-            is.get();
+            parsing_fraction = true;
         }
         else
         {
             auto c = static_cast<char>(Traits::to_char_type(ic));
             if (!('0' <= c && c <= '9'))
                 break;
-            buf += c;
-            (void)is.get();
+            if (!parsing_fraction)
+            {
+                i = 10*i + static_cast<unsigned>(c - '0');
+            }
+            else
+            {
+                f = 10*f + static_cast<unsigned>(c - '0');
+                ++fcount;
+            }
         }
+        (void)is.get();
         if (++count == M)
             break;
     }
     if (count < m)
     {
         is.setstate(std::ios::failbit);
         return 0;
     }
-    return std::stold(buf);
+    return i + f/std::pow(10.L, fcount);
 }
 
 struct rs
 {
     int& i;
     unsigned m;
     unsigned M;
@@ -6305,14 +6552,15 @@
     using std::numeric_limits;
     using std::ios;
     using std::chrono::duration;
     using std::chrono::duration_cast;
     using std::chrono::seconds;
     using std::chrono::minutes;
     using std::chrono::hours;
+    using detail::round_i;
     typename std::basic_istream<CharT, Traits>::sentry ok{is, true};
     if (ok)
     {
         date::detail::save_istream<CharT, Traits> ss(is);
         is.fill(' ');
         is.flags(std::ios::skipws | std::ios::dec);
         is.width(0);
@@ -6320,15 +6568,15 @@
         auto& f = std::use_facet<std::time_get<CharT>>(is.getloc());
         std::tm tm{};
 #endif
         const CharT* command = nullptr;
         auto modified = CharT{};
         auto width = -1;
 
-        CONSTDATA int not_a_year = numeric_limits<int>::min();
+        CONSTDATA int not_a_year = numeric_limits<short>::min();
         CONSTDATA int not_a_2digit_year = 100;
         CONSTDATA int not_a_century = not_a_year / 100;
         CONSTDATA int not_a_month = 0;
         CONSTDATA int not_a_day = 0;
         CONSTDATA int not_a_hour = numeric_limits<int>::min();
         CONSTDATA int not_a_hour_12_value = 0;
         CONSTDATA int not_a_minute = not_a_hour;
@@ -6518,15 +6766,15 @@
                         int tH;
                         int tM;
                         long double S;
                         read(is, ru{tH, 1, 2}, CharT{':'}, ru{tM, 1, 2},
                                                CharT{':'}, rld{S, 1, w});
                         checked_set(H, tH, not_a_hour, is);
                         checked_set(M, tM, not_a_minute, is);
-                        checked_set(s, round<Duration>(duration<long double>{S}),
+                        checked_set(s, round_i<Duration>(duration<long double>{S}),
                                     not_a_second, is);
                         ws(is);
                         int tY = not_a_year;
                         read(is, rs{tY, 1, 4u});
                         checked_set(Y, tY, not_a_year, is);
 #endif
                     }
@@ -6598,15 +6846,15 @@
                         int tH = not_a_hour;
                         int tM = not_a_minute;
                         long double S;
                         read(is, ru{tH, 1, 2}, CharT{':'}, ru{tM, 1, 2},
                                                CharT{':'}, rld{S, 1, w});
                         checked_set(H, tH, not_a_hour, is);
                         checked_set(M, tM, not_a_minute, is);
-                        checked_set(s, round<Duration>(duration<long double>{S}),
+                        checked_set(s, round_i<Duration>(duration<long double>{S}),
                                     not_a_second, is);
 #endif
                     }
                     else
                         read(is, CharT{'%'}, width, modified, *fmt);
                     command = nullptr;
                     width = -1;
@@ -6914,15 +7162,15 @@
                         else if (tm.tm_hour == 13)
                             tp = 1;
                         else
                             is.setstate(err);
 #else
                         auto nm = detail::ampm_names();
                         auto i = detail::scan_keyword(is, nm.first, nm.second) - nm.first;
-                        tp = i;
+                        tp = static_cast<decltype(tp)>(i);
 #endif
                         checked_set(p, tp, not_a_ampm, is);
                     }
                     else
                         read(is, CharT{'%'}, width, modified, *fmt);
                     command = nullptr;
                     width = -1;
@@ -6955,15 +7203,15 @@
                         long double S;
                         int tI = not_a_hour_12_value;
                         int tM = not_a_minute;
                         read(is, ru{tI, 1, 2}, CharT{':'}, ru{tM, 1, 2},
                                                CharT{':'}, rld{S, 1, w});
                         checked_set(I, tI, not_a_hour_12_value, is);
                         checked_set(M, tM, not_a_minute, is);
-                        checked_set(s, round<Duration>(duration<long double>{S}),
+                        checked_set(s, round_i<Duration>(duration<long double>{S}),
                                     not_a_second, is);
                         ws(is);
                         auto nm = detail::ampm_names();
                         auto i = detail::scan_keyword(is, nm.first, nm.second) - nm.first;
                         checked_set(p, static_cast<int>(i), not_a_ampm, is);
 #endif
                     }
@@ -7006,15 +7254,15 @@
                    if (modified != CharT{'E'})
 #endif
                     {
                         using dfs = detail::decimal_format_seconds<Duration>;
                         CONSTDATA auto w = Duration::period::den == 1 ? 2 : 3 + dfs::width;
                         long double S;
                         read(is, rld{S, 1, width == -1 ? w : static_cast<unsigned>(width)});
-                        checked_set(s, round<Duration>(duration<long double>{S}),
+                        checked_set(s, round_i<Duration>(duration<long double>{S}),
                                     not_a_second, is);
                     }
 #if !ONLY_C_LOCALE
                     else if (modified == CharT{'O'})
                     {
                         ios::iostate err = ios::goodbit;
                         f.get(is, nullptr, is, err, &tm, command, fmt+1);
@@ -7043,15 +7291,15 @@
                         int tH = not_a_hour;
                         int tM = not_a_minute;
                         long double S;
                         read(is, ru{tH, 1, 2}, CharT{':'}, ru{tM, 1, 2},
                                                CharT{':'}, rld{S, 1, w});
                         checked_set(H, tH, not_a_hour, is);
                         checked_set(M, tM, not_a_minute, is);
-                        checked_set(s, round<Duration>(duration<long double>{S}),
+                        checked_set(s, round_i<Duration>(duration<long double>{S}),
                                     not_a_second, is);
                     }
                     else
                         read(is, CharT{'%'}, width, modified, *fmt);
                     command = nullptr;
                     width = -1;
                     modified = CharT{};
@@ -7746,40 +7994,42 @@
 template <class Duration, class CharT, class Traits, class Alloc = std::allocator<CharT>>
 std::basic_istream<CharT, Traits>&
 from_stream(std::basic_istream<CharT, Traits>& is, const CharT* fmt,
             sys_time<Duration>& tp, std::basic_string<CharT, Traits, Alloc>* abbrev = nullptr,
             std::chrono::minutes* offset = nullptr)
 {
     using CT = typename std::common_type<Duration, std::chrono::seconds>::type;
+    using detail::round_i;
     std::chrono::minutes offset_local{};
     auto offptr = offset ? offset : &offset_local;
     fields<CT> fds{};
     fds.has_tod = true;
     from_stream(is, fmt, fds, abbrev, offptr);
     if (!fds.ymd.ok() || !fds.tod.in_conventional_range())
         is.setstate(std::ios::failbit);
     if (!is.fail())
-        tp = round<Duration>(sys_days(fds.ymd) - *offptr + fds.tod.to_duration());
+        tp = round_i<Duration>(sys_days(fds.ymd) - *offptr + fds.tod.to_duration());
     return is;
 }
 
 template <class Duration, class CharT, class Traits, class Alloc = std::allocator<CharT>>
 std::basic_istream<CharT, Traits>&
 from_stream(std::basic_istream<CharT, Traits>& is, const CharT* fmt,
             local_time<Duration>& tp, std::basic_string<CharT, Traits, Alloc>* abbrev = nullptr,
             std::chrono::minutes* offset = nullptr)
 {
     using CT = typename std::common_type<Duration, std::chrono::seconds>::type;
+    using detail::round_i;
     fields<CT> fds{};
     fds.has_tod = true;
     from_stream(is, fmt, fds, abbrev, offset);
     if (!fds.ymd.ok() || !fds.tod.in_conventional_range())
         is.setstate(std::ios::failbit);
     if (!is.fail())
-        tp = round<Duration>(local_seconds{local_days(fds.ymd)} + fds.tod.to_duration());
+        tp = round_i<Duration>(local_seconds{local_days(fds.ymd)} + fds.tod.to_duration());
     return is;
 }
 
 template <class Rep, class Period, class CharT, class Traits, class Alloc = std::allocator<CharT>>
 std::basic_istream<CharT, Traits>&
 from_stream(std::basic_istream<CharT, Traits>& is, const CharT* fmt,
             std::chrono::duration<Rep, Period>& d,
```

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/ios.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/ios.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/islamic.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/islamic.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/iso_week.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/iso_week.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/julian.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/julian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1651,17 +1651,20 @@
 CONSTCD11 inline julian::day month_day::day() const NOEXCEPT {return d_;}
 
 CONSTCD14
 inline
 bool
 month_day::ok() const NOEXCEPT
 {
-    CONSTDATA julian::day d[] =
-        {31_d, 29_d, 31_d, 30_d, 31_d, 30_d, 31_d, 31_d, 30_d, 31_d, 30_d, 31_d};
-    return m_.ok() && 1_d <= d_ && d_ <= d[static_cast<unsigned>(m_)-1];
+    CONSTDATA julian::day d[] = { 
+        julian::day(31), julian::day(29), julian::day(31), julian::day(30), 
+        julian::day(31), julian::day(30), julian::day(31), julian::day(31), 
+        julian::day(30), julian::day(31), julian::day(30), julian::day(31) 
+    };
+    return m_.ok() && julian::day(1) <= d_ && d_ <= d[static_cast<unsigned>(m_)-1];
 }
 
 CONSTCD11
 inline
 bool
 operator==(const month_day& x, const month_day& y) NOEXCEPT
 {
@@ -1942,17 +1945,20 @@
 }
 
 CONSTCD14
 inline
 day
 year_month_day_last::day() const NOEXCEPT
 {
-    CONSTDATA julian::day d[] =
-        {31_d, 28_d, 31_d, 30_d, 31_d, 30_d, 31_d, 31_d, 30_d, 31_d, 30_d, 31_d};
-    return month() != feb || !y_.is_leap() ? d[static_cast<unsigned>(month())-1] : 29_d;
+    CONSTDATA julian::day d[] = { 
+        julian::day(31), julian::day(28), julian::day(31), julian::day(30), 
+        julian::day(31), julian::day(30), julian::day(31), julian::day(31), 
+        julian::day(30), julian::day(31), julian::day(30), julian::day(31) 
+    };
+    return month() != feb || !y_.is_leap() ? d[static_cast<unsigned>(month())-1] : julian::day(29);
 }
 
 CONSTCD14
 inline
 year_month_day_last::operator sys_days() const NOEXCEPT
 {
     return sys_days(year()/month()/day());
@@ -2186,15 +2192,15 @@
 CONSTCD14
 inline
 bool
 year_month_day::ok() const NOEXCEPT
 {
     if (!(y_.ok() && m_.ok()))
         return false;
-    return 1_d <= d_ && d_ <= (y_/m_/last).day();
+    return julian::day(1) <= d_ && d_ <= (y_/m_/last).day();
 }
 
 CONSTCD11
 inline
 bool
 operator==(const year_month_day& x, const year_month_day& y) NOEXCEPT
 {
```

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/ptz.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/ptz.h`

 * *Files 18% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 // zoned_time<system_clock::duration, Posix::time_zone> zt{"EST5EDT,M3.2.0,M11.1.0",
 //                                                         system_clock::now()};
 // or:
 //
 // Posix::time_zone tz{"EST5EDT,M3.2.0,M11.1.0"};
 // zoned_time<system_clock::duration, Posix::time_zone> zt{tz, system_clock::now()};
 //
+// If the rule set is missing (everything starting with ','), then the rule is that the
+// alternate offset is never enabled.
+//
 // Note, Posix-style time zones are not recommended for all of the reasons described here:
 // https://stackoverflow.com/tags/timezone/info
 //
 // They are provided here as a non-trivial custom time zone example, and if you really
 // have to have Posix time zones, you're welcome to use this one.
 
 #include "date/tz.h"
@@ -66,15 +69,16 @@
 class rule;
 
 void throw_invalid(const string_t& s, unsigned i, const string_t& message);
 unsigned read_date(const string_t& s, unsigned i, rule& r);
 unsigned read_name(const string_t& s, unsigned i, std::string& name);
 unsigned read_signed_time(const string_t& s, unsigned i, std::chrono::seconds& t);
 unsigned read_unsigned_time(const string_t& s, unsigned i, std::chrono::seconds& t);
-unsigned read_unsigned(const string_t& s, unsigned i,  unsigned limit, unsigned& u);
+unsigned read_unsigned(const string_t& s, unsigned i,  unsigned limit, unsigned& u,
+                       const string_t& message = string_t{});
 
 class rule
 {
     enum {off, J, M, N};
 
     date::month m_;
     date::weekday wd_;
@@ -83,20 +87,47 @@
     std::chrono::duration<std::int32_t> time_ = std::chrono::hours{2};
 
 public:
     rule() : mode_(off) {}
 
     bool ok() const {return mode_ != off;}
     date::local_seconds operator()(date::year y) const;
+    std::string to_string() const;
 
     friend std::ostream& operator<<(std::ostream& os, const rule& r);
     friend unsigned read_date(const string_t& s, unsigned i, rule& r);
+    friend bool operator==(const rule& x, const rule& y);
 };
 
 inline
+bool
+operator==(const rule& x, const rule& y)
+{
+    if (x.mode_ != y.mode_)
+        return false;
+    switch (x.mode_)
+    {
+    case rule::J:
+    case rule::N:
+        return x.n_ == y.n_;
+    case rule::M:
+        return x.m_ == y.m_ && x.n_ == y.n_ && x.wd_ == y.wd_;
+    default:
+        return true;
+    }
+}
+
+inline
+bool
+operator!=(const rule& x, const rule& y)
+{
+    return !(x == y);
+}
+
+inline
 date::local_seconds
 rule::operator()(date::year y) const
 {
     using date::local_days;
     using date::January;
     using date::days;
     using date::last;
@@ -116,14 +147,70 @@
     default:
         assert(!"rule called with bad mode");
     }
     return t;
 }
 
 inline
+std::string
+rule::to_string() const
+{
+    using namespace std::chrono;
+    auto print_offset = [](seconds off)
+        {
+            std::string nm;
+            if (off != hours{2})
+            {
+                date::hh_mm_ss<seconds> offset{off};
+                nm = '/';
+                nm += std::to_string(offset.hours().count());
+                if (offset.minutes() != minutes{0} || offset.seconds() != seconds{0})
+                {
+                    nm += ':';
+                    if (offset.minutes() < minutes{10})
+                        nm += '0';
+                    nm += std::to_string(offset.minutes().count());
+                    if (offset.seconds() != seconds{0})
+                    {
+                        nm += ':';
+                        if (offset.seconds() < seconds{10})
+                            nm += '0';
+                        nm += std::to_string(offset.seconds().count());
+                    }
+                }
+            }
+            return nm;
+        };
+
+    std::string nm;
+    switch (mode_)
+    {
+    case rule::J:
+        nm = 'J';
+        nm += std::to_string(n_);
+        break;
+    case rule::M:
+        nm = 'M';
+        nm += std::to_string(static_cast<unsigned>(m_));
+        nm += '.';
+        nm += std::to_string(n_);
+        nm += '.';
+        nm += std::to_string(wd_.c_encoding());
+        break;
+    case rule::N:
+        nm = std::to_string(n_);
+        break;
+    default:
+        break;
+    }
+    nm += print_offset(time_);
+    return nm;
+}
+
+inline
 std::ostream&
 operator<<(std::ostream& os, const rule& r)
 {
     switch (r.mode_)
     {
     case rule::J:
         os << 'J' << r.n_ << date::format(" %T", r.time_);
@@ -174,17 +261,89 @@
     template <class Duration>
         date::local_time<typename std::common_type<Duration, std::chrono::seconds>::type>
         to_local(date::sys_time<Duration> tp) const;
 
     friend std::ostream& operator<<(std::ostream& os, const time_zone& z);
 
     const time_zone* operator->() const {return this;}
+
+    std::string name() const;
+
+    friend bool operator==(const time_zone& x, const time_zone& y);
+
+private:
+    date::sys_seconds get_start(date::year y) const;
+    date::sys_seconds get_prev_start(date::year y) const;
+    date::sys_seconds get_next_start(date::year y) const;
+    date::sys_seconds get_end(date::year y) const;
+    date::sys_seconds get_prev_end(date::year y) const;
+    date::sys_seconds get_next_end(date::year y) const;
+    date::sys_info contant_offset() const;
 };
 
 inline
+date::sys_seconds
+time_zone::get_start(date::year y) const
+{
+    return date::sys_seconds{(start_rule_(y) - offset_).time_since_epoch()};
+}
+
+inline
+date::sys_seconds
+time_zone::get_prev_start(date::year y) const
+{
+    return date::sys_seconds{(start_rule_(--y) - offset_).time_since_epoch()};
+}
+
+inline
+date::sys_seconds
+time_zone::get_next_start(date::year y) const
+{
+    return date::sys_seconds{(start_rule_(++y) - offset_).time_since_epoch()};
+}
+
+inline
+date::sys_seconds
+time_zone::get_end(date::year y) const
+{
+    return date::sys_seconds{(end_rule_(y) - (offset_ + save_)).time_since_epoch()};
+}
+
+inline
+date::sys_seconds
+time_zone::get_prev_end(date::year y) const
+{
+    return date::sys_seconds{(end_rule_(--y) - (offset_ + save_)).time_since_epoch()};
+}
+
+inline
+date::sys_seconds
+time_zone::get_next_end(date::year y) const
+{
+    return date::sys_seconds{(end_rule_(++y) - (offset_ + save_)).time_since_epoch()};
+}
+
+date::sys_info
+time_zone::contant_offset() const
+{
+    using date::year;
+    using date::sys_info;
+    using date::sys_days;
+    using date::January;
+    using date::December;
+    using date::last;
+    sys_info r;
+    r.begin = sys_days{year::min()/January/1};
+    r.end   = sys_days{year::max()/December/last};
+    r.abbrev = std_abbrev_;
+    r.offset = offset_;
+    return r;
+}
+
+inline
 time_zone::time_zone(const detail::string_t& s)
 {
     using detail::read_name;
     using detail::read_signed_time;
     using detail::throw_invalid;
     auto i = read_name(s, 0, std_abbrev_);
     i = read_signed_time(s, i, offset_);
@@ -218,161 +377,166 @@
 
 template <class Duration>
 date::sys_info
 time_zone::get_info(date::sys_time<Duration> st) const
 {
     using date::sys_info;
     using date::year_month_day;
-    using date::sys_seconds;
     using date::sys_days;
     using date::floor;
     using date::ceil;
     using date::days;
-    using date::years;
     using date::year;
     using date::January;
     using date::December;
     using date::last;
     using std::chrono::minutes;
     sys_info r{};
     r.offset = offset_;
     if (start_rule_.ok())
     {
         auto y = year_month_day{floor<days>(st)}.year();
-        auto start = sys_seconds{(start_rule_(y) - offset_).time_since_epoch()};
-        auto end   = sys_seconds{(end_rule_(y) - (offset_ + save_)).time_since_epoch()};
-        if (start <= st && st < end)
-        {
-            r.begin = start;
-            r.end = end;
-            r.offset += save_;
-            r.save = ceil<minutes>(save_);
-            r.abbrev = dst_abbrev_;
-        }
-        else if (st < start)
+        auto start = get_start(y);
+        auto end   = get_end(y);
+        if (start <= end)  // (northern hemisphere)
         {
-            r.begin = sys_seconds{(end_rule_(y-years{1}) -
-                                   (offset_ + save_)).time_since_epoch()};
-            r.end = start;
-            r.abbrev = std_abbrev_;
+            if (start <= st && st < end)
+            {
+                r.begin = start;
+                r.end = end;
+                r.offset += save_;
+                r.save = ceil<minutes>(save_);
+                r.abbrev = dst_abbrev_;
+            }
+            else if (st < start)
+            {
+                r.begin = get_prev_end(y);
+                r.end = start;
+                r.abbrev = std_abbrev_;
+            }
+            else  // st >= end
+            {
+                r.begin = end;
+                r.end = get_next_start(y);
+                r.abbrev = std_abbrev_;
+            }
         }
-        else  // st >= end
+        else  // end < start (southern hemisphere)
         {
-            r.begin = end;
-            r.end = sys_seconds{(start_rule_(y+years{1}) - offset_).time_since_epoch()};
-            r.abbrev = std_abbrev_;
+            if (end <= st && st < start)
+            {
+                r.begin = end;
+                r.end = start;
+                r.abbrev = std_abbrev_;
+            }
+            else if (st < end)
+            {
+                r.begin = get_prev_start(y);
+                r.end = end;
+                r.offset += save_;
+                r.save = ceil<minutes>(save_);
+                r.abbrev = dst_abbrev_;
+            }
+            else  // st >= start
+            {
+                r.begin = start;
+                r.end = get_next_end(y);
+                r.offset += save_;
+                r.save = ceil<minutes>(save_);
+                r.abbrev = dst_abbrev_;
+            }
         }
     }
-    else  //  constant offset
-    {
-        r.begin = sys_days{year::min()/January/1};
-        r.end   = sys_days{year::max()/December/last};
-        r.abbrev = std_abbrev_;
-    }
+    else
+        r = contant_offset();
     return r;
 }
 
 template <class Duration>
 date::local_info
 time_zone::get_info(date::local_time<Duration> tp) const
 {
     using date::local_info;
     using date::year_month_day;
     using date::days;
     using date::sys_days;
     using date::sys_seconds;
-    using date::years;
     using date::year;
     using date::ceil;
     using date::January;
     using date::December;
     using date::last;
     using std::chrono::seconds;
     using std::chrono::minutes;
     local_info r{};
     using date::floor;
     if (start_rule_.ok())
     {
         auto y = year_month_day{floor<days>(tp)}.year();
-        auto start = sys_seconds{(start_rule_(y) - offset_).time_since_epoch()};
-        auto end   = sys_seconds{(end_rule_(y) - (offset_ + save_)).time_since_epoch()};
+        auto start = get_start(y);
+        auto end   = get_end(y);
         auto utcs = sys_seconds{floor<seconds>(tp - offset_).time_since_epoch()};
         auto utcd = sys_seconds{floor<seconds>(tp - (offset_ + save_)).time_since_epoch()};
+        auto northern = start <= end;
         if ((utcs < start) != (utcd < start))
         {
-            r.first.begin = sys_seconds{(end_rule_(y-years{1}) -
-                                         (offset_ + save_)).time_since_epoch()};
+            if (northern)
+                r.first.begin = get_prev_end(y);
+            else
+                r.first.begin = end;
             r.first.end = start;
             r.first.offset = offset_;
             r.first.abbrev = std_abbrev_;
             r.second.begin = start;
-            r.second.end = end;
+            if (northern)
+                r.second.end = end;
+            else
+                r.second.end = get_next_end(y);
             r.second.abbrev = dst_abbrev_;
             r.second.offset = offset_ + save_;
             r.second.save = ceil<minutes>(save_);
             r.result = save_ > seconds{0} ? local_info::nonexistent
                                           : local_info::ambiguous;
         }
         else if ((utcs < end) != (utcd < end))
         {
-            r.first.begin = start;
+            if (northern)
+                r.first.begin = start;
+            else
+                r.first.begin = get_prev_start(y);
             r.first.end = end;
             r.first.offset = offset_ + save_;
             r.first.save = ceil<minutes>(save_);
             r.first.abbrev = dst_abbrev_;
             r.second.begin = end;
-            r.second.end = sys_seconds{(start_rule_(y+years{1}) -
-                                        offset_).time_since_epoch()};
+            if (northern)
+                r.second.end = get_next_start(y);
+            else
+                r.second.end = start;
             r.second.abbrev = std_abbrev_;
             r.second.offset = offset_;
             r.result = save_ > seconds{0} ? local_info::ambiguous
                                           : local_info::nonexistent;
         }
-        else if (utcs < start)
-        {
-            r.first.begin = sys_seconds{(end_rule_(y-years{1}) -
-                                   (offset_ + save_)).time_since_epoch()};
-            r.first.end = start;
-            r.first.offset = offset_;
-            r.first.abbrev = std_abbrev_;
-        }
-        else if (utcs < end)
-        {
-            r.first.begin = start;
-            r.first.end = end;
-            r.first.offset = offset_ + save_;
-            r.first.save = ceil<minutes>(save_);
-            r.first.abbrev = dst_abbrev_;
-        }
         else
-        {
-            r.first.begin = end;
-            r.first.end = sys_seconds{(start_rule_(y+years{1}) -
-                                       offset_).time_since_epoch()};
-            r.first.abbrev = std_abbrev_;
-            r.first.offset = offset_;
-        }
-    }
-    else  //  constant offset
-    {
-        r.first.begin = sys_days{year::min()/January/1};
-        r.first.end   = sys_days{year::max()/December/last};
-        r.first.abbrev = std_abbrev_;
-        r.first.offset = offset_;
+            r.first = get_info(utcs);
     }
+    else
+        r.first = contant_offset();
     return r;
 }
 
 template <class Duration>
 date::sys_time<typename std::common_type<Duration, std::chrono::seconds>::type>
 time_zone::to_sys(date::local_time<Duration> tp) const
 {
     using date::local_info;
     using date::sys_time;
     using date::ambiguous_local_time;
+    using date::nonexistent_local_time;
     auto i = get_info(tp);
     if (i.result == local_info::nonexistent)
         throw nonexistent_local_time(tp, i);
     else if (i.result == local_info::ambiguous)
         throw ambiguous_local_time(tp, i);
     return sys_time<Duration>{tp.time_since_epoch()} - i.first.offset;
 }
@@ -415,27 +579,93 @@
     using date::operator<<;
     os << '{';
     os << z.std_abbrev_ << ", " << z.dst_abbrev_ << date::format(", %T, ", z.offset_)
        << date::format("%T, [", z.save_) << z.start_rule_ << ", " << z.end_rule_ << ")}";
     return os;
 }
 
+inline
+std::string
+time_zone::name() const
+{
+    using namespace date;
+    using namespace std::chrono;
+    auto nm = std_abbrev_;
+    auto print_offset = [](seconds off)
+        {
+            std::string nm;
+            hh_mm_ss<seconds> offset{-off};
+            if (offset.is_negative())
+                nm += '-';
+            nm += std::to_string(offset.hours().count());
+            if (offset.minutes() != minutes{0} || offset.seconds() != seconds{0})
+            {
+                nm += ':';
+                if (offset.minutes() < minutes{10})
+                    nm += '0';
+                nm += std::to_string(offset.minutes().count());
+                if (offset.seconds() != seconds{0})
+                {
+                    nm += ':';
+                    if (offset.seconds() < seconds{10})
+                        nm += '0';
+                    nm += std::to_string(offset.seconds().count());
+                }
+            }
+            return nm;
+        };
+    nm += print_offset(offset_);
+    if (!dst_abbrev_.empty())
+    {
+        nm += dst_abbrev_;
+        if (save_ != hours{1})
+            nm += print_offset(offset_+save_);
+        if (start_rule_.ok())
+        {
+            nm += ',';
+            nm += start_rule_.to_string();
+            nm += ',';
+            nm += end_rule_.to_string();
+        }
+    }
+    return nm;
+}
+
+inline
+bool
+operator==(const time_zone& x, const time_zone& y)
+{
+    return x.std_abbrev_ == y.std_abbrev_ &&
+           x.dst_abbrev_ == y. dst_abbrev_ &&
+           x.offset_ == y.offset_ &&
+           x.save_ == y.save_ &&
+           x.start_rule_ == y.start_rule_ &&
+           x.end_rule_ == y.end_rule_;
+}
+
+inline
+bool
+operator!=(const time_zone& x, const time_zone& y)
+{
+    return !(x == y);
+}
+
 namespace detail
 {
 
 inline
 void
 throw_invalid(const string_t& s, unsigned i, const string_t& message)
 {
     throw std::runtime_error(std::string("Invalid time_zone initializer.\n") +
                              std::string(message) + ":\n" +
                              std::string(s) + '\n' +
                              "\x1b[1;32m" +
                              std::string(i, '~') + '^' +
-                             std::string(s.size()-i-1, '~') +
+                             std::string(i < s.size() ? s.size()-i-1 : 0, '~') +
                              "\x1b[0m");
 }
 
 inline
 unsigned
 read_date(const string_t& s, unsigned i, rule& r)
 {
@@ -443,33 +673,33 @@
     using date::weekday;
     if (i == s.size())
         throw_invalid(s, i, "Expected rule but found end of string");
     if (s[i] == 'J')
     {
         ++i;
         unsigned n;
-        i = read_unsigned(s, i, 3, n);
+        i = read_unsigned(s, i, 3, n, "Expected to find the Julian day [1, 365]");
         r.mode_ = rule::J;
         r.n_ = n;
     }
     else if (s[i] == 'M')
     {
         ++i;
         unsigned m;
-        i = read_unsigned(s, i, 2, m);
+        i = read_unsigned(s, i, 2, m, "Expected to find month [1, 12]");
         if (i == s.size() || s[i] != '.')
             throw_invalid(s, i, "Expected '.' after month");
         ++i;
         unsigned n;
-        i = read_unsigned(s, i, 1, n);
+        i = read_unsigned(s, i, 1, n, "Expected to find week number [1, 5]");
         if (i == s.size() || s[i] != '.')
             throw_invalid(s, i, "Expected '.' after weekday index");
         ++i;
         unsigned wd;
-        i = read_unsigned(s, i, 1, wd);
+        i = read_unsigned(s, i, 1, wd, "Expected to find day of week [0, 6]");
         r.mode_ = rule::M;
         r.m_ = month{m};
         r.wd_ = weekday{wd};
         r.n_ = n;
     }
     else if (std::isdigit(s[i]))
     {
@@ -551,37 +781,38 @@
 {
     using std::chrono::seconds;
     using std::chrono::minutes;
     using std::chrono::hours;
     if (i == s.size())
         throw_invalid(s, i, "Expected to read unsigned time, but found end of string");
     unsigned x;
-    i = read_unsigned(s, i, 2, x);
+    i = read_unsigned(s, i, 2, x, "Expected to find hours [0, 24]");
     t = hours{x};
     if (i != s.size() && s[i] == ':')
     {
         ++i;
-        i = read_unsigned(s, i, 2, x);
+        i = read_unsigned(s, i, 2, x, "Expected to find minutes [0, 59]");
         t += minutes{x};
         if (i != s.size() && s[i] == ':')
         {
             ++i;
-            i = read_unsigned(s, i, 2, x);
+            i = read_unsigned(s, i, 2, x, "Expected to find seconds [0, 59]");
             t += seconds{x};
         }
     }
     return i;
 }
 
 inline
 unsigned
-read_unsigned(const string_t& s, unsigned i, unsigned limit, unsigned& u)
+read_unsigned(const string_t& s, unsigned i, unsigned limit, unsigned& u,
+              const string_t& message)
 {
     if (i == s.size() || !std::isdigit(s[i]))
-        throw_invalid(s, i, "Expected to find a decimal digit");
+        throw_invalid(s, i, message);
     u = static_cast<unsigned>(s[i] - '0');
     unsigned count = 1;
     for (++i; count < limit && i != s.size() && std::isdigit(s[i]); ++i, ++count)
         u = u * 10 + static_cast<unsigned>(s[i] - '0');
     return i;
 }
```

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/solar_hijri.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/solar_hijri.h`

 * *Files 2% similar despite different names*

```diff
@@ -1703,17 +1703,21 @@
 CONSTCD11 inline solar_hijri::day month_day::day() const NOEXCEPT {return d_;}
 
 CONSTCD14
 inline
 bool
 month_day::ok() const NOEXCEPT
 {
-    CONSTDATA solar_hijri::day d[] =
-        {31_d, 31_d, 31_d, 31_d, 31_d, 31_d, 30_d, 30_d, 30_d, 30_d, 30_d, 30_d};
-    return m_.ok() && 1_d <= d_ && d_ <= d[static_cast<unsigned>(m_)-1];
+    CONSTDATA solar_hijri::day d[] = { 
+        solar_hijri::day(31), solar_hijri::day(31), solar_hijri::day(31), 
+        solar_hijri::day(31), solar_hijri::day(31), solar_hijri::day(31), 
+        solar_hijri::day(30), solar_hijri::day(30), solar_hijri::day(30), 
+        solar_hijri::day(30), solar_hijri::day(30), solar_hijri::day(30) 
+    };
+    return m_.ok() && solar_hijri::day(1) <= d_ && d_ <= d[static_cast<unsigned>(m_)-1];
 }
 
 CONSTCD11
 inline
 bool
 operator==(const month_day& x, const month_day& y) NOEXCEPT
 {
@@ -1994,18 +1998,22 @@
 }
 
 CONSTCD14
 inline
 day
 year_month_day_last::day() const NOEXCEPT
 {
-    CONSTDATA solar_hijri::day d[] =
-        {31_d, 31_d, 31_d, 31_d, 31_d, 31_d, 30_d, 30_d, 30_d, 30_d, 30_d, 29_d};
+    CONSTDATA solar_hijri::day d[] = { 
+        solar_hijri::day(31), solar_hijri::day(31), solar_hijri::day(31), 
+        solar_hijri::day(31), solar_hijri::day(31), solar_hijri::day(31), 
+        solar_hijri::day(30), solar_hijri::day(30), solar_hijri::day(30), 
+        solar_hijri::day(30), solar_hijri::day(30), solar_hijri::day(29) 
+    };
     return month() != esf || !y_.is_leap() ?
-        d[static_cast<unsigned>(month())-1] : 30_d;
+        d[static_cast<unsigned>(month()) - 1] : solar_hijri::day(30);
 }
 
 CONSTCD14
 inline
 year_month_day_last::operator sys_days() const NOEXCEPT
 {
     return sys_days(year()/month()/day());
@@ -2256,15 +2264,15 @@
 CONSTCD14
 inline
 bool
 year_month_day::ok() const NOEXCEPT
 {
     if (!(y_.ok() && m_.ok()))
         return false;
-    return 1_d <= d_ && d_ <= (y_/m_/last).day();
+    return solar_hijri::day(1) <= d_ && d_ <= (y_/m_/last).day();
 }
 
 CONSTCD11
 inline
 bool
 operator==(const year_month_day& x, const year_month_day& y) NOEXCEPT
 {
```

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/tz.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/tz.h`

 * *Files 2% similar despite different names*

```diff
@@ -82,23 +82,14 @@
 #  define USE_SHELL_API 1
 #endif
 
 #if USE_OS_TZDB
 #  ifdef _WIN32
 #    error "USE_OS_TZDB can not be used on Windows"
 #  endif
-#  ifndef MISSING_LEAP_SECONDS
-#    ifdef __APPLE__
-#      define MISSING_LEAP_SECONDS 1
-#    else
-#      define MISSING_LEAP_SECONDS 0
-#    endif
-#  endif
-#else
-#  define MISSING_LEAP_SECONDS 0
 #endif
 
 #ifndef HAS_DEDUCTION_GUIDES
 #  if __cplusplus >= 201703
 #    define HAS_DEDUCTION_GUIDES 1
 #  else
 #    define HAS_DEDUCTION_GUIDES 0
@@ -699,14 +690,19 @@
     friend
     std::basic_ostream<CharT, Traits>&
     operator<<(std::basic_ostream<CharT, Traits>& os,
                const zoned_time<Duration1, TimeZonePtr1>& t);
 
 private:
     template <class D, class T> friend class zoned_time;
+
+    template <class TimeZonePtr2>
+    static
+    TimeZonePtr2&&
+    check(TimeZonePtr2&& p);
 };
 
 using zoned_seconds = zoned_time<std::chrono::seconds>;
 
 #if HAS_DEDUCTION_GUIDES
 
 namespace detail
@@ -986,16 +982,14 @@
 inline bool operator!=(const time_zone_link& x, const time_zone_link& y) {return !(x == y);}
 inline bool operator> (const time_zone_link& x, const time_zone_link& y) {return   y < x;}
 inline bool operator<=(const time_zone_link& x, const time_zone_link& y) {return !(y < x);}
 inline bool operator>=(const time_zone_link& x, const time_zone_link& y) {return !(x < y);}
 
 #endif  // !USE_OS_TZDB
 
-#if !MISSING_LEAP_SECONDS
-
 class leap_second
 {
 private:
     sys_seconds date_;
 
 public:
 #if USE_OS_TZDB
@@ -1111,16 +1105,14 @@
 operator>=(const sys_time<Duration>& x, const leap_second& y)
 {
     return !(x < y);
 }
 
 using leap = leap_second;
 
-#endif  // !MISSING_LEAP_SECONDS
-
 #ifdef _WIN32
 
 namespace detail
 {
 
 // The time zone mapping is modelled after this data file:
 // http://unicode.org/repos/cldr/trunk/common/supplemental/windowsZones.xml
@@ -1158,17 +1150,15 @@
 struct tzdb
 {
     std::string                 version = "unknown";
     std::vector<time_zone>      zones;
 #if !USE_OS_TZDB
     std::vector<time_zone_link> links;
 #endif
-#if !MISSING_LEAP_SECONDS
     std::vector<leap_second>    leap_seconds;
-#endif
 #if !USE_OS_TZDB
     std::vector<detail::Rule>   rules;
 #endif
 #ifdef _WIN32
     std::vector<detail::timezone_mapping> mappings;
 #endif
     tzdb* next = nullptr;
@@ -1217,91 +1207,91 @@
 class tzdb_list
 {
     std::atomic<tzdb*> head_{nullptr};
 
 public:
     ~tzdb_list();
     tzdb_list() = default;
-    tzdb_list(tzdb_list&& x) noexcept;
+    tzdb_list(tzdb_list&& x) NOEXCEPT;
 
-    const tzdb& front() const noexcept {return *head_;}
-          tzdb& front()       noexcept {return *head_;}
+    const tzdb& front() const NOEXCEPT {return *head_;}
+          tzdb& front()       NOEXCEPT {return *head_;}
 
     class const_iterator;
 
-    const_iterator begin() const noexcept;
-    const_iterator end() const noexcept;
+    const_iterator begin() const NOEXCEPT;
+    const_iterator end() const NOEXCEPT;
 
-    const_iterator cbegin() const noexcept;
-    const_iterator cend() const noexcept;
+    const_iterator cbegin() const NOEXCEPT;
+    const_iterator cend() const NOEXCEPT;
 
-    const_iterator erase_after(const_iterator p) noexcept;
+    const_iterator erase_after(const_iterator p) NOEXCEPT;
 
     struct undocumented_helper;
 private:
-    void push_front(tzdb* tzdb) noexcept;
+    void push_front(tzdb* tzdb) NOEXCEPT;
 };
 
 class tzdb_list::const_iterator
 {
     tzdb* p_ = nullptr;
 
-    explicit const_iterator(tzdb* p) noexcept : p_{p} {}
+    explicit const_iterator(tzdb* p) NOEXCEPT : p_{p} {}
 public:
     const_iterator() = default;
 
     using iterator_category = std::forward_iterator_tag;
     using value_type        = tzdb;
     using reference         = const value_type&;
     using pointer           = const value_type*;
     using difference_type   = std::ptrdiff_t;
 
-    reference operator*() const noexcept {return *p_;}
-    pointer  operator->() const noexcept {return p_;}
+    reference operator*() const NOEXCEPT {return *p_;}
+    pointer  operator->() const NOEXCEPT {return p_;}
 
-    const_iterator& operator++() noexcept {p_ = p_->next; return *this;}
-    const_iterator  operator++(int) noexcept {auto t = *this; ++(*this); return t;}
+    const_iterator& operator++() NOEXCEPT {p_ = p_->next; return *this;}
+    const_iterator  operator++(int) NOEXCEPT {auto t = *this; ++(*this); return t;}
 
     friend
     bool
-    operator==(const const_iterator& x, const const_iterator& y) noexcept
+    operator==(const const_iterator& x, const const_iterator& y) NOEXCEPT
         {return x.p_ == y.p_;}
 
     friend
     bool
-    operator!=(const const_iterator& x, const const_iterator& y) noexcept
+    operator!=(const const_iterator& x, const const_iterator& y) NOEXCEPT
         {return !(x == y);}
 
     friend class tzdb_list;
 };
 
 inline
 tzdb_list::const_iterator
-tzdb_list::begin() const noexcept
+tzdb_list::begin() const NOEXCEPT
 {
     return const_iterator{head_};
 }
 
 inline
 tzdb_list::const_iterator
-tzdb_list::end() const noexcept
+tzdb_list::end() const NOEXCEPT
 {
     return const_iterator{nullptr};
 }
 
 inline
 tzdb_list::const_iterator
-tzdb_list::cbegin() const noexcept
+tzdb_list::cbegin() const NOEXCEPT
 {
     return begin();
 }
 
 inline
 tzdb_list::const_iterator
-tzdb_list::cend() const noexcept
+tzdb_list::cend() const NOEXCEPT
 {
     return end();
 }
 
 DATE_API tzdb_list& get_tzdb_list();
 
 #if !USE_OS_TZDB
@@ -1324,54 +1314,66 @@
 
 namespace detail
 {
 
 template <class T>
 inline
 T*
-to_raw_pointer(T* p) noexcept
+to_raw_pointer(T* p) NOEXCEPT
 {
     return p;
 }
 
 template <class Pointer>
 inline
 auto
-to_raw_pointer(Pointer p) noexcept
+to_raw_pointer(Pointer p) NOEXCEPT
     -> decltype(detail::to_raw_pointer(p.operator->()))
 {
     return detail::to_raw_pointer(p.operator->());
 }
 
 }  // namespace detail
 
 template <class Duration, class TimeZonePtr>
+template <class TimeZonePtr2>
+inline
+TimeZonePtr2&&
+zoned_time<Duration, TimeZonePtr>::check(TimeZonePtr2&& p)
+{
+    if (detail::to_raw_pointer(p) == nullptr)
+        throw std::runtime_error(
+            "zoned_time constructed with a time zone pointer == nullptr");
+    return std::forward<TimeZonePtr2>(p);
+}
+
+template <class Duration, class TimeZonePtr>
 #if !defined(_MSC_VER) || (_MSC_VER > 1916)
 template <class T, class>
 #endif
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time()
-    : zone_(zoned_traits<TimeZonePtr>::default_zone())
+    : zone_(check(zoned_traits<TimeZonePtr>::default_zone()))
     {}
 
 template <class Duration, class TimeZonePtr>
 #if !defined(_MSC_VER) || (_MSC_VER > 1916)
 template <class T, class>
 #endif
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time(const sys_time<Duration>& st)
-    : zone_(zoned_traits<TimeZonePtr>::default_zone())
+    : zone_(check(zoned_traits<TimeZonePtr>::default_zone()))
     , tp_(st)
     {}
 
 template <class Duration, class TimeZonePtr>
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time(TimeZonePtr z)
-    : zone_(std::move(z))
-    {assert(detail::to_raw_pointer(zone_) != nullptr);}
+    : zone_(check(std::move(z)))
+    {}
 
 #if HAS_STRING_VIEW
 
 template <class Duration, class TimeZonePtr>
 template <class T, class>
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time(std::string_view name)
@@ -1398,45 +1400,45 @@
     : zone_(zt.zone_)
     , tp_(zt.tp_)
     {}
 
 template <class Duration, class TimeZonePtr>
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time(TimeZonePtr z, const sys_time<Duration>& st)
-    : zone_(std::move(z))
+    : zone_(check(std::move(z)))
     , tp_(st)
     {}
 
 template <class Duration, class TimeZonePtr>
 #if !defined(_MSC_VER) || (_MSC_VER > 1916)
 template <class T, class>
 #endif
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time(TimeZonePtr z, const local_time<Duration>& t)
-    : zone_(std::move(z))
+    : zone_(check(std::move(z)))
     , tp_(zone_->to_sys(t))
     {}
 
 template <class Duration, class TimeZonePtr>
 #if !defined(_MSC_VER) || (_MSC_VER > 1916)
 template <class T, class>
 #endif
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time(TimeZonePtr z, const local_time<Duration>& t,
                                               choose c)
-    : zone_(std::move(z))
+    : zone_(check(std::move(z)))
     , tp_(zone_->to_sys(t, c))
     {}
 
 template <class Duration, class TimeZonePtr>
 template <class Duration2, class TimeZonePtr2, class>
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time(TimeZonePtr z,
                                               const zoned_time<Duration2, TimeZonePtr2>& zt)
-    : zone_(std::move(z))
+    : zone_(check(std::move(z)))
     , tp_(zt.tp_)
     {}
 
 template <class Duration, class TimeZonePtr>
 template <class Duration2, class TimeZonePtr2, class>
 inline
 zoned_time<Duration, TimeZonePtr>::zoned_time(TimeZonePtr z,
@@ -1843,16 +1845,14 @@
 std::basic_ostream<CharT, Traits>&
 operator<<(std::basic_ostream<CharT, Traits>& os, const zoned_time<Duration, TimeZonePtr>& t)
 {
     const CharT fmt[] = {'%', 'F', ' ', '%', 'T', ' ', '%', 'Z', CharT{}};
     return to_stream(os, fmt, t);
 }
 
-#if !MISSING_LEAP_SECONDS
-
 class utc_clock
 {
 public:
     using duration                  = std::chrono::system_clock::duration;
     using rep                       = duration::rep;
     using period                    = duration::period;
     using time_point                = std::chrono::time_point<utc_clock>;
@@ -2783,12 +2783,10 @@
 inline
 gps_time<typename std::common_type<Duration, std::chrono::seconds>::type>
 to_gps_time(const tai_time<Duration>& t)
 {
     return gps_clock::from_utc(tai_clock::to_utc(t));
 }
 
-#endif  // !MISSING_LEAP_SECONDS
-
 }  // namespace date
 
 #endif  // TZ_H
```

### Comparing `jotdown-2.0.1/moonlight/deps/date/include/date/tz_private.h` & `jotdown-2.0.2/moonlight/deps/date/include/date/tz_private.h`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,17 @@
 #endif // !defined(_MSC_VER) || (_MSC_VER >= 1900)
 
         U& operator=(const date::month_day& x);
         U& operator=(const date::month_weekday_last& x);
         U& operator=(const pair& x);
     } u;
 
-    std::chrono::hours           h_{};
-    std::chrono::minutes         m_{};
-    std::chrono::seconds         s_{};
+    std::chrono::hours           h_{0};
+    std::chrono::minutes         m_{0};
+    std::chrono::seconds         s_{0};
     tz                           zone_{tz::local};
 
 public:
     MonthDayTime() = default;
     MonthDayTime(local_seconds tp, tz timezone);
     MonthDayTime(const date::month_day& md, tz timezone);
 
@@ -241,15 +241,15 @@
 
     std::string                        format_;
     date::year                         until_year_{0};
     MonthDayTime                       until_date_;
     sys_seconds                        until_utc_;
     local_seconds                      until_std_;
     local_seconds                      until_loc_;
-    std::chrono::minutes               initial_save_{};
+    std::chrono::minutes               initial_save_{0};
     std::string                        initial_abbrev_;
     std::pair<const Rule*, date::year> first_rule_{nullptr, date::year::min()};
     std::pair<const Rule*, date::year> last_rule_{nullptr, date::year::max()};
 
     ~zonelet();
     zonelet();
     zonelet(const zonelet& i);
```

### Comparing `jotdown-2.0.1/moonlight/deps/date/test/tz_test/OffsetZone.h` & `jotdown-2.0.2/moonlight/deps/date/test/tz_test/OffsetZone.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/automata.h` & `jotdown-2.0.2/moonlight/include/moonlight/automata.h`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,24 @@
 #ifndef __MOONLIGHT_AUTOMATA_H
 #define __MOONLIGHT_AUTOMATA_H
 
 #include "moonlight/exceptions.h"
 
 #include <thread>
 #include <future>
+#include <optional>
 #include <map>
 
 namespace moonlight {
 namespace automata {
 
 template<class C, class K> class Lambda;
 
-//-------------------------------------------------------------------
-class Error : public core::Exception {
-   using Exception::Exception;
-};
-
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 template<class S>
 class StateMachine {
 public:
    typedef std::shared_ptr<S> StatePointer;
 
    enum class TraceEvent {
       PUSH,
@@ -65,19 +62,27 @@
       } else {
          return false;
       }
    }
 
    void run_until_complete() {
       if (! current()) {
-         throw Error("StateMachine has no initial state.");
+         THROW(core::UsageError, "StateMachine has no initial state.");
       }
 
-      while (current()) {
-         current()->run();
+      try {
+          while (current()) {
+             current()->run();
+          }
+
+      } catch (...) {
+#ifdef MOONLIGHT_AUTOMATA_DEBUG
+          _trace(TraceEvent::TERMINATE);
+#endif
+          throw;
       }
    }
 
    std::future<void> run() {
       return std::async(std::launch::async, [&] {
          this->run_until_complete();
       });
@@ -119,15 +124,15 @@
    void pop() {
 #ifdef MOONLIGHT_AUTOMATA_DEBUG
       _trace(TraceEvent::POP, stack.size() >= 2 ? stack[stack.size()-2] : nullptr);
 #endif
       try {
          stack.pop_back();
       } catch (...) {
-         throw Error("The stack is empty.");
+         THROW(core::RuntimeError, "The stack is empty.");
       }
    }
 
    StatePointer current() const {
       return current_state();
    }
 
@@ -210,29 +215,30 @@
          }
       }
    }
 #endif
 
    void _call_parent_impl() {
       if (snapshot->size() <= 1) {
-         throw Error("There are no more states on the stack.");
+         THROW(core::RuntimeError, "There are no more states on the stack.");
       }
 
       snapshot->pop_back();
       snapshot->back()->run();
    }
 
 private:
    typename S::Context& context_;
    std::vector<StatePointer> stack;
    std::vector<Tracer> tracers;
    std::optional<std::vector<StatePointer>> snapshot = {};
 };
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 template<class C>
 class State : public std::enable_shared_from_this<State<C>> {
 public:
    typedef C Context;
    typedef StateMachine<State<C>> Machine;
    typedef std::shared_ptr<State<C>> Pointer;
 
@@ -307,15 +313,16 @@
    }
 
    void call_parent() {
       return machine().call_parent();
    }
 };
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 template<class C, class K = std::string>
 class Lambda : public State<C> {
 public:
    class Builder;
    class Machine;
    typedef std::shared_ptr<Lambda<C, K>> Pointer;
    typedef std::function<void(Lambda<C, K>::Machine&)> Impl1;
@@ -364,15 +371,15 @@
       }
 
       Pointer state(const K& name) {
          auto iter = state_map.find(name);
          if (iter != state_map.end()) {
             return iter->second;
          } else {
-            throw Error(str::cat("Unknown state: ", name));
+            THROW(core::UsageError, str::cat("Undefined state: ", name));
          }
       }
 
       Pointer current() {
          return std::static_pointer_cast<Lambda<C, K>>(this->current_state());
       }
 
@@ -461,17 +468,17 @@
 
    static Builder builder(C& context) {
       return Builder(context);
    }
 
    void run() override {
       if (this->machine_ == nullptr) {
-         throw Error("Machine not injected into LambdaState. "
-                     "This is a bug in the state machine code.");
+          THROW(core::FrameworkError, "Machine not injected into LambdaState.");
       }
+
       if (impl1) {
          impl1.value()(*static_cast<Machine*>(this->machine_));
       } else {
          impl2.value()(*static_cast<Machine*>(this->machine_),
                        std::static_pointer_cast<Lambda<C, K>>(shared_from_this()));
       }
    }
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/cli.h` & `jotdown-2.0.2/moonlight/include/moonlight/cli.h`

 * *Files 10% similar despite different names*

```diff
@@ -19,223 +19,222 @@
 #include <sys/ioctl.h>
 #include <unistd.h>
 #endif
 
 namespace moonlight {
 namespace cli {
 
-/**
+/** -----------------------------------------------------------------
  * Convert argc and argv from main() into a vector of strings.
  */
-std::vector<std::string> argv_to_vector(int argc, char** argv) {
-   std::vector<std::string> vec;
+inline std::vector<std::string> argv_to_vector(int argc, char** argv) {
+    std::vector<std::string> vec;
 
-   for (int x = 0; x < argc; x++) {
-      vec.push_back(std::string(argv[x]));
-   }
+    for (int x = 0; x < argc; x++) {
+        vec.push_back(std::string(argv[x]));
+    }
 
-   return vec;
+    return vec;
 }
 
-//-------------------------------------------------------------------
-std::optional<std::string> getenv(const std::string& name) {
-   const char* value = std::getenv(name.c_str());
-   if (value != nullptr) {
-      return value;
-   } else {
-      return {};
-   }
+/** -----------------------------------------------------------------
+ */
+inline std::optional<std::string> getenv(const std::string& name) {
+    const char* value = std::getenv(name.c_str());
+    if (value != nullptr) {
+        return value;
+    } else {
+        return {};
+    }
 }
 
-//-------------------------------------------------------------------
-class CommandLineException : public core::Exception {
-   using core::Exception::Exception;
-};
-
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 class CommandLine {
 public:
-   CommandLine() { }
-   virtual ~CommandLine() { }
-
-   const std::string& get_program_name() const {
-      return program_name;
-   }
-
-   bool _check(const std::string& flag) const {
-      return collect::contains(flags, flag);
-   }
-
-   template<typename F, typename... FV>
-   bool check(const F& flag, const FV&... flags) {
-      if (_check(flag)) {
-         return true;
-      } else {
-         return check(flags...);
-      }
-   }
-
-   bool check() const {
-      return false;
-   }
-
-   std::optional<const std::string> _get(const std::string& opt) const {
-      if (collect::contains(opts, opt)) {
-         return maps::const_value(opts, opt);
-      } else {
-         return {};
-      }
-   }
-
-   std::optional<const std::string> get() const {
-      return {};
-   }
-
-   template<typename O, typename... OD>
-   std::optional<const std::string> get(const O& opt, const OD&... opts) {
-      auto value = _get(opt);
-      if (value) {
-         return *value;
-      } else {
-         return get(opts...);
-      }
-   }
-
-   template<typename... O>
-   std::string require(const O&... opts) {
-      auto value = get(opts...);
-      if (value) {
-         return *value;
-      } else {
-         throw CommandLineException(str::cat(
-                 std::string("Missing required option "),
-                 str::join(variadic::to_vector(std::string(opts)...), "/")));
-      }
-   }
-
-   const std::vector<std::string>& args() const {
-      return args_;
-   }
-
-   static CommandLine parse(const std::vector<std::string>& argv,
-                            const std::set<std::string>& flag_names = {},
-                            const std::set<std::string>& opt_names = {}) {
-      CommandLine results;
-      results.program_name = argv[0];
-
-      for (unsigned int x = 1; x < argv.size(); x++) {
-         auto& arg = argv[x];
-         if (arg == "--") {
-            // All following args are true args.
-            for (x++; x < argv.size(); x++) {
-               results.args_.push_back(argv[x]);
-            }
+    CommandLine() { }
+    virtual ~CommandLine() { }
 
-         } else if (str::startswith(arg, "--")) {
-            // This is a longopt.
-            auto longopt = slice(arg, 2, {});
-
-            if (collect::contains(longopt, '=')) {
-               // This is a longopt option with a value in the same arg.
-               auto parts = str::split(longopt, "=");
-               auto opt = parts[0];
-               auto value = str::join(slice(parts, 1, {}), "=");
-
-               if (collect::contains(opt_names, opt)) {
-                  results.opts[opt] = value;
-                  results.multi_opts.insert({opt, value});
-
-               } else {
-                  throw CommandLineException(str::cat(
-                     "Unknown option '", opt, "'."
-                  ));
-               }
-
-            } else if (collect::contains(flag_names, longopt)) {
-               // This is a longopt flag.
-               results.flags.insert(longopt);
-
-            } else if (collect::contains(opt_names, longopt)) {
-               // This is a longopt option, the next arg is the opt value.
-               if (x + 1 < argv.size()) {
-                  auto value = argv[++x];
-                  results.opts[longopt] = value;
-                  results.multi_opts.insert({longopt, value});
-
-               } else {
-                  throw CommandLineException(str::cat(
-                     "Missing required value for option '--", longopt, "'."
-                  ));
-               }
+    const std::string& get_program_name() const {
+        return program_name;
+    }
+
+    bool _check(const std::string& flag) const {
+        return collect::contains(flags, flag);
+    }
+
+    template<typename F, typename... FV>
+    bool check(const F& flag, const FV&... flags) {
+        if (_check(flag)) {
+            return true;
+        } else {
+            return check(flags...);
+        }
+    }
+
+    bool check() const {
+        return false;
+    }
+
+    std::optional<const std::string> _get(const std::string& opt) const {
+        if (collect::contains(opts, opt)) {
+            return opts.at(opt);
+        } else {
+            return {};
+        }
+    }
+
+    std::optional<const std::string> get() const {
+        return {};
+    }
+
+    template<typename O, typename... OD>
+    std::optional<const std::string> get(const O& opt, const OD&... opts) {
+        auto value = _get(opt);
+        if (value) {
+            return *value;
+        } else {
+            return get(opts...);
+        }
+    }
+
+    template<typename... O>
+    std::string require(const O&... opts) {
+        auto value = get(opts...);
+        if (value) {
+            return *value;
+        } else {
+            THROW(core::UsageError, str::cat(
+                  std::string("Missing required option "),
+                  str::join(variadic::to_vector(std::string(opts)...), "/")));
+        }
+    }
+
+    const std::vector<std::string>& args() const {
+        return args_;
+    }
+
+    static CommandLine parse(const std::vector<std::string>& argv,
+                             const std::set<std::string>& flag_names = {},
+                             const std::set<std::string>& opt_names = {}) {
+        CommandLine results;
+        results.program_name = argv[0];
+
+        for (unsigned int x = 1; x < argv.size(); x++) {
+            auto& arg = argv[x];
+            if (arg == "--") {
+                // All following args are true args.
+                for (x++; x < argv.size(); x++) {
+                    results.args_.push_back(argv[x]);
+                }
+
+            } else if (str::startswith(arg, "--")) {
+                // This is a longopt.
+                auto longopt = slice(arg, 2, {});
+
+                if (collect::contains(longopt, '=')) {
+                    // This is a longopt option with a value in the same arg.
+                    auto parts = str::split(longopt, "=");
+                    auto opt = parts[0];
+                    auto value = str::join(slice(parts, 1, {}), "=");
+
+                    if (collect::contains(opt_names, opt)) {
+                        results.opts[opt] = value;
+                        results.multi_opts.insert({opt, value});
+
+                    } else {
+                        THROW(core::UsageError, str::cat(
+                            "Unknown option '", opt, "'."
+                        ));
+                    }
+
+                } else if (collect::contains(flag_names, longopt)) {
+                    // This is a longopt flag.
+                    results.flags.insert(longopt);
+
+                } else if (collect::contains(opt_names, longopt)) {
+                    // This is a longopt option, the next arg is the opt value.
+                    if (x + 1 < argv.size()) {
+                        auto value = argv[++x];
+                        results.opts[longopt] = value;
+                        results.multi_opts.insert({longopt, value});
+
+                    } else {
+                        THROW(core::UsageError, str::cat(
+                            "Missing required value for option '--", longopt, "'."
+                        ));
+                    }
+
+                } else {
+                    THROW(core::UsageError, str::cat(
+                        "Unknown flag or option '--", longopt, "'."
+                    ));
+                }
+
+            } else if (str::startswith(arg, "-") && arg.size() > 1) {
+                // This is one or more shortopts.
+                auto shortopts = slice(arg, 1, {});
+                for (unsigned int y = 0; y < shortopts.size(); y++) {
+                    auto shortopt = str::chr(shortopts[y]);
+                    if (collect::contains(flag_names, shortopt)) {
+                        results.flags.insert(shortopt);
+
+                    } else if (collect::contains(opt_names, shortopt)) {
+                        if (y + 1 < shortopts.size()) {
+                            // The rest of shortopts is the opt value.
+                            results.opts.insert(
+                                {shortopt, slice(shortopts, y + 1, {})});
+                            y = shortopts.size();
+
+                        } else if (x + 1 < argv.size()) {
+                            // The next arg is the opt value.
+                            results.opts.insert({shortopt, argv[++x]});
+
+                        } else {
+                            THROW(core::UsageError, str::cat(
+                                "Missing required parameter for '-", shortopt, "'."
+                            ));
+                        }
+                    } else {
+                        THROW(core::UsageError, str::cat(
+                            "Unknown flag or option '-", shortopt, "'."
+                        ));
+                    }
+                }
 
             } else {
-               throw CommandLineException(str::cat(
-                  "Unknown flag or option '--", longopt, "'."
-               ));
+                // This is just a plain old arg.
+                results.args_.push_back(arg);
             }
+        }
 
-         } else if (str::startswith(arg, "-") && arg.size() > 1) {
-            // This is one or more shortopts.
-            auto shortopts = slice(arg, 1, {});
-            for (unsigned int y = 0; y < shortopts.size(); y++) {
-               auto shortopt = str::chr(shortopts[y]);
-               if (collect::contains(flag_names, shortopt)) {
-                  results.flags.insert(shortopt);
-
-               } else if (collect::contains(opt_names, shortopt)) {
-                  if (y + 1 < shortopts.size()) {
-                     // The rest of shortopts is the opt value.
-                     results.opts.insert(
-                         {shortopt, slice(shortopts, y + 1, {})});
-                     y = shortopts.size();
-
-                  } else if (x + 1 < argv.size()) {
-                     // The next arg is the opt value.
-                     results.opts.insert({shortopt, argv[++x]});
-
-                  } else {
-                     throw CommandLineException(str::cat(
-                        "Missing required parameter for '-", shortopt, "'."
-                     ));
-                  }
-               } else {
-                  throw CommandLineException(str::cat(
-                     "Unknown flag or option '-", shortopt, "'."
-                  ));
-               }
-            }
-
-         } else {
-            // This is just a plain old arg.
-            results.args_.push_back(arg);
-         }
-      }
-
-      return results;
-   }
+        return results;
+    }
 
 private:
-   std::string program_name;
-   std::set<std::string> flags;
-   std::map<std::string, int> flag_counts;
-   std::map<std::string, std::string> opts;
-   std::multimap<std::string, std::string> multi_opts;
-   std::vector<std::string> args_;
+    std::string program_name;
+    std::set<std::string> flags;
+    std::map<std::string, int> flag_counts;
+    std::map<std::string, std::string> opts;
+    std::multimap<std::string, std::string> multi_opts;
+    std::vector<std::string> args_;
 };
 
-//-------------------------------------------------------------------
-CommandLine parse(const std::vector<std::string>& argv,
+/** -----------------------------------------------------------------
+ */
+inline CommandLine parse(const std::vector<std::string>& argv,
                   const std::set<std::string>& flag_names = {},
                   const std::set<std::string>& opt_names = {}) {
-   return CommandLine::parse(argv, flag_names, opt_names);
+    return CommandLine::parse(argv, flag_names, opt_names);
 }
 
-//-------------------------------------------------------------------
-CommandLine parse(int argc_in, char** argv_in,
+/** -----------------------------------------------------------------
+ */
+inline CommandLine parse(int argc_in, char** argv_in,
                   const std::set<std::string>& flag_names = {},
                   const std::set<std::string>& opt_names = {}) {
-   return parse(argv_to_vector(argc_in, argv_in), flag_names, opt_names);
+    return parse(argv_to_vector(argc_in, argv_in), flag_names, opt_names);
 }
 }
 }
 
 #endif /* __MOONLIGHT_CLI_H */
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/collect.h` & `jotdown-2.0.2/moonlight/include/moonlight/collect.h`

 * *Files 15% similar despite different names*

```diff
@@ -15,107 +15,113 @@
 #include <map>
 #include <functional>
 #include <memory>
 
 namespace moonlight {
 namespace collect {
 
-//-------------------------------------------------------------------
 template<typename T>
 inline bool contains(const T& coll, const typename T::value_type& v) {
-   return std::find(coll.begin(), coll.end(), v) != coll.end();
+    return std::find(coll.begin(), coll.end(), v) != coll.end();
 }
 
-//-------------------------------------------------------------------
 template<typename T>
 inline bool contains(const std::set<T>& set, const T& v) {
-   return set.find(v) != set.end();
+    return set.find(v) != set.end();
 }
 
-//-------------------------------------------------------------------
 template<typename K, typename V>
 inline bool contains(const std::map<K, V>& map, const K& v) {
-   return map.find(v) != map.end();
+    return map.find(v) != map.end();
 }
 
-//-------------------------------------------------------------------
 template<typename T, typename... TV>
 inline std::vector<typename T::value_type> flatten(const T& coll, const TV&... collections) {
-   std::vector<typename T::value_type> flattened;
-   flatten(flattened, coll, collections...);
-   return flattened;
+    std::vector<typename T::value_type> flattened;
+    flatten(flattened, coll, collections...);
+    return flattened;
 }
 
-//-------------------------------------------------------------------
 template<typename T, typename... TV>
 inline void flatten(std::vector<typename T::value_type>& flattened, const T& coll, const TV&... collections) {
-   for (auto v : coll) {
-      flattened.push_back(v);
-   }
-   flatten(flattened, collections...);
+    for (auto v : coll) {
+        flattened.push_back(v);
+    }
+    flatten(flattened, collections...);
 }
 
-//-------------------------------------------------------------------
 template<typename T>
 inline void flatten(std::vector<T>& flattened) { (void) flattened; }
 
-//-------------------------------------------------------------------
 template<typename T>
 inline T filter(const T& coll, const std::function<bool(typename T::value_type)>& f) {
-   T result;
-   for (auto v : coll) {
-      if (f(v)) {
-         result.push_back(v);
-      }
-   }
-   return result;
+    T result;
+    for (auto v : coll) {
+        if (f(v)) {
+            result.push_back(v);
+        }
+    }
+    return result;
 }
 
-//-------------------------------------------------------------------
 template<typename T>
 inline std::shared_ptr<T> filter(const std::shared_ptr<T>& coll,
                                  const std::function<bool(typename T::value_type)>& f) {
-   return std::make_shared<T>(filter<typename std::shared_ptr<T>::element_type>(*coll, f));
+    return std::make_shared<T>(filter<typename std::shared_ptr<T>::element_type>(*coll, f));
 }
 
-//-------------------------------------------------------------------
 template<typename C1>
 inline C1 sorted(const C1& src) {
-   C1 result;
-   std::copy(src.begin(), src.end(), std::back_inserter(result));
-   std::sort(result.begin(), result.end());
-   return result;
+    C1 result;
+    std::copy(src.begin(), src.end(), std::back_inserter(result));
+    std::sort(result.begin(), result.end());
+    return result;
 }
 
-//-------------------------------------------------------------------
 template<typename C1>
 inline C1 sorted(const C1& src, std::function<bool (const typename C1::value_type& a,
                                                     const typename C1::value_type& b)> comp) {
-   C1 result;
-   std::copy(src.begin(), src.end(), std::back_inserter(result));
-   std::sort(result.begin(), result.end(), comp);
-   return result;
+    C1 result;
+    std::copy(src.begin(), src.end(), std::back_inserter(result));
+    std::sort(result.begin(), result.end(), comp);
+    return result;
 }
 
-//-------------------------------------------------------------------
 template<typename T, typename C1>
 inline std::vector<T> map(const C1& src, std::function<T (const typename C1::value_type&)> f) {
-   std::vector<T> result;
-   for (auto v : src) {
-      result.push_back(f(v));
-   }
-   return result;
+    std::vector<T> result;
+    for (auto v : src) {
+        result.push_back(f(v));
+    }
+    return result;
 }
 
-//-------------------------------------------------------------------
 template<typename C>
 inline std::set<typename C::value_type> set(const C& src) {
-   std::set<typename C::value_type> result;
-   std::copy(src.begin(), src.end(), std::back_inserter(result));
-   return result;
+    std::set<typename C::value_type> result;
+    std::copy(src.begin(), src.end(), std::back_inserter(result));
+    return result;
+}
+
+template<class R, class C1, class C2>
+inline std::vector<R> zip(const C1& srcA, const C2& srcB) {
+    std::vector<R> result;
+    if (srcA.size() >= srcB.size()) {
+        std::transform(srcA.begin(), srcA.end(), srcB.begin(), std::back_inserter(result),
+                       [](const auto& a, const auto& b) {
+                           return R(a, b);
+                       });
+    } else {
+        std::transform(srcB.begin(), srcB.end(), srcA.begin(), std::back_inserter(result),
+                       [](const auto& b, const auto& a) {
+                           return R(a, b);
+                       });
+    }
+
+    return result;
 }
 
 
 }
 }
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/curses.h` & `jotdown-2.0.2/moonlight/include/moonlight/curses.h`

 * *Files 6% similar despite different names*

```diff
@@ -8,92 +8,95 @@
  */
 
 #ifndef __MOONLIGHT_CURSES_H
 #define __MOONLIGHT_CURSES_H
 
 #include "moonlight/exceptions.h"
 #include "moonlight/posix.h"
-#include "tinyformat/tinyformat.h"
 
 #include <climits>
 #include <functional>
 #include <optional>
 
 #include <curses.h>
 #include <panel.h>
 
 namespace moonlight {
 namespace curses {
 
 using moonlight::time::posix::get_ticks;
 
-//-------------------------------------------------------------------
-class CursesError : public core::Exception {
-    using Exception::Exception;
-};
-
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 const int MAX_KEYCODE = 410;
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 struct XY {
     int x;
     int y;
 };
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline XY screen_size() {
     int x, y;
     getmaxyx(stdscr, y, x);
     return {x, y};
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline XY center_on_area(const XY& sz_A, const XY& sz_B) {
     if (sz_A.x > sz_B.x || sz_A.y > sz_B.y) {
-        throw CursesError("Can't center a smaller size inside another.");
+        THROW(core::UsageError, "Can't center a smaller size inside another.");
     }
 
     return {
         (sz_B.x - sz_A.x) / 2,
         (sz_B.y - sz_A.y) / 2
     };
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline XY center_on_screen(const XY& sz) {
     return center_on_area(sz, screen_size());
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline void cleanup() {
     endwin();
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline void init() {
     initscr();
     atexit(cleanup);
     cbreak();
     noecho();
     nodelay(stdscr, true);
     keypad(stdscr, true);
     start_color();
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline void init_color() {
     if (has_colors() == FALSE) {
-        throw CursesError("This terminal does not support color.");
+        THROW(core::UsageError, "This terminal does not support color.");
     }
     start_color();
     use_default_colors();
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline void make_color_pairs() {
     init_pair(0, COLOR_BLACK, -1);
     init_pair(1, COLOR_RED, -1);
     init_pair(2, COLOR_GREEN, -1);
     init_pair(3, COLOR_YELLOW, -1);
     init_pair(4, COLOR_BLUE, -1);
     init_pair(5, COLOR_MAGENTA, -1);
@@ -124,57 +127,64 @@
     init_pair(33, COLOR_WHITE, COLOR_YELLOW);
     init_pair(34, COLOR_WHITE, COLOR_BLUE);
     init_pair(35, COLOR_WHITE, COLOR_MAGENTA);
     init_pair(36, COLOR_WHITE, COLOR_CYAN);
     init_pair(37, COLOR_WHITE, COLOR_BLACK);
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline void init_mouse() {
     mousemask(ALL_MOUSE_EVENTS | REPORT_MOUSE_POSITION, NULL);
     std::cout << "\033[?1003h\n" << std::endl;
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline int get_keycode(const std::string& named_key) {
     for (int x = 0; x <= MAX_KEYCODE; x++) {
         auto name = keyname(x);
         if (name != NULL && name == named_key) {
             return x;
         }
     }
 
     return ERR;
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline std::string get_keycode_name(int keycode) {
     auto name = keyname(keycode);
     return name == nullptr ? "NULL" : name;
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline void dbg_print_all_keycodes() {
     for (int x = 0; x <= MAX_KEYCODE; x++) {
         auto name = keyname(x);
-        tfm::printf("%d\t%s\n", x, name == NULL ? "NULL" : name);
+        std::cout << x << "\t" << (name == NULL ? "NULL" : name) << std::endl;
     }
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline void show_cursor() {
     curs_set(1);
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 inline void hide_cursor() {
     curs_set(0);
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 class Window {
 public:
     Window(XY sz_) :
     Window(sz_, center_on_screen(sz_)) { }
     Window(XY sz_, XY pos_) {
         _window = newwin(sz_.y, sz_.x, pos_.y, pos_.x);
     }
@@ -276,15 +286,16 @@
         wattrset(raw_ptr(), A_NORMAL);
     }
 
 private:
     WINDOW* _window;
 };
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 class Panel : public std::enable_shared_from_this<Panel> {
 public:
     Panel(int x, int y) : Panel(XY({x, y})) { }
 
     Panel(const XY& sz_) : _win(Window(sz_)) {
         init_own_panel();
     }
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/file.h` & `jotdown-2.0.2/moonlight/include/moonlight/file.h`

 * *Files 7% similar despite different names*

```diff
@@ -14,33 +14,28 @@
 #include <fstream>
 #include <cstring>
 
 namespace moonlight {
 namespace file {
 
 //-------------------------------------------------------------------
-class FileException : public core::Exception {
-   using core::Exception::Exception;
-};
-
-//-------------------------------------------------------------------
 inline std::ifstream open_r(const std::string& filename,
                             std::ios::openmode mode = std::ios::in) {
    try {
       std::ifstream infile;
       infile.exceptions(std::ios::failbit);
       infile.open(filename, mode);
       infile.exceptions(std::ios::badbit);
       return infile;
 
    } catch (std::exception& e) {
       std::ostringstream sb;
       sb << "Cannot open file " << filename << " for reading: "
       << strerror(errno);
-      throw FileException(sb.str());
+      THROW(core::RuntimeError, sb.str());
    }
 }
 
 //-------------------------------------------------------------------
 inline std::ofstream open_w(const std::string& filename,
                             std::ios::openmode = std::ios::out) {
    try {
@@ -50,15 +45,15 @@
       outfile.exceptions(std::ios::badbit);
       return outfile;
 
    } catch (std::exception& e) {
       std::ostringstream sb;
       sb << "Cannot open file " << filename << " for writing: "
       << strerror(errno);
-      throw FileException(sb.str());
+      THROW(core::RuntimeError, sb.str());
    }
 }
 
 //-------------------------------------------------------------------
 inline std::fstream open_rw(const std::string& filename,
                             std::ios::openmode mode = std::ios::in | std::ios::out) {
    try {
@@ -68,15 +63,15 @@
       outfile.exceptions(std::ios::badbit);
       return outfile;
 
    } catch (std::exception& e) {
       std::ostringstream sb;
       sb << "Cannot open file " << filename << " for reading and writing: "
       << strerror(errno);
-      throw FileException(sb.str());
+      THROW(core::RuntimeError, sb.str());
    }
 }
 
 //-------------------------------------------------------------------
 inline std::string to_string(std::istream& infile) {
    return std::string(std::istreambuf_iterator<char>(infile), {});
 }
@@ -135,15 +130,17 @@
 
     std::string getline() {
         std::string line;
         for (int x = 1; peek(x) != '\n' && peek(x) != EOF; x++) {
             line.push_back(peek(x));
         }
         advance(line.size());
-        if (peek() == '\n') {
+        if (peek() == EOF) {
+            _exhausted = true;
+        } else if (peek() == '\n') {
             line.push_back(getc());
         }
         return line;
     }
 
     bool is_exhausted() const {
         return _exhausted;
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/generator.h` & `jotdown-2.0.2/moonlight/include/moonlight/color.h`

 * *Files 27% similar despite different names*

```diff
@@ -1,247 +1,249 @@
 /*
- * generator.h
+ * color.h
  *
  * Author: Lain Musgrove (lain.proliant@gmail.com)
- * Date: Tuesday May 26, 2020
+ * Date: Sunday March 14, 2021
+ *
+ * HSV/RGB conversion algorithms adapted from <http://dystopiancode.blogspot.com/2012/06/hsv-rgb-conversion-algorithms-in-c.html>
  *
  * Distributed under terms of the MIT license.
  */
 
-#ifndef __MOONLIGHT_GENERATOR_H
-#define __MOONLIGHT_GENERATOR_H
-
-#include "moonlight/automata.h"
+#ifndef __MOONLIGHT_COLOR_H
+#define __MOONLIGHT_COLOR_H
 
-#include <deque>
-#include <mutex>
-#include <condition_variable>
-#include <future>
-#include <optional>
+#include <cmath>
+#include <ostream>
+#include <regex>
+#include <inttypes.h>
+#include "moonlight/exceptions.h"
 
 namespace moonlight {
-namespace gen {
+namespace color {
+
+/** -----------------------------------------------------------------
+ */
+template<class T>
+bool in_range(T start, T end, T value) {
+    return value >= start && value <= end;
+}
+
+/** -----------------------------------------------------------------
+ */
+struct fRGB;
+struct uRGB;
 
-//-------------------------------------------------------------------
-class Error : public core::Exception {
-   using Exception::Exception;
+struct fHSV {
+    float h;
+    float s;
+    float v;
+
+    explicit operator fRGB() const;
+    explicit operator uRGB() const;
+
+    friend std::ostream& operator<<(std::ostream& out, const fHSV& hsv) {
+        std::ios out_state(nullptr);
+        out_state.copyfmt(out);
+        out << "fHSV<" << std::fixed << std::setprecision(2) <<
+            hsv.h << ", " << hsv.s << ", " << hsv.v << ">";
+        out.copyfmt(out_state);
+        return out;
+    }
+
+    fHSV normalize() const {
+        float hx = fmodf(h, 360.0);
+        if (hx < 0.0) {
+            hx += 360.0;
+        }
+
+        return {
+            hx,
+            fmaxf(fminf(1.0, s), 0.0),
+            fmaxf(fminf(1.0, v), 0.0),
+        };
+    }
 };
 
-//-------------------------------------------------------------------
-// A template allowing the results of a generator lambda, known
-// below as "Closure", to be wrapped in a standard library compatible
-// iterator type and used with constructs like algorithm templates
-// and the ranged-for loop.
-//
-template<class T>
-class Iterator {
-public:
-   typedef std::function<std::optional<T>()> Closure;
-
-   Iterator() : _value({}), _position(-1) { }
-   Iterator(const Closure& closure) : _closure(closure), _value(_closure()) { }
-
-   Iterator<T>& operator++() {
-      if (_value.has_value()) {
-         auto new_value = _closure();
-         if (new_value.has_value()) {
-            _value.emplace(new_value.value());
-            _position ++;
-         } else {
-            _value.reset();
-            _position = -1;
-         }
-      }
-      return *this;
-   }
-
-   Iterator<T> operator++(int) {
-      Iterator iter = *this;
-      ++(*this);
-      return iter;
-   }
-
-   bool operator==(const Iterator<T>& other) {
-      return (_position == -1 && other._position == -1) ||
-         (&_closure == &other._closure && _position == other._position);
-   }
-
-   bool operator==(Iterator<T>& other) {
-      return (_position == -1 && other._position == -1) ||
-         (&_closure == &other._closure && _position == other._position);
-   }
-
-   bool operator!=(const Iterator<T>& other) {
-      return !(*this == other);
-   }
-
-   bool operator!=(Iterator<T>& other) {
-      return !(*this == other);
-   }
-
-   const T& operator*() {
-      if (_value.has_value()) {
-         return *_value;
-      } else {
-         throw Error("Attempted to deference past the end of the sequence.");
-      }
-   }
-
-   using value_type = T;
-   using pointer = const T*;
-   using reference = const T&;
-   using iterator_category = std::forward_iterator_tag;
-
-private:
-   Closure _closure;
-   int _position = 0;
-   std::optional<T> _value;
+/** -----------------------------------------------------------------
+ */
+struct uRGB {
+    unsigned char r;
+    unsigned char g;
+    unsigned char b;
+
+    static uRGB of(unsigned int c) {
+        return {
+            (unsigned char)((c >> 16) & 0xFF),
+            (unsigned char)((c >> 8) & 0xFF),
+            (unsigned char)(c & 0xFF)
+        };
+    }
+
+    static uRGB of(const std::string& s) {
+        std::string sx;
+        if (s.starts_with("#")) {
+            sx = s.substr(1);
+        } else {
+            sx = s;
+        }
+
+        return of(std::stoul(sx, nullptr, 16));
+    }
+
+    static bool is_valid(const std::string& s) {
+        static const std::regex rx("#?[0-9a-fA-F]{6}");
+        return std::regex_match(s, rx);
+    }
+
+    static uRGB validate(const std::string& s) {
+        if (! is_valid(s)) {
+            THROW(core::ValueError, "RGB color string is not valid: " + s);
+        }
+        return of(s);
+    }
+
+    explicit operator fRGB() const;
+    explicit operator fHSV() const;
+
+    explicit operator unsigned int() const {
+        return (r << 16) | (g << 8) | b;
+    }
+
+    bool operator==(const uRGB& rhs) const {
+        return r == rhs.r && g == rhs.g && b == rhs.b;
+    }
+
+    std::string str() const {
+        char buf[16];
+        snprintf(buf, 16u, "#%06" PRIX8, static_cast<unsigned int>(*this));
+        return std::string(buf);
+    }
+
+    friend std::ostream& operator<<(std::ostream& out, const uRGB& rgb) {
+        std::ios out_state(nullptr);
+        out_state.copyfmt(out);
+        out << "uRGB<" << std::hex << rgb.str() << ">";
+        out.copyfmt(out_state);
+        return out;
+    }
 };
 
-//-------------------------------------------------------------------
-// A queue template for asynchronously communicating the output
-// of a generator running in another thread with one or more
-// consumer threads.
-//
-template<class T>
-class Queue {
-public:
-   typedef std::future<std::optional<T>> Future;
-   typedef std::function<void(const T&)> Handler;
-
-   // Indicates that the generator has no more results to provide.
-   void complete() {
-      std::unique_lock<std::mutex> lock(_mutex);
-      _completed = true;
-      lock.unlock();
-      _cv.notify_all();
-   }
-
-   // Called by the generator to yield a result into the queue.
-   void yield(const T& value) {
-      std::unique_lock<std::mutex> lock(_mutex);
-      _yielded_items.push_back(value);
-      lock.unlock();
-      _cv.notify_one();
-   }
-
-   // Called by the consumer to get the next result from the queue.
-   // Blocks until a result is provided, and may return an empty
-   // optional if the generator completes after this method is
-   // called on another thread and there are no more results to
-   // consume.
-   std::optional<T> next() {
-      std::unique_lock<std::mutex> lock(_mutex);
-      _cv.wait(lock, [&]{ return _yielded_items.empty() || _completed; });
-
-      if (_yielded_items.empty() && _completed) {
-         return {};
-      }
-
-      T value = _yielded_items.front();
-      _yielded_items.pop_front();
-      return value;
-   }
-
-   // See above, simply wraps the blocking behavior of `next()`
-   // in an async future.
-   Future async_next() {
-      return std::async(std::launch::async, [&] {
-         return this->next();
-      });
-   }
-
-   // Block until all values from the generator have been consumed
-   // and handled by the given handler callback.
-   void process(Handler handler) {
-      std::optional<T> value;
-      while (value = this->next(), value) {
-         handler(*value);
-      }
-   }
-
-   // Wraps the above `process()` behavior in an async future.
-   std::future<void> process_async(Handler handler) {
-      return std::async(std::launch::async, [&] {
-         std::optional<T> value;
-         while (value = this->next(), value) {
-            handler(*value);
-         }
-      });
-   }
-
-private:
-   std::deque<T> _yielded_items;
-   std::mutex _mutex;
-   std::condition_variable _cv;
-   bool _completed = false;
+/** -----------------------------------------------------------------
+ */
+struct fRGB {
+    float r;
+    float g;
+    float b;
+
+    explicit operator uRGB() const;
+    explicit operator fHSV() const;
+
+    friend std::ostream& operator<<(std::ostream& out, const fRGB& rgb) {
+        std::ios out_state(nullptr);
+        out_state.copyfmt(out);
+        out << "fRGB<" << std::fixed << std::setprecision(2) <<
+            rgb.r << ", " << rgb.g << ", " << rgb.b << ">";
+        out.copyfmt(out_state);
+        return out;
+    }
+
+    fRGB normalize() const {
+        return {
+            fmaxf(fminf(1.0, r), 0.0),
+            fmaxf(fminf(1.0, g), 0.0),
+            fmaxf(fminf(1.0, b), 0.0)
+        };
+    }
 };
 
-//-------------------------------------------------------------------
-// Return the beginning of a virtual range representing the values
-// yielded by the given generator lambda.
-template<class T>
-Iterator<T> begin(std::function<std::optional<T>()> lambda) {
-   return Iterator<T>(lambda);
+/** -----------------------------------------------------------------
+ */
+inline fHSV::operator uRGB() const {
+    return static_cast<uRGB>(static_cast<fRGB>(*this));
 }
 
-//-------------------------------------------------------------------
-// Return the end of a virtual range, any virtual range, of a type.
-template<class T>
-Iterator<T> end() {
-   return Iterator<T>();
+/** -----------------------------------------------------------------
+ */
+inline fHSV::operator fRGB() const {
+    fRGB rgb = { 0.0f, 0.0f, 0.0f };
+    float c = 0.0f, m = 0.0f, x = 0.0f;
+    float hx = fmodf(h, 360.0f);
+    c = v * s;
+    x = c * (1.0f - fabsf(fmodf(hx / 60.0f, 2) - 1.0f));
+    m = v - c;
+    if (hx >= 0.0 && hx < 60.0) {
+        rgb = { c + m, x + m, m };
+    } else if (hx >= 60.0f && hx < 120.0f) {
+        rgb = { x + m, c + m, m };
+    } else if (hx >= 120.0f && hx < 180.0f) {
+        rgb = { m, c + m, x + m };
+    } else if (hx >= 180.f && hx < 240.0f) {
+        rgb = { m, x + m, c + m };
+    } else if (hx >= 240.0f && hx < 300.0f) {
+        rgb = { x + m, m, c + m };
+    } else if (hx >= 300.0 && hx < 360.0) {
+        rgb = { c + m, m, x + m };
+    } else {
+        rgb = { m, m, m };
+    }
+
+    return rgb;
 }
 
-//-------------------------------------------------------------------
-// Returns a queue for processing the results of a generator
-// asynchronously.  The first parameter is a generator factory,
-// any subsequent parameters are forwarded to this factory to produce
-// the generator.
-//
-template<class T, class... TD>
-std::shared_ptr<Queue<T>> async(std::function<std::optional<T>(TD...)> factory, TD... params) {
-
-   std::shared_ptr<Queue<T>> queue = std::make_shared<Queue<T>>();
-   std::async(std::launch::async, [&] {
-      for (auto iter = begin(factory, std::forward(params)...);
-           iter != end<T>();
-           iter++) {
-         queue->yield(*iter);
-      }
-      queue->complete();
-   });
-   return queue;
-}
-
-//-------------------------------------------------------------------
-// Wraps the given set of iterators as a range into a generator.
-//
-template<class I>
-std::function<std::optional<typename I::value_type>()> iterate(I begin, I end) {
-    I current = begin;
-    return [=]() mutable -> std::optional<typename I::value_type> {
-        if (current == end) {
-            return {};
-        } else {
-            return *(current++);
-        }
+/** -----------------------------------------------------------------
+ */
+inline uRGB::operator fRGB() const {
+    return {
+        .r = r / 255.0f,
+        .g = g / 255.0f,
+        .b = b / 255.0f
     };
 }
 
-//-------------------------------------------------------------------
-// Wraps the given set of iterators as a range into a generator,
-// then returns the beginning of a virtual range wrapping that
-// generator.  Use this to reinterpret iterators of any type
-// into virtual iterators.
-//
-template<class I>
-Iterator<typename I::value_type> wrap(I begin_in, I end_in) {
-    if (begin_in == end_in) {
-        return Iterator<typename I::value_type>();
+/** -----------------------------------------------------------------
+ */
+inline uRGB::operator fHSV() const {
+    return static_cast<fHSV>(static_cast<fRGB>(*this));
+}
+
+/** -----------------------------------------------------------------
+ */
+inline fRGB::operator uRGB() const {
+    return {
+        .r = static_cast<unsigned char>(::floor(r * 255.0f)),
+        .g = static_cast<unsigned char>(::floor(g * 255.0f)),
+        .b = static_cast<unsigned char>(::floor(b * 255.0f))
+    };
+}
+
+/** -----------------------------------------------------------------
+ */
+inline fRGB::operator fHSV() const {
+    fHSV hsv = { 0.0f, 0.0f, 0.0f };
+    float M = ::fmaxf(r, ::fmaxf(g, b));
+    float m = ::fminf(r, ::fminf(g, b));
+    float c = M - m;
+    hsv.v = M;
+
+    if (c != 0.0f) {
+        if (M == r) {
+            hsv.h = ::fmodf(((g - b) / c), 6.0);
+        } else if (M == g) {
+            hsv.h = (b - r) / c + 2.0f;
+        } else /* if M == b */ {
+            hsv.h = (r - g) / c + 4.0f;
+        }
+        hsv.h *= 60.0f;
+        if (hsv.h < 0.0) {
+            hsv.h += 360.0f;
+        }
+        hsv.s = c / hsv.v;
     }
-    return begin<typename I::value_type>(iterate(begin_in, end_in));
+
+    return hsv;
 }
 
 }
 }
 
-#endif /* !__MOONLIGHT_GENERATOR_H */
+#endif /* !__MOONLIGHT_COLOR_H */
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/hash.h` & `jotdown-2.0.2/moonlight/include/moonlight/hash.h`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 #define __MOONLIGHT_HASH_H
 
 #include <functional>
 
 namespace moonlight {
 namespace hash {
 
-/**
-* Lifted from boost::hash_combine.
-*/
+/** -----------------------------------------------------------------
+ * Lifted from boost::hash_combine.
+ */
 template<class T>
 inline void combine(std::size_t& seed, const T& value) {
   std::hash<T> hash_function;
   seed ^= hash_function(value) + 0x9e3779b9 + (seed << 6) + (seed >> 2);
 }
 
 }
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/mmap.h` & `jotdown-2.0.2/moonlight/include/moonlight/mmap.h`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,26 @@
 
 #include <vector>
 #include <map>
 
 namespace moonlight {
 namespace mmap {
 
-/**------------------------------------------------------------------
+/** -----------------------------------------------------------------
  * Template class used as parameter type for mmaps::build().
  */
 template<typename K, typename T>
 struct mapping {
    K key;
    std::vector<T> values;
 };
 
-/**------------------------------------------------------------------
- * Build a multimap from the given constant mapping.  Intended for use
- * in statically defining multimaps, e.g.:
+/** -----------------------------------------------------------------
+ * Build a multimap from the given constant mapping.  Intended for
+ * use in statically defining multimaps, e.g.:
  *
  * ```
  * static const auto mmap = build({
  *    {"even",    {2, 4, 6, 8}},
  *    {"odd",     {1, 3, 5, 7}}
  * });
  * ```
@@ -44,15 +44,15 @@
          mmap.insert(std::make_pair(mapping.key, value));
       }
    }
 
    return mmap;
 }
 
-/**------------------------------------------------------------------
+/** -----------------------------------------------------------------
  * Variadic version of mmap::build().
  *
  * ```
  * static const auto mmap = build(
  *    "even",    {2, 4, 6, 8},
  *    "odd",     {1, 3, 5, 7}
  * );
@@ -61,26 +61,27 @@
 template<typename K, typename T, typename... KTV>
 inline std::multimap<K, T> build(const K& key, const T& value, const KTV&... mappings) {
    std::multimap<K, T> mmap;
    build(mmap, key, value, mappings...);
    return mmap;
 }
 
-//-------------------------------------------------------------------
+/** -----------------------------------------------------------------
+ */
 template<typename K, typename T, typename... KTV>
 inline void build(std::multimap<K, T>& mmap, const K& key, const T& value,
                   const KTV&... mappings) {
    mmap.insert({key, value});
    build(mmap, mappings...);
 }
 
 template<typename K, typename T>
 inline void build(std::multimap<K, T>& mmap) { (void) mmap; }
 
-/**------------------------------------------------------------------
+/** -----------------------------------------------------------------
  * Collect all values from the given multimap-like iterable that match
  * the given key.
  */
 template<typename M>
 inline std::vector<typename M::mapped_type> collect(const M& mmap,
                                                     const typename M::key_type& key) {
    std::vector<typename M::mapped_type> values;
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/posix.h` & `jotdown-2.0.2/moonlight/include/moonlight/posix.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/sdl2.h` & `jotdown-2.0.2/moonlight/include/moonlight/sdl2.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/slice.h` & `jotdown-2.0.2/moonlight/include/moonlight/slice.h`

 * *Files 12% similar despite different names*

```diff
@@ -12,37 +12,32 @@
 
 #include "moonlight/exceptions.h"
 #include <optional>
 
 namespace moonlight {
 
 //-------------------------------------------------------------------
-class SliceError : public moonlight::core::Exception {
-    using Exception::Exception;
-};
-
-//-------------------------------------------------------------------
 template<class C>
 inline size_t slice_offset(const C& coll, int offset, bool clip = false) {
     if (offset < 0) {
         offset += coll.size();
         if (offset < 0) {
             if (clip) {
                 offset = 0;
             } else {
-                throw SliceError("Index out of range (-).");
+                THROW(core::IndexError, "Index out of range (-).");
             }
         }
     }
 
     if (offset >= coll.size()) {
         if (clip) {
             offset = coll.size();
         } else {
-            throw SliceError("Index out of range (+).");
+            THROW(core::IndexError, "Index out of range (+).");
         }
     }
 
     return offset;
 }
 
 //-------------------------------------------------------------------
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/string.h` & `jotdown-2.0.2/moonlight/include/moonlight/string.h`

 * *Files 23% similar despite different names*

```diff
@@ -9,19 +9,43 @@
 
 #ifndef __MOONLIGHT_STRING_H
 #define __MOONLIGHT_STRING_H
 
 #include <algorithm>
 #include <functional>
 #include <sstream>
+#include <iomanip>
 #include <string>
 #include <vector>
+#include <map>
+#include "moonlight/traits.h"
 
 namespace moonlight {
+
 namespace str {
+
+template<typename T>
+inline std::string coerce(const T& value) {
+    std::ostringstream sb;
+
+    if constexpr (is_streamable<T>()) {
+        sb << value;
+
+    } else {
+        sb << "<" << type_name<T>() << ">";
+    }
+
+    return sb.str();
+}
+
+template<>
+inline std::string coerce(const std::string& value) {
+    return value;
+}
+
 inline void _cat(std::ostringstream& sb) {
    (void) sb;
 }
 
 template<typename T, typename... TD>
 inline void _cat(std::ostringstream& sb, const T& element, const TD&... elements) {
    sb << element;
@@ -98,21 +122,46 @@
 /**------------------------------------------------------------------
  * Split the given string into a list of strings based on
  * the delimiter provided.
  *
  * @return The contents of the string, minus the delimiters,
  *    split along the delimiter boundaries in a linked list.
  */
-inline std::vector<std::string> split(const std::string& s, const std::string&
-                                      delimiter) {
+inline std::vector<std::string> split(const std::string& s,
+                                      const std::string& delimiter) {
    std::vector<std::string> tokens;
    split(tokens, s, delimiter);
    return tokens;
 }
 
+/**
+ * Split the given string into a list of strings based on the
+ * single character delimiter provided, with escape ('\\' by default)
+ */
+inline std::vector<std::string> split(const std::string& s, int delim, int escape = '\\') {
+    std::vector<std::string> tokens;
+    std::string token;
+
+    for (size_t x = 0; x < s.size(); x++) {
+        auto c = s[x];
+        if (c == escape) {
+            x++;
+            continue;
+        }
+        if (c == delim) {
+            tokens.push_back(token);
+            token.clear();
+        } else {
+            token.push_back(c);
+        }
+    }
+
+    return tokens;
+}
+
 /**------------------------------------------------------------------
  * Create a string consisting of a single character.
  */
 inline std::string chr(char c) {
    std::string str;
    str.push_back(c);
    return str;
@@ -149,14 +198,27 @@
  * Trim all whitespace from the left or right.
  */
 inline std::string trim(const std::string& s) {
    return trim_left(trim_right(s));
 }
 
 /**------------------------------------------------------------------
+ * Trim a string from the beginning of another if present.
+ */
+inline std::string trim_prefix(const std::string& prefix, const std::string& s) {
+    if (s.starts_with(prefix)) {
+        std::string s_copy = s;
+        s_copy.erase(0, prefix.size());
+        return s_copy;
+    }
+
+    return s;
+}
+
+/**------------------------------------------------------------------
  * Apply a function to each character in the string.
  */
 inline std::string map(const std::string& s, std::function<char(char)> transformer) {
    std::string result;
    std::transform(s.begin(), s.end(), std::back_inserter(result), transformer);
    return result;
 }
@@ -171,11 +233,54 @@
 /**------------------------------------------------------------------
  * Apply `tolower` to each character in the string.
  */
 inline std::string to_lower(const std::string& s) {
    return map(s, [](char c) { return tolower(c); });
 }
 
+// ------------------------------------------------------------------
+inline std::string literal(const std::string& str) {
+    static const std::map<char, std::string> ESCAPE_SEQUENCES = {
+        {'\a', "\\a"},
+        {'\b', "\\b"},
+        {'\e', "\\e"},
+        {'\f', "\\f"},
+        {'\n', "\\n"},
+        {'\r', "\\r"},
+        {'\t', "\\t"},
+        {'\v', "\\v"},
+        {'\\', "\\\\"},
+        {'"', "\\\""}
+    };
+
+    std::stringstream sb;
+
+    for (size_t x = 0; str[x] != '\0'; x++) {
+        char c = str[x];
+        std::string repr = "";
+
+        auto iter = ESCAPE_SEQUENCES.find(c);
+        if (iter != ESCAPE_SEQUENCES.end()) {
+            repr = iter->second;
+        }
+
+        if (repr == "" && !isprint(c)) {
+            std::ios sb_state(nullptr);
+            sb_state.copyfmt(sb);
+            sb << std::hex << std::setfill('0') << std::setw(2);
+            sb << "\\x" << (0xFF & c);
+            sb.copyfmt(sb_state);
+
+        } else if (repr != "") {
+            sb << repr;
+        } else {
+            sb << c;
+        }
+    }
+
+    return sb.str();
+}
+
 }
 }
 
 #endif /* !__MOONLIGHT_STRING_H */
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/test.h` & `jotdown-2.0.2/moonlight/include/moonlight/json/mapping.h`

 * *Files 26% similar despite different names*

```diff
@@ -1,220 +1,208 @@
 /*
- * moonlight/test.h: A very simple to use unit testing framework
- *    built around lambda expressions.
+ * mapping.h
  *
- * Author: Lain Supe (lainproliant)
- * Date: Thu October 9, 2014
+ * Author: Lain Musgrove (lain.proliant@gmail.com)
+ * Date: Monday September 13, 2021
+ *
+ * Distributed under terms of the MIT license.
  */
-#ifndef __MOONLIGHT_TEST_H
-#define __MOONLIGHT_TEST_H
 
-#include "moonlight/exceptions.h"
-#include "moonlight/system.h"
+#ifndef __MOONLIGHT_JSON_MAPPING_H
+#define __MOONLIGHT_JSON_MAPPING_H
 
-#include <csignal>
-#include <cstdlib>
-#include <cstring>
-#include <cmath>
-#include <cfloat>
-#include <iostream>
+#include <functional>
+#include <type_traits>
+#include "moonlight/traits.h"
+#include "moonlight/json/array.h"
+#include "moonlight/json/object.h"
 
 namespace moonlight {
-namespace test {
-//-------------------------------------------------------------------
-class TestException : public core::Exception {
-public:
-   using core::Exception::Exception;
-};
+namespace json {
 
 //-------------------------------------------------------------------
-class AssertionFailed : public TestException {
+class Mapping {
 public:
-   using TestException::TestException;
+    typedef std::unique_ptr<Mapping> Pointer;
+
+    Mapping(const char* name, bool required)
+    : _name(name), _required(required) { }
+
+    virtual ~Mapping() { }
+
+    virtual Value::Pointer get() const = 0;
+    virtual void set(Value::Pointer value) const = 0;
+
+    std::string name() const {
+        return _name;
+    }
+
+    bool required() const {
+        return _required;
+    }
+
+private:
+    const char* _name;
+    bool _required;
 };
 
 //-------------------------------------------------------------------
-class UnitTest {
+template<typename T>
+class PropertyMapping : public Mapping {
 public:
-   UnitTest(const std::string& name, std::function<void()> test_fn) :
-   test_fn(test_fn), name(name) {}
-   virtual ~UnitTest() {}
-
-   void run() const {
-      test_fn();
-   }
-
-   std::string get_name() const {
-      return name;
-   }
+    typedef typename std::remove_const<T>::type Type;
+    typedef std::function<const Type()> Getter;
+    typedef std::function<void(const Type&)> Setter;
+
+    PropertyMapping(const char* name,
+                    Getter getter,
+                    Setter setter,
+                    bool required)
+    : Mapping(name, required), _getter(getter), _setter(setter) { }
+
+    Value::Pointer get() const override {
+        return Value::of(_getter());
+    }
+
+    void set(Value::Pointer value) const override {
+        if (! value->is<Type>()) {
+            THROW(core::TypeError, "Can't save value of type " + value->type_name() + "to the \"" + name() + "\" property mapping.");
+        }
+
+        _setter(value->get<Type>());
+    }
 
 private:
-   std::function<void()> test_fn;
-   std::string name;
+    Getter _getter;
+    Setter _setter;
 };
 
 //-------------------------------------------------------------------
-class TestSuite {
+template<typename T>
+class FieldMapping : public Mapping {
 public:
-   TestSuite(const std::string& name) : name(name) {}
-   virtual ~TestSuite() {}
+    typedef typename std::remove_const<T>::type Type;
 
-   TestSuite& test(std::string name, std::function<void()> test_fn) {
-      return test(UnitTest(name, test_fn));
-   }
-
-   TestSuite& test(const UnitTest& test) {
-      tests.push_back(test);
-      return *this;
-   }
-
-   TestSuite& die_on_signal(int signalId) {
-      signal(signalId, signal_callback);
-      return *this;
-   }
-
-   int run(std::ostream& out = std::cout) const {
-      int tests_failed = 0;
-
-      out << "===== " << name << " =====" << std::endl;
-
-      for (const UnitTest& test : tests) {
-         try {
-            out << "Running test: '" << test.get_name() << "'..." << std::endl;
-            test.run();
-            out << "    PASSED" << std::endl;
-
-         } catch (...) {
-            std::exception_ptr eptr = std::current_exception();
-
-            try {
-               std::rethrow_exception(eptr);
-            } catch (const std::exception& e) {
-               out << "    FAILED (" << typeid(e).name() << "): " << e.what() << std::endl;
-#ifdef MOONLIGHT_ENABLE_STACKTRACE
-               out << core::format_stacktrace(core::generate_stacktrace()) << std::endl;
-#endif
-               if (sys::getenv("MOONLIGHT_TEST_RETHROW")) {
-                  throw e;
-               }
-            }
+    FieldMapping(const char* name, T& field, bool required)
+    : Mapping(name, required), _field(field) { }
 
-            tests_failed ++;
-         }
-      }
-
-      out << std::endl;
-
-      return tests_failed;
-   }
-
-   int size() const {
-      return tests.size();
-   }
+    Value::Pointer get() const override {
+        return Value::of(_field);
+    }
+
+    void set(Value::Pointer value) const override {
+        if (! value->is<Type>()) {
+            THROW(core::TypeError, "Can't save value of type " + value->type_name() + "to the \"" + name() + "\" field mapping.");
+        }
 
-private:
-   static void signal_callback(int signal) {
-      std::cerr << std::endl << "FATAL: Caught signal " << signal
-      << " (" << strsignal(signal) << ")"
-      << std::endl;
-
-#ifdef MOONLIGHT_ENABLE_STACKTRACE
-      std::cerr << core::format_stacktrace(core::generate_stacktrace()) << std::endl;
-#endif
-      exit(1);
-   }
+        _field = value->get<Type>();
+    }
 
-   std::vector<UnitTest> tests;
-   std::string name;
+private:
+    T& _field;
 };
 
 //-------------------------------------------------------------------
-inline void fail(const std::string& message = "Failed.")
-{
-   throw TestException(message);
-}
-
-//-------------------------------------------------------------------
-inline void assert_true(bool expr, const std::string& message = "Assertion failed.") {
-   if (! expr) {
-      throw AssertionFailed(message);
-   }
-}
-
-//-------------------------------------------------------------------
-inline void assert_false(bool expr, const std::string& message = "Negative assertion failed.") {
-   if (expr) {
-      throw AssertionFailed(message);
-   }
-}
+template<typename T>
+class ObjectMapping : public Mapping {
+public:
+    typedef typename std::remove_const<T>::type Type;
 
-//-------------------------------------------------------------------
-inline void epsilon_assert(double a, double b,
-                           double epsilon = DBL_EPSILON,
-                           const std::string& message = "Value equivalence assertion failed. (double epsilon)") {
-
-   if (fabs(a - b) > epsilon) {
-      throw AssertionFailed(message);
-   }
-}
+    ObjectMapping(const char* name, Type& obj_ref, bool required)
+    : Mapping(name, required), _obj_ref(obj_ref) { }
 
-//-------------------------------------------------------------------
-inline void epsilon_assert(float a, float b,
-                           float epsilon = FLT_EPSILON,
-                           const std::string& message = "Value equivalence assertion failed. (float epsilon)") {
-   if (fabs(a - b) > epsilon) {
-      throw AssertionFailed(message);
-   }
-}
+    Value::Pointer get() const override {
+        auto obj = std::make_shared<Object>();
 
-//-------------------------------------------------------------------
-template<class T>
-inline void assert_equal(const T& a, const T& b,
-                         const std::string& message = "Value equivalence assertion failed.") {
-   if (a != b) {
-      throw AssertionFailed(message);
-   }
-}
+        for (auto mapping : _obj_ref.json_mapper()) {
+            obj->set(mapping->name(), Value::of(mapping->get()));
+        }
+
+        return obj;
+    }
+
+    void set(Value::Pointer value) const override {
+        if (! value->is<Object>()) {
+            THROW(core::TypeError, "Can't apply non-object mapping to \"" + name() + "\" object.");
+        }
+    }
 
-//-------------------------------------------------------------------
-template<>
-inline void assert_equal<double>(const double& a, const double& b, const std::string& message) {
-   try {
-      epsilon_assert(a, b);
-
-   } catch (const AssertionFailed& e) {
-      throw AssertionFailed(message);
-   }
-}
+private:
+    Type& _obj_ref;
+};
 
 //-------------------------------------------------------------------
-template<>
-inline void assert_equal<float>(const float& a, const float& b, const std::string& message) {
-   try {
-      epsilon_assert(a, b);
-
-   } catch (const AssertionFailed& e) {
-      throw AssertionFailed(message);
-   }
-}
+template<class C>
+class Mapper {
+public:
+    Mapper(C* instance) : _instance(instance) { }
+    Mapper(Mapper& other)
+    : _instance(other._instance), _mappings(std::move(other._mappings)) { }
+
+    template<class UnboundGetter, class UnboundSetter>
+    Mapper& property(const char* name,
+                     const UnboundGetter& getter,
+                     const UnboundSetter& setter,
+                     bool required = false) {
+        using namespace std::placeholders;
+
+        typedef typename std::remove_reference<typename std::result_of<decltype(std::bind(getter, _instance))()>::type>::type Type;
+
+        C* instance = _instance;
+        std::function<const Type()> getter_proxy = [=]() {
+            const auto bound_getter = std::bind(getter, instance);
+            return bound_getter();
+        };
+
+        std::function<void(Type)> setter_proxy = [=](const Type& p) {
+            const auto bound_setter = std::bind(setter, instance, _1);
+            bound_setter(p);
+        };
+
+        _mappings.push_back(std::make_unique<PropertyMapping<Type>>(
+            name,
+            getter_proxy,
+            setter_proxy,
+            required
+        ));
+        return *this;
+    }
+
+    template<class T>
+    Mapper& field(const char* name, T& ref, bool required = false) {
+        _mappings.push_back(std::make_unique<FieldMapping<T>>(
+            name, ref, required
+        ));
+        return *this;
+    }
+
+    json::Object map_to_json() const {
+        json::Object obj;
+        for (auto& mapping : _mappings) {
+            obj.set(mapping->name(), mapping->get());
+        }
+        return obj;
+    }
+
+    C& map_from_json(const json::Object& obj) const {
+        for (auto& mapping : _mappings) {
+            if (mapping->required() && !obj.contains(mapping->name())) {
+                THROW(core::TypeError, "Missing required field \"" + mapping->name() + "\" on JSON object.");
+            }
 
-//-------------------------------------------------------------------
-template<class T>
-inline size_t generic_list_size(const T& listA) {
-   size_t sz = 0;
-   for (auto iter = listA.begin(); iter != listA.end(); iter++) {
-      sz++;
-   }
-   return sz;
-}
+            auto value = obj.get<Value::Pointer>(mapping->name());
+            if (value != nullptr) {
+                mapping->set(obj.get<Value::Pointer>(mapping->name()));
+            }
+        }
+        return *_instance;
+    }
 
-//-------------------------------------------------------------------
-template<class T>
-inline bool lists_equal(const T& listA, const T& listB) {
+private:
+    std::vector<Mapping::Pointer> _mappings;
+    C* _instance;
+};
 
-   return generic_list_size(listA) == generic_list_size(listB) &&
-   equal(listA.begin(), listA.end(), listB.begin());
-}
 }
 }
 
-#endif /* __MOONLIGHT_TEST_H */
+#endif /* !__MOONLIGHT_JSON_MAPPING_H */
```

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/time.h` & `jotdown-2.0.2/moonlight/include/moonlight/time.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/moonlight/include/moonlight/variadic.h` & `jotdown-2.0.2/moonlight/include/moonlight/variadic.h`

 * *Files 21% similar despite different names*

```diff
@@ -10,56 +10,55 @@
 #ifndef __MOONLIGHT_VARIADIC_H
 #define __MOONLIGHT_VARIADIC_H
 
 #include <vector>
 
 namespace moonlight {
 namespace variadic {
-/**------------------------------------------------------------------
- * An empty base structure used for iterating across variadic
- * template parameters in order.  Takes advantage of the fact
- * that initialization lists preserve order of parameters
- * when variadic template parameters are expanded in them.
- *
- * ```
- * template<typename T, typename... TV>
- * T sum(T init, const TV&&... values) {
- *    T total = init;
- *    variadic::pass{(total += values)...};
- * }
- * ```
- *
- * To use with void function calls or statements, provide
- * a second statement that yields a value, e.g. a const statement:
- *
- * ```
- * template<typename T, typename... TV>
- * void foreach(std::function<void(T)> f, const TV&&... values) {
- *    variadic::pass{(f(values), 0)...};
- * }
- * ```
- */
+// ------------------------------------------------------------------
+// An empty base structure used for iterating across variadic
+// template parameters in order.  Takes advantage of the fact
+// that initialization lists preserve order of parameters
+// when variadic template parameters are expanded in them.
+//
+// ```
+// template<typename T, typename... TV>
+// T sum(T init, const TV&&... values) {
+//    T total = init;
+//    variadic::pass{(total += values)...};
+// }
+// ```
+//
+// To use with void function calls or statements, provide
+// a second statement that yields a value, e.g. a const statement:
+//
+// ```
+// template<typename T, typename... TV>
+// void foreach(std::function<void(T)> f, const TV&&... values) {
+//    variadic::pass{(f(values), 0)...};
+// }
+// ```
 struct pass {
    template<typename... T> pass(T...) { }
 };
 
-//-------------------------------------------------------------------
+// ------------------------------------------------------------------
 template<typename T, typename... TD>
 inline void _to_vector(std::vector<T>& vec) {
    (void)vec;
 }
 
-//-------------------------------------------------------------------
+// ------------------------------------------------------------------
 template<typename T, typename... TD>
 inline void _to_vector(std::vector<T>& vec, const T& item, const TD&... items) {
    vec.push_back(item);
    _to_vector(vec, items...);
 }
 
-//-------------------------------------------------------------------
+// ------------------------------------------------------------------
 template<typename T, typename... TD>
 inline std::vector<T> to_vector(const T& item, const TD&... items) {
    std::vector<T> vec;
    _to_vector(vec, item, items...);
    return vec;
 }
 }
```

### Comparing `jotdown-2.0.1/moonlight/include/tinyformat/tinyformat.h` & `jotdown-2.0.2/moonlight/deps/tinyformat/tinyformat.h`

 * *Files 8% similar despite different names*

```diff
@@ -29,33 +29,42 @@
 // Tinyformat: A minimal type safe printf replacement
 //
 // tinyformat.h is a type safe printf replacement library in a single C++
 // header file.  Design goals include:
 //
 // * Type safety and extensibility for user defined types.
 // * C99 printf() compatibility, to the extent possible using std::ostream
+// * POSIX extension for positional arguments
 // * Simplicity and minimalism.  A single header file to include and distribute
 //   with your projects.
 // * Augment rather than replace the standard stream formatting mechanism
 // * C++98 support, with optional C++11 niceties
 //
 //
 // Main interface example usage
 // ----------------------------
 //
-// To print a date to std::cout:
+// To print a date to std::cout for American usage:
 //
 //   std::string weekday = "Wednesday";
 //   const char* month = "July";
 //   size_t day = 27;
 //   long hour = 14;
 //   int min = 44;
 //
 //   tfm::printf("%s, %s %d, %.2d:%.2d\n", weekday, month, day, hour, min);
 //
+// POSIX extension for positional arguments is available.
+// The ability to rearrange formatting arguments is an important feature
+// for localization because the word order may vary in different languages.
+//
+// Previous example for German usage. Arguments are reordered:
+//
+//   tfm::printf("%1$s, %3$d. %2$s, %4$d:%5$.2d\n", weekday, month, day, hour, min);
+//
 // The strange types here emphasize the type safety of the interface; it is
 // possible to print a std::string using the "%s" conversion, and a
 // size_t using the "%d" conversion.  A similar result could be achieved
 // using either of the tfm::format() functions.  One prints on a user provided
 // stream:
 //
 //   tfm::format(std::cerr, "%s, %s %d, %.2d:%.2d\n",
@@ -129,36 +138,42 @@
 // general.  If you don't define this, C++11 support is autodetected below.
 // #define TINYFORMAT_USE_VARIADIC_TEMPLATES
 
 
 //------------------------------------------------------------------------------
 // Implementation details.
 #include <algorithm>
-#include <cassert>
 #include <iostream>
 #include <sstream>
+#include <cmath>
+
+#ifndef TINYFORMAT_ASSERT
+#   include <cassert>
+#   define TINYFORMAT_ASSERT(cond) assert(cond)
+#endif
 
 #ifndef TINYFORMAT_ERROR
+#   include <cassert>
 #   define TINYFORMAT_ERROR(reason) assert(0 && reason)
 #endif
 
 #if !defined(TINYFORMAT_USE_VARIADIC_TEMPLATES) && !defined(TINYFORMAT_NO_VARIADIC_TEMPLATES)
 #   ifdef __GXX_EXPERIMENTAL_CXX0X__
 #       define TINYFORMAT_USE_VARIADIC_TEMPLATES
 #   endif
 #endif
 
 #if defined(__GLIBCXX__) && __GLIBCXX__ < 20080201
-//  std::showpos is broken on old libstdc++ as provided with OSX.  See
+//  std::showpos is broken on old libstdc++ as provided with macOS.  See
 //  http://gcc.gnu.org/ml/libstdc++/2007-11/msg00075.html
 #   define TINYFORMAT_OLD_LIBSTDCPLUSPLUS_WORKAROUND
 #endif
 
 #ifdef __APPLE__
-// Workaround OSX linker warning: xcode uses different default symbol
+// Workaround macOS linker warning: Xcode uses different default symbol
 // visibilities for static libs vs executables (see issue #25)
 #   define TINYFORMAT_HIDDEN __attribute__((visibility("hidden")))
 #else
 #   define TINYFORMAT_HIDDEN
 #endif
 
 namespace tinyformat {
@@ -206,15 +221,15 @@
 
 
 // Format the value by casting to type fmtT.  This default implementation
 // should never be called.
 template<typename T, typename fmtT, bool convertible = is_convertible<T, fmtT>::value>
 struct formatValueAsType
 {
-    static void invoke(std::ostream& /*out*/, const T& /*value*/) { assert(0); }
+    static void invoke(std::ostream& /*out*/, const T& /*value*/) { TINYFORMAT_ASSERT(0); }
 };
 // Specialized version for types that can actually be converted to fmtT, as
 // indicated by the "convertible" template parameter.
 template<typename T, typename fmtT>
 struct formatValueAsType<T,fmtT,true>
 {
     static void invoke(std::ostream& out, const T& value)
@@ -228,16 +243,15 @@
     static bool invoke(std::ostream& /**/, const T& /**/) { return false; }
 };
 template<typename T>
 struct formatZeroIntegerWorkaround<T,true>
 {
     static bool invoke(std::ostream& out, const T& value)
     {
-        if (static_cast<int>(value) == 0 && out.flags() & std::ios::showpos)
-        {
+        if (static_cast<int>(value) == 0 && out.flags() & std::ios::showpos) {
             out << "+0";
             return true;
         }
         return false;
     }
 };
 #endif // TINYFORMAT_OLD_LIBSTDCPLUSPLUS_WORKAROUND
@@ -270,24 +284,39 @@
     std::string result = tmp.str();
     out.write(result.c_str(), (std::min)(ntrunc, static_cast<int>(result.size())));
 }
 #define TINYFORMAT_DEFINE_FORMAT_TRUNCATED_CSTR(type)       \
 inline void formatTruncated(std::ostream& out, type* value, int ntrunc) \
 {                                                           \
     std::streamsize len = 0;                                \
-    while(len < ntrunc && value[len] != 0)                  \
+    while (len < ntrunc && value[len] != 0)                 \
         ++len;                                              \
     out.write(value, len);                                  \
 }
 // Overload for const char* and char*.  Could overload for signed & unsigned
 // char too, but these are technically unneeded for printf compatibility.
 TINYFORMAT_DEFINE_FORMAT_TRUNCATED_CSTR(const char)
 TINYFORMAT_DEFINE_FORMAT_TRUNCATED_CSTR(char)
 #undef TINYFORMAT_DEFINE_FORMAT_TRUNCATED_CSTR
 
+template<typename T>
+void spaceFillIfNotFinite(std::ostream& out, const T& value) { }
+// TODO: type_traits would clearly be better here. Should consider moving all
+// these workarounds into a big pre-C++11 section.
+#define TINYFORMAT_SETFILL_NOT_FINITE_FLOATING(type)             \
+inline void spaceFillIfNotFinite(std::ostream& out, type value)  \
+{                                                                \
+    if (out.fill() == '0' && !std::isfinite(value))              \
+        out.fill(' ');                                           \
+}
+TINYFORMAT_SETFILL_NOT_FINITE_FLOATING(float)
+TINYFORMAT_SETFILL_NOT_FINITE_FLOATING(double)
+TINYFORMAT_SETFILL_NOT_FINITE_FLOATING(long double)
+#undef TINYFORMAT_SETFILL_NOT_FINITE_FLOATING
+
 } // namespace detail
 
 
 //------------------------------------------------------------------------------
 // Variable formatting functions.  May be overridden for user-defined types if
 // desired.
 
@@ -316,39 +345,38 @@
     // The mess here is to support the %c and %p conversions: if these
     // conversions are active we try to convert the type to a char or const
     // void* respectively and format that instead of the value itself.  For the
     // %p conversion it's important to avoid dereferencing the pointer, which
     // could otherwise lead to a crash when printing a dangling (const char*).
     const bool canConvertToChar = detail::is_convertible<T,char>::value;
     const bool canConvertToVoidPtr = detail::is_convertible<T, const void*>::value;
-    if(canConvertToChar && *(fmtEnd-1) == 'c')
+    detail::spaceFillIfNotFinite(out, value);
+    if (canConvertToChar && *(fmtEnd-1) == 'c')
         detail::formatValueAsType<T, char>::invoke(out, value);
-    else if(canConvertToVoidPtr && *(fmtEnd-1) == 'p')
+    else if (canConvertToVoidPtr && *(fmtEnd-1) == 'p')
         detail::formatValueAsType<T, const void*>::invoke(out, value);
 #ifdef TINYFORMAT_OLD_LIBSTDCPLUSPLUS_WORKAROUND
-    else if(detail::formatZeroIntegerWorkaround<T>::invoke(out, value)) /**/;
+    else if (detail::formatZeroIntegerWorkaround<T>::invoke(out, value)) /**/;
 #endif
-    else if(ntrunc >= 0)
-    {
+    else if (ntrunc >= 0) {
         // Take care not to overread C strings in truncating conversions like
         // "%.4s" where at most 4 characters may be read.
         detail::formatTruncated(out, value, ntrunc);
     }
     else
         out << value;
 }
 
 
 // Overloaded version for char types to support printing as an integer
 #define TINYFORMAT_DEFINE_FORMATVALUE_CHAR(charType)                  \
 inline void formatValue(std::ostream& out, const char* /*fmtBegin*/,  \
                         const char* fmtEnd, int /**/, charType value) \
 {                                                                     \
-    switch(*(fmtEnd-1))                                               \
-    {                                                                 \
+    switch (*(fmtEnd-1)) {                                            \
         case 'u': case 'd': case 'i': case 'o': case 'X': case 'x':   \
             out << static_cast<int>(value); break;                    \
         default:                                                      \
             out << value;                   break;                    \
     }                                                                 \
 }
 // per 3.9.1: char, signed char and unsigned char are all distinct types
@@ -365,19 +393,19 @@
 
 #define TINYFORMAT_ARGTYPES(n) TINYFORMAT_ARGTYPES_ ## n
 #define TINYFORMAT_VARARGS(n) TINYFORMAT_VARARGS_ ## n
 #define TINYFORMAT_PASSARGS(n) TINYFORMAT_PASSARGS_ ## n
 #define TINYFORMAT_PASSARGS_TAIL(n) TINYFORMAT_PASSARGS_TAIL_ ## n
 
 // To keep it as transparent as possible, the macros below have been generated
-// using python via the excellent cog.py code generation script.  This avoids
+// using python via the excellent cog code generation script.  This avoids
 // the need for a bunch of complex (but more general) preprocessor tricks as
 // used in boost.preprocessor.
 //
-// To rerun the code generation in place, use `cog.py -r tinyformat.h`
+// To rerun the code generation in place, use `cog -r tinyformat.h`
 // (see http://nedbatchelder.com/code/cog).  Alternatively you can just create
 // extra versions by hand.
 
 /*[[[cog
 maxParams = 16
 
 def makeCommaSepLists(lineTemplate, elemTemplate, startInd=1):
@@ -478,44 +506,46 @@
 
 
 
 namespace detail {
 
 // Type-opaque holder for an argument to format(), with associated actions on
 // the type held as explicit function pointers.  This allows FormatArg's for
-// each argument to be allocated as a homogenous array inside FormatList
+// each argument to be allocated as a homogeneous array inside FormatList
 // whereas a naive implementation based on inheritance does not.
 class FormatArg
 {
     public:
         FormatArg()
             : m_value(NULL),
             m_formatImpl(NULL),
             m_toIntImpl(NULL)
         { }
 
         template<typename T>
         FormatArg(const T& value)
-            : m_value(static_cast<const void*>(&value)),
+            // C-style cast here allows us to also remove volatile; we put it
+            // back in the *Impl functions before dereferencing to avoid UB.
+            : m_value((const void*)(&value)),
             m_formatImpl(&formatImpl<T>),
             m_toIntImpl(&toIntImpl<T>)
         { }
 
         void format(std::ostream& out, const char* fmtBegin,
                     const char* fmtEnd, int ntrunc) const
         {
-            assert(m_value);
-            assert(m_formatImpl);
+            TINYFORMAT_ASSERT(m_value);
+            TINYFORMAT_ASSERT(m_formatImpl);
             m_formatImpl(out, fmtBegin, fmtEnd, ntrunc, m_value);
         }
 
         int toInt() const
         {
-            assert(m_value);
-            assert(m_toIntImpl);
+            TINYFORMAT_ASSERT(m_value);
+            TINYFORMAT_ASSERT(m_toIntImpl);
             return m_toIntImpl(m_value);
         }
 
     private:
         template<typename T>
         TINYFORMAT_HIDDEN static void formatImpl(std::ostream& out, const char* fmtBegin,
                         const char* fmtEnd, int ntrunc, const void* value)
@@ -537,175 +567,240 @@
 
 
 // Parse and return an integer from the string c, as atoi()
 // On return, c is set to one past the end of the integer.
 inline int parseIntAndAdvance(const char*& c)
 {
     int i = 0;
-    for(;*c >= '0' && *c <= '9'; ++c)
+    for (;*c >= '0' && *c <= '9'; ++c)
         i = 10*i + (*c - '0');
     return i;
 }
 
-// Print literal part of format string and return next format spec
-// position.
+// Parse width or precision `n` from format string pointer `c`, and advance it
+// to the next character. If an indirection is requested with `*`, the argument
+// is read from `args[argIndex]` and `argIndex` is incremented (or read
+// from `args[n]` in positional mode). Returns true if one or more
+// characters were read.
+inline bool parseWidthOrPrecision(int& n, const char*& c, bool positionalMode,
+                                  const detail::FormatArg* args,
+                                  int& argIndex, int numArgs)
+{
+    if (*c >= '0' && *c <= '9') {
+        n = parseIntAndAdvance(c);
+    }
+    else if (*c == '*') {
+        ++c;
+        n = 0;
+        if (positionalMode) {
+            int pos = parseIntAndAdvance(c) - 1;
+            if (*c != '$')
+                TINYFORMAT_ERROR("tinyformat: Non-positional argument used after a positional one");
+            if (pos >= 0 && pos < numArgs)
+                n = args[pos].toInt();
+            else
+                TINYFORMAT_ERROR("tinyformat: Positional argument out of range");
+            ++c;
+        }
+        else {
+            if (argIndex < numArgs)
+                n = args[argIndex++].toInt();
+            else
+                TINYFORMAT_ERROR("tinyformat: Not enough arguments to read variable width or precision");
+        }
+    }
+    else {
+        return false;
+    }
+    return true;
+}
+
+// Print literal part of format string and return next format spec position.
 //
-// Skips over any occurrences of '%%', printing a literal '%' to the
-// output.  The position of the first % character of the next
-// nontrivial format spec is returned, or the end of string.
+// Skips over any occurrences of '%%', printing a literal '%' to the output.
+// The position of the first % character of the next nontrivial format spec is
+// returned, or the end of string.
 inline const char* printFormatStringLiteral(std::ostream& out, const char* fmt)
 {
     const char* c = fmt;
-    for(;; ++c)
-    {
-        switch(*c)
-        {
-            case '\0':
-                out.write(fmt, c - fmt);
+    for (;; ++c) {
+        if (*c == '\0') {
+            out.write(fmt, c - fmt);
+            return c;
+        }
+        else if (*c == '%') {
+            out.write(fmt, c - fmt);
+            if (*(c+1) != '%')
                 return c;
-            case '%':
-                out.write(fmt, c - fmt);
-                if(*(c+1) != '%')
-                    return c;
-                // for "%%", tack trailing % onto next literal section.
-                fmt = ++c;
-                break;
-            default:
-                break;
+            // for "%%", tack trailing % onto next literal section.
+            fmt = ++c;
         }
     }
 }
 
 
 // Parse a format string and set the stream state accordingly.
 //
 // The format mini-language recognized here is meant to be the one from C99,
-// with the form "%[flags][width][.precision][length]type".
+// with the form "%[flags][width][.precision][length]type" with POSIX
+// positional arguments extension.
+//
+// POSIX positional arguments extension:
+// Conversions can be applied to the nth argument after the format in
+// the argument list, rather than to the next unused argument. In this case,
+// the conversion specifier character % (see below) is replaced by the sequence
+// "%n$", where n is a decimal integer in the range [1,{NL_ARGMAX}],
+// giving the position of the argument in the argument list. This feature
+// provides for the definition of format strings that select arguments
+// in an order appropriate to specific languages.
+//
+// The format can contain either numbered argument conversion specifications
+// (that is, "%n$" and "*m$"), or unnumbered argument conversion specifications
+// (that is, % and * ), but not both. The only exception to this is that %%
+// can be mixed with the "%n$" form. The results of mixing numbered and
+// unnumbered argument specifications in a format string are undefined.
+// When numbered argument specifications are used, specifying the Nth argument
+// requires that all the leading arguments, from the first to the (N-1)th,
+// are specified in the format string.
+//
+// In format strings containing the "%n$" form of conversion specification,
+// numbered arguments in the argument list can be referenced from the format
+// string as many times as required.
 //
 // Formatting options which can't be natively represented using the ostream
 // state are returned in spacePadPositive (for space padded positive numbers)
 // and ntrunc (for truncating conversions).  argIndex is incremented if
-// necessary to pull out variable width and precision .  The function returns a
+// necessary to pull out variable width and precision.  The function returns a
 // pointer to the character after the end of the current format spec.
-inline const char* streamStateFromFormat(std::ostream& out, bool& spacePadPositive,
+inline const char* streamStateFromFormat(std::ostream& out, bool& positionalMode,
+                                         bool& spacePadPositive,
                                          int& ntrunc, const char* fmtStart,
-                                         const detail::FormatArg* formatters,
-                                         int& argIndex, int numFormatters)
+                                         const detail::FormatArg* args,
+                                         int& argIndex, int numArgs)
 {
-    if(*fmtStart != '%')
-    {
-        TINYFORMAT_ERROR("tinyformat: Not enough conversion specifiers in format string");
-        return fmtStart;
-    }
+    TINYFORMAT_ASSERT(*fmtStart == '%');
     // Reset stream state to defaults.
     out.width(0);
     out.precision(6);
     out.fill(' ');
     // Reset most flags; ignore irrelevant unitbuf & skipws.
     out.unsetf(std::ios::adjustfield | std::ios::basefield |
                std::ios::floatfield | std::ios::showbase | std::ios::boolalpha |
                std::ios::showpoint | std::ios::showpos | std::ios::uppercase);
     bool precisionSet = false;
     bool widthSet = false;
     int widthExtra = 0;
     const char* c = fmtStart + 1;
-    // 1) Parse flags
-    for(;; ++c)
-    {
-        switch(*c)
-        {
-            case '#':
-                out.setf(std::ios::showpoint | std::ios::showbase);
-                continue;
-            case '0':
-                // overridden by left alignment ('-' flag)
-                if(!(out.flags() & std::ios::left))
-                {
-                    // Use internal padding so that numeric values are
-                    // formatted correctly, eg -00010 rather than 000-10
-                    out.fill('0');
-                    out.setf(std::ios::internal, std::ios::adjustfield);
-                }
-                continue;
-            case '-':
-                out.fill(' ');
-                out.setf(std::ios::left, std::ios::adjustfield);
-                continue;
-            case ' ':
-                // overridden by show positive sign, '+' flag.
-                if(!(out.flags() & std::ios::showpos))
-                    spacePadPositive = true;
-                continue;
-            case '+':
-                out.setf(std::ios::showpos);
-                spacePadPositive = false;
-                widthExtra = 1;
-                continue;
-            default:
-                break;
+
+    // 1) Parse an argument index (if followed by '$') or a width possibly
+    // preceded with '0' flag.
+    if (*c >= '0' && *c <= '9') {
+        const char tmpc = *c;
+        int value = parseIntAndAdvance(c);
+        if (*c == '$') {
+            // value is an argument index
+            if (value > 0 && value <= numArgs)
+                argIndex = value - 1;
+            else
+                TINYFORMAT_ERROR("tinyformat: Positional argument out of range");
+            ++c;
+            positionalMode = true;
+        }
+        else if (positionalMode) {
+            TINYFORMAT_ERROR("tinyformat: Non-positional argument used after a positional one");
+        }
+        else {
+            if (tmpc == '0') {
+                // Use internal padding so that numeric values are
+                // formatted correctly, eg -00010 rather than 000-10
+                out.fill('0');
+                out.setf(std::ios::internal, std::ios::adjustfield);
+            }
+            if (value != 0) {
+                // Nonzero value means that we parsed width.
+                widthSet = true;
+                out.width(value);
+            }
         }
-        break;
     }
-    // 2) Parse width
-    if(*c >= '0' && *c <= '9')
-    {
-        widthSet = true;
-        out.width(parseIntAndAdvance(c));
+    else if (positionalMode) {
+        TINYFORMAT_ERROR("tinyformat: Non-positional argument used after a positional one");
     }
-    if(*c == '*')
-    {
-        widthSet = true;
+    // 2) Parse flags and width if we did not do it in previous step.
+    if (!widthSet) {
+        // Parse flags
+        for (;; ++c) {
+            switch (*c) {
+                case '#':
+                    out.setf(std::ios::showpoint | std::ios::showbase);
+                    continue;
+                case '0':
+                    // overridden by left alignment ('-' flag)
+                    if (!(out.flags() & std::ios::left)) {
+                        // Use internal padding so that numeric values are
+                        // formatted correctly, eg -00010 rather than 000-10
+                        out.fill('0');
+                        out.setf(std::ios::internal, std::ios::adjustfield);
+                    }
+                    continue;
+                case '-':
+                    out.fill(' ');
+                    out.setf(std::ios::left, std::ios::adjustfield);
+                    continue;
+                case ' ':
+                    // overridden by show positive sign, '+' flag.
+                    if (!(out.flags() & std::ios::showpos))
+                        spacePadPositive = true;
+                    continue;
+                case '+':
+                    out.setf(std::ios::showpos);
+                    spacePadPositive = false;
+                    widthExtra = 1;
+                    continue;
+                default:
+                    break;
+            }
+            break;
+        }
+        // Parse width
         int width = 0;
-        if(argIndex < numFormatters)
-            width = formatters[argIndex++].toInt();
-        else
-            TINYFORMAT_ERROR("tinyformat: Not enough arguments to read variable width");
-        if(width < 0)
-        {
-            // negative widths correspond to '-' flag set
-            out.fill(' ');
-            out.setf(std::ios::left, std::ios::adjustfield);
-            width = -width;
+        widthSet = parseWidthOrPrecision(width, c, positionalMode,
+                                         args, argIndex, numArgs);
+        if (widthSet) {
+            if (width < 0) {
+                // negative widths correspond to '-' flag set
+                out.fill(' ');
+                out.setf(std::ios::left, std::ios::adjustfield);
+                width = -width;
+            }
+            out.width(width);
         }
-        out.width(width);
-        ++c;
     }
     // 3) Parse precision
-    if(*c == '.')
-    {
+    if (*c == '.') {
         ++c;
         int precision = 0;
-        if(*c == '*')
-        {
-            ++c;
-            if(argIndex < numFormatters)
-                precision = formatters[argIndex++].toInt();
-            else
-                TINYFORMAT_ERROR("tinyformat: Not enough arguments to read variable precision");
-        }
-        else
-        {
-            if(*c >= '0' && *c <= '9')
-                precision = parseIntAndAdvance(c);
-            else if(*c == '-') // negative precisions ignored, treated as zero.
-                parseIntAndAdvance(++c);
-        }
-        out.precision(precision);
-        precisionSet = true;
+        parseWidthOrPrecision(precision, c, positionalMode,
+                              args, argIndex, numArgs);
+        // Presence of `.` indicates precision set, unless the inferred value
+        // was negative in which case the default is used.
+        precisionSet = precision >= 0;
+        if (precisionSet)
+            out.precision(precision);
     }
     // 4) Ignore any C99 length modifier
-    while(*c == 'l' || *c == 'h' || *c == 'L' ||
-          *c == 'j' || *c == 'z' || *c == 't')
+    while (*c == 'l' || *c == 'h' || *c == 'L' ||
+           *c == 'j' || *c == 'z' || *c == 't') {
         ++c;
+    }
     // 5) We're up to the conversion specifier character.
     // Set stream flags based on conversion specifier (thanks to the
     // boost::format class for forging the way here).
     bool intConversion = false;
-    switch(*c)
-    {
+    switch (*c) {
         case 'u': case 'd': case 'i':
             out.setf(std::ios::dec, std::ios::basefield);
             intConversion = true;
             break;
         case 'o':
             out.setf(std::ios::oct, std::ios::basefield);
             intConversion = true;
@@ -726,112 +821,126 @@
             break;
         case 'F':
             out.setf(std::ios::uppercase);
             // Falls through
         case 'f':
             out.setf(std::ios::fixed, std::ios::floatfield);
             break;
+        case 'A':
+            out.setf(std::ios::uppercase);
+            // Falls through
+        case 'a':
+#           ifdef _MSC_VER
+            // Workaround https://developercommunity.visualstudio.com/content/problem/520472/hexfloat-stream-output-does-not-ignore-precision-a.html
+            // by always setting maximum precision on MSVC to avoid precision
+            // loss for doubles.
+            out.precision(13);
+#           endif
+            out.setf(std::ios::fixed | std::ios::scientific, std::ios::floatfield);
+            break;
         case 'G':
             out.setf(std::ios::uppercase);
             // Falls through
         case 'g':
             out.setf(std::ios::dec, std::ios::basefield);
             // As in boost::format, let stream decide float format.
             out.flags(out.flags() & ~std::ios::floatfield);
             break;
-        case 'a': case 'A':
-            TINYFORMAT_ERROR("tinyformat: the %a and %A conversion specs "
-                             "are not supported");
-            break;
         case 'c':
             // Handled as special case inside formatValue()
             break;
         case 's':
-            if(precisionSet)
+            if (precisionSet)
                 ntrunc = static_cast<int>(out.precision());
-            // Make %s print booleans as "true" and "false"
+            // Make %s print Booleans as "true" and "false"
             out.setf(std::ios::boolalpha);
             break;
         case 'n':
             // Not supported - will cause problems!
             TINYFORMAT_ERROR("tinyformat: %n conversion spec not supported");
             break;
         case '\0':
             TINYFORMAT_ERROR("tinyformat: Conversion spec incorrectly "
                              "terminated by end of string");
             return c;
         default:
             break;
     }
-    if(intConversion && precisionSet && !widthSet)
-    {
+    if (intConversion && precisionSet && !widthSet) {
         // "precision" for integers gives the minimum number of digits (to be
         // padded with zeros on the left).  This isn't really supported by the
         // iostreams, but we can approximately simulate it with the width if
         // the width isn't otherwise used.
         out.width(out.precision() + widthExtra);
         out.setf(std::ios::internal, std::ios::adjustfield);
         out.fill('0');
     }
     return c+1;
 }
 
 
 //------------------------------------------------------------------------------
 inline void formatImpl(std::ostream& out, const char* fmt,
-                       const detail::FormatArg* formatters,
-                       int numFormatters)
+                       const detail::FormatArg* args,
+                       int numArgs)
 {
     // Saved stream state
     std::streamsize origWidth = out.width();
     std::streamsize origPrecision = out.precision();
     std::ios::fmtflags origFlags = out.flags();
     char origFill = out.fill();
 
-    for (int argIndex = 0; argIndex < numFormatters; ++argIndex)
-    {
-        // Parse the format string
+    // "Positional mode" means all format specs should be of the form "%n$..."
+    // with `n` an integer. We detect this in `streamStateFromFormat`.
+    bool positionalMode = false;
+    int argIndex = 0;
+    while (true) {
         fmt = printFormatStringLiteral(out, fmt);
+        if (*fmt == '\0') {
+            if (!positionalMode && argIndex < numArgs) {
+                TINYFORMAT_ERROR("tinyformat: Not enough conversion specifiers in format string");
+            }
+            break;
+        }
         bool spacePadPositive = false;
         int ntrunc = -1;
-        const char* fmtEnd = streamStateFromFormat(out, spacePadPositive, ntrunc, fmt,
-                                                   formatters, argIndex, numFormatters);
-        if (argIndex >= numFormatters)
-        {
-            // Check args remain after reading any variable width/precision
-            TINYFORMAT_ERROR("tinyformat: Not enough format arguments");
+        const char* fmtEnd = streamStateFromFormat(out, positionalMode, spacePadPositive, ntrunc, fmt,
+                                                   args, argIndex, numArgs);
+        // NB: argIndex may be incremented by reading variable width/precision
+        // in `streamStateFromFormat`, so do the bounds check here.
+        if (argIndex >= numArgs) {
+            TINYFORMAT_ERROR("tinyformat: Too many conversion specifiers in format string");
             return;
         }
-        const FormatArg& arg = formatters[argIndex];
+        const FormatArg& arg = args[argIndex];
         // Format the arg into the stream.
-        if(!spacePadPositive)
+        if (!spacePadPositive) {
             arg.format(out, fmt, fmtEnd, ntrunc);
-        else
-        {
+        }
+        else {
             // The following is a special case with no direct correspondence
             // between stream formatting and the printf() behaviour.  Simulate
             // it crudely by formatting into a temporary string stream and
             // munging the resulting string.
             std::ostringstream tmpStream;
             tmpStream.copyfmt(out);
             tmpStream.setf(std::ios::showpos);
             arg.format(tmpStream, fmt, fmtEnd, ntrunc);
             std::string result = tmpStream.str(); // allocates... yuck.
-            for(size_t i = 0, iend = result.size(); i < iend; ++i)
-                if(result[i] == '+') result[i] = ' ';
+            for (size_t i = 0, iend = result.size(); i < iend; ++i) {
+                if (result[i] == '+')
+                    result[i] = ' ';
+            }
             out << result;
         }
+        if (!positionalMode)
+            ++argIndex;
         fmt = fmtEnd;
     }
 
-    // Print remaining part of format string.
-    fmt = printFormatStringLiteral(out, fmt);
-    if(*fmt != '\0')
-        TINYFORMAT_ERROR("tinyformat: Too many conversion specifiers in format string");
-
     // Restore stream state
     out.width(origWidth);
     out.precision(origPrecision);
     out.flags(origFlags);
     out.fill(origFill);
 }
 
@@ -843,61 +952,65 @@
 /// A const reference to FormatList (typedef'd as FormatListRef) may be
 /// conveniently used to pass arguments to non-template functions: All type
 /// information has been stripped from the arguments, leaving just enough of a
 /// common interface to perform formatting as required.
 class FormatList
 {
     public:
-        FormatList(detail::FormatArg* formatters, int N)
-            : m_formatters(formatters), m_N(N) { }
+        FormatList(detail::FormatArg* args, int N)
+            : m_args(args), m_N(N) { }
 
         friend void vformat(std::ostream& out, const char* fmt,
                             const FormatList& list);
 
     private:
-        const detail::FormatArg* m_formatters;
+        const detail::FormatArg* m_args;
         int m_N;
 };
 
 /// Reference to type-opaque format list for passing to vformat()
 typedef const FormatList& FormatListRef;
 
 
 namespace detail {
 
 // Format list subclass with fixed storage to avoid dynamic allocation
-template<int N>
+template<std::size_t N>
 class FormatListN : public FormatList
 {
     public:
 #ifdef TINYFORMAT_USE_VARIADIC_TEMPLATES
         template<typename... Args>
         FormatListN(const Args&... args)
             : FormatList(&m_formatterStore[0], N),
             m_formatterStore { FormatArg(args)... }
         { static_assert(sizeof...(args) == N, "Number of args must be N"); }
 #else // C++98 version
         void init(int) {}
-#       define TINYFORMAT_MAKE_FORMATLIST_CONSTRUCTOR(n)       \
-                                                               \
-        template<TINYFORMAT_ARGTYPES(n)>                       \
-        FormatListN(TINYFORMAT_VARARGS(n))                     \
-            : FormatList(&m_formatterStore[0], n)              \
-        { assert(n == N); init(0, TINYFORMAT_PASSARGS(n)); }   \
-                                                               \
-        template<TINYFORMAT_ARGTYPES(n)>                       \
-        void init(int i, TINYFORMAT_VARARGS(n))                \
-        {                                                      \
-            m_formatterStore[i] = FormatArg(v1);               \
-            init(i+1 TINYFORMAT_PASSARGS_TAIL(n));             \
+#       define TINYFORMAT_MAKE_FORMATLIST_CONSTRUCTOR(n)                \
+                                                                        \
+        template<TINYFORMAT_ARGTYPES(n)>                                \
+        FormatListN(TINYFORMAT_VARARGS(n))                              \
+            : FormatList(&m_formatterStore[0], n)                       \
+        { TINYFORMAT_ASSERT(n == N); init(0, TINYFORMAT_PASSARGS(n)); } \
+                                                                        \
+        template<TINYFORMAT_ARGTYPES(n)>                                \
+        void init(int i, TINYFORMAT_VARARGS(n))                         \
+        {                                                               \
+            m_formatterStore[i] = FormatArg(v1);                        \
+            init(i+1 TINYFORMAT_PASSARGS_TAIL(n));                      \
         }
 
         TINYFORMAT_FOREACH_ARGNUM(TINYFORMAT_MAKE_FORMATLIST_CONSTRUCTOR)
 #       undef TINYFORMAT_MAKE_FORMATLIST_CONSTRUCTOR
 #endif
+        FormatListN(const FormatListN& other)
+            : FormatList(&m_formatterStore[0], N)
+        { std::copy(&other.m_formatterStore[0], &other.m_formatterStore[N],
+                    &m_formatterStore[0]); }
 
     private:
         FormatArg m_formatterStore[N];
 };
 
 // Special 0-arg version - MSVC says zero-sized C array in struct is nonstandard
 template<> class FormatListN<0> : public FormatList
@@ -944,15 +1057,15 @@
 
 /// Format list of arguments to the stream according to the given format string.
 ///
 /// The name vformat() is chosen for the semantic similarity to vprintf(): the
 /// list of format arguments is held in a single function argument.
 inline void vformat(std::ostream& out, const char* fmt, FormatListRef list)
 {
-    detail::formatImpl(out, fmt, list.m_formatters, list.m_N);
+    detail::formatImpl(out, fmt, list.m_args, list.m_N);
 }
 
 
 #ifdef TINYFORMAT_USE_VARIADIC_TEMPLATES
 
 /// Format list of arguments to the stream according to given format string.
 template<typename... Args>
```

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/attr.h` & `jotdown-2.0.2/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/buffer_info.h` & `jotdown-2.0.2/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/cast.h` & `jotdown-2.0.2/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/chrono.h` & `jotdown-2.0.2/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/complex.h` & `jotdown-2.0.2/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/detail/class.h` & `jotdown-2.0.2/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/detail/common.h` & `jotdown-2.0.2/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/detail/descr.h` & `jotdown-2.0.2/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/detail/init.h` & `jotdown-2.0.2/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/detail/internals.h` & `jotdown-2.0.2/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/detail/typeid.h` & `jotdown-2.0.2/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/eigen.h` & `jotdown-2.0.2/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/embed.h` & `jotdown-2.0.2/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/eval.h` & `jotdown-2.0.2/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/functional.h` & `jotdown-2.0.2/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/iostream.h` & `jotdown-2.0.2/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/numpy.h` & `jotdown-2.0.2/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/operators.h` & `jotdown-2.0.2/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/options.h` & `jotdown-2.0.2/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/pybind11.h` & `jotdown-2.0.2/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/pytypes.h` & `jotdown-2.0.2/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/stl.h` & `jotdown-2.0.2/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/include/pybind11/stl_bind.h` & `jotdown-2.0.2/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/tests/constructor_stats.h` & `jotdown-2.0.2/pybind11/tests/constructor_stats.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/tests/local_bindings.h` & `jotdown-2.0.2/pybind11/tests/local_bindings.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/tests/object.h` & `jotdown-2.0.2/pybind11/tests/object.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/pybind11/tests/pybind11_tests.h` & `jotdown-2.0.2/pybind11/tests/pybind11_tests.h`

 * *Files identical despite different names*

### Comparing `jotdown-2.0.1/setup.py` & `jotdown-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 # Get the long description from the README file
 with open(Path("README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="jotdown",
-    version="2.0.1",
+    version="2.0.2",
     description="Jotdown structrured document language, C++ to python wrapper module.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lainproliant/jotdown",
     author="Lain Musgrove (lainproliant)",
     author_email="lainproliant@gmail.com",
     license="BSD",
```

### Comparing `jotdown-2.0.1/src/jotdown.cpp` & `jotdown-2.0.2/src/jotdown.cpp`

 * *Files 18% similar despite different names*

```diff
@@ -17,43 +17,44 @@
 
 #include <functional>
 
 namespace jotdown {
 namespace python {
 
 namespace py = pybind11;
+namespace json = moonlight::json;
 
 //-------------------------------------------------------------------
 // Utilities and Typedefs
 //
 template<class T, typename... options>
 using shared_class = py::class_<T, std::shared_ptr<T>, options...>;
 
 //-------------------------------------------------------------------
-inline py::dict json_to_dict(const JSON& json) {
+inline py::dict json_to_dict(const json::Object& json) {
     auto pyjson = py::module::import("json");
-    return pyjson.attr("loads")(json.to_string());
+    return pyjson.attr("loads")(json::to_string(json));
 }
 
 //-------------------------------------------------------------------
-class ObjectTrampoline : public object::Object {
+class ObjectTrampoline : public Object {
 public:
-    using object::Object::Object;
+    using Object::Object;
 
-    object::obj_t clone() const override {
+    obj_t clone() const override {
         PYBIND11_OVERLOAD_PURE(
-            object::obj_t,
-            object::Object,
+            obj_t,
+            Object,
             clone
         );
     }
 };
 
 //-------------------------------------------------------------------
-using obj_class = shared_class<object::Object, ObjectTrampoline>;
+using obj_class = shared_class<Object, ObjectTrampoline>;
 
 
 //-------------------------------------------------------------------
 // API Declaration
 //
 void declare_api(py::module& m) {
     m.def("load", [](const std::string& filename) {
@@ -62,34 +63,34 @@
     m.def("load", [](std::istream& infile) {
         return load(infile);
     });
     m.def("save", [](std::shared_ptr<const Document> document,
                      const std::string& filename) {
         save(document, filename);
     });
-    m.def("q", [](const std::vector<object::obj_t>& objects, const std::string& query_str) {
-        return query::parse(query_str).select(objects);
+    m.def("q", [](const std::vector<obj_t>& objects, const std::string& query_str) {
+        return q::parse(query_str).select(objects);
     });
 }
 
 
 //-------------------------------------------------------------------
 // Object Declaration
 //
-py::class_<object::Config> declare_object_config(py::module& m) {
-    py::class_<object::Config> object_config(m, "ObjectConfig");
+py::class_<Config> declare_object_config(py::module& m) {
+    py::class_<Config> object_config(m, "ObjectConfig");
     object_config
         .def(py::init<>())
-        .def_readwrite("list_indent", &object::Config::list_indent);
+        .def_readwrite("list_indent", &Config::list_indent);
     return object_config;
 }
 
 //-------------------------------------------------------------------
 void declare_object_error(py::module& m) {
-    py::register_exception<object::ObjectError>(m, "ObjectError");
+    py::register_exception<ObjectError>(m, "ObjectError");
 }
 
 //-------------------------------------------------------------------
 py::class_<Location> declare_location(py::module& m) {
     auto location = py::class_<Location>(m, "Location")
         .def(py::init([]() {
             return NOWHERE;
@@ -149,395 +150,392 @@
         });
     return range;
 }
 
 //-------------------------------------------------------------------
 obj_class declare_object(py::module& m) {
     auto object = obj_class(m, "Object");
-    py::enum_<object::Object::Type>(object, "Type")
-        .value("NONE", object::Object::Type::NONE)
-        .value("ANCHOR", object::Object::Type::ANCHOR)
-        .value("CODE", object::Object::Type::CODE)
-        .value("CODE_BLOCK", object::Object::Type::CODE_BLOCK)
-        .value("DOCUMENT", object::Object::Type::DOCUMENT)
-        .value("HASHTAG", object::Object::Type::HASHTAG)
-        .value("LINE_BREAK", object::Object::Type::LINE_BREAK)
-        .value("ORDERED_LIST", object::Object::Type::ORDERED_LIST)
-        .value("ORDERED_LIST_ITEM", object::Object::Type::ORDERED_LIST_ITEM)
-        .value("REF", object::Object::Type::REF)
-        .value("REF_INDEX", object::Object::Type::REF_INDEX)
-        .value("SECTION", object::Object::Type::SECTION)
-        .value("TEXT", object::Object::Type::TEXT)
-        .value("TEXT_BLOCK", object::Object::Type::TEXT_CONTENT)
-        .value("UNORDERED_LIST", object::Object::Type::UNORDERED_LIST)
-        .value("UNORDERED_LIST_ITEM", object::Object::Type::UNORDERED_LIST_ITEM);
+    py::enum_<Object::Type>(object, "Type")
+        .value("NONE", Object::Type::NONE)
+        .value("ANCHOR", Object::Type::ANCHOR)
+        .value("CODE", Object::Type::CODE)
+        .value("CODE_BLOCK", Object::Type::CODE_BLOCK)
+        .value("DOCUMENT", Object::Type::DOCUMENT)
+        .value("HASHTAG", Object::Type::HASHTAG)
+        .value("LINE_BREAK", Object::Type::LINE_BREAK)
+        .value("ORDERED_LIST", Object::Type::ORDERED_LIST)
+        .value("ORDERED_LIST_ITEM", Object::Type::ORDERED_LIST_ITEM)
+        .value("REF", Object::Type::REF)
+        .value("REF_INDEX", Object::Type::REF_INDEX)
+        .value("SECTION", Object::Type::SECTION)
+        .value("TEXT", Object::Type::TEXT)
+        .value("TEXT_BLOCK", Object::Type::TEXT_CONTENT)
+        .value("UNORDERED_LIST", Object::Type::UNORDERED_LIST)
+        .value("UNORDERED_LIST_ITEM", Object::Type::UNORDERED_LIST_ITEM);
 
-    object.def("type", &object::Object::type);
-    object.def("range", [](const object::Object& self) {
+    object.def("type", &Object::type);
+    object.def("range", [](const Object& self) {
         return self.range();
     });
     object.def_property(
         "range",
-        [](const object::Object& self) {
+        [](const Object& self) {
             return self.range();
         },
-        [](object::Object& self, const Range& range) {
+        [](Object& self, const Range& range) {
             self.range(range);
         });
     object.def_property_readonly(
         "parent",
-        [](const object::Object& self) {
+        [](const Object& self) {
             return self.cparent();
         });
-    object.def_static("type_name", [](object::Object::Type type) {
-        return object::Object::type_name(type);
+    object.def_static("type_name", [](Object::Type type) {
+        return Object::type_name(type);
     });
     object.def_property_static(
         "config",
         []() {
-            return object::Object::config();
+            return Object::config();
         },
-        [](const object::Config& config) {
-            object::Object::config() = config;
+        [](const Config& config) {
+            Object::config() = config;
         });
-    object.def("clone", [](const object::Object& obj) {
+    object.def("clone", [](const Object& obj) {
         return obj.clone();
     });
-    object.def("q", [](std::shared_ptr<object::Object> object, const std::string& query_str) {
-        return query::parse(query_str).select({object});
+    object.def("query", [](std::shared_ptr<Object> object, const std::string& query_str) {
+        return q::parse(query_str).select({object});
     });
-    object.def("to_json", [](const object::Object& obj) {
+    object.def("to_json", [](const Object& obj) {
         return json_to_dict(obj.to_json());
     });
-    object.def("to_jotdown", [](const object::Object& obj) {
+    object.def("to_jotdown", [](const Object& obj) {
         return obj.to_jotdown();
     });
-    object.def("query", [](object::obj_t obj, const std::string& query_str) {
-        return query::parse(query_str).select({obj});
-    });
-    object.def("__repr__", [](const object::Object& obj) {
+    object.def("__repr__", [](const Object& obj) {
         return obj.repr();
     });
 
     return object;
 }
 
 
 //-------------------------------------------------------------------
 // Container Declaration
 //
-shared_class<object::Container> declare_container(
+shared_class<Container> declare_container(
     py::module& m, obj_class& obj) {
-    auto container = shared_class<object::Container>(m, "Container", obj)
-        .def_property_readonly("contents", [](const object::Container& self) {
+    auto container = shared_class<Container>(m, "Container", obj)
+        .def_property_readonly("contents", [](const Container& self) {
             return self.contents();
         })
-    .def("clear", [](object::Container& self) {
+    .def("clear", [](Container& self) {
         self.clear();
     })
-    .def("add", [](object::Container& self, object::obj_t obj) {
+    .def("add", [](Container& self, obj_t obj) {
         return self.add(obj);
     })
-    .def("insert_before", [](object::Container& self, object::cobj_t pivot, object::obj_t obj) {
+    .def("insert_before", [](Container& self, cobj_t pivot, obj_t obj) {
         return self.insert_before(pivot, obj);
     })
-    .def("insert_after", [](object::Container& self, object::cobj_t pivot, object::obj_t obj) {
+    .def("insert_after", [](Container& self, cobj_t pivot, obj_t obj) {
         return self.insert_after(pivot, obj);
     })
-    .def("remove", [](object::Container& self, object::obj_t obj) {
+    .def("remove", [](Container& self, obj_t obj) {
         self.remove(obj);
     }, py::arg("obj"))
-    .def("shift_up", [](object::Container& self, object::cobj_t obj) {
+    .def("shift_up", [](Container& self, cobj_t obj) {
         self.shift_up(obj);
     }, py::arg("obj"))
-    .def("shift_down", [](object::Container& self, object::cobj_t obj) {
+    .def("shift_down", [](Container& self, cobj_t obj) {
         self.shift_down(obj);
     }, py::arg("obj"))
-    .def("__call__", [](std::shared_ptr<object::Container> self) {
+    .def("__call__", [](std::shared_ptr<Container> self) {
         return self->contents();
     })
-    .def("__call__", [](std::shared_ptr<object::Container> self, py::args args) {
+    .def("__call__", [](std::shared_ptr<Container> self, py::args args) {
         for (auto arg : args) {
-            self->add(arg.cast<object::obj_t>());
+            self->add(arg.cast<obj_t>());
         }
         return self;
     });
 
     return container;
 }
 
 
 //-------------------------------------------------------------------
 // Document Declaration
 //
-shared_class<object::Document> declare_document(
+shared_class<Document> declare_document(
     py::module& m,
-    shared_class<object::Container>& container) {
+    shared_class<Container>& container) {
 
-    auto document = shared_class<object::Document>(m, "Document", container)
+    auto document = shared_class<Document>(m, "Document", container)
         .def(py::init<>())
         .def_property(
             "front_matter",
-            [](const object::Document& self) {
+            [](const Document& self) {
                 return self.front_matter();
             },
-            [](object::Document& self, std::shared_ptr<object::FrontMatter> front_matter) {
+            [](Document& self, std::shared_ptr<FrontMatter> front_matter) {
                 self.front_matter(front_matter);
             })
         .def("save", [](std::shared_ptr<const Document> document,
                         const std::string& filename) {
             jotdown::save(document, filename);
         });
     return document;
 }
 
 
 //-------------------------------------------------------------------
 // Declare Section
 //
-shared_class<object::Section> declare_section(
+shared_class<Section> declare_section(
     py::module& m,
-    shared_class<object::Container>& container) {
+    shared_class<Container>& container) {
 
-    auto section = shared_class<object::Section>(m, "Section", container)
+    auto section = shared_class<Section>(m, "Section", container)
     .def(py::init([](int level) {
-        return object::Section::create(level);
+        return Section::create(level);
     }), py::arg("level") = 1)
     .def(py::init([](const std::string& header_text, int level) {
-        auto header = std::make_shared<object::TextContent>();
-        header->add(std::make_shared<object::Text>(header_text));
-        auto section = object::Section::create(level);
+        auto header = TextContent::create();
+        header->add(Text::create(header_text));
+        auto section = Section::create(level);
         section->header(header);
         return section;
     }), py::arg("header_text"), py::arg("level") = 1)
-    .def(py::init([](std::shared_ptr<object::TextContent> header, int level) {
-        auto section = object::Section::create(level);
+    .def(py::init([](std::shared_ptr<TextContent> header, int level) {
+        auto section = Section::create(level);
         section->header(header);
         return section;
     }), py::arg("header"), py::arg("level") = 1)
     .def_property(
         "header",
-        [](const object::Section& self) {
+        [](const Section& self) {
             return self.cheader();
         },
-        [&](object::Section& self, std::shared_ptr<object::TextContent> header) {
+        [&](Section& self, std::shared_ptr<TextContent> header) {
             self.header(header);
         });
 
     return section;
 }
 
 
 //-------------------------------------------------------------------
 // List Declaration
 //
-shared_class<object::List> declare_list(
+shared_class<List> declare_list(
     py::module& m,
-    shared_class<object::Container>& container) {
+    shared_class<Container>& container) {
 
-    auto list = shared_class<object::List>(m, "List", container)
-        .def_property_readonly("level", [](const object::List& list) {
+    auto list = shared_class<List>(m, "List", container)
+        .def_property_readonly("level", [](const List& list) {
             return list.level();
         });
     return list;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::ListItem> declare_list_item(
+shared_class<ListItem> declare_list_item(
     py::module& m,
-    shared_class<object::Container>& container) {
+    shared_class<Container>& container) {
 
-    auto li = shared_class<object::ListItem>(m, "ListItem", container)
+    auto li = shared_class<ListItem>(m, "ListItem", container)
         .def_property(
             "text",
-            [](const object::ListItem& li) {
+            [](const ListItem& li) {
                 return li.ctext();
             },
-            [](object::ListItem& li,
-               std::shared_ptr<object::TextContent> text) {
+            [](ListItem& li,
+               std::shared_ptr<TextContent> text) {
                 li.text(text);
             }
         )
         .def_property_readonly(
             "level",
-            [](const object::ListItem& li) {
+            [](const ListItem& li) {
                 return li.level();
             }
         )
         .def_property(
             "status",
-            [](const object::ListItem& li) {
+            [](const ListItem& li) {
                 return li.status();
             },
-            [](object::ListItem& li, const std::string& status) {
+            [](ListItem& li, const std::string& status) {
                 li.status(status);
             });
     return li;
 }
 
 
 //-------------------------------------------------------------------
 // Declare OrderedList
 //
-shared_class<object::OrderedList> declare_ordered_list(
+shared_class<OrderedList> declare_ordered_list(
     py::module& m,
-    shared_class<object::List>& list) {
+    shared_class<List>& list) {
 
-    auto ol = shared_class<object::OrderedList>(m, "OrderedList", list)
+    auto ol = shared_class<OrderedList>(m, "OrderedList", list)
         .def(py::init<>());
     return ol;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::OrderedListItem> declare_ordered_list_item(
+shared_class<OrderedListItem> declare_ordered_list_item(
     py::module& m,
-    shared_class<object::ListItem>& li) {
+    shared_class<ListItem>& li) {
 
-    auto oli = shared_class<object::OrderedListItem>(m, "OrderedListItem", li)
+    auto oli = shared_class<OrderedListItem>(m, "OrderedListItem", li)
     .def(py::init([](const std::string& ordinal) {
-        return object::OrderedListItem::create(ordinal);
+        return OrderedListItem::create(ordinal);
     }), py::arg("ordinal"));
     return oli;
 }
 
 
 //-------------------------------------------------------------------
 // Declare UnorderedList
 //
-shared_class<object::UnorderedList> declare_unordered_list(
+shared_class<UnorderedList> declare_unordered_list(
     py::module& m,
-    shared_class<object::List>& list) {
+    shared_class<List>& list) {
 
-    auto ul = shared_class<object::UnorderedList>(m, "UnorderedList", list)
+    auto ul = shared_class<UnorderedList>(m, "UnorderedList", list)
         .def(py::init<>());
     return ul;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::UnorderedListItem> declare_unordered_list_item(
+shared_class<UnorderedListItem> declare_unordered_list_item(
     py::module& m,
-    shared_class<object::ListItem>& li) {
+    shared_class<ListItem>& li) {
 
-    auto uli = shared_class<object::UnorderedListItem>(
+    auto uli = shared_class<UnorderedListItem>(
         m, "UnorderedListItem", li)
         .def(py::init([]() {
-            return object::UnorderedListItem::create();
+            return UnorderedListItem::create();
         }));
     return uli;
 }
 
 
 //-------------------------------------------------------------------
 // Declare TextContent
 //
-shared_class<object::TextContent> declare_text_content(
+shared_class<TextContent> declare_text_content(
     py::module& m,
-    shared_class<object::Container>& container) {
+    shared_class<Container>& container) {
 
-    auto text_content = shared_class<object::TextContent>(
+    auto text_content = shared_class<TextContent>(
         m, "TextContent", container)
         .def(py::init<>())
         .def(py::init([](const std::string& text) {
-            auto content = std::make_shared<object::TextContent>();
-            content->add(std::make_shared<object::Text>(text));
+            auto content = TextContent::create();
+            content->add(Text::create(text));
             return content;
         }));
 
     return text_content;
 }
 
 
 //-------------------------------------------------------------------
 // Declare Simple Types
 //
-shared_class<object::Anchor> declare_anchor(py::module& m, obj_class& obj) {
-    auto anchor = shared_class<object::Anchor>(m, "Anchor", obj)
+shared_class<Anchor> declare_anchor(py::module& m, obj_class& obj) {
+    auto anchor = shared_class<Anchor>(m, "Anchor", obj)
         .def(py::init<const std::string&>(), py::arg("name"))
-        .def_property_readonly("name", &object::Anchor::name);
+        .def_property_readonly("name", &Anchor::name);
     return anchor;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::Text> declare_text(py::module& m, obj_class& obj) {
-    auto text = shared_class<object::Text>(m, "Text", obj)
+shared_class<Text> declare_text(py::module& m, obj_class& obj) {
+    auto text = shared_class<Text>(m, "Text", obj)
         .def(py::init<const std::string&>(), py::arg("text"))
-        .def_property_readonly("text", &object::Text::text);
+        .def_property_readonly("text", &Text::text);
     return text;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::Hashtag> declare_hashtag(py::module& m, obj_class& obj) {
-    auto hashtag = shared_class<object::Hashtag>(m, "Hashtag", obj)
+shared_class<Hashtag> declare_hashtag(py::module& m, obj_class& obj) {
+    auto hashtag = shared_class<Hashtag>(m, "Hashtag", obj)
         .def(py::init<const std::string&>(), py::arg("tag"))
-        .def_property_readonly("tag", &object::Hashtag::tag);
+        .def_property_readonly("tag", &Hashtag::tag);
     return hashtag;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::LineBreak> declare_line_break(py::module& m, obj_class& obj) {
-    auto line_break = shared_class<object::LineBreak>(m, "LineBreak", obj)
+shared_class<LineBreak> declare_line_break(py::module& m, obj_class& obj) {
+    auto line_break = shared_class<LineBreak>(m, "LineBreak", obj)
         .def(py::init<>());
     return line_break;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::Code> declare_code(py::module& m, obj_class& obj) {
-    auto code = shared_class<object::Code>(m, "Code", obj)
+shared_class<Code> declare_code(py::module& m, obj_class& obj) {
+    auto code = shared_class<Code>(m, "Code", obj)
         .def(py::init<const std::string&>(), py::arg("code"))
-        .def_property_readonly("code", &object::Code::code);
+        .def_property_readonly("code", &Code::code);
     return code;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::Ref> declare_ref(py::module& m, obj_class& obj) {
-    auto ref = shared_class<object::Ref>(m, "Ref", obj)
+shared_class<Ref> declare_ref(py::module& m, obj_class& obj) {
+    auto ref = shared_class<Ref>(m, "Ref", obj)
         .def(py::init<const std::string&, const std::string&>(),
              py::arg("link"), py::arg("text") = "")
-        .def_property_readonly("link", &object::Ref::link)
-        .def_property_readonly("text", &object::Ref::text);
+        .def_property_readonly("link", &Ref::link)
+        .def_property_readonly("text", &Ref::text);
     return ref;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::IndexedRef> declare_indexed_ref(py::module& m, obj_class& obj) {
-    auto indexed_ref = shared_class<object::IndexedRef>(m, "IndexedRef", obj)
+shared_class<IndexedRef> declare_indexed_ref(py::module& m, obj_class& obj) {
+    auto indexed_ref = shared_class<IndexedRef>(m, "IndexedRef", obj)
         .def(py::init<const std::string&, const std::string&>(),
              py::arg("text"), py::arg("index_name"))
-        .def_property_readonly("index_name", &object::IndexedRef::index_name)
-        .def_property_readonly("text", &object::IndexedRef::text);
+        .def_property_readonly("index_name", &IndexedRef::index_name)
+        .def_property_readonly("text", &IndexedRef::text);
     return indexed_ref;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::CodeBlock> declare_code_block(py::module& m, obj_class& obj) {
-    auto code_block = shared_class<object::CodeBlock>(m, "CodeBlock", obj)
+shared_class<CodeBlock> declare_code_block(py::module& m, obj_class& obj) {
+    auto code_block = shared_class<CodeBlock>(m, "CodeBlock", obj)
         .def(py::init<const std::string&, const std::string&>(),
              py::arg("code"), py::arg("language") = "")
-        .def_property_readonly("code", &object::CodeBlock::code)
-        .def_property_readonly("language", &object::CodeBlock::language);
+        .def_property_readonly("code", &CodeBlock::code)
+        .def_property_readonly("language", &CodeBlock::language);
     return code_block;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::FrontMatter> declare_front_matter(py::module& m, obj_class& obj) {
-    auto code_block = shared_class<object::FrontMatter>(m, "FrontMatter", obj)
+shared_class<FrontMatter> declare_front_matter(py::module& m, obj_class& obj) {
+    auto code_block = shared_class<FrontMatter>(m, "FrontMatter", obj)
         .def(py::init<const std::string&, const std::string&>(),
              py::arg("code"), py::arg("language") = "")
-        .def_property_readonly("code", &object::FrontMatter::code)
-        .def_property_readonly("language", &object::FrontMatter::language);
+        .def_property_readonly("code", &FrontMatter::code)
+        .def_property_readonly("language", &FrontMatter::language);
     return code_block;
 }
 
 //-------------------------------------------------------------------
-shared_class<object::RefIndex> declare_ref_index(py::module& m, obj_class& obj) {
-    auto ref_index = shared_class<object::RefIndex>(m, "RefIndex", obj)
+shared_class<RefIndex> declare_ref_index(py::module& m, obj_class& obj) {
+    auto ref_index = shared_class<RefIndex>(m, "RefIndex", obj)
         .def(py::init<const std::string&, const std::string&>(),
              py::arg("name"), py::arg("link"))
-        .def_property_readonly("name", &object::RefIndex::name)
-        .def_property_readonly("link", &object::RefIndex::link);
+        .def_property_readonly("name", &RefIndex::name)
+        .def_property_readonly("link", &RefIndex::link);
     return ref_index;
 }
 
 //-------------------------------------------------------------------
 // Declare Python Module
 //
 PYBIND11_MODULE(jotdown, m) {
```

