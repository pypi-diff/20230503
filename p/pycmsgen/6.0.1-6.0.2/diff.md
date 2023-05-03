# Comparing `tmp/pycmsgen-6.0.1.tar.gz` & `tmp/pycmsgen-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycmsgen-6.0.1.tar", last modified: Wed May  3 19:07:01 2023, max compression
+gzip compressed data, was "pycmsgen-6.0.2.tar", last modified: Wed May  3 19:44:57 2023, max compression
```

## Comparing `pycmsgen-6.0.1.tar` & `pycmsgen-6.0.2.tar`

### file list

```diff
@@ -1,124 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:07:01.062220 pycmsgen-6.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-03 19:07:01.062220 pycmsgen-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:07:01.050220 pycmsgen-6.0.1/python/
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/python/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:07:01.050220 pycmsgen-6.0.1/python/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/python/src/GitSHA1.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26460 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/python/src/pycmsgen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-03 19:07:01.062220 pycmsgen-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3377 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:07:01.062220 pycmsgen-6.0.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/GitSHA1.h
--rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/MersenneTwister.h
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/Vec.h
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/XAlloc.h
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/alg.h
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/avgcalc.h
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/bitarray.h
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/boundedqueue.h
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/clabstraction.h
--rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/clause.h
--rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/clauseallocator.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/clauseallocator.h
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/clausecleaner.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/clausecleaner.h
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/clauseusagestats.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/clauseusagestats.h
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/cloffset.h
--rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/cmsgen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/cmsgen.h
--rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/cnf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/cnf.h
--rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/completedetachreattacher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/completedetachreattacher.h
--rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/constants.h
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/cset.h
--rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/dimacsparser.h
--rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/distillerlong.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/distillerlong.h
--rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/distillerlongwithimpl.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/distillerlongwithimpl.h
--rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/drat.h
--rw-r--r--   0 runner    (1001) docker     (123)    32702 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/gaussian.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/gaussian.h
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/gausswatched.h
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/gqueuedata.h
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/hasher.h
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/heap.h
--rw-r--r--   0 runner    (1001) docker     (123)    31093 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/hyperengine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/hyperengine.h
--rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/implcache.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/implcache.h
--rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/intree.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/intree.h
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/main.h
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/main_common.h
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/matrixfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/matrixfinder.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:07:01.062220 pycmsgen-6.0.1/src/msvc/
--rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/msvc/stdint.h
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/mystack.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/nomutex.h
--rw-r--r--   0 runner    (1001) docker     (123)    95034 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/occsimplifier.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/occsimplifier.h
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/packedmatrix.h
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/packedrow.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/packedrow.h
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/popcnt.h
--rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/prober.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/prober.h
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/propby.h
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/propby_backup.h
--rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/propbyforgraph.h
--rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/propengine.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/propengine.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:07:01.062220 pycmsgen-6.0.1/src/pycmsgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-03 19:07:01.000000 pycmsgen-6.0.1/src/pycmsgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-03 19:07:01.000000 pycmsgen-6.0.1/src/pycmsgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/reducedb.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/reducedb.h
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/sccfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/sccfinder.h
--rw-r--r--   0 runner    (1001) docker     (123)    83433 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/searcher.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/searcher.h
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/searchhist.h
--rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/searchstats.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/searchstats.h
--rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/shareddata.h
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/signalcode.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/signalcode.h
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/simplefile.h
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/solutionextender.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/solutionextender.h
--rw-r--r--   0 runner    (1001) docker     (123)    95762 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/solver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    19985 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/solver.h
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/solverconf.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/solverconf.h
--rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/solvertypes.h
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/solvertypesmini.h
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/stamp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/stamp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/str_impl_w_impl_stamp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/str_impl_w_impl_stamp.h
--rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/streambuffer.h
--rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/subsumeimplicit.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/subsumeimplicit.h
--rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/subsumestrengthen.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/subsumestrengthen.h
--rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/time_mem.h
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/touchlist.h
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/trim.h
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/vardata.h
--rw-r--r--   0 runner    (1001) docker     (123)    32001 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/varreplacer.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/varreplacer.h
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/varupdatehelper.h
--rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/watchalgos.h
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/watcharray.h
--rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/watched.h
--rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/watched_backup.h
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/xor.h
--rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/xorfinder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-03 19:06:41.000000 pycmsgen-6.0.1/src/xorfinder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.676194 pycmsgen-6.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-03 19:44:57.676194 pycmsgen-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.652193 pycmsgen-6.0.2/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/python/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.652193 pycmsgen-6.0.2/python/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/python/src/GitSHA1.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26826 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/python/src/pycmsgen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-03 19:44:57.676194 pycmsgen-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.672193 pycmsgen-6.0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/GitSHA1.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14105 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/MersenneTwister.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/Vec.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/XAlloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/alg.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/avgcalc.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/bitarray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/boundedqueue.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clabstraction.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9958 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clause.h
+-rw-r--r--   0 runner    (1001) docker     (123)    13152 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clauseallocator.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clauseallocator.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clausecleaner.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clausecleaner.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clauseusagestats.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/clauseusagestats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cloffset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20528 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cmsgen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cmsgen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19298 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cnf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cnf.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5793 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/completedetachreattacher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/completedetachreattacher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/constants.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/cset.h
+-rw-r--r--   0 runner    (1001) docker     (123)    15765 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/dimacsparser.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/distillerlong.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/distillerlong.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16705 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/distillerlongwithimpl.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/distillerlongwithimpl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7445 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/drat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32702 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/gaussian.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/gaussian.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/gausswatched.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/gqueuedata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/hasher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/heap.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31093 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/hyperengine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/hyperengine.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19182 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/implcache.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/implcache.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12949 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/intree.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/intree.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/main.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/main_common.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/matrixfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/matrixfinder.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.672193 pycmsgen-6.0.2/src/msvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7728 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/msvc/stdint.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/mystack.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/nomutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)    95034 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/occsimplifier.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16439 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/occsimplifier.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/packedmatrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/packedrow.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/packedrow.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/popcnt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    28904 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/prober.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9618 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/prober.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propby.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propby_backup.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propbyforgraph.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14124 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propengine.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/propengine.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:44:57.676194 pycmsgen-6.0.2/src/pycmsgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-03 19:44:57.000000 pycmsgen-6.0.2/src/pycmsgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-03 19:44:57.000000 pycmsgen-6.0.2/src/pycmsgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/reducedb.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/reducedb.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/sccfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/sccfinder.h
+-rw-r--r--   0 runner    (1001) docker     (123)    83433 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searcher.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    18542 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searcher.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searchhist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searchstats.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/searchstats.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/shareddata.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/signalcode.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/simplefile.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solutionextender.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solutionextender.h
+-rw-r--r--   0 runner    (1001) docker     (123)    95790 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19985 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solver.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solverconf.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solverconf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10261 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solvertypes.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/solvertypesmini.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/stamp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/stamp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6136 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/str_impl_w_impl_stamp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/str_impl_w_impl_stamp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6101 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/streambuffer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6233 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/subsumeimplicit.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/subsumeimplicit.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27861 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/subsumestrengthen.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/subsumestrengthen.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4195 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/time_mem.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/touchlist.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/trim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/vardata.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32001 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/varreplacer.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     9286 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/varreplacer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/varupdatehelper.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4446 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/watchalgos.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/watcharray.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8200 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/watched.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8636 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/watched_backup.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/xor.h
+-rw-r--r--   0 runner    (1001) docker     (123)    25049 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/xorfinder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10171 2023-05-03 19:44:33.000000 pycmsgen-6.0.2/src/xorfinder.h
```

### Comparing `pycmsgen-6.0.1/LICENSE.txt` & `pycmsgen-6.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/PKG-INFO` & `pycmsgen-6.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycmsgen
-Version: 6.0.1
+Version: 6.0.2
 Summary: Bindings to CMSGen, uniform-like sampler
 Home-page: https://github.com/meelgroup/cmsgen
 Author-email: Mate Soos <soos.mate@gmail.com>
 Maintainer-email: Mate Soos <soos.mate@gmail.com>
 License: CryptoMiniSat Copyright (c) Mate Soos 2009-2018
         All rights reserved.
