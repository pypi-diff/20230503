# Comparing `tmp/flux-python-0.48.0rc0.tar.gz` & `tmp/flux-python-0.50.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-python-0.48.0rc0.tar", last modified: Tue May  2 18:24:22 2023, max compression
+gzip compressed data, was "flux-python-0.50.0rc0.tar", last modified: Wed May  3 05:14:03 2023, max compression
```

## Comparing `flux-python-0.48.0rc0.tar` & `flux-python-0.50.0rc0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      186 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6108 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/PKG-INFO
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4326 2023-05-02 18:19:53.000000 flux-python-0.48.0rc0/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.082467 flux-python-0.48.0rc0/flux/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26956 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26465 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/Makefile.in
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      668 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.082467 flux-python-0.48.0rc0/flux/cli/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    27800 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/cli/_fortune.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      754 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/constants.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.082467 flux-python-0.48.0rc0/flux/constraint/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17451 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/constraint/parser.out
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2862 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/constraint/parsetab.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.082467 flux-python-0.48.0rc0/flux/core/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12153 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/handle.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      815 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/inner.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1309 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/trampoline.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5167 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/core/watchers.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      567 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/debugged.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7721 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/future.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6219 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/hostlist.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    10040 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/idset.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1674 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/importer.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.086467 flux-python-0.48.0rc0/flux/job/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3059 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/JobID.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    35872 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/Jobspec.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1189 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      597 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/_wrapper.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7170 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/event.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    26007 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/executor.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.086467 flux-python-0.48.0rc0/flux/job/frobnicator/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      460 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/frobnicator/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4929 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/frobnicator/frobnicator.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.086467 flux-python-0.48.0rc0/flux/job/frobnicator/plugins/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/frobnicator/plugins/constraints.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3088 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/frobnicator/plugins/defaults.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21558 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/info.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2449 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/kill.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1104 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/kvs.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    10098 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/list.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3580 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/stats.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4598 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/submit.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.086467 flux-python-0.48.0rc0/flux/job/validator/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      452 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/job/validator/plugins/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1710 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/plugins/feasibility.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/plugins/jobspec.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1427 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/plugins/require-instance.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/plugins/schema.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7594 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/validator/validator.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6988 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/job/wait.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     9456 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/kvs.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2629 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/memoized_property.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5394 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/message.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    11771 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/progress.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/resource/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7954 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/ResourceSet.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2767 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/ResourceSetImplementation.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4408 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/Rlist.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      533 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2663 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/resource/list.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2474 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/rpc.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3691 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/security.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/uri/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      470 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/uri/resolvers/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2490 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/resolvers/jobid.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3468 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/resolvers/lsf.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3916 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/resolvers/pid.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3357 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/resolvers/slurm.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6461 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/uri/uri.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    36871 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/util.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.090467 flux-python-0.48.0rc0/flux/utils/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      201 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.094467 flux-python-0.48.0rc0/flux/utils/parsedatetime/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)   105234 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4652 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/context.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       61 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/parsedatetime.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.094467 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      719 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/base.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3130 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      380 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/en_AU.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      157 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/en_US.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      959 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/es.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6090 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2998 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4577 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      485 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/parsedatetime/warns.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/flux/utils/tomli/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1072 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/LICENSE
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      294 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21649 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/_parser.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2813 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/_re.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      126 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/_types.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       26 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/utils/tomli/py.typed
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12713 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/flux/wrapper.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/flux_python.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6108 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2825 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.48.0rc0/flux_python.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-02 18:24:22.000000 flux-python-0.48.0rc0/flux_python.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    14019 2023-05-02 14:05:24.000000 flux-python-0.48.0rc0/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-02 18:24:22.098467 flux-python-0.48.0rc0/src/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1386 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_core_build.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)   134328 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_core_clean.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    54497 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_core_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1241 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_hostlist_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4739 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_hostlist_clean.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_hostlist_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1667 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_idset_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4483 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_idset_clean.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1876 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_idset_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2177 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_rlist_build.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21443 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_rlist_clean.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4552 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_rlist_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1533 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/_security_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_security_clean.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2048 2023-05-02 18:24:13.000000 flux-python-0.48.0rc0/src/_security_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      516 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/callbacks.h
--rwxrwxr-x   0 vscode    (1000) vscode    (1000)     2804 2023-05-02 05:33:04.000000 flux-python-0.48.0rc0/src/make_clean_header.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.185129 flux-python-0.50.0rc0/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      186 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6982 2023-05-03 05:14:03.185129 flux-python-0.50.0rc0/PKG-INFO
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5088 2023-05-03 00:25:02.000000 flux-python-0.50.0rc0/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.173129 flux-python-0.50.0rc0/flux/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/.gitignore
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26956 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    26465 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/Makefile.in
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      668 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.173129 flux-python-0.50.0rc0/flux/cli/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    27800 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/cli/_fortune.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      754 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/constants.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.173129 flux-python-0.50.0rc0/flux/constraint/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    17451 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/constraint/parser.out
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2862 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/constraint/parsetab.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.173129 flux-python-0.50.0rc0/flux/core/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12153 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/handle.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      815 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/inner.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1309 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/trampoline.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5167 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/core/watchers.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      567 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/debugged.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7721 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/future.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6219 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/hostlist.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    10040 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/idset.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1674 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/importer.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3059 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/JobID.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    35872 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/Jobspec.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1189 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      597 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/_wrapper.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7170 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/event.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    26007 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/executor.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/frobnicator/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      460 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/frobnicator/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4929 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/frobnicator/frobnicator.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/frobnicator/plugins/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/frobnicator/plugins/constraints.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3088 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/frobnicator/plugins/defaults.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21558 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/info.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2449 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/kill.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1104 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/kvs.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    10098 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/list.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3580 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/stats.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4598 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/submit.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/validator/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      452 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/job/validator/plugins/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1710 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/plugins/feasibility.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/plugins/jobspec.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1427 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/plugins/require-instance.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/plugins/schema.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7594 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/validator/validator.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6988 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/job/wait.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     9456 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/kvs.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2629 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/memoized_property.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     5394 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/message.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    11771 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/progress.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/resource/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     7954 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/ResourceSet.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2767 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/ResourceSetImplementation.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4408 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/Rlist.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      533 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2663 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/resource/list.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2474 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/rpc.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3691 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/security.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/uri/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      470 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/__init__.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/uri/resolvers/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2490 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/resolvers/jobid.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3468 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/resolvers/lsf.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3916 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/resolvers/pid.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3357 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/resolvers/slurm.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6461 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/uri/uri.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    36871 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/util.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.177129 flux-python-0.50.0rc0/flux/utils/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      201 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.181129 flux-python-0.50.0rc0/flux/utils/parsedatetime/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)   105234 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4652 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/context.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       61 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/parsedatetime.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.181129 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      719 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/base.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     3130 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      380 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/en_AU.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      157 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/en_US.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      959 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/es.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     6090 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2998 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4577 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      485 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/parsedatetime/warns.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.181129 flux-python-0.50.0rc0/flux/utils/tomli/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1072 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/LICENSE
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      294 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21649 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/_parser.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2813 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/_re.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      126 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/_types.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)       26 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/utils/tomli/py.typed
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12713 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/flux/wrapper.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.181129 flux-python-0.50.0rc0/flux_python.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     6982 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     2825 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.50.0rc0/flux_python.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-03 05:14:03.000000 flux-python-0.50.0rc0/flux_python.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-03 05:14:03.185129 flux-python-0.50.0rc0/setup.cfg
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    12040 2023-05-03 05:08:54.000000 flux-python-0.50.0rc0/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:14:03.185129 flux-python-0.50.0rc0/src/
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/src/__init__.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1637 2023-05-03 05:01:59.000000 flux-python-0.50.0rc0/src/_core_build.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)   133080 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_core_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    54367 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_core_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      876 2023-05-03 05:10:48.000000 flux-python-0.50.0rc0/src/_hostlist_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4268 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_hostlist_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_hostlist_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      961 2023-05-03 05:10:41.000000 flux-python-0.50.0rc0/src/_idset_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4483 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_idset_clean.h
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1876 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_idset_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-03 05:13:26.000000 flux-python-0.50.0rc0/src/_rlist_build.py
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)    21443 2023-05-03 00:05:27.000000 flux-python-0.50.0rc0/src/_rlist_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     4552 2023-05-03 00:05:27.000000 flux-python-0.50.0rc0/src/_rlist_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     1218 2023-05-03 05:13:39.000000 flux-python-0.50.0rc0/src/_security_build.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_security_clean.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)     2048 2023-05-03 05:13:54.000000 flux-python-0.50.0rc0/src/_security_preproc.h
+-rw-rw-r--   0 vscode    (1000) vscode    (1000)      516 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/src/callbacks.h
+-rwxrwxr-x   0 vscode    (1000) vscode    (1000)     2804 2023-05-02 05:33:04.000000 flux-python-0.50.0rc0/src/make_clean_header.py
```

### Comparing `flux-python-0.48.0rc0/PKG-INFO` & `flux-python-0.50.0rc0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-python
-Version: 0.48.0rc0
+Version: 0.50.0rc0
 Summary: Python bindings for the flux resource manager API
 Home-page: https://github.com/flux-framework/flux-python
 License: UNKNOWN
 Description: # Flux Python Bindings
         
         > 🐍️ You called me?
         
@@ -26,15 +26,15 @@
         to have an environment ready to go with Flux (and Flux Security). You can follow
         the instructions in the DevContainer to build the Flux Python bindings.
         By default, this environment installs the latest flux-core.
         If you want to build a custom version with Flux core you can do:
         
         ```bash
         rm -rf ~/flux-core
-        export FLUX_VERSION=0.48.0
+        export FLUX_VERSION=0.50.0
         wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
         tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
         sudo mv flux-core-${FLUX_VERSION} ~/flux-core
         rm flux-core-${FLUX_VERSION}.tar.gz
         cd ~/flux-core
         ./configure --prefix=/usr/local
         make
@@ -50,14 +50,28 @@
         
         And if you want to upload:
         
         ```bash
         $ twine upload dist/*.tar.gz
         ```
         
+        ## Install on a System
+        
+        Since we need to link to Flux libraries, you generally will need to choose a version, and provide the same flags. We
+        require access to the source repository, so you need to do:
+        
+        ```bash
+        wget https://files.pythonhosted.org/packages/25/fb/02951d80e44a19db291f0e7370d4e7d82c0c1b17709a37913881f958dff7/flux-python-0.48.0rc0.tar.gz
+        tar -xzvf flux-python-0.48.0rc0.tar.git clone https://github.com/flux-framework/flux-security security
+        git clone https://github.com/flux-framework/flux-core core
+        tar -xzvf flux-python-0.48.0rc0.tar.gz
+        cd flux-python-0.48.0rc0
+        python3 setup.py install flux-python-0.48.0rc0.tar.gz --version 0.48.0rc0 --security-src $HOME/security --flux-root /usr/include/flux --security-include /usr/include/flux/security
+        ```
+        
         ### Building Modules
         
         We will need to build the tarball providing paths to the flux-core and flux-security
         sources. This can be improved upon to just be one path if all the dependencies
         are provided with the flux install (and we don't need the source). Note
         that we also provide a custom version for the pypi package:
```

### Comparing `flux-python-0.48.0rc0/README.md` & `flux-python-0.50.0rc0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 to have an environment ready to go with Flux (and Flux Security). You can follow
 the instructions in the DevContainer to build the Flux Python bindings.
 By default, this environment installs the latest flux-core.
 If you want to build a custom version with Flux core you can do:
 
 ```bash
 rm -rf ~/flux-core
-export FLUX_VERSION=0.48.0
+export FLUX_VERSION=0.50.0
 wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
 tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
 sudo mv flux-core-${FLUX_VERSION} ~/flux-core
 rm flux-core-${FLUX_VERSION}.tar.gz
 cd ~/flux-core
 ./configure --prefix=/usr/local
 make
@@ -44,14 +44,28 @@
 
 And if you want to upload:
 
 ```bash
 $ twine upload dist/*.tar.gz
 ```
 
+## Install on a System
+
+Since we need to link to Flux libraries, you generally will need to choose a version, and provide the same flags. We
+require access to the source repository, so you need to do:
+
+```bash
+wget https://files.pythonhosted.org/packages/25/fb/02951d80e44a19db291f0e7370d4e7d82c0c1b17709a37913881f958dff7/flux-python-0.48.0rc0.tar.gz
+tar -xzvf flux-python-0.48.0rc0.tar.git clone https://github.com/flux-framework/flux-security security
+git clone https://github.com/flux-framework/flux-core core
+tar -xzvf flux-python-0.48.0rc0.tar.gz
+cd flux-python-0.48.0rc0
+python3 setup.py install flux-python-0.48.0rc0.tar.gz --version 0.48.0rc0 --security-src $HOME/security --flux-root /usr/include/flux --security-include /usr/include/flux/security
+```
+
 ### Building Modules
 
 We will need to build the tarball providing paths to the flux-core and flux-security
 sources. This can be improved upon to just be one path if all the dependencies
 are provided with the flux install (and we don't need the source). Note
 that we also provide a custom version for the pypi package:
```

### Comparing `flux-python-0.48.0rc0/flux/Makefile` & `flux-python-0.50.0rc0/flux/Makefile`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/Makefile.in` & `flux-python-0.50.0rc0/flux/Makefile.in`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/__init__.py` & `flux-python-0.50.0rc0/flux/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/cli/_fortune.py` & `flux-python-0.50.0rc0/flux/cli/_fortune.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/constants.py` & `flux-python-0.50.0rc0/flux/constants.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/constraint/parser.out` & `flux-python-0.50.0rc0/flux/constraint/parser.out`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/constraint/parsetab.py` & `flux-python-0.50.0rc0/flux/constraint/parsetab.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/core/handle.py` & `flux-python-0.50.0rc0/flux/core/handle.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/core/inner.py` & `flux-python-0.50.0rc0/flux/core/inner.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/core/trampoline.py` & `flux-python-0.50.0rc0/flux/core/trampoline.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/core/watchers.py` & `flux-python-0.50.0rc0/flux/core/watchers.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/debugged.py` & `flux-python-0.50.0rc0/flux/debugged.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/future.py` & `flux-python-0.50.0rc0/flux/future.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/hostlist.py` & `flux-python-0.50.0rc0/flux/hostlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/idset.py` & `flux-python-0.50.0rc0/flux/idset.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/importer.py` & `flux-python-0.50.0rc0/flux/importer.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/JobID.py` & `flux-python-0.50.0rc0/flux/job/JobID.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/Jobspec.py` & `flux-python-0.50.0rc0/flux/job/Jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/__init__.py` & `flux-python-0.50.0rc0/flux/job/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/_wrapper.py` & `flux-python-0.50.0rc0/flux/job/_wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/event.py` & `flux-python-0.50.0rc0/flux/job/event.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/executor.py` & `flux-python-0.50.0rc0/flux/job/executor.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/frobnicator/frobnicator.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/frobnicator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/frobnicator/plugins/constraints.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/plugins/constraints.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/frobnicator/plugins/defaults.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/info.py` & `flux-python-0.50.0rc0/flux/job/info.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/kill.py` & `flux-python-0.50.0rc0/flux/job/kill.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/kvs.py` & `flux-python-0.50.0rc0/flux/job/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/list.py` & `flux-python-0.50.0rc0/flux/job/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/stats.py` & `flux-python-0.50.0rc0/flux/job/stats.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/submit.py` & `flux-python-0.50.0rc0/flux/job/submit.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/validator/plugins/feasibility.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/feasibility.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/validator/plugins/jobspec.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/validator/plugins/require-instance.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/require-instance.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/validator/plugins/schema.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/schema.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/validator/validator.py` & `flux-python-0.50.0rc0/flux/job/validator/validator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/job/wait.py` & `flux-python-0.50.0rc0/flux/job/wait.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/kvs.py` & `flux-python-0.50.0rc0/flux/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/memoized_property.py` & `flux-python-0.50.0rc0/flux/memoized_property.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/message.py` & `flux-python-0.50.0rc0/flux/message.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/progress.py` & `flux-python-0.50.0rc0/flux/progress.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/resource/ResourceSet.py` & `flux-python-0.50.0rc0/flux/resource/ResourceSet.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/resource/ResourceSetImplementation.py` & `flux-python-0.50.0rc0/flux/resource/ResourceSetImplementation.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/resource/Rlist.py` & `flux-python-0.50.0rc0/flux/resource/Rlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/resource/__init__.py` & `flux-python-0.50.0rc0/flux/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/resource/list.py` & `flux-python-0.50.0rc0/flux/resource/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/rpc.py` & `flux-python-0.50.0rc0/flux/rpc.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/security.py` & `flux-python-0.50.0rc0/flux/security.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/uri/resolvers/jobid.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/jobid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/uri/resolvers/lsf.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/lsf.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/uri/resolvers/pid.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/pid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/uri/resolvers/slurm.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/slurm.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/uri/uri.py` & `flux-python-0.50.0rc0/flux/uri/uri.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/util.py` & `flux-python-0.50.0rc0/flux/util.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/__init__.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/context.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/context.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/base.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/base.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/es.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/es.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/tomli/LICENSE` & `flux-python-0.50.0rc0/flux/utils/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/tomli/_parser.py` & `flux-python-0.50.0rc0/flux/utils/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/utils/tomli/_re.py` & `flux-python-0.50.0rc0/flux/utils/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux/wrapper.py` & `flux-python-0.50.0rc0/flux/wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/flux_python.egg-info/PKG-INFO` & `flux-python-0.50.0rc0/flux_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-python
-Version: 0.48.0rc0
+Version: 0.50.0rc0
 Summary: Python bindings for the flux resource manager API
 Home-page: https://github.com/flux-framework/flux-python
 License: UNKNOWN
 Description: # Flux Python Bindings
         
         > 🐍️ You called me?
         
@@ -26,15 +26,15 @@
         to have an environment ready to go with Flux (and Flux Security). You can follow
         the instructions in the DevContainer to build the Flux Python bindings.
         By default, this environment installs the latest flux-core.
         If you want to build a custom version with Flux core you can do:
         
         ```bash
         rm -rf ~/flux-core
-        export FLUX_VERSION=0.48.0
+        export FLUX_VERSION=0.50.0
         wget https://github.com/flux-framework/flux-core/releases/download/v${FLUX_VERSION}/flux-core-${FLUX_VERSION}.tar.gz
         tar -xzvf flux-core-${FLUX_VERSION}.tar.gz
         sudo mv flux-core-${FLUX_VERSION} ~/flux-core
         rm flux-core-${FLUX_VERSION}.tar.gz
         cd ~/flux-core
         ./configure --prefix=/usr/local
         make
@@ -50,14 +50,28 @@
         
         And if you want to upload:
         
         ```bash
         $ twine upload dist/*.tar.gz
         ```
         
+        ## Install on a System
+        
+        Since we need to link to Flux libraries, you generally will need to choose a version, and provide the same flags. We
+        require access to the source repository, so you need to do:
+        
+        ```bash
+        wget https://files.pythonhosted.org/packages/25/fb/02951d80e44a19db291f0e7370d4e7d82c0c1b17709a37913881f958dff7/flux-python-0.48.0rc0.tar.gz
+        tar -xzvf flux-python-0.48.0rc0.tar.git clone https://github.com/flux-framework/flux-security security
+        git clone https://github.com/flux-framework/flux-core core
+        tar -xzvf flux-python-0.48.0rc0.tar.gz
+        cd flux-python-0.48.0rc0
+        python3 setup.py install flux-python-0.48.0rc0.tar.gz --version 0.48.0rc0 --security-src $HOME/security --flux-root /usr/include/flux --security-include /usr/include/flux/security
+        ```
+        
         ### Building Modules
         
         We will need to build the tarball providing paths to the flux-core and flux-security
         sources. This can be improved upon to just be one path if all the dependencies
         are provided with the flux install (and we don't need the source). Note
         that we also provide a custom version for the pypi package:
```

### Comparing `flux-python-0.48.0rc0/flux_python.egg-info/SOURCES.txt` & `flux-python-0.50.0rc0/flux_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/setup.py` & `flux-python-0.50.0rc0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,97 +1,96 @@
 ###############################################################
 # Copyright 2014-2023 Lawrence Livermore National Security, LLC
 # (c.f. AUTHORS, NOTICE.LLNS, COPYING)
 #
-# This file is part of the Flux resource manager framework.
+# This file is part of the Flux resource manager framework.f
 # For details, see https://github.com/flux-framework.
 #
 # SPDX-License-Identifier: LGPL-3.0
 ###############################################################
 
 # Usage
 # This should only be used to generate a wheel, as the build will not be
 # portable to a system with different Flux / Flux Security paths.
 
-import argparse
-import copy
 import os
 import re
 import shutil
 import subprocess
 import sys
 from contextlib import contextmanager
 
 from setuptools import find_packages
 from setuptools import setup as _setup
 from distutils.core import setup, Command
 
 # Metadata
 package_name = "flux-python"
-package_version = "0.46.0"
+package_version = "0.50.0-rc0"
 package_description = "Python bindings for the flux resource manager API"
 package_url = "https://github.com/flux-framework/flux-python"
 package_keywords = "flux, job manager, orchestration, hpc"
 
 try:
     with open("README.md") as filey:
         package_long_description = filey.read()
 except Exception:
-    package_long_description = description
+    package_long_description = package_description
 
 # Setup variables for dependencies
 cffi_dep = "cffi>=1.1"
 
 # src/bindings/python
-here = os.path.dirname(os.path.abspath(__file__))
+root = os.path.dirname(os.path.abspath(__file__))
+source = os.path.join(root, "src")
 
-# top level with src, etc (/code here)
-root = here
+def find_flux():
+    """
+    Find flux install via the executable!
+    """
+    path = shutil.which('flux')
+    if not path:
+        sys.exit('Cannot find executable flux, which is required to be on PATH to find the install location.')
+    # /usr/local/bin/flux --> /usr/local
+    return os.path.dirname(os.path.dirname(path))
+
+flux_root = find_flux()
 
 # Module specific default options files. Format strings below will be populated
 # after receiving the custom varibles from the user
 options = {
     "core": {
-        "path": "{root}",
-        "search": [os.path.join("{root}", "src", "common", "libflux")],
-        "header": "src/include/flux/core.h",
-        "additional_headers": [
-            os.path.join(here, "src/callbacks.h"),
-            "src/common/libdebugged/debugged.h",
-        ],
+        "header": "include/flux/core.h",
+        "additional_headers": [os.path.join(source, "callbacks.h")]
     },
     "hostlist": {
-        "path": "{root}/src/common/libhostlist",
-        "header": "src/include/flux/hostlist.h",
+        "header": "include/flux/hostlist.h",
     },
+
+    # Note that rlist is currently disabled, so this
+    # set of metadata doesn't matter
     "rlist": {
-        "path": "{root}/src/common/librlist",
-        "search": [
-            "{root}",
-            os.path.join("{root}", "config"),
-        ],
-        "header": "src/common/librlist/rlist.h",
+        "header": "include/flux/rlist.h",
         "ignore_headers": ["czmq_containers"],
     },
     "idset": {
-        "path": "{root}/src/common/libidset",
-        "header": "src/common/libidset/idset.h",
+        "header": "include/flux/idset.h",
     },
     # path and header are set by --flux-security
-    "security": {},
+    "security": {
+        "header": "include/flux/security/sign.h",
+        "search": ["{root}/include/flux/security"],
+    },
 }
 
 # Global variables for build type, corresponds to
-build_types = {"core", "idset", "rlist", "security", "hostlist"}
-
-# Flux root (with source code) to install for
-flux_root = None
-security_src = None
-security_include = None
+build_types = {"core", "idset", "security", "hostlist"}
 
+# rlist.h is disabled for now, as it requires the flux-core build
+# build_types = {"core", "idset", "rlist", "security", "hostlist"}
 
 @contextmanager
 def workdir(dirname):
     """
     Allow a temporary working directory to run commands
     """
     original = os.getcwd()
@@ -141,18 +140,16 @@
     Custom setuptools install command prepared cleaned headers.
 
     This currently requires the Python install to live alongside Flux,
     but is a first step to removing it from the automake system and having
     a proper setup.py. We might eventually be able to separate them further.
     """
 
-    def __init__(self, root, security_src, security_include):
+    def __init__(self, root):
         self.flux_root = root
-        self.security_src = security_src
-        self.security_include = security_include
         self.search = ""
         self.skip_build = False
         self.search = []
 
     def _parse_comma_list(self, attr):
         """
         Given an attribute (user argument) convert string with csv to list
@@ -160,67 +157,50 @@
         value = getattr(self, attr, None)
         if value:
             value = value.split(",")
         elif not value:
             value = []
         setattr(self, attr, value)
 
-    def set_builds(self):
-        """
-        Given user preferences on the command line, set build flags
-        for additional modules.
-        """
-        global options
-        options["security"]["path"] = self.security_include
-        options["security"]["search"] = [self.security_src]
-        options["security"]["header"] = os.path.join(
-            self.security_src, "src", "lib", "sign.h"
-        )
 
     def run(self):
         """
         Run the install
         """
-        self.set_builds()
         for build_type in build_types:
             cleaner = HeaderCleaner(
                 self.flux_root,
-                custom_search=self.search,
                 build_type=build_type,
                 **options[build_type],
             )
             cleaner.clean_headers()
 
 
 class HeaderCleaner:
-    def __init__(self, root, custom_search, build_type, **kwargs):
+    def __init__(self, root, build_type, **kwargs):
         """
         Main class to run a clean!
         """
         self.options = [
             "flux_root",
             "search",
             "skip_build",
             "hostlist",
-            "rlist",
             "idset",
-            "security",
-            "security_include",
-            "security_src",
         ]
         self.root = root
-        self.path = kwargs["path"].format(root=root)
         self.build_type = build_type
-        self.preproc_output = os.path.join(here, "src", "_%s_preproc.h" % build_type)
-        self.output = os.path.join(here, "src", "_%s_clean.h" % build_type)
+        self.preproc_output = os.path.join(source, "_%s_preproc.h" % build_type)
+        self.output = os.path.join(source, "_%s_clean.h" % build_type)
 
         # Relative path to header is required
         self.header = kwargs["header"]
 
         # Update search to include defaults
+        custom_search = [os.path.join(self.root, "include"), os.path.join(self.root, "lib"), os.path.join(self.root, "include", "flux")]
         self.search = custom_search + [
             x.format(root=root) for x in kwargs.get("search", [])
         ]
 
         # Not required
         self.additional_headers = kwargs.get("additional_headers", [])
         self.ignore_headers = kwargs.get("ignore_headers", [])
@@ -241,50 +221,51 @@
         Prepare cleaned headers for cffi
         """
         # Reset checked headers and final "mega header"
         self.checked_heads = {}
         self.mega_header = ""
 
         # Prepend 'path' option to search list:
-        self.search.insert(0, self.path)
+        self.search.insert(0, flux_root)
         self.search = [os.path.abspath(f) for f in self.search]
         with workdir(self.root):
             self.process_header()
 
             # Process additional headers
             for header in self.additional_headers or []:
                 self.process_header(header)
 
         # Write the clean header!
         print(f"Writing stage 1 clean header to {self.output}")
         with open(self.output, "w") as clean_header:
             clean_header.write(self.mega_header)
 
         # -E '-D__attribute__(...)=' and re-read
-        self.preprocess_gcc(self.output)
+        self.preprocess_gcc()
         self.mega_header = read_file(self.output)
 
         # Remove compiler directives
         self.clean_compiler_directives()
 
-    def preprocess_gcc(self, filename):
+    def preprocess_gcc(self):
         """
-        Compile with gcc -E '-D__attribute__(...)='
+        Compile with gcc -E '-D__attribute__(...)=' etc.
         """
         gcc = shutil.which("gcc")
         if not gcc:
             sys.exit("Cannot find gcc compiler.")
         cmd = [
-            gcc,
-            "-E",
-            "-D__attribute__(...)=",
-            self.output,
-            "-o",
-            self.preproc_output,
-        ]
+              gcc,
+              "-E",
+              "-D __attribute__(...)=",
+              '-DFLUX_DEPRECATED(...)=',
+              self.output,
+              "-o",
+              self.preproc_output,
+          ]
         print(" ".join(cmd))
         res = subprocess.call(cmd)
         if res != 0:
             sys.exit("Issue preprocessing header to %s" % self.preproc_output)
 
     def clean_compiler_directives(self):
         """
@@ -332,91 +313,34 @@
                     self.process_header(nf, os.path.dirname(os.path.abspath(nf)))
                 if not re.match("#\s*include", l):
                     self.mega_header += l
 
         # Flag as checked
         self.checked_heads[f] = 1
 
-
-# Setup.py logic goes here
-def get_parser():
-    parser = argparse.ArgumentParser(
-        description="Build Parser",
-        formatter_class=argparse.RawTextHelpFormatter,
-    )
-    parser.add_argument(
-        "--flux-root", dest="flux_root", help="Root to flux source code.", required=True
-    )
-    parser.add_argument("--version", help="version to install", required=True)
-    parser.add_argument(
-        "--security-src",
-        dest="security_src",
-        help="Security source code.",
-        required=True,
-    )
-    parser.add_argument(
-        "--security-include",
-        dest="security_include",
-        help="Security include path.",
-        required=True,
-    )
-    return parser
-
-
-def clean_args():
-    """
-    Ensure we remove extra flags that the second installed won't know about.
-    """
-    removed = ["--security-src", "--security-include", "--flux-root", "--version"]
-    cleaned = []
-    contenders = copy.deepcopy(sys.argv)
-    while contenders:
-        arg = contenders.pop(0)
-        if arg in removed:
-            contenders.pop(0)
-        else:
-            cleaned.append(arg)
-    sys.argv = cleaned
-
-
 def setup():
     """
     A wrapper to run setup. This likely isn't best practice, but is a first effort.
     """
-    parser = get_parser()
-
-    # If an error occurs while parsing the arguments, the interpreter will exit with value 2
-    args, extra = parser.parse_known_args()
-
-    global package_version
     global flux_root
-    global security_src
     global security_include
 
-    # Did we set a custom version
-    if args.version:
-        package_version = args.version
-
-    flux_root = args.flux_root
-    security_src = args.security_src
-    security_include = args.security_include
-
     # Always set the install root to the environment
     set_envar("FLUX_INSTALL_ROOT", flux_root)
-    set_envar("FLUX_SECURITY_SOURCE", security_src)
-    set_envar("FLUX_SECURITY_INCLUDE", security_include)
 
-    # Clean arguments we added
-    clean_args()
+    # The flux security path should be in the same root, under includes
+    security_include = os.path.join(flux_root, "include", "flux", "security")
+    if not os.path.exists(security_include):
+        sys.exit(f'Cannot find flux security under expected path {security_include}')
 
     # We only want this to run on creating the tarball
     command = sys.argv[1]
     if command in ["sdist", "build", "build_ext"]:
         # Custom setup commands, first without cffi to prepare headers
-        prepare = PrepareFluxHeaders(flux_root, security_src, security_include)
+        prepare = PrepareFluxHeaders(flux_root)
         prepare.run()
 
     # Request to install additional modules (we always do core0
     # We also have to remove the setup.py flags that aren't known
     cffi_modules = ["src/_core_build.py:ffi"]
     for build_type in build_types:
         # We always include / require core (may not be necessary)
```

### Comparing `flux-python-0.48.0rc0/src/_core_build.py` & `flux-python-0.50.0rc0/src/_hostlist_build.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,63 +1,46 @@
 import os
 from pathlib import Path
 
 from cffi import FFI
 
-ffi = FFI()
-
 # Ensure paths are in _flux
 here = os.path.abspath(os.path.dirname(__file__))
 root = os.environ.get("FLUX_INSTALL_ROOT")
 
-preproc_file = os.path.join(here, "_core_preproc.h")
-core_c_file = os.path.join(here, "_core.c")
+preproc_file = os.path.join(here, "_hostlist_preproc.h")
+core_c_file = os.path.join(here, "_hostlist.c")
+
+ffi = FFI()
 
 ffi.set_source(
-    "_flux._core",
+    "_flux._hostlist",
     """
-#include <src/include/flux/core.h>
-#include <src/common/libdebugged/debugged.h>
-
-
-void * unpack_long(ptrdiff_t num){
-  return (void*)num;
-}
-""",
-    libraries=["flux-core", "debugged", "flux"],
+#include <flux/hostlist.h>
+            """,
+    libraries=["flux-core", "flux-hostlist"],
     library_dirs=[
-        f"{root}/src/common/.libs",
-        f"{root}/src/common/libdebugged/.libs",
-        f"{root}/src/common/libflux/.libs",
+        root,
+        f"{root}/lib",
     ],
     include_dirs=[
         root,
-        f"{root}/src/include",
-        f"{root}/src/common/libflux",
-        f"{root}/src/common/libdebugged",
+        f"{root}/include",
     ],
     extra_compile_args=[
-        f"-L{root}/src/common/.libs",
-        f"-L{root}/src/common/libflux/.libs",
-        f"-L{root}/src/common/libdebugged/.libs",
+        f"-L{root}/lib",
     ],
 )
 
 cdefs = """
-typedef int... ptrdiff_t;
-typedef int... pid_t;
-typedef ... va_list;
-void * unpack_long(ptrdiff_t num);
-void free(void *ptr);
-#define FLUX_JOBID_ANY 0xFFFFFFFFFFFFFFFF
-
-    """
+    void free (void *);
+"""
 
 with open(preproc_file) as h:
     cdefs = cdefs + h.read()
 
 ffi.cdef(cdefs)
-ffi.emit_c_code(core_c_file)
 
-# ensure mtime of target is updated
+# If this is in main it's not called by setuptools
+ffi.emit_c_code(core_c_file)
 Path(core_c_file).touch()
 ffi.compile(verbose=True)
```

### Comparing `flux-python-0.48.0rc0/src/_core_clean.h` & `flux-python-0.50.0rc0/src/_core_clean.h`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,20 @@
  *
  * This file is part of the Flux resource manager framework.
  * For details, see https://github.com/flux-framework.
  *
  * SPDX-License-Identifier: LGPL-3.0
 \************************************************************/
 
-/* Allow in-tree programs to #include <flux/core.h> like out-of-tree would.
- */
+#ifndef _FLUX_CORE_H
+#define _FLUX_CORE_H
 
-#ifndef FLUX_CORE_H
-#define FLUX_CORE_H
+/* NOTE: these programming interfaces should be considered EXPERIMENTAL
+ * and are subject to change in flux-core releases prefixed with "0."
+ */
 
 /************************************************************\
  * Copyright 2014 Lawrence Livermore National Security, LLC
  * (c.f. AUTHORS, NOTICE.LLNS, COPYING)
  *
  * This file is part of the Flux resource manager framework.
  * For details, see https://github.com/flux-framework.
@@ -49,14 +50,20 @@
 /*  Generic container for holding textual errors from selected libflux
  *   functions:
  */
 typedef struct {
     char text[160];
 } flux_error_t;
 