```

### Comparing `pycmsgen-6.0.1/pyproject.toml` & `pycmsgen-6.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel", "toml", "pathlib"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycmsgen"
-version = "6.0.1"
+version = "6.0.2"
 description = "Bindings to CMSGen, uniform-like sampler"
 keywords = ["sat", "sampling"]
 license = { file = "LICENSE.txt" }
 maintainers = [{name="Mate Soos", email="soos.mate@gmail.com"}]
 authors = [{name="Mate Soos", email="soos.mate@gmail.com"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `pycmsgen-6.0.1/python/README.md` & `pycmsgen-6.0.2/python/README.md`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/python/src/GitSHA1.cpp` & `pycmsgen-6.0.2/python/src/GitSHA1.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/python/src/pycmsgen.cpp` & `pycmsgen-6.0.2/python/src/pycmsgen.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 **********************************/
 
 #include <Python.h>
 #include <structmember.h>
 #include <limits>
 #include <cassert>
 #include <algorithm>
+#include <signal.h>
 #include "../../src/cmsgen.h"
 #include "solvertypesmini.h"
 using namespace CMSGen;
 
 #define MODULE_NAME "pycmsgen"
 #define MODULE_DOC "CMSGen almost-uniform sampler."
 
@@ -48,14 +49,16 @@
     std::vector<Lit> tmp_cl_lits;
 
     int verbose;
     double time_limit;
     long confl_limit;
 } Solver;
 
+typedef void (*sighandler_t)(int);
+
 static const char solver_create_docstring[] = \
 "Solver(verbose=0, time_limit=max_numeric_limits, confl_limit=max_numeric_limits)\n\
 Create Solver object.\n\
 \n\
 :param verbose: Verbosity level: 0: nothing printed; 15: very verbose.\n\
 :param time_limit: Propagation limit: abort after this many seconds has elapsed.\n\
 :param confl_limit: Propagation limit: abort after this many conflicts.\n\
@@ -631,17 +634,28 @@
 :param confl_limit: (Optional) Allows the user to set a conflict limit for just\n\
     this solve.\n\
 :type confl_limit: <long>\n\
 :return: Whether we succeeded\n\
 :rtype: <Bool>"
 );
 