+/* FLUX_DEPRECATED may be altered during pre-processing, check for
+ * definition */
+#ifndef FLUX_DEPRECATED
+#define FLUX_DEPRECATED(...) __VA_ARGS__ __attribute__((deprecated))
+#endif
+
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !_FLUX_CORE_TYPES_H */
 
 /*
@@ -523,15 +530,15 @@
 
 /* Create a new handle that is an alias for 'orig' in all respects
  * except it adds FLUX_O_CLONE to flags and has its own 'aux' hash
  * (which means it has its own reactor and dispatcher).
  */
 flux_t *flux_clone (flux_t *orig);
 
-/* Drop connection to broker and re-establish, if suported by connector.
+/* Drop connection to broker and re-establish, if supported by connector.
  */
 int flux_reconnect (flux_t *h);
 
 /* Get/set handle options.  Options are interpreted by connectors.
  * Returns 0 on success, or -1 on failure with errno set (e.g. EINVAL).
  */
 int flux_opt_set (flux_t *h, const char *option, const void *val, size_t len);
@@ -597,15 +604,15 @@
 /* Obtain a file descriptor that can be used to integrate a flux_t handle
  * into an external event loop.  When one of FLUX_POLLIN, FLUX_POLLOUT, or
  * FLUX_POLLERR is raised in flux_pollevents(), this file descriptor will
  * become readable in an edge triggered fashion.  The external event loop
  * should then call flux_pollevents().  See src/common/libflux/ev_flux.[ch]
  * for an example of a libev "composite watcher" based on these interfaces,
  * that is used internally by the flux reactor.
- * Returns fd on sucess, -1 on failure with errno set.
+ * Returns fd on success, -1 on failure with errno set.
  */
 int flux_pollfd (flux_t *h);
 
 /* Get/clear handle message counters.
  */
 void flux_get_msgcounters (flux_t *h, flux_msgcounters_t *mcs);
 void flux_clr_msgcounters (flux_t *h);
@@ -1035,14 +1042,20 @@
     int typemask;
     const char *topic_glob;
     flux_msg_handler_f cb;
     uint32_t rolemask;
 };
 #define FLUX_MSGHANDLER_TABLE_END { 0, NULL, NULL, 0 }
 
+int flux_msg_handler_addvec_ex (flux_t *h,
+                                const char *service_name,
+                                const struct flux_msg_handler_spec tab[],
+                                void *arg,
+                                flux_msg_handler_t **hp[]);
+
 int flux_msg_handler_addvec (flux_t *h,
                              const struct flux_msg_handler_spec tab[],
                              void *arg,
                              flux_msg_handler_t **msg_handlers[]);
 void flux_msg_handler_delvec (flux_msg_handler_t *msg_handlers[]);
 
 /* Requeue any unmatched messages, if handle was cloned.
@@ -1794,18 +1807,14 @@
  *
  * SPDX-License-Identifier: LGPL-3.0
 \************************************************************/
 
 #ifndef _FLUX_CORE_MODULE_H
 #define _FLUX_CORE_MODULE_H
 
-/* Module management messages are constructed according to Flux RFC 5.
- * https://flux-framework.rtfd.io/projects/flux-rfc/en/latest/spec_5.html
- */
-
 
 
 #ifdef __cplusplus
 extern "C" {
 #endif
 
 /* Module states, for embedding in keepalive messages (rfc 5)
@@ -1818,30 +1827,14 @@
 };
 
 /* Mandatory symbols for modules
  */
 #define MOD_NAME(x) const char *mod_name = x
 typedef int (mod_main_f)(flux_t *h, int argc, char *argv[]);
 
-typedef void (flux_moderr_f)(const char *errmsg, void *arg);
-
-/* Read the value of 'mod_name' from the specified module filename.
- * Caller must free the returned name.  Returns NULL on failure.
- * If 'cb' is non-NULL, any dlopen/dlsym errors are reported via callback.
- */
-char *flux_modname (const char *filename, flux_moderr_f *cb, void *arg);
-
-/* Search a colon-separated list of directories (recursively) for a .so file
- * with the requested module name and return its path, or NULL on failure.
- * Caller must free the returned path.
- * If 'cb' is non-NULL, any dlopen/dlsym errors are reported via callback.
- */
-char *flux_modfind (const char *searchpath, const char *modname,
-                    flux_moderr_f *cb, void *arg);
-
 /* Test and optionally clear module debug bit from within a module, as
  * described in RFC 5.  Return true if 'flag' bit is set.  If clear=true,
  * clear the bit after testing.  The flux-module(1) debug subcommand
  * manipulates these bits externally to set up test conditions.
  */
 bool flux_module_debug_test (flux_t *h, int flag, bool clear);
 
@@ -1880,15 +1873,15 @@
  * Values are local to a particular broker rank.
  * Some may be overridden on the broker command line with -Sattr=val.
  * The following commands are available for manipulating attributes
  * on the running system:
  *   flux lsattr [-v]
  *   flux setattr name value
  *   flux getattr name
- * In additon, the following functions may be used to get/set broker
+ * In addition, the following functions may be used to get/set broker
  * attributes programmatically.
  */
 
 
 #ifdef __cplusplus
 extern "C" {
 #endif
@@ -3007,14 +3000,411 @@
  *
  * This file is part of the Flux resource manager framework.
  * For details, see https://github.com/flux-framework.
  *
  * SPDX-License-Identifier: LGPL-3.0
 \************************************************************/
 
+#ifndef _FLUX_CORE_JOB_H
+#define _FLUX_CORE_JOB_H
+
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+enum job_submit_flags {
+    FLUX_JOB_PRE_SIGNED = 1,    // 'jobspec' is already signed
+    FLUX_JOB_DEBUG = 2,
+    FLUX_JOB_WAITABLE = 4,      // flux_job_wait() will be used on this job
+    FLUX_JOB_NOVALIDATE = 8,    // don't validate jobspec (instance owner only)
+};
+
+enum job_urgency {
+    FLUX_JOB_URGENCY_MIN = 0,
+    FLUX_JOB_URGENCY_HOLD = FLUX_JOB_URGENCY_MIN,
+    FLUX_JOB_URGENCY_DEFAULT = 16,
+    FLUX_JOB_URGENCY_MAX = 31,
+    FLUX_JOB_URGENCY_EXPEDITE = FLUX_JOB_URGENCY_MAX,
+};
+
+enum job_queue_priority {
+    FLUX_JOB_PRIORITY_MIN = 0,
+    FLUX_JOB_PRIORITY_MAX = 4294967295,
+};
+
+// N.B. value is duplicated in python bindings
+#define FLUX_JOBID_ANY 0xFFFFFFFFFFFFFFFF // ~(uint64_t)0
+
+typedef enum {
+    FLUX_JOB_STATE_NEW                    = 1,
+    FLUX_JOB_STATE_DEPEND                 = 2,
+    FLUX_JOB_STATE_PRIORITY               = 4,
+    FLUX_JOB_STATE_SCHED                  = 8,
+    FLUX_JOB_STATE_RUN                    = 16,
+    FLUX_JOB_STATE_CLEANUP                = 32,
+    FLUX_JOB_STATE_INACTIVE               = 64,   // captive end state
+} flux_job_state_t;
+
+#define FLUX_JOB_NR_STATES 7
+
+/* Virtual states, for convenience.
+ */
+enum {
+    /* FLUX_JOB_STATE_DEPEND | FLUX_JOB_STATE_PRIORITY | FLUX_JOB_STATE_SCHED */
+    FLUX_JOB_STATE_PENDING    = 14,
+    /* FLUX_JOB_STATE_RUN | FLUX_JOB_STATE_CLEANUP */
+    FLUX_JOB_STATE_RUNNING    = 48,
+    /* FLUX_JOB_STATE_PENDING | FLUX_JOB_STATE_RUNNING */
+    FLUX_JOB_STATE_ACTIVE     = 62,
+};
+
+/* Result of a job
+ */
+typedef enum {
+    FLUX_JOB_RESULT_COMPLETED = 1,
+    FLUX_JOB_RESULT_FAILED = 2,
+    FLUX_JOB_RESULT_CANCELED = 4,
+    FLUX_JOB_RESULT_TIMEOUT = 8,
+} flux_job_result_t;
+
+typedef uint64_t flux_jobid_t;
+
+/*  Parse a jobid from NULL-terminated string 's' in any supported encoding.
+ *  Returns 0 on success, -1 on failure.
+ */
+int flux_job_id_parse (const char *s, flux_jobid_t *id);
+
+/*  Encode a jobid into encoding "type", writing the result to buffer
+ *   buf of size bufsz.
+ *  Supported encoding types include:
+ *   "dec", "hex", "kvs", "dothex", "words", or "f58".
+ *  Returns 0 on success, -1 on failure with errno set:
+ *   EPROTO: Invalid encoding type
+ *   EINVAL: Invalid other argument
+ */
+int flux_job_id_encode (flux_jobid_t id, const char *type,
+                        char *buf, size_t bufsz);
+
+/* Convert state to string.  'fmt' may be:
+ * "s" - lower case short name
+ * "S" - upper case short name
+ * "l" - lower case long name
+ * "L" - upper case long name
+ * This function always returns a valid string, though it may
+ * be something like "(unknown)".
+ */
+const char *flux_job_statetostr (flux_job_state_t state, const char *fmt);
+
+/* Convert state string in any of the forms produced by flux_job_statetostr()
+ * back to state.  Returns 0 on success, -1 on failure with errno set.
+ */
+int flux_job_strtostate (const char *s, flux_job_state_t *state);
+
+const char *flux_job_resulttostr (flux_job_result_t result, const char *fmt);
+
+int flux_job_strtoresult (const char *s, flux_job_result_t *result);
+
+/* Submit a job to the system.
+ * 'jobspec' should be RFC 14 jobspec.
+ * 'urgency' should be a value from 0 to 31 (16 if not instance owner).
+ * 'flags' should be 0 for now.
+ * The system assigns a jobid and returns it in the response.
+ */
+flux_future_t *flux_job_submit (flux_t *h, const char *jobspec,
+                                int urgency, int flags);
+
+/* Parse jobid from response to flux_job_submit() request.
+ * Returns 0 on success, -1 on failure with errno set - and an extended
+ * error message may be available with flux_future_error_string().
+ */
+int flux_job_submit_get_id (flux_future_t *f, flux_jobid_t *id);
+
+/* Wait for jobid to enter INACTIVE state.
+ * If jobid=FLUX_JOBID_ANY, wait for the next waitable job.
+ * Fails with ECHILD if there is nothing to wait for.
+ */
+flux_future_t *flux_job_wait (flux_t *h, flux_jobid_t id);
+int flux_job_wait_get_status (flux_future_t *f,
+                              bool *success,
+                              const char **errstr);
+int flux_job_wait_get_id (flux_future_t *f, flux_jobid_t *id);
+
+FLUX_DEPRECATED(flux_future_t *flux_job_list (flux_t *,
+                                              int,
+                                              const char *,
+                                              uint32_t,
+                                              int));
+
+FLUX_DEPRECATED(flux_future_t *flux_job_list_inactive (flux_t *,
+                                                       int,
+                                                       double,
+                                                       const char *));
+
+/* Similar to flux_job_list(), but retrieve job info for a single
+ * job id */
+flux_future_t *flux_job_list_id (flux_t *h,
+                                 flux_jobid_t id,
+                                 const char *attrs_json_str);
+
+/* Raise an exception for job.
+ * Severity is 0-7, with severity=0 causing the job to abort.
+ * Note may be NULL or a human readable message.
+ */
+flux_future_t *flux_job_raise (flux_t *h, flux_jobid_t id,
+                               const char *type, int severity,
+                               const char *note);
+
+/* Cancel a job.
+ * Reason may be NULL or a human readable message.
+ */
+flux_future_t *flux_job_cancel (flux_t *h, flux_jobid_t id, const char *reason);
+
+/* Deliver a signal to a job.
+ */
+flux_future_t *flux_job_kill (flux_t *h, flux_jobid_t id, int signum);
+
+/* Change job urgency.
+ */
+flux_future_t *flux_job_set_urgency (flux_t *h, flux_jobid_t id, int urgency);
+
+/* Write KVS path to 'key' relative to job directory for job 'id'.
+ * If key=NULL, write the job directory.
+ * Returns string length on success, or -1 on failure.
+ */
+int flux_job_kvs_key (char *buf, int bufsz, flux_jobid_t id, const char *key);
+
+/* Same as above but construct key relative to job guest directory,
+ * and if FLUX_KVS_NAMESPACE is set, assume guest is the root directory.
+ */
+int flux_job_kvs_guest_key (char *buf,
+                            int bufsz,
+                            flux_jobid_t id,
+                            const char *key);
+
+
+/* Write KVS job namespace name to to buffer 'buf'.
+ * Returns string length on success or < 0 on failure.
+ */
+int flux_job_kvs_namespace (char *buf,
+                            int bufsz,
+                            flux_jobid_t id);
+
+/* Job eventlog watch functions
+ * - path specifies optional alternate eventlog path
+ */
+flux_future_t *flux_job_event_watch (flux_t *h, flux_jobid_t id,
+                                     const char *path, int flags);
+int flux_job_event_watch_get (flux_future_t *f, const char **event);
+int flux_job_event_watch_cancel (flux_future_t *f);
+
+/*  Wait for job to reach its terminal state and fetch the job result
+ *   along with other ancillary information from the job eventlog.
+ */
+flux_future_t *flux_job_result (flux_t *h, flux_jobid_t id, int flags);
+
+/*  Get the job result "payload" as a JSON string
+ */
+int flux_job_result_get (flux_future_t *f,
+                         const char **json_str);
+
+/*  Decode and unpack the result payload from future `f`.
+ *  The result object contains the following information:
+ *
+ *   {
+ *     "id":i,                 jobid
+ *     "result:i,              flux_job_result_t
+ *     "t_submit":f,           timestamp of job submit event
+ *     "t_run":f,              timestamp of job alloc event
+ *     "t_cleanup":f,          timestamp of job finish event
+ *     "waitstatus"?i,         wait status (if job started)
+ *     "exception_occurred":b, true if job exception occurred
+ *     "exception_severity"?i, exception severity (if exception)
+ *     "exception_type"?s,     exception type (if exception)
+ *     "exception_note"?s      exception note (if exception)
+ *   }
+ *
+ */
+int flux_job_result_get_unpack (flux_future_t *f, const char *fmt, ...);
+
+
+/*  Get remaining time in floating point seconds for the current job or
+ *  enclosing instancce (i.e., if the current process is associated with
+ *  a flux instance, but is not part of a parallel job).
+ *
+ *  Returns 0 on success with timeleft assigned to the remaining time.
+ *  If there is no expiration in the current context (e.g. the job has
+ *  no timelimit), then timeleft is set to infinity. If the job is not
+ *  in RUN state, or the job has expired, then timeleft is set to 0.
+ *
+ *  Returns -1 with error string assigned to 'errp' on failure.
+ */
+int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
+
+#ifdef __cplusplus
+}
+#endif
+
+#endif /* !_FLUX_CORE_JOB_H */
+
+/*
+ * vi:tabstop=4 shiftwidth=4 expandtab
+ */
+/************************************************************\
+ * Copyright 2021 Lawrence Livermore National Security, LLC
+ * (c.f. AUTHORS, NOTICE.LLNS, COPYING)
+ *
+ * This file is part of the Flux resource manager framework.
+ * For details, see https://github.com/flux-framework.
+ *
+ * SPDX-License-Identifier: LGPL-3.0
+\************************************************************/
+
+#ifndef _FLUX_CORE_JOBSPEC1_H
+#define _FLUX_CORE_JOBSPEC1_H
+
+
+typedef struct flux_jobspec1 flux_jobspec1_t;
+typedef flux_error_t flux_jobspec1_error_t;
+
+/* Remove the value in the jobspec's attributes section at the given path,
+ * where "." is treated as a path separator.
+ * It is not an error if 'path' does not exist.
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_attr_del (flux_jobspec1_t *jobspec, const char *path);
+
+/* Set the value in the jobspec's attributes section at the given path,
+ * where "." is treated as a path separator.  'fmt' should be a jansson
+ * pack-style string corresponding to the remaining arguments.
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_attr_pack (flux_jobspec1_t *jobspec,
+                             const char *path,
+                             const char *fmt,
+                             ...);
+
+/* Unpack the values in the jobspec's attributes section at the given path,
+ * where "." is treated as a path separator.  'fmt' should be a jansson
+ * unpack-style string corresponding to the remaining args.
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_attr_unpack (flux_jobspec1_t *jobspec,
+                               const char *path,
+                               const char *fmt,
+                               ...);
+
+/* Check the validity of only the attributes section of a jobspec, sufficient
+ * if the jobspec object was created by flux_jobspec1_from_command(), then
+ * modified with the other jobspec1 functions.
+ * Return 0 on success, -1 on error with errno set.
+ * On error, write an error message written to 'error', if non-NULL.
+ */
+int flux_jobspec1_attr_check (flux_jobspec1_t *jobspec,
+                              flux_jobspec1_error_t *error);
+
+/* Check the validity of the full jobspec, which may be necessary if the
+ * jobspec object was created by flux_jobspec1_decode().
+ * Return 0 on success, -1 on error with errno set.
+ * On error, write an error message written to 'error', if non-NULL.
+ */
+int flux_jobspec1_check (flux_jobspec1_t *jobspec,
+                         flux_jobspec1_error_t *error);
+
+/* Remove the variable 'name' from the environment.
+ * This function succeeds if 'name' does not exist.
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_unsetenv (flux_jobspec1_t *jobspec, const char *name);
+
+/* Add the variable 'name' to the environment with the value 'value'.
+ * If 'name' exists in the environment and 'overwrite' is nonzero, change
+ * value to 'value'.  If 'name' exists and 'overwrite' is zero, do not
+ * change the value (and return success).
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_setenv (flux_jobspec1_t *jobspec,
+                           const char *name,
+                           const char *value,
+                           int overwrite);
+
+/* Redirect job stdin from the KVS to a file system path given by 'path'.
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_set_stdin (flux_jobspec1_t *jobspec, const char *path);
+
+/* Redirect job stdout from the KVS to a file system path given by 'path'.
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_set_stdout (flux_jobspec1_t *jobspec, const char *path);
+
+/* Redirect job stderr from the KVS to a file system path given by 'path'.
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_set_stderr (flux_jobspec1_t *jobspec, const char *path);
+
+/* Set the working directory of a jobspec.
+ * Return 0 on success, -1 on error with errno set.
+ */
+int flux_jobspec1_set_cwd (flux_jobspec1_t *jobspec, const char *cwd);
+
+/* Encode a jobspec to a string, e.g. for usage with flux_job_submit().
+ * 'flags' should be 0.  The returned string must be released with free().
+ * Return NULL on error with errno set.
+ */
+char *flux_jobspec1_encode (flux_jobspec1_t *jobspec, size_t flags);
+
+/* Decode a string to jobspec.  No validation is performed on the content.
+ * The returned jobspec must be released with flux_jobspec1_destroy().
+ * Return NULL on error with errno set.
+ * On error, write an error message to 'error', if non-NULL.
+ */
+flux_jobspec1_t *flux_jobspec1_decode (const char *s,
+                                       flux_jobspec1_error_t *error);
+
+
+/* Create and return a minimum viable V1 Jobspec.
+ * The jobspec must be released with flux_jobspec1_destroy()'
+ * The jobspec will have stdin, stdout, stderr all directed to the KVS.
+ * 'argc' and 'argv' define the command and its arguments.
+ * 'env' should be an environ(7)-style array, or NULL for empty.
+ * 'tasks' should be the number of tasks to launch
+ * 'cores_per_task' should be the number of cores per task to allocate
+ * 'gpus_per_task' should be the number of gpus per task to allocate
+ * 'nodes' should be the number of nodes to spread the allocated cores
+ * and gpus across. If 0, the scheduler will determine the node allocation.
+ * Return NULL on error with errno set.
+ */
+flux_jobspec1_t *flux_jobspec1_from_command (int argc,
+                                             char **argv,
+                                             char **env,
+                                             int ntasks,
+                                             int cores_per_task,
+                                             int gpus_per_task,
+                                             int nnodes,
+                                             double duration);
+
+/* Free a jobspec. */
+void flux_jobspec1_destroy (flux_jobspec1_t *jobspec);
+
+#endif /* _FLUX_CORE_JOBSPEC1_H */
+
+/*
+ * vi:tabstop=4 shiftwidth=4 expandtab
+ */
+/************************************************************\
+ * Copyright 2018 Lawrence Livermore National Security, LLC
+ * (c.f. AUTHORS, NOTICE.LLNS, COPYING)
+ *
+ * This file is part of the Flux resource manager framework.
+ * For details, see https://github.com/flux-framework.
+ *
+ * SPDX-License-Identifier: LGPL-3.0
+\************************************************************/
+
 #ifndef _FLUX_CORE_SUBPROCESS_H
 #define _FLUX_CORE_SUBPROCESS_H
 
 
 
 #ifdef __cplusplus
 extern "C" {
@@ -3104,14 +3494,27 @@
     flux_subprocess_hook_f pre_exec;
     void *pre_exec_arg;
     flux_subprocess_hook_f post_fork;
     void *post_fork_arg;
 } flux_subprocess_hooks_t;
 
 /*
+ *  llog-compatible callback
+ */
+typedef void (*subprocess_log_f) (void *arg,
+                                  const char *file,
+                                  int line,
+                                  const char *func,
+                                  const char *subsys,
+                                  int level,
+                                  const char *fmt,
+                                  va_list args);
+
+
+/*
  * Convenience Functions:
  */
 
 /*  General output callback that will send output from the subprocess
  *  to stdout or stderr.  Set the `on_stdout` and/or `on_stderr`
  *  callbacks in flux_subprocess_ops_t and this function will output
  *  to stdout/stderr respectively.  You can also set 'on_channel_out'
@@ -3175,15 +3578,15 @@
 char *flux_cmd_stringify (const flux_cmd_t *cmd);
 
 /*
  *  Set a single environment variable (name) to formatted string `fmt`.
  *   If `overwrite` is non-zero then overwrite any existing setting for `name`.
  */
 int flux_cmd_setenvf (flux_cmd_t *cmd, int overwrite,
-		      const char *name, const char *fmt, ...)
+                      const char *name, const char *fmt, ...)
                       __attribute__ ((format (printf, 4, 5)));
 
 /*
  *  Unset environment variable `name` in the command object `cmd`.
  */
 void flux_cmd_unsetenv (flux_cmd_t *cmd, const char *name);
 
@@ -3267,42 +3670,55 @@
 
 /*
  *  Subprocesses:
  */
 
 /*
  *  Asynchronously create a new subprocess described by command object
- *   `cmd`.  flux_exec() and flux_local_exec() create a new subprocess
- *   locally.  flux_rexec() creates a new subprocess on Flux rank
+ *   `cmd`.  flux_local_exec() create a new subprocess locally.
+ *   flux_rexec() creates a new subprocess on Flux rank
  *   `rank`. Callbacks in `ops` structure that are non-NULL will be
  *   called to process state changes, I/O, and completion.
  *
  *  'rank' can be set to FLUX_NODEID_ANY or FLUX_NODEID_UPSTREAM.
  *
  *  This function may return NULL (with errno set) on invalid
  *   argument(s) (EINVAL), or failure of underlying Flux messaging
  *   calls. Otherwise, a valid subprocess object is returned, though
  *   there is no guarantee the subprocess has started running anywhere
  *   by the time the call returns.
  *
  */
-flux_subprocess_t *flux_exec (flux_t *h, int flags,
-                              const flux_cmd_t *cmd,
-                              const flux_subprocess_ops_t *ops,
-                              const flux_subprocess_hooks_t *hooks);
-
-flux_subprocess_t *flux_local_exec (flux_reactor_t *r, int flags,
+flux_subprocess_t *flux_local_exec (flux_reactor_t *r,
+                                    int flags,
                                     const flux_cmd_t *cmd,
-                                    const flux_subprocess_ops_t *ops,
-                                    const flux_subprocess_hooks_t *hooks);
+                                    const flux_subprocess_ops_t *ops);
+
+flux_subprocess_t *flux_local_exec_ex (flux_reactor_t *r,
+                                       int flags,
+                                       const flux_cmd_t *cmd,
+                                       const flux_subprocess_ops_t *ops,
+                                       const flux_subprocess_hooks_t *hooks,
+                                       subprocess_log_f log_fn,
+                                       void *log_data);
 
 flux_subprocess_t *flux_rexec (flux_t *h, int rank, int flags,
                                const flux_cmd_t *cmd,
                                const flux_subprocess_ops_t *ops);
 
+flux_subprocess_t *flux_rexec_ex (flux_t *h,
+                                  const char *service_name,
+                                  int rank,
+                                  int flags,
+                                  const flux_cmd_t *cmd,
+                                  const flux_subprocess_ops_t *ops,
+                                  subprocess_log_f log_fn,
+                                  void *log_data);
+
+
 /* Start / stop a read stream temporarily on local processes.  This
  * may be useful for flow control.  If you desire to have a stream not
  * call 'on_stdout' or 'on_stderr' when the local subprocess has
  * started, see STREAM_STOP configuration above.
  *
  * start and stop return 0 for success, -1 on error
  * status returns > 0 for started, 0 for stopped, -1 on error
@@ -3463,489 +3879,29 @@
 
 /*
  *  Return pointer to any context associated with `p` under `name`. If
  *   no such context exists, then NULL is returned.
  */
 void *flux_subprocess_aux_get (flux_subprocess_t *p, const char *name);
 
-typedef void (*subprocess_log_f) (void *arg,
-                                  const char *file,
-                                  int line,
-                                  const char *func,
-                                  const char *subsys,
-                                  int level,
-                                  const char *fmt,
-                                  va_list args);
-
-/* Set default internal logging function.
- */
-int flux_set_default_subprocess_log (flux_t *h,
-                                     subprocess_log_f log_fn,
-                                     void *log_data);
-
-
 
 #ifdef __cplusplus
 }
 #endif
 
 #endif /* !_FLUX_CORE_SUBPROCESS_H */
-/************************************************************\
- * Copyright 2018 Lawrence Livermore National Security, LLC
- * (c.f. AUTHORS, NOTICE.LLNS, COPYING)
- *
- * This file is part of the Flux resource manager framework.
- * For details, see https://github.com/flux-framework.
- *
- * SPDX-License-Identifier: LGPL-3.0
-\************************************************************/
-
-#ifndef _FLUX_CORE_JOB_H
-#define _FLUX_CORE_JOB_H
-
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-enum job_submit_flags {
-    FLUX_JOB_PRE_SIGNED = 1,    // 'jobspec' is already signed
-    FLUX_JOB_DEBUG = 2,
-    FLUX_JOB_WAITABLE = 4,      // flux_job_wait() will be used on this job
-    FLUX_JOB_NOVALIDATE = 8,    // don't validate jobspec (instance owner only)
-};
-
-enum job_urgency {
-    FLUX_JOB_URGENCY_MIN = 0,
-    FLUX_JOB_URGENCY_HOLD = FLUX_JOB_URGENCY_MIN,
-    FLUX_JOB_URGENCY_DEFAULT = 16,
-    FLUX_JOB_URGENCY_MAX = 31,
-    FLUX_JOB_URGENCY_EXPEDITE = FLUX_JOB_URGENCY_MAX,
-};
-
-enum job_queue_priority {
-    FLUX_JOB_PRIORITY_MIN = 0,
-    FLUX_JOB_PRIORITY_MAX = 4294967295,
-};
-
-// N.B. value is duplicated in python bindings
-#define FLUX_JOBID_ANY 0xFFFFFFFFFFFFFFFF // ~(uint64_t)0
-
-typedef enum {
-    FLUX_JOB_STATE_NEW                    = 1,
-    FLUX_JOB_STATE_DEPEND                 = 2,
-    FLUX_JOB_STATE_PRIORITY               = 4,
-    FLUX_JOB_STATE_SCHED                  = 8,
-    FLUX_JOB_STATE_RUN                    = 16,
-    FLUX_JOB_STATE_CLEANUP                = 32,
-    FLUX_JOB_STATE_INACTIVE               = 64,   // captive end state
-} flux_job_state_t;
-
-#define FLUX_JOB_NR_STATES 7
-
-/* Virtual states, for convenience.
- */
-enum {
-    /* FLUX_JOB_STATE_DEPEND | FLUX_JOB_STATE_PRIORITY | FLUX_JOB_STATE_SCHED */
-    FLUX_JOB_STATE_PENDING    = 14,
-    /* FLUX_JOB_STATE_RUN | FLUX_JOB_STATE_CLEANUP */
-    FLUX_JOB_STATE_RUNNING    = 48,
-    /* FLUX_JOB_STATE_PENDING | FLUX_JOB_STATE_RUNNING */
-    FLUX_JOB_STATE_ACTIVE     = 62,
-};
-
-/* Result of a job
- */
-typedef enum {
-    FLUX_JOB_RESULT_COMPLETED = 1,
-    FLUX_JOB_RESULT_FAILED = 2,
-    FLUX_JOB_RESULT_CANCELED = 4,
-    FLUX_JOB_RESULT_TIMEOUT = 8,
-} flux_job_result_t;
-
-typedef uint64_t flux_jobid_t;
-
-/*  Parse a jobid from NULL-teminated string 's' in any supported encoding.
- *  Returns 0 on success, -1 on failure.
- */
-int flux_job_id_parse (const char *s, flux_jobid_t *id);
-
-/*  Encode a jobid into encoding "type", writing the result to buffer
- *   buf of size bufsz.
- *  Supported encoding types include:
- *   "dec", "hex", "kvs", "dothex", "words", or "f58".
- *  Returns 0 on success, -1 on failure with errno set:
- *   EPROTO: Invalid encoding type
- *   EINVAL: Invalid other argument
- */
-int flux_job_id_encode (flux_jobid_t id, const char *type,
-                        char *buf, size_t bufsz);
-
-/* Convert state to string.  'fmt' may be:
- * "s" - lower case short name
- * "S" - upper case short name
- * "l" - lower case long name
- * "L" - upper case long name
- * This function always returns a valid string, though it may
- * be something like "(unknown)".
- */
-const char *flux_job_statetostr (flux_job_state_t state, const char *fmt);
-
-/* Convert state string in any of the forms produced by flux_job_statetostr()
- * back to state.  Returns 0 on success, -1 on failure with errno set.
- */
-int flux_job_strtostate (const char *s, flux_job_state_t *state);
-
-const char *flux_job_resulttostr (flux_job_result_t result, const char *fmt);
-
-int flux_job_strtoresult (const char *s, flux_job_result_t *result);
-
-/* Submit a job to the system.
- * 'jobspec' should be RFC 14 jobspec.
- * 'urgency' should be a value from 0 to 31 (16 if not instance owner).
- * 'flags' should be 0 for now.
- * The system assigns a jobid and returns it in the response.
- */
-flux_future_t *flux_job_submit (flux_t *h, const char *jobspec,
-                                int urgency, int flags);
-
-/* Parse jobid from response to flux_job_submit() request.
- * Returns 0 on success, -1 on failure with errno set - and an extended
- * error message may be available with flux_future_error_string().
- */
-int flux_job_submit_get_id (flux_future_t *f, flux_jobid_t *id);
-
-/* Wait for jobid to enter INACTIVE state.
- * If jobid=FLUX_JOBID_ANY, wait for the next waitable job.
- * Fails with ECHILD if there is nothing to wait for.
- */
-flux_future_t *flux_job_wait (flux_t *h, flux_jobid_t id);
-int flux_job_wait_get_status (flux_future_t *f,
-                              bool *success,
-                              const char **errstr);
-int flux_job_wait_get_id (flux_future_t *f, flux_jobid_t *id);
-
-/* Request a list of jobs.
- * If 'max_entries' > 0, fetch at most that many jobs.
- * 'attrs_json_str' is an encoded JSON array of attribute strings, e.g.
- * ["id","userid",...] that will be returned in response.
- *
- * Process the response payload with flux_rpc_get() or flux_rpc_get_unpack().
- * It is a JSON object containing an array of job objects, e.g.
- * { "jobs":[
- *   {"id":m, "userid":n},
- *   {"id":m, "userid":n},
- *   ...
- * ])
- *
- * states can be set to an OR of any job state or any virtual job
- * states to retrieve jobs of only those states.  Specify 0 for all
- * states.
- */
-flux_future_t *flux_job_list (flux_t *h,
-                              int max_entries,
-                              const char *attrs_json_str,
-                              uint32_t userid,
-                              int states);
-
-/* Similar to flux_job_list(), but retrieve inactive jobs newer
- * than a timestamp.
- */
-flux_future_t *flux_job_list_inactive (flux_t *h,
-                                       int max_entries,
-                                       double since,
-                                       const char *attrs_json_str);
-
-/* Similar to flux_job_list(), but retrieve job info for a single
- * job id */
-flux_future_t *flux_job_list_id (flux_t *h,
-                                 flux_jobid_t id,
-                                 const char *attrs_json_str);
-
-/* Raise an exception for job.
- * Severity is 0-7, with severity=0 causing the job to abort.
- * Note may be NULL or a human readable message.
- */
-flux_future_t *flux_job_raise (flux_t *h, flux_jobid_t id,
-                               const char *type, int severity,
-                               const char *note);
-
-/* Cancel a job.
- * Reason may be NULL or a human readable message.
- */
-flux_future_t *flux_job_cancel (flux_t *h, flux_jobid_t id, const char *reason);
-
-/* Deliver a signal to a job.
- */
-flux_future_t *flux_job_kill (flux_t *h, flux_jobid_t id, int signum);
-
-/* Change job urgency.
- */
-flux_future_t *flux_job_set_urgency (flux_t *h, flux_jobid_t id, int urgency);
-
-/* Write KVS path to 'key' relative to job directory for job 'id'.
- * If key=NULL, write the job directory.
- * Returns string length on success, or -1 on failure.
- */
-int flux_job_kvs_key (char *buf, int bufsz, flux_jobid_t id, const char *key);
-
-/* Same as above but construct key relative to job guest directory,
- * and if FLUX_KVS_NAMESPACE is set, assume guest is the root directory.
- */
-int flux_job_kvs_guest_key (char *buf,
-                            int bufsz,
-                            flux_jobid_t id,
-                            const char *key);
-
-
-/* Write KVS job namespace name to to buffer 'buf'.
- * Returns string length on success or < 0 on failure.
- */
-int flux_job_kvs_namespace (char *buf,
-                            int bufsz,
-                            flux_jobid_t id);
-
-/* Job eventlog watch functions
- * - path specifies optional alternate eventlog path
- */
-flux_future_t *flux_job_event_watch (flux_t *h, flux_jobid_t id,
-                                     const char *path, int flags);
-int flux_job_event_watch_get (flux_future_t *f, const char **event);
-int flux_job_event_watch_cancel (flux_future_t *f);
-
-/*  Wait for job to reach its terminal state and fetch the job result
- *   along with other ancillary information from the job eventlog.
- */
-flux_future_t *flux_job_result (flux_t *h, flux_jobid_t id, int flags);
-
-/*  Get the job result "payload" as a JSON string
- */
-int flux_job_result_get (flux_future_t *f,
-                         const char **json_str);
-
-/*  Decode and unpack the result payload from future `f`.
- *  The result object contains the following information:
- *
- *   {
- *     "id":i,                 jobid
- *     "result:i,              flux_job_result_t
- *     "t_submit":f,           timestamp of job submit event
- *     "t_run":f,              timestamp of job alloc event
- *     "t_cleanup":f,          timestamp of job finish event
- *     "waitstatus"?i,         wait status (if job started)
- *     "exception_occurred":b, true if job exception occurred
- *     "exception_severity"?i, exception severity (if exception)
- *     "exception_type"?s,     exception type (if exception)
- *     "exception_note"?s      exception note (if exception)
- *   }
- *
- */
-int flux_job_result_get_unpack (flux_future_t *f, const char *fmt, ...);
-
-
-/*  Get remaining time in floating point seconds for the current job or
- *  enclosing instancce (i.e., if the current process is associated with
- *  a flux instance, but is not part of a parallel job).
- *
- *  Returns 0 on success with timeleft assigned to the remaining time.
- *  If there is no expiration in the current context (e.g. the job has
- *  no timelimit), then timeleft is set to infinity. If the job is not
- *  in RUN state, or the job has expired, then timeleft is set to 0.
- *
- *  Returns -1 with error string assinged to 'errp' on failure.
- */
-int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
-
-#ifdef __cplusplus
-}
-#endif
 