+static SATSolver* solverToInterrupt = NULL;
+void SIGINT_handler(int)
+{
+    SATSolver* solver = solverToInterrupt;
+    if (solverToInterrupt == NULL) { exit(-1); }
+    solver->interrupt_asap();
+}
+
 static PyObject* solve(Solver *self, PyObject *args, PyObject *kwds)
 {
     PyObject* assumptions = NULL;
+    solverToInterrupt = self->cmsat;
+    sighandler_t old_sig_int_handler = signal(SIGINT, SIGINT_handler);
+    sighandler_t old_sig_term_handler = signal(SIGTERM, SIGINT_handler);
 
     int verbose = self->verbose;
     double time_limit = self->time_limit;
     long confl_limit = self->confl_limit;
 
     static char const* kwlist[] = {"assumptions", "verbose", "time_limit", "confl_limit", NULL};
     if (!PyArg_ParseTupleAndKeywords(args, kwds, "|Oidl", const_cast<char**>(kwlist), &assumptions, &verbose, &time_limit, &confl_limit)) {
@@ -668,18 +682,17 @@
     }
 
     self->cmsat->set_verbosity(verbose);
     self->cmsat->set_max_time(time_limit);
     self->cmsat->set_max_confl(confl_limit);
 
     lbool res;
-    Py_BEGIN_ALLOW_THREADS      /* release GIL */
     res = self->cmsat->solve(&assumption_lits);
-    Py_END_ALLOW_THREADS
-
+    signal(SIGINT, old_sig_int_handler);
+    signal(SIGTERM, old_sig_term_handler);
     self->cmsat->set_verbosity(self->verbose);
     self->cmsat->set_max_time(self->time_limit);
     self->cmsat->set_max_confl(self->confl_limit);
 
     PyObject *result;
     if (res == l_True) {
         result = Py_True;
@@ -705,17 +718,15 @@
 :return: True or False\n\
 :rtype: <boolean>"
 );
 
 static PyObject* is_satisfiable(Solver *self)
 {
     lbool res;
-    Py_BEGIN_ALLOW_THREADS      /* release GIL */
     res = self->cmsat->solve();
-    Py_END_ALLOW_THREADS
 
     if (res == l_True) {
         Py_INCREF(Py_True);
         return Py_True;
     } else if (res == l_False) {
         Py_INCREF(Py_False);
         return Py_False;
```

### Comparing `pycmsgen-6.0.1/setup.py` & `pycmsgen-6.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
                    "src/packedrow.cpp",
                    "src/prober.cpp",
                    "src/propengine.cpp",
                    "src/reducedb.cpp",
                    "src/sccfinder.cpp",
                    "src/searcher.cpp",
                    "src/searchstats.cpp",
-                   "src/signalcode.cpp",
                    "src/solutionextender.cpp",
                    "src/solverconf.cpp",
                    "src/solver.cpp",
                    "src/stamp.cpp",
                    "src/str_impl_w_impl_stamp.cpp",
                    "src/subsumeimplicit.cpp",
                    "src/subsumestrengthen.cpp",
```

### Comparing `pycmsgen-6.0.1/src/GitSHA1.h` & `pycmsgen-6.0.2/src/GitSHA1.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/MersenneTwister.h` & `pycmsgen-6.0.2/src/MersenneTwister.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/Vec.h` & `pycmsgen-6.0.2/src/Vec.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/XAlloc.h` & `pycmsgen-6.0.2/src/XAlloc.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/alg.h` & `pycmsgen-6.0.2/src/alg.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/avgcalc.h` & `pycmsgen-6.0.2/src/avgcalc.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/bitarray.h` & `pycmsgen-6.0.2/src/bitarray.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/boundedqueue.h` & `pycmsgen-6.0.2/src/boundedqueue.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/clabstraction.h` & `pycmsgen-6.0.2/src/clabstraction.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/clause.h` & `pycmsgen-6.0.2/src/clause.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/clauseallocator.cpp` & `pycmsgen-6.0.2/src/clauseallocator.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/clauseallocator.h` & `pycmsgen-6.0.2/src/clauseallocator.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/clausecleaner.cpp` & `pycmsgen-6.0.2/src/clausecleaner.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/clausecleaner.h` & `pycmsgen-6.0.2/src/clausecleaner.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/clauseusagestats.cpp` & `pycmsgen-6.0.2/src/clauseusagestats.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/clauseusagestats.h` & `pycmsgen-6.0.2/src/clauseusagestats.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/cloffset.h` & `pycmsgen-6.0.2/src/cloffset.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/cmsgen.cpp` & `pycmsgen-6.0.2/src/cmsgen.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/cmsgen.h` & `pycmsgen-6.0.2/src/cmsgen.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/cnf.cpp` & `pycmsgen-6.0.2/src/cnf.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/cnf.h` & `pycmsgen-6.0.2/src/cnf.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/completedetachreattacher.cpp` & `pycmsgen-6.0.2/src/completedetachreattacher.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/completedetachreattacher.h` & `pycmsgen-6.0.2/src/completedetachreattacher.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/constants.h` & `pycmsgen-6.0.2/src/constants.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/cset.h` & `pycmsgen-6.0.2/src/cset.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/dimacsparser.h` & `pycmsgen-6.0.2/src/dimacsparser.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/distillerlong.cpp` & `pycmsgen-6.0.2/src/distillerlong.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/distillerlong.h` & `pycmsgen-6.0.2/src/distillerlong.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/distillerlongwithimpl.cpp` & `pycmsgen-6.0.2/src/distillerlongwithimpl.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/distillerlongwithimpl.h` & `pycmsgen-6.0.2/src/distillerlongwithimpl.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/drat.h` & `pycmsgen-6.0.2/src/drat.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/gaussian.cpp` & `pycmsgen-6.0.2/src/gaussian.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/gaussian.h` & `pycmsgen-6.0.2/src/gaussian.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/gausswatched.h` & `pycmsgen-6.0.2/src/gausswatched.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/gqueuedata.h` & `pycmsgen-6.0.2/src/gqueuedata.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/hasher.h` & `pycmsgen-6.0.2/src/hasher.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/heap.h` & `pycmsgen-6.0.2/src/heap.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/hyperengine.cpp` & `pycmsgen-6.0.2/src/hyperengine.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/hyperengine.h` & `pycmsgen-6.0.2/src/hyperengine.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/implcache.cpp` & `pycmsgen-6.0.2/src/implcache.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/implcache.h` & `pycmsgen-6.0.2/src/implcache.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/intree.cpp` & `pycmsgen-6.0.2/src/intree.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/intree.h` & `pycmsgen-6.0.2/src/intree.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/main.h` & `pycmsgen-6.0.2/src/main.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/main_common.h` & `pycmsgen-6.0.2/src/main_common.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/matrixfinder.cpp` & `pycmsgen-6.0.2/src/matrixfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/matrixfinder.h` & `pycmsgen-6.0.2/src/matrixfinder.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/msvc/stdint.h` & `pycmsgen-6.0.2/src/msvc/stdint.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/mystack.h` & `pycmsgen-6.0.2/src/mystack.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/nomutex.h` & `pycmsgen-6.0.2/src/nomutex.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/occsimplifier.cpp` & `pycmsgen-6.0.2/src/occsimplifier.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/occsimplifier.h` & `pycmsgen-6.0.2/src/occsimplifier.h`

 * *Files 2% similar despite different names*

```diff
@@ -41,18 +41,15 @@
 #include "watched.h"
 #include "watcharray.h"
 #include "simplefile.h"
 
 namespace CMSGen {
 
 using std::vector;
-using std::map;
-using std::set;
 using std::pair;
-using std::priority_queue;
 
 class ClauseCleaner;
 class SolutionExtender;
 class Solver;
 class SubsumeStrengthen;
 
 struct BlockedClauses {
@@ -553,21 +550,14 @@
 }
 
 inline bool OccSimplifier::getAnythingHasBeenBlocked() const
 {
     return anythingHasBeenBlocked;
 }
 
-/*inline std::ostream& operator<<(std::ostream& os, const BlockedClauses& bl)
-{
-    os << bl.lits << " to remove: " << bl.toRemove;
-
-    return os;
-}*/
-
 inline bool OccSimplifier::subsetReverse(const Clause& B) const
 {
     for (uint32_t i = 0; i != B.size(); i++) {
         if (!seen[B[i].toInt()])
             return false;
     }
     return true;
```

### Comparing `pycmsgen-6.0.1/src/packedmatrix.h` & `pycmsgen-6.0.2/src/packedmatrix.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/packedrow.cpp` & `pycmsgen-6.0.2/src/packedrow.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/packedrow.h` & `pycmsgen-6.0.2/src/packedrow.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/popcnt.h` & `pycmsgen-6.0.2/src/popcnt.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/prober.cpp` & `pycmsgen-6.0.2/src/prober.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/prober.h` & `pycmsgen-6.0.2/src/prober.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/propby.h` & `pycmsgen-6.0.2/src/propby.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/propby_backup.h` & `pycmsgen-6.0.2/src/propby_backup.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/propbyforgraph.h` & `pycmsgen-6.0.2/src/propbyforgraph.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/propengine.cpp` & `pycmsgen-6.0.2/src/propengine.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/propengine.h` & `pycmsgen-6.0.2/src/propengine.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/pycmsgen.egg-info/PKG-INFO` & `pycmsgen-6.0.2/src/pycmsgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycmsgen
-Version: 6.0.1
+Version: 6.0.2
 Summary: Bindings to CMSGen, uniform-like sampler
 Home-page: https://github.com/meelgroup/cmsgen
 Author-email: Mate Soos <soos.mate@gmail.com>
 Maintainer-email: Mate Soos <soos.mate@gmail.com>
 License: CryptoMiniSat Copyright (c) Mate Soos 2009-2018
         All rights reserved.
```

### Comparing `pycmsgen-6.0.1/src/pycmsgen.egg-info/SOURCES.txt` & `pycmsgen-6.0.2/src/pycmsgen.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,14 @@
 src/sccfinder.h
 src/searcher.cpp
 src/searcher.h
 src/searchhist.h
 src/searchstats.cpp
 src/searchstats.h
 src/shareddata.h
-src/signalcode.cpp
 src/signalcode.h
 src/simplefile.h
 src/solutionextender.cpp
 src/solutionextender.h
 src/solver.cpp
 src/solver.h
 src/solverconf.cpp
```

### Comparing `pycmsgen-6.0.1/src/reducedb.cpp` & `pycmsgen-6.0.2/src/reducedb.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/reducedb.h` & `pycmsgen-6.0.2/src/reducedb.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/sccfinder.cpp` & `pycmsgen-6.0.2/src/sccfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/sccfinder.h` & `pycmsgen-6.0.2/src/sccfinder.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/searcher.cpp` & `pycmsgen-6.0.2/src/searcher.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/searcher.h` & `pycmsgen-6.0.2/src/searcher.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/searchhist.h` & `pycmsgen-6.0.2/src/searchhist.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/searchstats.cpp` & `pycmsgen-6.0.2/src/searchstats.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/searchstats.h` & `pycmsgen-6.0.2/src/searchstats.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/shareddata.h` & `pycmsgen-6.0.2/src/shareddata.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/signalcode.h` & `pycmsgen-6.0.2/src/trim.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-/*
-Copyright (c) 2010-2015 Mate Soos
-Copyright (c) Kuldeep S. Meel, Daniel J. Fremont
+/******************************************
+Copyright (c) 2016, Mate Soos
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -15,26 +14,31 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
-*/
+***********************************************/
 
-#ifndef SIGNALCODE_H_
-#define SIGNALCODE_H_
+#ifndef TRIM_H
+#define TRIM_H
 
-#include <string>
+#include <string.h>
 
-namespace CMSGen {
-    class SATSolver;
-}
-using namespace CMSGen;
+static inline std::string trim(const std::string& str)
+{
+    std::string ret;
+    for(const char c: str)
+    {
+        if (c != ' '
+            && c != '\n'
+            && c != '\r'
+        ) {
+            ret += c;
+        }
+    }
 
-extern SATSolver* solverToInterrupt;
-extern int need_clean_exit;
-extern std::string redDumpFname;
-extern std::string irredDumpFname;
-void SIGINT_handler(int);
+    return ret;
+}
 
-#endif //SIGNALCODE_H_
+#endif //TRIM_H
```

### Comparing `pycmsgen-6.0.1/src/simplefile.h` & `pycmsgen-6.0.2/src/simplefile.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/solutionextender.cpp` & `pycmsgen-6.0.2/src/solutionextender.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/solutionextender.h` & `pycmsgen-6.0.2/src/solutionextender.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/solver.cpp` & `pycmsgen-6.0.2/src/solver.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,14 @@
     const vector<Lit>& lits
     , const bool attach
     , const bool addDrat
 ) {
     //cout << "add_every_combination got: " << lits << endl;
 
     size_t at = 0;
-    size_t num = 0;
     vector<Lit> xorlits;
     Lit lastlit_added = lit_Undef;
     while(at != lits.size()) {
         xorlits.clear();
         size_t last_at = at;
         for(; at < last_at+conf.xor_var_per_cut && at < lits.size(); at++) {
             xorlits.push_back(lits[at]);
@@ -200,16 +199,14 @@
             xorlits.push_back(toadd);
             lastlit_added = toadd;
         }
 
         add_xor_clause_inter_cleaned_cut(xorlits, attach, addDrat);
         if (!ok)
             break;
-
-        num++;
     }
 }
 
 void Solver::add_xor_clause_inter_cleaned_cut(
     const vector<Lit>& lits
     , const bool attach
     , const bool addDrat
@@ -1744,44 +1741,44 @@
             , stats_line_percent(prober->get_stats().cpu_time, cpu_time)
             , "% time"
         );
     }
     //OccSimplifier stats
     if (conf.perform_occur_based_simp) {
         if (conf.do_print_times)
-        print_stats_line("c OccSimplifier time"
+            print_stats_line("c OccSimplifier time"
             , occsimplifier->get_stats().total_time(occsimplifier)
             , stats_line_percent(occsimplifier->get_stats().total_time(occsimplifier) ,cpu_time)
             , "% time"
         );
         occsimplifier->get_sub_str()->get_stats().print_short(this);
     }
     if (conf.do_print_times)
-    print_stats_line("c SCC time"
+        print_stats_line("c SCC time"
         , varReplacer->get_scc_finder()->get_stats().cpu_time
         , stats_line_percent(varReplacer->get_scc_finder()->get_stats().cpu_time, cpu_time)
         , "% time"
     );
     varReplacer->get_scc_finder()->get_stats().print_short(NULL);
 
     //varReplacer->get_stats().print_short(nVars());
     if (conf.do_print_times)
-    print_stats_line("c distill time"
+        print_stats_line("c distill time"
                     , distill_long_cls->get_stats().time_used
                     , stats_line_percent(distill_long_cls->get_stats().time_used, cpu_time)
                     , "% time"
     );
     if (conf.do_print_times)
-    print_stats_line("c strength cache-irred time"
+        print_stats_line("c strength cache-irred time"
                     , dist_long_with_impl->get_stats().irredCacheBased.cpu_time
                     , stats_line_percent(dist_long_with_impl->get_stats().irredCacheBased.cpu_time, cpu_time)
                     , "% time"
     );
     if (conf.do_print_times)
-    print_stats_line("c strength cache-red time"
+        print_stats_line("c strength cache-red time"
                     , dist_long_with_impl->get_stats().redCacheBased.cpu_time
                     , stats_line_percent(dist_long_with_impl->get_stats().redCacheBased.cpu_time, cpu_time)
                     , "% time"
     );
 
     if (conf.do_print_times) {
         print_stats_line("c Conflicts in UIP"
@@ -1837,19 +1834,19 @@
 
     //Failed lit stats
     if (conf.doProbe
         && prober
     ) {
         prober->get_stats().print_short(this, 0, 0);
         if (conf.do_print_times)
-        print_stats_line("c probing time"
+            print_stats_line("c probing time"
             , prober->get_stats().cpu_time
             , stats_line_percent(prober->get_stats().cpu_time, cpu_time)
             , "% time"
-        );
+            );
 
         prober->get_stats().print_short(this, 0, 0);
     }
     //OccSimplifier stats
     if (conf.perform_occur_based_simp) {
         if (conf.do_print_times)
         print_stats_line("c OccSimplifier time"
@@ -1928,68 +1925,68 @@
         , stats_line_percent(zeroLevAssignsByCNF, nVarsOutside())
         , "% vars"
     );
 
     //Failed lit stats
     if (conf.doProbe) {
         if (conf.do_print_times)
-        print_stats_line("c probing time"
+            print_stats_line("c probing time"
             , prober->get_stats().cpu_time
             , stats_line_percent(prober->get_stats().cpu_time, cpu_time)
             , "% time"
-        );
+            );
 
         prober->get_stats().print(nVarsOuter(), conf.do_print_times);
     }
 
     //OccSimplifier stats
     if (conf.perform_occur_based_simp) {
         if (conf.do_print_times)
-        print_stats_line("c OccSimplifier time"
+            print_stats_line("c OccSimplifier time"
             , occsimplifier->get_stats().total_time(occsimplifier)
             , stats_line_percent(occsimplifier->get_stats().total_time(occsimplifier), cpu_time)
             , "% time"
-        );
+            );
 
         occsimplifier->get_stats().print(nVarsOuter(), occsimplifier);
         occsimplifier->get_sub_str()->get_stats().print();
     }
 
     //TODO after TRI to LONG conversion
     /*if (occsimplifier && conf.doGateFind) {
         occsimplifier->print_gatefinder_stats();
     }*/
 
     //VarReplacer stats
     if (conf.do_print_times)
-    print_stats_line("c SCC time"
+        print_stats_line("c SCC time"
         , varReplacer->get_scc_finder()->get_stats().cpu_time
         , stats_line_percent(varReplacer->get_scc_finder()->get_stats().cpu_time, cpu_time)
         , "% time"
-    );
+        );
     varReplacer->get_scc_finder()->get_stats().print();
 
     varReplacer->get_stats().print(nVarsOuter());
     varReplacer->print_some_stats(cpu_time);
 
     //DistillerAllWithAll stats
     if (conf.do_print_times)
-    print_stats_line("c distill time"
+        print_stats_line("c distill time"
                     , distill_long_cls->get_stats().time_used
                     , stats_line_percent(distill_long_cls->get_stats().time_used, cpu_time)
                     , "% time");
     distill_long_cls->get_stats().print(nVarsOuter());
 
     if (conf.do_print_times)
-    print_stats_line("c strength cache-irred time"
+        print_stats_line("c strength cache-irred time"
                     , dist_long_with_impl->get_stats().irredCacheBased.cpu_time
                     , stats_line_percent(dist_long_with_impl->get_stats().irredCacheBased.cpu_time, cpu_time)
                     , "% time");
     if (conf.do_print_times)
-    print_stats_line("c strength cache-red time"
+        print_stats_line("c strength cache-red time"
                     , dist_long_with_impl->get_stats().redCacheBased.cpu_time
                     , stats_line_percent(dist_long_with_impl->get_stats().redCacheBased.cpu_time, cpu_time)
                     , "% time");
     dist_long_with_impl->get_stats().print();
 
     if (conf.doStrSubImplicit) {
         subsumeImplicit->get_stats().print("");
```

### Comparing `pycmsgen-6.0.1/src/solver.h` & `pycmsgen-6.0.2/src/solver.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/solverconf.cpp` & `pycmsgen-6.0.2/src/solverconf.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/solverconf.h` & `pycmsgen-6.0.2/src/solverconf.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/solvertypes.h` & `pycmsgen-6.0.2/src/solvertypes.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/solvertypesmini.h` & `pycmsgen-6.0.2/src/solvertypesmini.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/stamp.cpp` & `pycmsgen-6.0.2/src/stamp.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/stamp.h` & `pycmsgen-6.0.2/src/stamp.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/str_impl_w_impl_stamp.cpp` & `pycmsgen-6.0.2/src/str_impl_w_impl_stamp.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/str_impl_w_impl_stamp.h` & `pycmsgen-6.0.2/src/str_impl_w_impl_stamp.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/streambuffer.h` & `pycmsgen-6.0.2/src/streambuffer.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/subsumeimplicit.cpp` & `pycmsgen-6.0.2/src/subsumeimplicit.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/subsumeimplicit.h` & `pycmsgen-6.0.2/src/subsumeimplicit.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/subsumestrengthen.cpp` & `pycmsgen-6.0.2/src/subsumestrengthen.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/subsumestrengthen.h` & `pycmsgen-6.0.2/src/subsumestrengthen.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/time_mem.h` & `pycmsgen-6.0.2/src/time_mem.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/touchlist.h` & `pycmsgen-6.0.2/src/touchlist.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/trim.h` & `pycmsgen-6.0.2/src/vardata.h`

 * *Files 22% similar despite different names*

```diff
@@ -16,29 +16,41 @@
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 THE SOFTWARE.
 ***********************************************/
 
-#ifndef TRIM_H
-#define TRIM_H
+#ifndef __VARDATA_H__
+#define __VARDATA_H__
 
-#include <string.h>
+#include "constants.h"
+#include "propby.h"
+#include "avgcalc.h"
 
-static inline std::string trim(const std::string& str)
+namespace CMSGen
 {
-    std::string ret;
-    for(const char c: str)
-    {
-        if (c != ' '
-            && c != '\n'
-            && c != '\r'
-        ) {
-            ret += c;
-        }
-    }
 
-    return ret;
+struct VarData
+{
+    ///contains the decision level at which the assignment was made.
+    uint32_t level = 0;
+    double weight = 0.5;
+    uint32_t cancelled = 0;
+
+    //Reason this got propagated. NULL means decision/toplevel
+    PropBy reason = PropBy();
+
+    lbool assumption = l_Undef;
+
+    ///Whether var has been eliminated (var-elim, different component, etc.)
+    Removed removed = Removed::none;
+
+    ///The preferred polarity of each variable.
+    bool polarity = false;
+    bool is_bva = false;
+    bool added_for_xor = false;
+};
+
 }
 
-#endif //TRIM_H
+#endif //__VARDATA_H__
```

### Comparing `pycmsgen-6.0.1/src/varreplacer.cpp` & `pycmsgen-6.0.2/src/varreplacer.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/varreplacer.h` & `pycmsgen-6.0.2/src/varreplacer.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/varupdatehelper.h` & `pycmsgen-6.0.2/src/varupdatehelper.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/watchalgos.h` & `pycmsgen-6.0.2/src/watchalgos.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/watcharray.h` & `pycmsgen-6.0.2/src/watcharray.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/watched.h` & `pycmsgen-6.0.2/src/watched.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/watched_backup.h` & `pycmsgen-6.0.2/src/watched_backup.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/xor.h` & `pycmsgen-6.0.2/src/xor.h`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/xorfinder.cpp` & `pycmsgen-6.0.2/src/xorfinder.cpp`

 * *Files identical despite different names*

### Comparing `pycmsgen-6.0.1/src/xorfinder.h` & `pycmsgen-6.0.2/src/xorfinder.h`

 * *Files identical despite different names*