-#endif /* !_FLUX_CORE_JOB_H */
+#endif /* !_FLUX_CORE_H */
 
 /*
  * vi:tabstop=4 shiftwidth=4 expandtab
  */
-/************************************************************\
- * Copyright 2021 Lawrence Livermore National Security, LLC
- * (c.f. AUTHORS, NOTICE.LLNS, COPYING)
- *
- * This file is part of the Flux resource manager framework.
- * For details, see https://github.com/flux-framework.
- *
- * SPDX-License-Identifier: LGPL-3.0
-\************************************************************/
-
-#ifndef _FLUX_CORE_JOBSPEC1_H
-#define _FLUX_CORE_JOBSPEC1_H
-
-
-typedef struct flux_jobspec1 flux_jobspec1_t;
-typedef flux_error_t flux_jobspec1_error_t;
-
-/* Remove the value in the jobspec's attributes section at the given path,
- * where "." is treated as a path separator.
- * It is not an error if 'path' does not exist.
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_attr_del (flux_jobspec1_t *jobspec, const char *path);
-
-/* Set the value in the jobspec's attributes section at the given path,
- * where "." is treated as a path separator.  'fmt' should be a jansson
- * pack-style string corresponding to the remaining arguments.
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_attr_pack (flux_jobspec1_t *jobspec,
-                             const char *path,
-                             const char *fmt,
-                             ...);
-
-/* Unpack the values in the jobspec's attributes section at the given path,
- * where "." is treated as a path separator.  'fmt' should be a jansson
- * unpack-style string corresponding to the remaining args.
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_attr_unpack (flux_jobspec1_t *jobspec,
-                               const char *path,
-                               const char *fmt,
-                               ...);
-
-/* Check the validity of only the attributes section of a jobspec, sufficient
- * if the jobspec object was created by flux_jobspec1_from_command(), then
- * modified with the other jobspec1 functions.
- * Return 0 on success, -1 on error with errno set.
- * On error, write an error message written to 'error', if non-NULL.
- */
-int flux_jobspec1_attr_check (flux_jobspec1_t *jobspec,
-                              flux_jobspec1_error_t *error);
-
-/* Check the validity of the full jobspec, which may be necessary if the
- * jobspec object was created by flux_jobspec1_decode().
- * Return 0 on success, -1 on error with errno set.
- * On error, write an error message written to 'error', if non-NULL.
- */
-int flux_jobspec1_check (flux_jobspec1_t *jobspec,
-                         flux_jobspec1_error_t *error);
-
-/* Remove the variable 'name' from the environment.
- * This function succeeds if 'name' does not exist.
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_unsetenv (flux_jobspec1_t *jobspec, const char *name);
-
-/* Add the variable 'name' to the environment with the value 'value'.
- * If 'name' exists in the environment and 'overwrite' is nonzero, change
- * value to 'value'.  If 'name' exists and 'overwrite' is zero, do not
- * change the value (and return success).
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_setenv (flux_jobspec1_t *jobspec,
-                           const char *name,
-                           const char *value,
-                           int overwrite);
-
-/* Redirect job stdin from the KVS to a file system path given by 'path'.
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_set_stdin (flux_jobspec1_t *jobspec, const char *path);
-
-/* Redirect job stdout from the KVS to a file system path given by 'path'.
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_set_stdout (flux_jobspec1_t *jobspec, const char *path);
-
-/* Redirect job stderr from the KVS to a file system path given by 'path'.
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_set_stderr (flux_jobspec1_t *jobspec, const char *path);
-
-/* Set the working directory of a jobspec.
- * Return 0 on success, -1 on error with errno set.
- */
-int flux_jobspec1_set_cwd (flux_jobspec1_t *jobspec, const char *cwd);
-
-/* Encode a jobspec to a string, e.g. for usage with flux_job_submit().
- * 'flags' should be 0.  The returned string must be released with free().
- * Return NULL on error with errno set.
- */
-char *flux_jobspec1_encode (flux_jobspec1_t *jobspec, size_t flags);
-
-/* Decode a string to jobspec.  No validation is performed on the content.
- * The returned jobspec must be released with flux_jobspec1_destroy().
- * Return NULL on error with errno set.
- * On error, write an error message to 'error', if non-NULL.
- */
-flux_jobspec1_t *flux_jobspec1_decode (const char *s,
-                                       flux_jobspec1_error_t *error);
-
-
-/* Create and return a minimum viable V1 Jobspec.
- * The jobspec must be released with flux_jobspec1_destroy()'
- * The jobspec will have stdin, stdout, stderr all directed to the KVS.
- * 'argc' and 'argv' define the command and its arguments.
- * 'env' should be an environ(7)-style array, or NULL for empty.
- * 'tasks' should be the number of tasks to launch
- * 'cores_per_task' should be the number of cores per task to allocate
- * 'gpus_per_task' should be the number of gpus per task to allocate
- * 'nodes' should be the number of nodes to spread the allocated cores
- * and gpus across. If 0, the scheduler will determine the node allocation.
- * Return NULL on error with errno set.
- */
-flux_jobspec1_t *flux_jobspec1_from_command (int argc,
-                                             char **argv,
-                                             char **env,
-                                             int ntasks,
-                                             int cores_per_task,
-                                             int gpus_per_task,
-                                             int nnodes,
-                                             double duration);
-
-/* Free a jobspec. */
-void flux_jobspec1_destroy (flux_jobspec1_t *jobspec);
-
-#endif /* _FLUX_CORE_JOBSPEC1_H */
-
-/*
- * vi:tabstop=4 shiftwidth=4 expandtab
- */
-
-#endif /* FLUX_CORE_H */
 //flux_msg_handler_f
 extern "Python" void message_handler_wrapper(flux_t *, flux_msg_handler_t *, const flux_msg_t *, void *);
 
 //flux_watcher_f
 extern "Python" void timeout_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void fd_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void signal_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 
 //flux_continuation_f
 extern "Python" void continuation_callback(flux_future_t *, void *);
-/************************************************************\
- * Copyright 2020 Lawrence Livermore National Security, LLC
- * (c.f. AUTHORS, NOTICE.LLNS, COPYING)
- *
- * This file is part of the Flux resource manager framework.
- * For details, see https://github.com/flux-framework.
- *
- * SPDX-License-Identifier: LGPL-3.0
-\************************************************************/
-
-#ifndef _FLUX_CORE_DEBUGGED_H
-#define _FLUX_CORE_DEBUGGED_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-extern int MPIR_being_debugged;
-extern void MPIR_Breakpoint (void);
-extern int get_mpir_being_debugged (void);
-extern void set_mpir_being_debugged (int v);
-
-#ifdef __cplusplus
-}
-#endif
-
-#endif /* !_FLUX_CORE_DEBUGGED_H */
-
-/*
- * vi:tabstop=4 shiftwidth=4 expandtab
- */
```

### Comparing `flux-python-0.48.0rc0/src/_core_preproc.h` & `flux-python-0.50.0rc0/src/_core_preproc.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # 1 "/workspaces/flux-python/src/_core_clean.h"
 # 1 "<built-in>"
 # 1 "<command-line>"
 # 1 "/usr/include/stdc-predef.h" 1 3 4
 # 1 "<command-line>" 2
 # 1 "/workspaces/flux-python/src/_core_clean.h"
-# 47 "/workspaces/flux-python/src/_core_clean.h"
+# 48 "/workspaces/flux-python/src/_core_clean.h"
 typedef void (*flux_free_f)(void *arg);
 
 
 
 
 typedef struct {
     char text[160];
 } flux_error_t;
-# 97 "/workspaces/flux-python/src/_core_clean.h"
+# 104 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_msg flux_msg_t;
 
 enum {
     FLUX_MSGTYPE_REQUEST = 0x01,
     FLUX_MSGTYPE_RESPONSE = 0x02,
     FLUX_MSGTYPE_EVENT = 0x04,
     FLUX_MSGTYPE_CONTROL = 0x08,
@@ -56,15 +56,15 @@
                                    const char *topic_glob);
 
 void flux_match_free (struct flux_match m);
 
 int flux_match_asprintf (struct flux_match *m,
                          const char *topic_glob_fmt,
                          ...);
-# 171 "/workspaces/flux-python/src/_core_clean.h"
+# 178 "/workspaces/flux-python/src/_core_clean.h"
 flux_msg_t *flux_msg_create (int type);
 void flux_msg_destroy (flux_msg_t *msg);
 
 
 
 
 int flux_msg_aux_set (const flux_msg_t *msg, const char *name,
@@ -165,15 +165,15 @@
 
 
 int flux_msg_pack (flux_msg_t *msg, const char *fmt, ...);
 int flux_msg_vpack (flux_msg_t *msg, const char *fmt, va_list ap);
 
 int flux_msg_unpack (const flux_msg_t *msg, const char *fmt, ...);
 int flux_msg_vunpack (const flux_msg_t *msg, const char *fmt, va_list ap);
-# 287 "/workspaces/flux-python/src/_core_clean.h"
+# 294 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_msg_last_error (const flux_msg_t *msg);
 
 
 
 int flux_msg_set_nodeid (flux_msg_t *msg, uint32_t nodeid);
 int flux_msg_get_nodeid (const flux_msg_t *msg, uint32_t *nodeid);
 
@@ -251,15 +251,15 @@
 void flux_msg_fprint (FILE *f, const flux_msg_t *msg);
 void flux_msg_fprint_ts (FILE *f, const flux_msg_t *msg, double timestamp);
 
 
 
 
 const char *flux_msg_typestr (int type);
-# 382 "/workspaces/flux-python/src/_core_clean.h"
+# 389 "/workspaces/flux-python/src/_core_clean.h"
 void flux_msg_route_enable (flux_msg_t *msg);
 
 
 
 
 
 void flux_msg_route_disable (flux_msg_t *msg);
@@ -310,15 +310,15 @@
 char *flux_msg_route_string (const flux_msg_t *msg);
 
 
 
 
 bool flux_msg_route_match_first (const flux_msg_t *msg1,
                                  const flux_msg_t *msg2);
-# 456 "/workspaces/flux-python/src/_core_clean.h"
+# 463 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_handle_struct flux_t;
 
 typedef struct {
     int request_tx;
     int request_rx;
     int response_tx;
     int response_rx;
@@ -351,15 +351,15 @@
 
 
 enum {
     FLUX_POLLIN = 1,
     FLUX_POLLOUT = 2,
     FLUX_POLLERR = 4,
 };
-# 509 "/workspaces/flux-python/src/_core_clean.h"
+# 516 "/workspaces/flux-python/src/_core_clean.h"
 flux_t *flux_open (const char *uri, int flags);
 
 
 
 
 
 flux_t *flux_open_ex (const char *uri, int flags, flux_error_t *error);
@@ -387,15 +387,15 @@
 int flux_opt_set (flux_t *h, const char *option, const void *val, size_t len);
 int flux_opt_get (flux_t *h, const char *option, void *val, size_t len);
 
 
 
 
 void flux_comms_error_set (flux_t *h, flux_comms_error_f fun, void *arg);
-# 553 "/workspaces/flux-python/src/_core_clean.h"
+# 560 "/workspaces/flux-python/src/_core_clean.h"
 void *flux_aux_get (flux_t *h, const char *name);
 int flux_aux_set (flux_t *h, const char *name, void *aux, flux_free_f destroy);
 
 
 
 void flux_flags_set (flux_t *h, int flags);
 void flux_flags_unset (flux_t *h, int flags);
@@ -409,37 +409,37 @@
 uint32_t flux_matchtag_avail (flux_t *h);
 
 
 
 
 
 int flux_send (flux_t *h, const flux_msg_t *msg, int flags);
-# 582 "/workspaces/flux-python/src/_core_clean.h"
+# 589 "/workspaces/flux-python/src/_core_clean.h"
 flux_msg_t *flux_recv (flux_t *h, struct flux_match match, int flags);
 
 
 
 
 
 
 int flux_requeue (flux_t *h, const flux_msg_t *msg, int flags);
 
 
 
 
 
 int flux_pollevents (flux_t *h);
-# 606 "/workspaces/flux-python/src/_core_clean.h"
+# 613 "/workspaces/flux-python/src/_core_clean.h"
 int flux_pollfd (flux_t *h);
 
 
 
 void flux_get_msgcounters (flux_t *h, flux_msgcounters_t *mcs);
 void flux_clr_msgcounters (flux_t *h);
-# 654 "/workspaces/flux-python/src/_core_clean.h"
+# 661 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_buffer flux_buffer_t;
 
 
 
 flux_buffer_t *flux_buffer_create (int size);
 
 void flux_buffer_destroy (void *fb);
@@ -448,25 +448,25 @@
 int flux_buffer_size (flux_buffer_t *fb);
 
 
 int flux_buffer_bytes (flux_buffer_t *fb);
 
 
 int flux_buffer_space (flux_buffer_t *fb);
-# 680 "/workspaces/flux-python/src/_core_clean.h"
+# 687 "/workspaces/flux-python/src/_core_clean.h"
 int flux_buffer_readonly (flux_buffer_t *fb);
 bool flux_buffer_is_readonly (flux_buffer_t *fb);
 
 
 
 
 int flux_buffer_drop (flux_buffer_t *fb, int len);
-# 695 "/workspaces/flux-python/src/_core_clean.h"
+# 702 "/workspaces/flux-python/src/_core_clean.h"
 const void *flux_buffer_peek (flux_buffer_t *fb, int len, int *lenp);
-# 705 "/workspaces/flux-python/src/_core_clean.h"
+# 712 "/workspaces/flux-python/src/_core_clean.h"
 const void *flux_buffer_read (flux_buffer_t *fb, int len, int *lenp);
 
 
 
 
 int flux_buffer_write (flux_buffer_t *fb, const void *data, int len);
 
@@ -519,15 +519,15 @@
 int flux_buffer_read_to_fd (flux_buffer_t *fb, int fd, int len);
 
 
 
 
 
 int flux_buffer_write_from_fd (flux_buffer_t *fb, int fd, int len);
-# 781 "/workspaces/flux-python/src/_core_clean.h"
+# 788 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_reactor flux_reactor_t;
 
 
 
 enum {
     FLUX_REACTOR_NOWAIT = 1,
     FLUX_REACTOR_ONCE = 2,
@@ -616,15 +616,15 @@
 
 
 flux_watcher_t *flux_buffer_write_watcher_create (flux_reactor_t *r, int fd,
                                                   int size, flux_watcher_f cb,
                                                   int flags, void *arg);
 
 flux_buffer_t *flux_buffer_write_watcher_get_buffer (flux_watcher_t *w);
-# 887 "/workspaces/flux-python/src/_core_clean.h"
+# 894 "/workspaces/flux-python/src/_core_clean.h"
 int flux_buffer_write_watcher_close (flux_watcher_t *w);
 
 
 int flux_buffer_write_watcher_is_closed (flux_watcher_t *w, int *close_err);
 
 
 
@@ -694,27 +694,27 @@
 
 
 struct flux_watcher_ops {
     void (*start) (flux_watcher_t *w);
     void (*stop) (flux_watcher_t *w);
     void (*destroy) (flux_watcher_t *w);
 };
-# 972 "/workspaces/flux-python/src/_core_clean.h"
+# 979 "/workspaces/flux-python/src/_core_clean.h"
 flux_watcher_t * flux_watcher_create (flux_reactor_t *r, size_t data_size,
                                       struct flux_watcher_ops *ops,
                                       flux_watcher_f fn, void *arg);
 
 
 
 void * flux_watcher_get_data (flux_watcher_t *w);
 
 
 
 struct flux_watcher_ops * flux_watcher_get_ops (flux_watcher_t *w);
-# 1011 "/workspaces/flux-python/src/_core_clean.h"
+# 1018 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_msg_handler flux_msg_handler_t;
 
 typedef void (*flux_msg_handler_f)(flux_t *h, flux_msg_handler_t *mh,
                                    const flux_msg_t *msg, void *arg);
 
 flux_msg_handler_t *flux_msg_handler_create (flux_t *h,
                                              const struct flux_match match,
@@ -738,24 +738,30 @@
     int typemask;
     const char *topic_glob;
     flux_msg_handler_f cb;
     uint32_t rolemask;
 };
 
 
+int flux_msg_handler_addvec_ex (flux_t *h,
+                                const char *service_name,
+                                const struct flux_msg_handler_spec tab[],
+                                void *arg,
+                                flux_msg_handler_t **hp[]);
+
 int flux_msg_handler_addvec (flux_t *h,
                              const struct flux_msg_handler_spec tab[],
                              void *arg,
                              flux_msg_handler_t **msg_handlers[]);
 void flux_msg_handler_delvec (flux_msg_handler_t *msg_handlers[]);
 
 
 
 int flux_dispatch_requeue (flux_t *h);
-# 1082 "/workspaces/flux-python/src/_core_clean.h"
+# 1095 "/workspaces/flux-python/src/_core_clean.h"
 typedef flux_t *(connector_init_f)(const char *uri,
                                    int flags,
                                    flux_error_t *errp);
 
 struct flux_handle_ops {
     int (*setopt)(void *impl, const char *option,
                           const void *val, size_t len);
@@ -768,32 +774,32 @@
     int (*reconnect)(void *impl);
 
     void (*impl_destroy)(void *impl);
 };
 
 flux_t *flux_handle_create (void *impl, const struct flux_handle_ops *ops, int flags);
 void flux_handle_destroy (flux_t *hp);
-# 1133 "/workspaces/flux-python/src/_core_clean.h"
+# 1146 "/workspaces/flux-python/src/_core_clean.h"
 struct flux_msglist *flux_msglist_create (void);
 void flux_msglist_destroy (struct flux_msglist *l);
 
 int flux_msglist_push (struct flux_msglist *l, const flux_msg_t *msg);
 int flux_msglist_append (struct flux_msglist *l, const flux_msg_t *msg);
 void flux_msglist_delete (struct flux_msglist *l);
 const flux_msg_t *flux_msglist_pop (struct flux_msglist *l);
 
 const flux_msg_t *flux_msglist_first (struct flux_msglist *l);
 const flux_msg_t *flux_msglist_next (struct flux_msglist *l);
 const flux_msg_t *flux_msglist_last (struct flux_msglist *l);
 
 int flux_msglist_count (struct flux_msglist *l);
-# 1154 "/workspaces/flux-python/src/_core_clean.h"
+# 1167 "/workspaces/flux-python/src/_core_clean.h"
 int flux_msglist_pollevents (struct flux_msglist *l);
 int flux_msglist_pollfd (struct flux_msglist *l);
-# 1190 "/workspaces/flux-python/src/_core_clean.h"
+# 1203 "/workspaces/flux-python/src/_core_clean.h"
 int flux_request_decode (const flux_msg_t *msg, const char **topic,
                          const char **s);
 
 
 
 
 
@@ -816,18 +822,18 @@
 
 
 
 
 
 flux_msg_t *flux_request_encode_raw (const char *topic,
                                      const void *data, int len);
-# 1256 "/workspaces/flux-python/src/_core_clean.h"
+# 1269 "/workspaces/flux-python/src/_core_clean.h"
 int flux_response_decode (const flux_msg_t *msg, const char **topic,
                           const char **s);
-# 1267 "/workspaces/flux-python/src/_core_clean.h"
+# 1280 "/workspaces/flux-python/src/_core_clean.h"
 int flux_response_decode_raw (const flux_msg_t *msg, const char **topic,
                               const void **data, int *len);
 
 
 
 
 
@@ -874,19 +880,19 @@
 
 
 
 
 
 int flux_respond_error (flux_t *h, const flux_msg_t *request,
                         int errnum, const char *errstr);
-# 1349 "/workspaces/flux-python/src/_core_clean.h"
+# 1362 "/workspaces/flux-python/src/_core_clean.h"
 flux_msg_t *flux_control_encode (int type, int status);
 
 int flux_control_decode (const flux_msg_t *msg, int *type, int *status);
-# 1410 "/workspaces/flux-python/src/_core_clean.h"
+# 1423 "/workspaces/flux-python/src/_core_clean.h"
 typedef void (*flux_log_f)(const char *buf, int len, void *arg);
 
 
 
 
 void flux_log_set_appname (flux_t *h, const char *s);
 
@@ -930,15 +936,15 @@
                 const char *file,
                 int line,
                 const char *func,
                 const char *subsys,
                 int level,
                 const char *fmt,
                 va_list ap);
-# 1480 "/workspaces/flux-python/src/_core_clean.h"
+# 1493 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_future flux_future_t;
 
 typedef void (*flux_continuation_f)(flux_future_t *f, void *arg);
 
 int flux_future_then (flux_future_t *f, double timeout,
                       flux_continuation_f cb, void *arg);
 
@@ -996,15 +1002,15 @@
 
 int flux_future_push (flux_future_t *cf, const char *name, flux_future_t *f);
 
 const char * flux_future_first_child (flux_future_t *cf);
 const char * flux_future_next_child (flux_future_t *cf);
 
 flux_future_t *flux_future_get_child (flux_future_t *cf, const char *name);
-# 1558 "/workspaces/flux-python/src/_core_clean.h"
+# 1571 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_future_and_then (flux_future_t *f,
                                      flux_continuation_f cb, void *arg);
 
 
 
 
 flux_future_t *flux_future_or_then (flux_future_t *f,
@@ -1024,15 +1030,15 @@
                                  const char *errstr);
 
 
 
 int flux_future_fulfill_next (flux_future_t *prev,
                               void *result,
                               flux_free_f free_fn);
-# 1600 "/workspaces/flux-python/src/_core_clean.h"
+# 1613 "/workspaces/flux-python/src/_core_clean.h"
 enum {
     FLUX_RPC_NORESPONSE = 1,
     FLUX_RPC_STREAMING = 2,
 };
 
 flux_future_t *flux_rpc (flux_t *h, const char *topic, const char *s,
                          uint32_t nodeid, int flags);
@@ -1062,17 +1068,17 @@
 
 
 uint32_t flux_rpc_get_matchtag (flux_future_t *f);
 
 
 
 uint32_t flux_rpc_get_nodeid (flux_future_t *f);
-# 1669 "/workspaces/flux-python/src/_core_clean.h"
+# 1682 "/workspaces/flux-python/src/_core_clean.h"
 int flux_panic (flux_t *h, uint32_t nodeid, int flags, const char *reason);
-# 1698 "/workspaces/flux-python/src/_core_clean.h"
+# 1711 "/workspaces/flux-python/src/_core_clean.h"
 enum event_flags {
     FLUX_EVENT_PRIVATE = 1,
 };
 
 
 
 int flux_event_subscribe (flux_t *h, const char *topic);
@@ -1145,57 +1151,41 @@
                                        const char *topic, int flags,
                                        const void *data, int len);
 
 
 
 
 int flux_event_publish_get_seq (flux_future_t *f, int *seq);
-# 1813 "/workspaces/flux-python/src/_core_clean.h"
+# 1822 "/workspaces/flux-python/src/_core_clean.h"
 enum {
     FLUX_MODSTATE_INIT = 0,
     FLUX_MODSTATE_RUNNING = 1,
     FLUX_MODSTATE_FINALIZING = 2,
     FLUX_MODSTATE_EXITED = 3,
 };
 
 
 
 
 typedef int (mod_main_f)(flux_t *h, int argc, char *argv[]);
 
-typedef void (flux_moderr_f)(const char *errmsg, void *arg);
-
-
-
-
-
-char *flux_modname (const char *filename, flux_moderr_f *cb, void *arg);
-
-
-
-
-
-
-char *flux_modfind (const char *searchpath, const char *modname,
-                    flux_moderr_f *cb, void *arg);
-
 
 
 
 
 
 bool flux_module_debug_test (flux_t *h, int flag, bool clear);
 
 
 
 
 
 
 int flux_module_set_running (flux_t *h);
-# 1902 "/workspaces/flux-python/src/_core_clean.h"
+# 1895 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_attr_get (flux_t *h, const char *name);
 
 
 
 
 
 
@@ -1222,26 +1212,26 @@
 const char *flux_get_hostbyrank (flux_t *h, uint32_t rank);
 
 
 
 
 
 int flux_get_rankbyhost (flux_t *h, const char *host);
-# 1950 "/workspaces/flux-python/src/_core_clean.h"
+# 1943 "/workspaces/flux-python/src/_core_clean.h"
 char *flux_hostmap_lookup (flux_t *h,
                            const char *targets,
                            flux_error_t *errp);
 
 
 
 
 
 
 int flux_get_instance_starttime (flux_t *h, double *starttime);
-# 1988 "/workspaces/flux-python/src/_core_clean.h"
+# 1981 "/workspaces/flux-python/src/_core_clean.h"
 enum flux_conf_flags {
     FLUX_CONF_INSTALLED=0,
     FLUX_CONF_INTREE=1,
     FLUX_CONF_AUTO=2,
 };
 
 
@@ -1286,30 +1276,30 @@
                        flux_error_t *error,
                        const char *fmt,
                        va_list ap);
 
 int flux_conf_unpack (const flux_conf_t *conf,
                       flux_error_t *error,
                       const char *fmt, ...);
-# 2072 "/workspaces/flux-python/src/_core_clean.h"
+# 2065 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_barrier (flux_t *h, const char *name, int nprocs);
-# 2115 "/workspaces/flux-python/src/_core_clean.h"
+# 2108 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_service_register (flux_t *h, const char *name);
-# 2127 "/workspaces/flux-python/src/_core_clean.h"
+# 2120 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_service_unregister (flux_t *h, const char *name);
-# 2179 "/workspaces/flux-python/src/_core_clean.h"
+# 2172 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_core_version_string (void);
 
 
 
 
 
 
 int flux_core_version (int *major, int *minor, int *patch);
-# 2217 "/workspaces/flux-python/src/_core_clean.h"
+# 2210 "/workspaces/flux-python/src/_core_clean.h"
 enum {
     FLUX_PLUGIN_RTLD_LAZY = 1,
     FLUX_PLUGIN_RTLD_NOW = 2,
     FLUX_PLUGIN_RTLD_GLOBAL = 4,
     FLUX_PLUGIN_RTLD_DEEPBIND = 8,
 };
 
@@ -1379,15 +1369,15 @@
 
 
 
 
 int flux_plugin_register (flux_plugin_t *p,
                           const char *name,
                           const struct flux_plugin_handler t[]);
-# 2304 "/workspaces/flux-python/src/_core_clean.h"
+# 2297 "/workspaces/flux-python/src/_core_clean.h"
 int flux_plugin_aux_set (flux_plugin_t *p,
                          const char *key,
                          void *val,
                          flux_free_f free_fn);
 
 
 
@@ -1441,22 +1431,22 @@
 int flux_plugin_arg_vpack (flux_plugin_arg_t *args, int flags,
                            const char *fmt, va_list ap);
 
 int flux_plugin_arg_unpack (flux_plugin_arg_t *args, int flags,
                             const char *fmt, ...);
 int flux_plugin_arg_vunpack (flux_plugin_arg_t *args, int flags,
                              const char *fmt, va_list ap);
-# 2373 "/workspaces/flux-python/src/_core_clean.h"
+# 2366 "/workspaces/flux-python/src/_core_clean.h"
 int flux_plugin_call (flux_plugin_t *p, const char *name,
                       flux_plugin_arg_t *args);
-# 2383 "/workspaces/flux-python/src/_core_clean.h"
+# 2376 "/workspaces/flux-python/src/_core_clean.h"
 int flux_plugin_load_dso (flux_plugin_t *p, const char *path);
-# 2416 "/workspaces/flux-python/src/_core_clean.h"
+# 2409 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_sync_create (flux_t *h, double minimum);
-# 2448 "/workspaces/flux-python/src/_core_clean.h"
+# 2441 "/workspaces/flux-python/src/_core_clean.h"
 bool flux_disconnect_match (const flux_msg_t *msg1, const flux_msg_t *msg2);
 
 
 
 
 int flux_msglist_disconnect (struct flux_msglist *l, const flux_msg_t *msg);
 
@@ -1468,15 +1458,15 @@
 
 
 
 
 int flux_msglist_cancel (flux_t *h,
                          struct flux_msglist *l,
                          const flux_msg_t *msg);
-# 2517 "/workspaces/flux-python/src/_core_clean.h"
+# 2510 "/workspaces/flux-python/src/_core_clean.h"
 void flux_stats_count (flux_t *h, const char *name, ssize_t count);
 
 
 
 
 void flux_stats_gauge_set (flux_t *h, const char *name, ssize_t value);
 
@@ -1504,18 +1494,18 @@
 
 void flux_stats_set_prefix (flux_t *h, const char *fmt, ...);
 
 
 
 
 bool flux_stats_enabled (flux_t *h, const char *metric);
-# 2600 "/workspaces/flux-python/src/_core_clean.h"
+# 2593 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_kvsdir flux_kvsdir_t;
 typedef struct flux_kvsitr flux_kvsitr_t;
-# 2615 "/workspaces/flux-python/src/_core_clean.h"
+# 2608 "/workspaces/flux-python/src/_core_clean.h"
 flux_kvsdir_t *flux_kvsdir_create (flux_t *handle, const char *rootref,
                                    const char *key, const char *json_str);
 void flux_kvsdir_destroy (flux_kvsdir_t *dir);
 
 flux_kvsdir_t *flux_kvsdir_copy (const flux_kvsdir_t *dir);
 void flux_kvsdir_incref (flux_kvsdir_t *dir);
 
@@ -1553,15 +1543,15 @@
 void *flux_kvsdir_handle (const flux_kvsdir_t *dir);
 const char *flux_kvsdir_rootref (const flux_kvsdir_t *dir);
 
 
 
 
 char *flux_kvsdir_key_at (const flux_kvsdir_t *dir, const char *key);
-# 2688 "/workspaces/flux-python/src/_core_clean.h"
+# 2681 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_lookup (flux_t *h, const char *ns, int flags,
                                 const char *key);
 flux_future_t *flux_kvs_lookupat (flux_t *h, int flags, const char *key,
                                   const char *treeobj);
 
 int flux_kvs_lookup_get (flux_future_t *f, const char **value);
 int flux_kvs_lookup_get_unpack (flux_future_t *f, const char *fmt, ...);
@@ -1576,22 +1566,22 @@
 
 
 
 
 
 
 int flux_kvs_lookup_cancel (flux_future_t *f);
-# 2738 "/workspaces/flux-python/src/_core_clean.h"
+# 2731 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_getroot (flux_t *h, const char *ns, int flags);
-# 2747 "/workspaces/flux-python/src/_core_clean.h"
+# 2740 "/workspaces/flux-python/src/_core_clean.h"
 int flux_kvs_getroot_get_treeobj (flux_future_t *f, const char **treeobj);
 int flux_kvs_getroot_get_blobref (flux_future_t *f, const char **blobref);
 int flux_kvs_getroot_get_sequence (flux_future_t *f, int *seq);
 int flux_kvs_getroot_get_owner (flux_future_t *f, uint32_t *owner);
-# 2779 "/workspaces/flux-python/src/_core_clean.h"
+# 2772 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_kvs_txn flux_kvs_txn_t;
 
 flux_kvs_txn_t *flux_kvs_txn_create (void);
 void flux_kvs_txn_destroy (flux_kvs_txn_t *txn);
 
 int flux_kvs_txn_put (flux_kvs_txn_t *txn, int flags,
                       const char *key, const char *value);
@@ -1613,15 +1603,15 @@
 
 int flux_kvs_txn_unlink (flux_kvs_txn_t *txn, int flags,
                          const char *key);
 
 int flux_kvs_txn_symlink (flux_kvs_txn_t *txn, int flags,
                           const char *key, const char *ns,
                           const char *target);
-# 2857 "/workspaces/flux-python/src/_core_clean.h"
+# 2850 "/workspaces/flux-python/src/_core_clean.h"
 enum kvs_commit_flags {
     FLUX_KVS_NO_MERGE = 1,
     FLUX_KVS_TXN_COMPACT = 2,
     FLUX_KVS_SYNC = 4,
 };
 
 flux_future_t *flux_kvs_commit (flux_t *h, const char *ns, int flags,
@@ -1631,41 +1621,41 @@
                                const char *name, int nprocs,
                                flux_kvs_txn_t *txn);
 
 
 int flux_kvs_commit_get_treeobj (flux_future_t *f, const char **treeobj);
 int flux_kvs_commit_get_rootref (flux_future_t *f, const char **rootref);
 int flux_kvs_commit_get_sequence (flux_future_t *f, int *rootseq);
-# 2913 "/workspaces/flux-python/src/_core_clean.h"
+# 2906 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_copy (flux_t *h,
                               const char *srcns,
                               const char *srckey,
                               const char *dstns,
                               const char *dstkey,
                               int commit_flags);
-# 2930 "/workspaces/flux-python/src/_core_clean.h"
+# 2923 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_move (flux_t *h,
                               const char *srcns,
                               const char *srckey,
                               const char *dstns,
                               const char *dstkey,
                               int commit_flags);
-# 2953 "/workspaces/flux-python/src/_core_clean.h"
+# 2946 "/workspaces/flux-python/src/_core_clean.h"
 enum kvs_op {
     FLUX_KVS_READDIR = 1,
     FLUX_KVS_READLINK = 2,
     FLUX_KVS_WATCH = 4,
     FLUX_KVS_WAITCREATE = 8,
     FLUX_KVS_TREEOBJ = 16,
     FLUX_KVS_APPEND = 32,
     FLUX_KVS_WATCH_FULL = 64,
     FLUX_KVS_WATCH_UNIQ = 128,
     FLUX_KVS_WATCH_APPEND = 256
 };
-# 2974 "/workspaces/flux-python/src/_core_clean.h"
+# 2967 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_namespace_create (flux_t *h, const char *ns,
                                           uint32_t owner, int flags);
 flux_future_t *flux_kvs_namespace_create_with (flux_t *h, const char *ns,
                                                const char *rootref,
                                                uint32_t owner, int flags);
 flux_future_t *flux_kvs_namespace_remove (flux_t *h, const char *ns);
 
@@ -1678,605 +1668,606 @@
 
 
 
 
 
 
 int flux_kvs_dropcache (flux_t *h);
-# 3029 "/workspaces/flux-python/src/_core_clean.h"
-typedef struct flux_command flux_cmd_t;
-
+# 3015 "/workspaces/flux-python/src/_core_clean.h"
+enum job_submit_flags {
+    FLUX_JOB_PRE_SIGNED = 1,
+    FLUX_JOB_DEBUG = 2,
+    FLUX_JOB_WAITABLE = 4,
+    FLUX_JOB_NOVALIDATE = 8,
+};
 
+enum job_urgency {
+    FLUX_JOB_URGENCY_MIN = 0,
+    FLUX_JOB_URGENCY_HOLD = FLUX_JOB_URGENCY_MIN,
+    FLUX_JOB_URGENCY_DEFAULT = 16,
+    FLUX_JOB_URGENCY_MAX = 31,
+    FLUX_JOB_URGENCY_EXPEDITE = FLUX_JOB_URGENCY_MAX,
+};
 
+enum job_queue_priority {
+    FLUX_JOB_PRIORITY_MIN = 0,
+    FLUX_JOB_PRIORITY_MAX = 4294967295,
+};
 
 
 
 
-typedef struct flux_subprocess flux_subprocess_t;
-# 3049 "/workspaces/flux-python/src/_core_clean.h"
 typedef enum {
-    FLUX_SUBPROCESS_INIT,
-    FLUX_SUBPROCESS_RUNNING,
-    FLUX_SUBPROCESS_EXITED,
-    FLUX_SUBPROCESS_FAILED,
-    FLUX_SUBPROCESS_STOPPED,
-} flux_subprocess_state_t;
+    FLUX_JOB_STATE_NEW = 1,
+    FLUX_JOB_STATE_DEPEND = 2,
+    FLUX_JOB_STATE_PRIORITY = 4,
+    FLUX_JOB_STATE_SCHED = 8,
+    FLUX_JOB_STATE_RUN = 16,
+    FLUX_JOB_STATE_CLEANUP = 32,
+    FLUX_JOB_STATE_INACTIVE = 64,
+} flux_job_state_t;
+
 
 
 
 
 enum {
 
+    FLUX_JOB_STATE_PENDING = 14,
 
+    FLUX_JOB_STATE_RUNNING = 48,
 
+    FLUX_JOB_STATE_ACTIVE = 62,
+};
 
 
-    FLUX_SUBPROCESS_FLAGS_STDIO_FALLTHROUGH = 1,
 
-    FLUX_SUBPROCESS_FLAGS_SETPGRP = 2,
+typedef enum {
+    FLUX_JOB_RESULT_COMPLETED = 1,
+    FLUX_JOB_RESULT_FAILED = 2,
+    FLUX_JOB_RESULT_CANCELED = 4,
+    FLUX_JOB_RESULT_TIMEOUT = 8,
+} flux_job_result_t;
 
-    FLUX_SUBPROCESS_FLAGS_FORK_EXEC = 4,
-};
+typedef uint64_t flux_jobid_t;
 
 
 
 
+int flux_job_id_parse (const char *s, flux_jobid_t *id);
+# 3085 "/workspaces/flux-python/src/_core_clean.h"
+int flux_job_id_encode (flux_jobid_t id, const char *type,
+                        char *buf, size_t bufsz);
+# 3096 "/workspaces/flux-python/src/_core_clean.h"
+const char *flux_job_statetostr (flux_job_state_t state, const char *fmt);
 
-typedef void (*flux_subprocess_f) (flux_subprocess_t *p);
-typedef void (*flux_subprocess_output_f) (flux_subprocess_t *p,
-                                          const char *stream);
-typedef void (*flux_subprocess_state_f) (flux_subprocess_t *p,
-                                         flux_subprocess_state_t state);
-typedef void (*flux_subprocess_hook_f) (flux_subprocess_t *p, void *arg);
 
 
 
+int flux_job_strtostate (const char *s, flux_job_state_t *state);
 
+const char *flux_job_resulttostr (flux_job_result_t result, const char *fmt);
 
-typedef struct {
-    flux_subprocess_f on_completion;
+int flux_job_strtoresult (const char *s, flux_job_result_t *result);
 
 
 
-    flux_subprocess_state_f on_state_change;
-    flux_subprocess_output_f on_channel_out;
-    flux_subprocess_output_f on_stdout;
-    flux_subprocess_output_f on_stderr;
-} flux_subprocess_ops_t;
 
 
 
 
+flux_future_t *flux_job_submit (flux_t *h, const char *jobspec,
+                                int urgency, int flags);
 
-typedef struct {
-    flux_subprocess_hook_f pre_exec;
-    void *pre_exec_arg;
-    flux_subprocess_hook_f post_fork;
-    void *post_fork_arg;
-} flux_subprocess_hooks_t;
-# 3120 "/workspaces/flux-python/src/_core_clean.h"
-void flux_standard_output (flux_subprocess_t *p, const char *stream);
-# 3129 "/workspaces/flux-python/src/_core_clean.h"
-flux_cmd_t * flux_cmd_create (int argc, char *argv[], char **env);
 
 
 
 
-flux_cmd_t * flux_cmd_copy (const flux_cmd_t *cmd);
+int flux_job_submit_get_id (flux_future_t *f, flux_jobid_t *id);
 
 
 
 
-void flux_cmd_destroy (flux_cmd_t *cmd);
 
+flux_future_t *flux_job_wait (flux_t *h, flux_jobid_t id);
+int flux_job_wait_get_status (flux_future_t *f,
+                              bool *success,
+                              const char **errstr);
+int flux_job_wait_get_id (flux_future_t *f, flux_jobid_t *id);
 
 
 
-int flux_cmd_argv_appendf (flux_cmd_t *cmd, const char *fmt, ...)
-                           ;
 
 
+                                                   ;
 
 
-int flux_cmd_argv_append (flux_cmd_t *cmd, const char *arg);
 
 
+                                                                     ;
 
 
-int flux_cmd_argv_delete (flux_cmd_t *cmd, int n);
 
+flux_future_t *flux_job_list_id (flux_t *h,
+                                 flux_jobid_t id,
+                                 const char *attrs_json_str);
 
 
 
-int flux_cmd_argv_insert (flux_cmd_t *cmd, int n, const char *arg);
 
 
+flux_future_t *flux_job_raise (flux_t *h, flux_jobid_t id,
+                               const char *type, int severity,
+                               const char *note);
 
 
-int flux_cmd_argc (const flux_cmd_t *cmd);
 
 
+flux_future_t *flux_job_cancel (flux_t *h, flux_jobid_t id, const char *reason);
 
 
-const char *flux_cmd_arg (const flux_cmd_t *cmd, int n);
 
+flux_future_t *flux_job_kill (flux_t *h, flux_jobid_t id, int signum);
 
 
 
-char *flux_cmd_stringify (const flux_cmd_t *cmd);
+flux_future_t *flux_job_set_urgency (flux_t *h, flux_jobid_t id, int urgency);
 
 
 
 
 
-int flux_cmd_setenvf (flux_cmd_t *cmd, int overwrite,
-        const char *name, const char *fmt, ...)
-                      ;
+int flux_job_kvs_key (char *buf, int bufsz, flux_jobid_t id, const char *key);
 
 
 
 
-void flux_cmd_unsetenv (flux_cmd_t *cmd, const char *name);
+int flux_job_kvs_guest_key (char *buf,
+                            int bufsz,
+                            flux_jobid_t id,
+                            const char *key);
 
 
 
 
 
+int flux_job_kvs_namespace (char *buf,
+                            int bufsz,
+                            flux_jobid_t id);
 
-const char *flux_cmd_getenv (const flux_cmd_t *cmd, const char *name);
 
 
 
+flux_future_t *flux_job_event_watch (flux_t *h, flux_jobid_t id,
+                                     const char *path, int flags);
+int flux_job_event_watch_get (flux_future_t *f, const char **event);
+int flux_job_event_watch_cancel (flux_future_t *f);
 
-int flux_cmd_setcwd (flux_cmd_t *cmd, const char *cwd);
-const char *flux_cmd_getcwd (const flux_cmd_t *cmd);
-# 3215 "/workspaces/flux-python/src/_core_clean.h"
-int flux_cmd_add_channel (flux_cmd_t *cmd, const char *name);
-# 3265 "/workspaces/flux-python/src/_core_clean.h"
-int flux_cmd_setopt (flux_cmd_t *cmd, const char *var, const char *val);
-const char *flux_cmd_getopt (flux_cmd_t *cmd, const char *var);
-# 3288 "/workspaces/flux-python/src/_core_clean.h"
-flux_subprocess_t *flux_exec (flux_t *h, int flags,
-                              const flux_cmd_t *cmd,
-                              const flux_subprocess_ops_t *ops,
-                              const flux_subprocess_hooks_t *hooks);
 
-flux_subprocess_t *flux_local_exec (flux_reactor_t *r, int flags,
-                                    const flux_cmd_t *cmd,
-                                    const flux_subprocess_ops_t *ops,
-                                    const flux_subprocess_hooks_t *hooks);
 
-flux_subprocess_t *flux_rexec (flux_t *h, int rank, int flags,
-                               const flux_cmd_t *cmd,
-                               const flux_subprocess_ops_t *ops);
-# 3310 "/workspaces/flux-python/src/_core_clean.h"
-int flux_subprocess_stream_start (flux_subprocess_t *p, const char *stream);
-int flux_subprocess_stream_stop (flux_subprocess_t *p, const char *stream);
-int flux_subprocess_stream_status (flux_subprocess_t *p, const char *stream);
 
+flux_future_t *flux_job_result (flux_t *h, flux_jobid_t id, int flags);
 
 
 
+int flux_job_result_get (flux_future_t *f,
+                         const char **json_str);
+# 3227 "/workspaces/flux-python/src/_core_clean.h"
+int flux_job_result_get_unpack (flux_future_t *f, const char *fmt, ...);
+# 3241 "/workspaces/flux-python/src/_core_clean.h"
+int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
+# 3266 "/workspaces/flux-python/src/_core_clean.h"
+typedef struct flux_jobspec1 flux_jobspec1_t;
+typedef flux_error_t flux_jobspec1_error_t;
 
 
 
-int flux_subprocess_write (flux_subprocess_t *p, const char *stream,
-                           const char *buf, size_t len);
 
 
 
+int flux_jobspec1_attr_del (flux_jobspec1_t *jobspec, const char *path);
 
 
 
-int flux_subprocess_close (flux_subprocess_t *p, const char *stream);
-# 3341 "/workspaces/flux-python/src/_core_clean.h"
-const char *flux_subprocess_read (flux_subprocess_t *p,
-                                  const char *stream,
-                                  int len, int *lenp);
-# 3356 "/workspaces/flux-python/src/_core_clean.h"
-const char *flux_subprocess_read_line (flux_subprocess_t *p,
-                                       const char *stream,
-                                       int *lenp);
 
 
 
+int flux_jobspec1_attr_pack (flux_jobspec1_t *jobspec,
+                             const char *path,
+                             const char *fmt,
+                             ...);
 
-const char *flux_subprocess_read_trimmed_line (flux_subprocess_t *p,
-                                               const char *stream,
-                                               int *lenp);
-# 3376 "/workspaces/flux-python/src/_core_clean.h"
-int flux_subprocess_read_stream_closed (flux_subprocess_t *p,
-                                        const char *stream);
-# 3395 "/workspaces/flux-python/src/_core_clean.h"
-const char *flux_subprocess_getline (flux_subprocess_t *p,
-                                     const char *stream,
-                                     int *lenp);
 
 
 
 
 
+int flux_jobspec1_attr_unpack (flux_jobspec1_t *jobspec,
+                               const char *path,
+                               const char *fmt,
+                               ...);
 
 
-flux_future_t *flux_subprocess_kill (flux_subprocess_t *p, int signo);
 
 
 
 
 
+int flux_jobspec1_attr_check (flux_jobspec1_t *jobspec,
+                              flux_jobspec1_error_t *error);
 
-void flux_subprocess_ref (flux_subprocess_t *p);
-void flux_subprocess_unref (flux_subprocess_t *p);
-# 3422 "/workspaces/flux-python/src/_core_clean.h"
-flux_subprocess_state_t flux_subprocess_state (flux_subprocess_t *p);
 
 
 
-const char *flux_subprocess_state_string (flux_subprocess_state_t state);
 
-int flux_subprocess_rank (flux_subprocess_t *p);
 
+int flux_jobspec1_check (flux_jobspec1_t *jobspec,
+                         flux_jobspec1_error_t *error);
 
 
-int flux_subprocess_fail_errno (flux_subprocess_t *p);
 
 
 
-int flux_subprocess_status (flux_subprocess_t *p);
+int flux_jobspec1_unsetenv (flux_jobspec1_t *jobspec, const char *name);
 
 
 
-int flux_subprocess_exit_code (flux_subprocess_t *p);
 
 
 
-int flux_subprocess_signaled (flux_subprocess_t *p);
 
-pid_t flux_subprocess_pid (flux_subprocess_t *p);
+int flux_jobspec1_setenv (flux_jobspec1_t *jobspec,
+                           const char *name,
+                           const char *value,
+                           int overwrite);
 
 
 
-flux_cmd_t *flux_subprocess_get_cmd (flux_subprocess_t *p);
 
+int flux_jobspec1_set_stdin (flux_jobspec1_t *jobspec, const char *path);
 
 
-flux_reactor_t * flux_subprocess_get_reactor (flux_subprocess_t *p);
 
 
+int flux_jobspec1_set_stdout (flux_jobspec1_t *jobspec, const char *path);
 
 
 
 
-int flux_subprocess_aux_set (flux_subprocess_t *p,
-                             const char *name, void *ctx, flux_free_f free);
+int flux_jobspec1_set_stderr (flux_jobspec1_t *jobspec, const char *path);
 
 
 
 
+int flux_jobspec1_set_cwd (flux_jobspec1_t *jobspec, const char *cwd);
 
-void *flux_subprocess_aux_get (flux_subprocess_t *p, const char *name);
 
-typedef void (*subprocess_log_f) (void *arg,
-                                  const char *file,
-                                  int line,
-                                  const char *func,
-                                  const char *subsys,
-                                  int level,
-                                  const char *fmt,
-                                  va_list args);
 
 
 
-int flux_set_default_subprocess_log (flux_t *h,
-                                     subprocess_log_f log_fn,
-                                     void *log_data);
-# 3510 "/workspaces/flux-python/src/_core_clean.h"
-enum job_submit_flags {
-    FLUX_JOB_PRE_SIGNED = 1,
-    FLUX_JOB_DEBUG = 2,
-    FLUX_JOB_WAITABLE = 4,
-    FLUX_JOB_NOVALIDATE = 8,
-};
+char *flux_jobspec1_encode (flux_jobspec1_t *jobspec, size_t flags);
 
-enum job_urgency {
-    FLUX_JOB_URGENCY_MIN = 0,
-    FLUX_JOB_URGENCY_HOLD = FLUX_JOB_URGENCY_MIN,
-    FLUX_JOB_URGENCY_DEFAULT = 16,
-    FLUX_JOB_URGENCY_MAX = 31,
-    FLUX_JOB_URGENCY_EXPEDITE = FLUX_JOB_URGENCY_MAX,
-};
 
-enum job_queue_priority {
-    FLUX_JOB_PRIORITY_MIN = 0,
-    FLUX_JOB_PRIORITY_MAX = 4294967295,
-};
 
 
 
 
-typedef enum {
-    FLUX_JOB_STATE_NEW = 1,
-    FLUX_JOB_STATE_DEPEND = 2,
-    FLUX_JOB_STATE_PRIORITY = 4,
-    FLUX_JOB_STATE_SCHED = 8,
-    FLUX_JOB_STATE_RUN = 16,
-    FLUX_JOB_STATE_CLEANUP = 32,
-    FLUX_JOB_STATE_INACTIVE = 64,
-} flux_job_state_t;
+flux_jobspec1_t *flux_jobspec1_decode (const char *s,
+                                       flux_jobspec1_error_t *error);
+# 3377 "/workspaces/flux-python/src/_core_clean.h"
+flux_jobspec1_t *flux_jobspec1_from_command (int argc,
+                                             char **argv,
+                                             char **env,
+                                             int ntasks,
+                                             int cores_per_task,
+                                             int gpus_per_task,
+                                             int nnodes,
+                                             double duration);
 
 
+void flux_jobspec1_destroy (flux_jobspec1_t *jobspec);
+# 3419 "/workspaces/flux-python/src/_core_clean.h"
+typedef struct flux_command flux_cmd_t;
 
 
 
-enum {
 
-    FLUX_JOB_STATE_PENDING = 14,
 
-    FLUX_JOB_STATE_RUNNING = 48,
 
-    FLUX_JOB_STATE_ACTIVE = 62,
-};
 
+typedef struct flux_subprocess flux_subprocess_t;
+# 3439 "/workspaces/flux-python/src/_core_clean.h"
+typedef enum {
+    FLUX_SUBPROCESS_INIT,
+    FLUX_SUBPROCESS_RUNNING,
+    FLUX_SUBPROCESS_EXITED,
+    FLUX_SUBPROCESS_FAILED,
+    FLUX_SUBPROCESS_STOPPED,
+} flux_subprocess_state_t;
 
 
-typedef enum {
-    FLUX_JOB_RESULT_COMPLETED = 1,
-    FLUX_JOB_RESULT_FAILED = 2,
-    FLUX_JOB_RESULT_CANCELED = 4,
-    FLUX_JOB_RESULT_TIMEOUT = 8,
-} flux_job_result_t;
 
-typedef uint64_t flux_jobid_t;
 
+enum {
 
 
 
-int flux_job_id_parse (const char *s, flux_jobid_t *id);
-# 3580 "/workspaces/flux-python/src/_core_clean.h"
-int flux_job_id_encode (flux_jobid_t id, const char *type,
-                        char *buf, size_t bufsz);
-# 3591 "/workspaces/flux-python/src/_core_clean.h"
-const char *flux_job_statetostr (flux_job_state_t state, const char *fmt);
 
 
+    FLUX_SUBPROCESS_FLAGS_STDIO_FALLTHROUGH = 1,
 
+    FLUX_SUBPROCESS_FLAGS_SETPGRP = 2,
 
-int flux_job_strtostate (const char *s, flux_job_state_t *state);
+    FLUX_SUBPROCESS_FLAGS_FORK_EXEC = 4,
+};
 
-const char *flux_job_resulttostr (flux_job_result_t result, const char *fmt);
 
-int flux_job_strtoresult (const char *s, flux_job_result_t *result);
 
 
 
+typedef void (*flux_subprocess_f) (flux_subprocess_t *p);
+typedef void (*flux_subprocess_output_f) (flux_subprocess_t *p,
+                                          const char *stream);
+typedef void (*flux_subprocess_state_f) (flux_subprocess_t *p,
+                                         flux_subprocess_state_t state);
+typedef void (*flux_subprocess_hook_f) (flux_subprocess_t *p, void *arg);
 
 
 
 
-flux_future_t *flux_job_submit (flux_t *h, const char *jobspec,
-                                int urgency, int flags);
 
+typedef struct {
+    flux_subprocess_f on_completion;
 
 
 
+    flux_subprocess_state_f on_state_change;
+    flux_subprocess_output_f on_channel_out;
+    flux_subprocess_output_f on_stdout;
+    flux_subprocess_output_f on_stderr;
+} flux_subprocess_ops_t;
 
-int flux_job_submit_get_id (flux_future_t *f, flux_jobid_t *id);
 
 
 
 
+typedef struct {
+    flux_subprocess_hook_f pre_exec;
+    void *pre_exec_arg;
+    flux_subprocess_hook_f post_fork;
+    void *post_fork_arg;
+} flux_subprocess_hooks_t;
 
-flux_future_t *flux_job_wait (flux_t *h, flux_jobid_t id);
-int flux_job_wait_get_status (flux_future_t *f,
-                              bool *success,
-                              const char **errstr);
-int flux_job_wait_get_id (flux_future_t *f, flux_jobid_t *id);
-# 3644 "/workspaces/flux-python/src/_core_clean.h"
-flux_future_t *flux_job_list (flux_t *h,
-                              int max_entries,
-                              const char *attrs_json_str,
-                              uint32_t userid,
-                              int states);
 
 
 
+typedef void (*subprocess_log_f) (void *arg,
+                                  const char *file,
+                                  int line,
+                                  const char *func,
+                                  const char *subsys,
+                                  int level,
+                                  const char *fmt,
+                                  va_list args);
+# 3523 "/workspaces/flux-python/src/_core_clean.h"
+void flux_standard_output (flux_subprocess_t *p, const char *stream);
+# 3532 "/workspaces/flux-python/src/_core_clean.h"
+flux_cmd_t * flux_cmd_create (int argc, char *argv[], char **env);
 
-flux_future_t *flux_job_list_inactive (flux_t *h,
-                                       int max_entries,
-                                       double since,
-                                       const char *attrs_json_str);
 
 
 
-flux_future_t *flux_job_list_id (flux_t *h,
-                                 flux_jobid_t id,
-                                 const char *attrs_json_str);
+flux_cmd_t * flux_cmd_copy (const flux_cmd_t *cmd);
 
 
 
 
+void flux_cmd_destroy (flux_cmd_t *cmd);
 
-flux_future_t *flux_job_raise (flux_t *h, flux_jobid_t id,
-                               const char *type, int severity,
-                               const char *note);
 
 
 
+int flux_cmd_argv_appendf (flux_cmd_t *cmd, const char *fmt, ...)
+                           ;
 
-flux_future_t *flux_job_cancel (flux_t *h, flux_jobid_t id, const char *reason);
 
 
 
-flux_future_t *flux_job_kill (flux_t *h, flux_jobid_t id, int signum);
+int flux_cmd_argv_append (flux_cmd_t *cmd, const char *arg);
 
 
 
-flux_future_t *flux_job_set_urgency (flux_t *h, flux_jobid_t id, int urgency);
 
+int flux_cmd_argv_delete (flux_cmd_t *cmd, int n);
 
 
 
 
-int flux_job_kvs_key (char *buf, int bufsz, flux_jobid_t id, const char *key);
+int flux_cmd_argv_insert (flux_cmd_t *cmd, int n, const char *arg);
 
 
 
 
-int flux_job_kvs_guest_key (char *buf,
-                            int bufsz,
-                            flux_jobid_t id,
-                            const char *key);
+int flux_cmd_argc (const flux_cmd_t *cmd);
 
 
 
 
+const char *flux_cmd_arg (const flux_cmd_t *cmd, int n);
 
-int flux_job_kvs_namespace (char *buf,
-                            int bufsz,
-                            flux_jobid_t id);
 
 
 
+char *flux_cmd_stringify (const flux_cmd_t *cmd);
 
-flux_future_t *flux_job_event_watch (flux_t *h, flux_jobid_t id,
-                                     const char *path, int flags);
-int flux_job_event_watch_get (flux_future_t *f, const char **event);
-int flux_job_event_watch_cancel (flux_future_t *f);
 
 
 
 
-flux_future_t *flux_job_result (flux_t *h, flux_jobid_t id, int flags);
+int flux_cmd_setenvf (flux_cmd_t *cmd, int overwrite,
+                      const char *name, const char *fmt, ...)
+                      ;
 
 
 
-int flux_job_result_get (flux_future_t *f,
-                         const char **json_str);
-# 3742 "/workspaces/flux-python/src/_core_clean.h"
-int flux_job_result_get_unpack (flux_future_t *f, const char *fmt, ...);
-# 3756 "/workspaces/flux-python/src/_core_clean.h"
-int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
-# 3781 "/workspaces/flux-python/src/_core_clean.h"
-typedef struct flux_jobspec1 flux_jobspec1_t;
-typedef flux_error_t flux_jobspec1_error_t;
 
+void flux_cmd_unsetenv (flux_cmd_t *cmd, const char *name);
 
 
 
 
 
-int flux_jobspec1_attr_del (flux_jobspec1_t *jobspec, const char *path);
+
+const char *flux_cmd_getenv (const flux_cmd_t *cmd, const char *name);
 
 
 
 
+int flux_cmd_setcwd (flux_cmd_t *cmd, const char *cwd);
+const char *flux_cmd_getcwd (const flux_cmd_t *cmd);
+# 3618 "/workspaces/flux-python/src/_core_clean.h"
+int flux_cmd_add_channel (flux_cmd_t *cmd, const char *name);
+# 3668 "/workspaces/flux-python/src/_core_clean.h"
+int flux_cmd_setopt (flux_cmd_t *cmd, const char *var, const char *val);
+const char *flux_cmd_getopt (flux_cmd_t *cmd, const char *var);
+# 3691 "/workspaces/flux-python/src/_core_clean.h"
+flux_subprocess_t *flux_local_exec (flux_reactor_t *r,
+                                    int flags,
+                                    const flux_cmd_t *cmd,
+                                    const flux_subprocess_ops_t *ops);
 
+flux_subprocess_t *flux_local_exec_ex (flux_reactor_t *r,
+                                       int flags,
+                                       const flux_cmd_t *cmd,
+                                       const flux_subprocess_ops_t *ops,
+                                       const flux_subprocess_hooks_t *hooks,
+                                       subprocess_log_f log_fn,
+                                       void *log_data);
 
-int flux_jobspec1_attr_pack (flux_jobspec1_t *jobspec,
-                             const char *path,
-                             const char *fmt,
-                             ...);
+flux_subprocess_t *flux_rexec (flux_t *h, int rank, int flags,
+                               const flux_cmd_t *cmd,
+                               const flux_subprocess_ops_t *ops);
 
+flux_subprocess_t *flux_rexec_ex (flux_t *h,
+                                  const char *service_name,
+                                  int rank,
+                                  int flags,
+                                  const flux_cmd_t *cmd,
+                                  const flux_subprocess_ops_t *ops,
+                                  subprocess_log_f log_fn,
+                                  void *log_data);
+# 3726 "/workspaces/flux-python/src/_core_clean.h"
+int flux_subprocess_stream_start (flux_subprocess_t *p, const char *stream);
+int flux_subprocess_stream_stop (flux_subprocess_t *p, const char *stream);
+int flux_subprocess_stream_status (flux_subprocess_t *p, const char *stream);
 
 
 
 
 
-int flux_jobspec1_attr_unpack (flux_jobspec1_t *jobspec,
-                               const char *path,
-                               const char *fmt,
-                               ...);
 
 
+int flux_subprocess_write (flux_subprocess_t *p, const char *stream,
+                           const char *buf, size_t len);
 
 
 
 
 
-int flux_jobspec1_attr_check (flux_jobspec1_t *jobspec,
-                              flux_jobspec1_error_t *error);
+
+int flux_subprocess_close (flux_subprocess_t *p, const char *stream);
+# 3757 "/workspaces/flux-python/src/_core_clean.h"
+const char *flux_subprocess_read (flux_subprocess_t *p,
+                                  const char *stream,
+                                  int len, int *lenp);
+# 3772 "/workspaces/flux-python/src/_core_clean.h"
+const char *flux_subprocess_read_line (flux_subprocess_t *p,
+                                       const char *stream,
+                                       int *lenp);
 
 
 
 
+const char *flux_subprocess_read_trimmed_line (flux_subprocess_t *p,
+                                               const char *stream,
+                                               int *lenp);
+# 3792 "/workspaces/flux-python/src/_core_clean.h"
+int flux_subprocess_read_stream_closed (flux_subprocess_t *p,
+                                        const char *stream);
+# 3811 "/workspaces/flux-python/src/_core_clean.h"
+const char *flux_subprocess_getline (flux_subprocess_t *p,
+                                     const char *stream,
+                                     int *lenp);
 
 
-int flux_jobspec1_check (flux_jobspec1_t *jobspec,
-                         flux_jobspec1_error_t *error);
 
 
 
 
 
-int flux_jobspec1_unsetenv (flux_jobspec1_t *jobspec, const char *name);
+flux_future_t *flux_subprocess_kill (flux_subprocess_t *p, int signo);
 
 
 
 
 
 
+void flux_subprocess_ref (flux_subprocess_t *p);
+void flux_subprocess_unref (flux_subprocess_t *p);
+# 3838 "/workspaces/flux-python/src/_core_clean.h"
+flux_subprocess_state_t flux_subprocess_state (flux_subprocess_t *p);
 
-int flux_jobspec1_setenv (flux_jobspec1_t *jobspec,
-                           const char *name,
-                           const char *value,
-                           int overwrite);
 
 
+const char *flux_subprocess_state_string (flux_subprocess_state_t state);
+
+int flux_subprocess_rank (flux_subprocess_t *p);
 
 
-int flux_jobspec1_set_stdin (flux_jobspec1_t *jobspec, const char *path);
 
+int flux_subprocess_fail_errno (flux_subprocess_t *p);
 
 
 
-int flux_jobspec1_set_stdout (flux_jobspec1_t *jobspec, const char *path);
+int flux_subprocess_status (flux_subprocess_t *p);
 
 
 
+int flux_subprocess_exit_code (flux_subprocess_t *p);
 
-int flux_jobspec1_set_stderr (flux_jobspec1_t *jobspec, const char *path);
 
 
+int flux_subprocess_signaled (flux_subprocess_t *p);
 
+pid_t flux_subprocess_pid (flux_subprocess_t *p);
 
-int flux_jobspec1_set_cwd (flux_jobspec1_t *jobspec, const char *cwd);
 
 
+flux_cmd_t *flux_subprocess_get_cmd (flux_subprocess_t *p);
 
 
 
-char *flux_jobspec1_encode (flux_jobspec1_t *jobspec, size_t flags);
+flux_reactor_t * flux_subprocess_get_reactor (flux_subprocess_t *p);
 
 
 
 
 
 
-flux_jobspec1_t *flux_jobspec1_decode (const char *s,
-                                       flux_jobspec1_error_t *error);
-# 3892 "/workspaces/flux-python/src/_core_clean.h"
-flux_jobspec1_t *flux_jobspec1_from_command (int argc,
-                                             char **argv,
-                                             char **env,
-                                             int ntasks,
-                                             int cores_per_task,
-                                             int gpus_per_task,
-                                             int nnodes,
-                                             double duration);
+int flux_subprocess_aux_set (flux_subprocess_t *p,
+                             const char *name, void *ctx, flux_free_f free);
 
 
-void flux_jobspec1_destroy (flux_jobspec1_t *jobspec);
-# 3912 "/workspaces/flux-python/src/_core_clean.h"
+
+
+
+void *flux_subprocess_aux_get (flux_subprocess_t *p, const char *name);
+# 3899 "/workspaces/flux-python/src/_core_clean.h"
 extern "Python" void message_handler_wrapper(flux_t *, flux_msg_handler_t *, const flux_msg_t *, void *);
 
 
 extern "Python" void timeout_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void fd_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void signal_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 
 
 extern "Python" void continuation_callback(flux_future_t *, void *);
-# 3938 "/workspaces/flux-python/src/_core_clean.h"
-extern int MPIR_being_debugged;
-extern void MPIR_Breakpoint (void);
-extern int get_mpir_being_debugged (void);
-extern void set_mpir_being_debugged (int v);
```

### Comparing `flux-python-0.48.0rc0/src/_hostlist_clean.h` & `flux-python-0.50.0rc0/src/_hostlist_clean.h`

 * *Files 17% similar despite different names*

```diff
@@ -4,27 +4,14 @@
  *
  * This file is part of the Flux resource manager framework.
  * For details, see https://github.com/flux-framework.
  *
  * SPDX-License-Identifier: LGPL-3.0
 \************************************************************/
 
-/* Allow in-tree programs to #include <flux/hostlist.h> like out-of-tree would.
- */
-
-/************************************************************\
- * Copyright 2020 Lawrence Livermore National Security, LLC
- * (c.f. AUTHORS, NOTICE.LLNS, COPYING)
- *
- * This file is part of the Flux resource manager framework.
- * For details, see https://github.com/flux-framework.
- *
- * SPDX-License-Identifier: LGPL-3.0
-\************************************************************/
-
 /* Functions for encoding/decoding and manipulating RFC 29 Hostlists */
 
 #ifndef FLUX_HOSTLIST_H
 #define FLUX_HOSTLIST_H
 
 #ifdef __cplusplus
 extern "C" {
```

### Comparing `flux-python-0.48.0rc0/src/_hostlist_preproc.h` & `flux-python-0.50.0rc0/src/_hostlist_preproc.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # 1 "/workspaces/flux-python/src/_hostlist_clean.h"
 # 1 "<built-in>"
 # 1 "<command-line>"
 # 1 "/usr/include/stdc-predef.h" 1 3 4
 # 1 "<command-line>" 2
 # 1 "/workspaces/flux-python/src/_hostlist_clean.h"
-# 33 "/workspaces/flux-python/src/_hostlist_clean.h"
+# 20 "/workspaces/flux-python/src/_hostlist_clean.h"
 struct hostlist *hostlist_create (void);
 
 void hostlist_destroy (struct hostlist *hl);
 
 
 
 
@@ -40,15 +40,15 @@
 int hostlist_append_list (struct hostlist *hl1, struct hostlist *hl2);
 
 
 
 
 
 const char * hostlist_nth (struct hostlist * hl, int n);
-# 81 "/workspaces/flux-python/src/_hostlist_clean.h"
+# 68 "/workspaces/flux-python/src/_hostlist_clean.h"
 int hostlist_find (struct hostlist * hl, const char *hostname);
 
 
 
 
 
 
@@ -67,21 +67,21 @@
 
 void hostlist_sort (struct hostlist * hl);
 
 
 
 
 void hostlist_uniq (struct hostlist *hl);
-# 116 "/workspaces/flux-python/src/_hostlist_clean.h"
+# 103 "/workspaces/flux-python/src/_hostlist_clean.h"
 const char * hostlist_first (struct hostlist *hl);
-# 126 "/workspaces/flux-python/src/_hostlist_clean.h"
+# 113 "/workspaces/flux-python/src/_hostlist_clean.h"
 const char * hostlist_last (struct hostlist *hl);
-# 136 "/workspaces/flux-python/src/_hostlist_clean.h"
+# 123 "/workspaces/flux-python/src/_hostlist_clean.h"
 const char * hostlist_next (struct hostlist *hl);
-# 145 "/workspaces/flux-python/src/_hostlist_clean.h"
+# 132 "/workspaces/flux-python/src/_hostlist_clean.h"
 const char * hostlist_current (struct hostlist *hl);
 
 
 
 
 
 int hostlist_remove_current (struct hostlist *hl);
```

### Comparing `flux-python-0.48.0rc0/src/_idset_clean.h` & `flux-python-0.50.0rc0/src/_idset_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/src/_idset_preproc.h` & `flux-python-0.50.0rc0/src/_idset_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/src/_rlist_clean.h` & `flux-python-0.50.0rc0/src/_rlist_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/src/_rlist_preproc.h` & `flux-python-0.50.0rc0/src/_rlist_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/src/_security_clean.h` & `flux-python-0.50.0rc0/src/_security_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/src/_security_preproc.h` & `flux-python-0.50.0rc0/src/_security_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/src/callbacks.h` & `flux-python-0.50.0rc0/src/callbacks.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc0/src/make_clean_header.py` & `flux-python-0.50.0rc0/src/make_clean_header.py`

 * *Files identical despite different names*

