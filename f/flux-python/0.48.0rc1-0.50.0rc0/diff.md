# Comparing `tmp/flux-python-0.48.0rc1.tar.gz` & `tmp/flux-python-0.50.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-python-0.48.0rc1.tar", last modified: Wed May  3 05:27:58 2023, max compression
+gzip compressed data, was "flux-python-0.50.0rc0.tar", last modified: Wed May  3 05:14:03 2023, max compression
```

## Comparing `flux-python-0.48.0rc1.tar` & `flux-python-0.50.0rc0.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.163875 flux-python-0.48.0rc1/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      186 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6827 2023-05-03 05:27:58.163875 flux-python-0.48.0rc1/PKG-INFO
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4933 2023-05-03 05:27:34.000000 flux-python-0.48.0rc1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.147875 flux-python-0.48.0rc1/flux/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       52 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/.gitignore
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26956 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)    26465 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/Makefile.in
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      668 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.147875 flux-python-0.48.0rc1/flux/cli/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    27800 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/cli/_fortune.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      754 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/constants.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.147875 flux-python-0.48.0rc1/flux/constraint/
--rw-r--r--   0 vscode    (1000) vscode    (1000)    17451 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/constraint/parser.out
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2862 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/constraint/parsetab.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.147875 flux-python-0.48.0rc1/flux/core/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/core/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12153 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/core/handle.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      815 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/core/inner.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1309 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/core/trampoline.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5167 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/core/watchers.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      567 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/debugged.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7721 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/future.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6219 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/hostlist.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    10040 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/idset.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1674 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/importer.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.151875 flux-python-0.48.0rc1/flux/job/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3059 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/JobID.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    35872 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/Jobspec.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1189 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      597 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/_wrapper.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7170 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/event.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    26007 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/executor.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.151875 flux-python-0.48.0rc1/flux/job/frobnicator/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      460 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/frobnicator/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4929 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/frobnicator/frobnicator.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.151875 flux-python-0.48.0rc1/flux/job/frobnicator/plugins/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1938 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/frobnicator/plugins/constraints.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3088 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/frobnicator/plugins/defaults.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21558 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/info.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2449 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/kill.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1104 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/kvs.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    10098 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/list.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3580 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/stats.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4598 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/submit.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.151875 flux-python-0.48.0rc1/flux/job/validator/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      452 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/validator/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.151875 flux-python-0.48.0rc1/flux/job/validator/plugins/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1710 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/validator/plugins/feasibility.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/validator/plugins/jobspec.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1427 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/validator/plugins/require-instance.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1408 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/validator/plugins/schema.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7594 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/validator/validator.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6988 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/job/wait.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     9456 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/kvs.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2629 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/memoized_property.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     5394 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/message.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    11771 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/progress.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.155875 flux-python-0.48.0rc1/flux/resource/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     7954 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/resource/ResourceSet.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2767 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/resource/ResourceSetImplementation.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4408 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/resource/Rlist.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      533 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/resource/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2663 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/resource/list.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2474 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/rpc.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3691 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/security.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.155875 flux-python-0.48.0rc1/flux/uri/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      470 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/uri/__init__.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.155875 flux-python-0.48.0rc1/flux/uri/resolvers/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2490 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/uri/resolvers/jobid.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3468 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/uri/resolvers/lsf.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3916 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/uri/resolvers/pid.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3357 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/uri/resolvers/slurm.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6461 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/uri/uri.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    36871 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/util.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.155875 flux-python-0.48.0rc1/flux/utils/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      201 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.155875 flux-python-0.48.0rc1/flux/utils/parsedatetime/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)   105234 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4652 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/context.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       61 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/parsedatetime.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.159875 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      719 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4611 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/base.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     3130 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/de_DE.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      380 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/en_AU.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      157 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/en_US.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      959 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/es.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     6090 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/fr_FR.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4566 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/icu.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2998 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/nl_NL.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1128 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/pt_BR.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4577 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/ru_RU.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      485 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/parsedatetime/warns.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.159875 flux-python-0.48.0rc1/flux/utils/tomli/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1072 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/tomli/LICENSE
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      294 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/tomli/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21649 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/tomli/_parser.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2813 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/tomli/_re.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      126 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/tomli/_types.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)       26 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/utils/tomli/py.typed
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12713 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/flux/wrapper.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.159875 flux-python-0.48.0rc1/flux_python.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     6827 2023-05-03 05:27:58.000000 flux-python-0.48.0rc1/flux_python.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2825 2023-05-03 05:27:58.000000 flux-python-0.48.0rc1/flux_python.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-03 05:27:58.000000 flux-python-0.48.0rc1/flux_python.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-02 13:16:43.000000 flux-python-0.48.0rc1/flux_python.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       58 2023-05-03 05:27:58.000000 flux-python-0.48.0rc1/flux_python.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       15 2023-05-03 05:27:58.000000 flux-python-0.48.0rc1/flux_python.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-03 05:27:58.163875 flux-python-0.48.0rc1/setup.cfg
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    12040 2023-05-03 05:25:31.000000 flux-python-0.48.0rc1/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-03 05:27:58.163875 flux-python-0.48.0rc1/src/
--rw-rw-r--   0 vscode    (1000) vscode    (1000)        0 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/src/__init__.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1637 2023-05-03 05:01:59.000000 flux-python-0.48.0rc1/src/_core_build.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)   133689 2023-05-03 05:27:50.000000 flux-python-0.48.0rc1/src/_core_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)    54290 2023-05-03 05:27:50.000000 flux-python-0.48.0rc1/src/_core_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      876 2023-05-03 05:10:48.000000 flux-python-0.48.0rc1/src/_hostlist_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4268 2023-05-03 05:27:50.000000 flux-python-0.48.0rc1/src/_hostlist_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1524 2023-05-03 05:27:50.000000 flux-python-0.48.0rc1/src/_hostlist_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      961 2023-05-03 05:10:41.000000 flux-python-0.48.0rc1/src/_idset_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4483 2023-05-03 05:27:50.000000 flux-python-0.48.0rc1/src/_idset_clean.h
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1876 2023-05-03 05:27:50.000000 flux-python-0.48.0rc1/src/_idset_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1755 2023-05-03 05:13:26.000000 flux-python-0.48.0rc1/src/_rlist_build.py
--rw-rw-r--   0 vscode    (1000) vscode    (1000)    21443 2023-05-03 00:05:27.000000 flux-python-0.48.0rc1/src/_rlist_clean.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     4552 2023-05-03 00:05:27.000000 flux-python-0.48.0rc1/src/_rlist_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     1218 2023-05-03 05:13:39.000000 flux-python-0.48.0rc1/src/_security_build.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     5186 2023-05-03 05:27:50.000000 flux-python-0.48.0rc1/src/_security_clean.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)     2048 2023-05-03 05:27:50.000000 flux-python-0.48.0rc1/src/_security_preproc.h
--rw-rw-r--   0 vscode    (1000) vscode    (1000)      516 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/src/callbacks.h
--rwxrwxr-x   0 vscode    (1000) vscode    (1000)     2804 2023-05-02 05:33:04.000000 flux-python-0.48.0rc1/src/make_clean_header.py
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

### Comparing `flux-python-0.48.0rc1/PKG-INFO` & `flux-python-0.50.0rc0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-python
-Version: 0.48.0rc1
+Version: 0.50.0rc0
 Summary: Python bindings for the flux resource manager API
 Home-page: https://github.com/flux-framework/flux-python
 License: UNKNOWN
 Description: # Flux Python Bindings
         
         > 🐍️ You called me?
         
@@ -26,30 +26,30 @@
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
         sudo make install
         ```
         
         And then build your custom wheel:
         
         ```bash
         $ cd /workspaces/flux-python
-        $ python3 setup.py sdist bdist_wheel
+        $ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version ${FLUX_VERSION}-rc-0
         ```
         
         And if you want to upload:
         
         ```bash
         $ twine upload dist/*.tar.gz
         ```
```

### Comparing `flux-python-0.48.0rc1/README.md` & `flux-python-0.50.0rc0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,30 +20,30 @@
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
 sudo make install
 ```
 
 And then build your custom wheel:
 
 ```bash
 $ cd /workspaces/flux-python
-$ python3 setup.py sdist bdist_wheel
+$ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version ${FLUX_VERSION}-rc-0
 ```
 
 And if you want to upload:
 
 ```bash
 $ twine upload dist/*.tar.gz
 ```
```

### Comparing `flux-python-0.48.0rc1/flux/Makefile` & `flux-python-0.50.0rc0/flux/Makefile`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/Makefile.in` & `flux-python-0.50.0rc0/flux/Makefile.in`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/__init__.py` & `flux-python-0.50.0rc0/flux/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/cli/_fortune.py` & `flux-python-0.50.0rc0/flux/cli/_fortune.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/constants.py` & `flux-python-0.50.0rc0/flux/constants.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/constraint/parser.out` & `flux-python-0.50.0rc0/flux/constraint/parser.out`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/constraint/parsetab.py` & `flux-python-0.50.0rc0/flux/constraint/parsetab.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/core/handle.py` & `flux-python-0.50.0rc0/flux/core/handle.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/core/inner.py` & `flux-python-0.50.0rc0/flux/core/inner.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/core/trampoline.py` & `flux-python-0.50.0rc0/flux/core/trampoline.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/core/watchers.py` & `flux-python-0.50.0rc0/flux/core/watchers.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/debugged.py` & `flux-python-0.50.0rc0/flux/debugged.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/future.py` & `flux-python-0.50.0rc0/flux/future.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/hostlist.py` & `flux-python-0.50.0rc0/flux/hostlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/idset.py` & `flux-python-0.50.0rc0/flux/idset.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/importer.py` & `flux-python-0.50.0rc0/flux/importer.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/JobID.py` & `flux-python-0.50.0rc0/flux/job/JobID.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/Jobspec.py` & `flux-python-0.50.0rc0/flux/job/Jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/__init__.py` & `flux-python-0.50.0rc0/flux/job/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/_wrapper.py` & `flux-python-0.50.0rc0/flux/job/_wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/event.py` & `flux-python-0.50.0rc0/flux/job/event.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/executor.py` & `flux-python-0.50.0rc0/flux/job/executor.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/frobnicator/frobnicator.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/frobnicator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/frobnicator/plugins/constraints.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/plugins/constraints.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/frobnicator/plugins/defaults.py` & `flux-python-0.50.0rc0/flux/job/frobnicator/plugins/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/info.py` & `flux-python-0.50.0rc0/flux/job/info.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/kill.py` & `flux-python-0.50.0rc0/flux/job/kill.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/kvs.py` & `flux-python-0.50.0rc0/flux/job/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/list.py` & `flux-python-0.50.0rc0/flux/job/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/stats.py` & `flux-python-0.50.0rc0/flux/job/stats.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/submit.py` & `flux-python-0.50.0rc0/flux/job/submit.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/validator/plugins/feasibility.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/feasibility.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/validator/plugins/jobspec.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/jobspec.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/validator/plugins/require-instance.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/require-instance.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/validator/plugins/schema.py` & `flux-python-0.50.0rc0/flux/job/validator/plugins/schema.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/validator/validator.py` & `flux-python-0.50.0rc0/flux/job/validator/validator.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/job/wait.py` & `flux-python-0.50.0rc0/flux/job/wait.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/kvs.py` & `flux-python-0.50.0rc0/flux/kvs.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/memoized_property.py` & `flux-python-0.50.0rc0/flux/memoized_property.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/message.py` & `flux-python-0.50.0rc0/flux/message.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/progress.py` & `flux-python-0.50.0rc0/flux/progress.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/resource/ResourceSet.py` & `flux-python-0.50.0rc0/flux/resource/ResourceSet.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/resource/ResourceSetImplementation.py` & `flux-python-0.50.0rc0/flux/resource/ResourceSetImplementation.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/resource/Rlist.py` & `flux-python-0.50.0rc0/flux/resource/Rlist.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/resource/__init__.py` & `flux-python-0.50.0rc0/flux/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/resource/list.py` & `flux-python-0.50.0rc0/flux/resource/list.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/rpc.py` & `flux-python-0.50.0rc0/flux/rpc.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/security.py` & `flux-python-0.50.0rc0/flux/security.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/uri/resolvers/jobid.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/jobid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/uri/resolvers/lsf.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/lsf.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/uri/resolvers/pid.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/pid.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/uri/resolvers/slurm.py` & `flux-python-0.50.0rc0/flux/uri/resolvers/slurm.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/uri/uri.py` & `flux-python-0.50.0rc0/flux/uri/uri.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/util.py` & `flux-python-0.50.0rc0/flux/util.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/__init__.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/context.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/context.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/__init__.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/base.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/base.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/de_DE.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/de_DE.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/es.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/es.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/fr_FR.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/fr_FR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/icu.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/icu.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/nl_NL.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/nl_NL.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/pt_BR.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/pt_BR.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/parsedatetime/pdt_locales/ru_RU.py` & `flux-python-0.50.0rc0/flux/utils/parsedatetime/pdt_locales/ru_RU.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/tomli/LICENSE` & `flux-python-0.50.0rc0/flux/utils/tomli/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/tomli/_parser.py` & `flux-python-0.50.0rc0/flux/utils/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/utils/tomli/_re.py` & `flux-python-0.50.0rc0/flux/utils/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux/wrapper.py` & `flux-python-0.50.0rc0/flux/wrapper.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/flux_python.egg-info/PKG-INFO` & `flux-python-0.50.0rc0/flux_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-python
-Version: 0.48.0rc1
+Version: 0.50.0rc0
 Summary: Python bindings for the flux resource manager API
 Home-page: https://github.com/flux-framework/flux-python
 License: UNKNOWN
 Description: # Flux Python Bindings
         
         > 🐍️ You called me?
         
@@ -26,30 +26,30 @@
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
         sudo make install
         ```
         
         And then build your custom wheel:
         
         ```bash
         $ cd /workspaces/flux-python
-        $ python3 setup.py sdist bdist_wheel
+        $ python3 setup.py sdist bdist_wheel --flux-root /home/vscode/flux-core --security-src /home/vscode/security --security-include /usr/local/include/flux/security --version ${FLUX_VERSION}-rc-0
         ```
         
         And if you want to upload:
         
         ```bash
         $ twine upload dist/*.tar.gz
         ```
```

### Comparing `flux-python-0.48.0rc1/flux_python.egg-info/SOURCES.txt` & `flux-python-0.50.0rc0/flux_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/setup.py` & `flux-python-0.50.0rc0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 from setuptools import find_packages
 from setuptools import setup as _setup
 from distutils.core import setup, Command
 
 # Metadata
 package_name = "flux-python"
-package_version = "0.48.0-rc1"
+package_version = "0.50.0-rc0"
 package_description = "Python bindings for the flux resource manager API"
 package_url = "https://github.com/flux-framework/flux-python"
 package_keywords = "flux, job manager, orchestration, hpc"
 
 try:
     with open("README.md") as filey:
         package_long_description = filey.read()
```

### Comparing `flux-python-0.48.0rc1/src/_core_build.py` & `flux-python-0.50.0rc0/src/_core_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_core_clean.h` & `flux-python-0.50.0rc0/src/_core_clean.h`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,20 @@
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
@@ -524,15 +530,15 @@
 
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
@@ -598,15 +604,15 @@
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
@@ -1036,14 +1042,20 @@
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
@@ -1795,18 +1807,14 @@
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
@@ -1819,30 +1827,14 @@
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
 
@@ -1881,15 +1873,15 @@
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
@@ -3073,15 +3065,15 @@
     FLUX_JOB_RESULT_FAILED = 2,
     FLUX_JOB_RESULT_CANCELED = 4,
     FLUX_JOB_RESULT_TIMEOUT = 8,
 } flux_job_result_t;
 
 typedef uint64_t flux_jobid_t;
 
-/*  Parse a jobid from NULL-teminated string 's' in any supported encoding.
+/*  Parse a jobid from NULL-terminated string 's' in any supported encoding.
  *  Returns 0 on success, -1 on failure.
  */
 int flux_job_id_parse (const char *s, flux_jobid_t *id);
 
 /*  Encode a jobid into encoding "type", writing the result to buffer
  *   buf of size bufsz.
  *  Supported encoding types include:
@@ -3133,44 +3125,24 @@
  */
 flux_future_t *flux_job_wait (flux_t *h, flux_jobid_t id);
 int flux_job_wait_get_status (flux_future_t *f,
                               bool *success,
                               const char **errstr);
 int flux_job_wait_get_id (flux_future_t *f, flux_jobid_t *id);
 
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
 
 /* Similar to flux_job_list(), but retrieve job info for a single
  * job id */
 flux_future_t *flux_job_list_id (flux_t *h,
                                  flux_jobid_t id,
                                  const char *attrs_json_str);
 
@@ -3260,15 +3232,15 @@
  *  a flux instance, but is not part of a parallel job).
  *
  *  Returns 0 on success with timeleft assigned to the remaining time.
  *  If there is no expiration in the current context (e.g. the job has
  *  no timelimit), then timeleft is set to infinity. If the job is not
  *  in RUN state, or the job has expired, then timeleft is set to 0.
  *
- *  Returns -1 with error string assinged to 'errp' on failure.
+ *  Returns -1 with error string assigned to 'errp' on failure.
  */
 int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
 
 #ifdef __cplusplus
 }
 #endif
 
@@ -3522,14 +3494,27 @@
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
@@ -3593,15 +3578,15 @@
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
 
@@ -3685,42 +3670,55 @@
 
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
@@ -3881,30 +3879,14 @@
 
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
```

### Comparing `flux-python-0.48.0rc1/src/_core_preproc.h` & `flux-python-0.50.0rc0/src/_core_preproc.h`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 
 
 typedef struct {
     char text[160];
 } flux_error_t;
-# 98 "/workspaces/flux-python/src/_core_clean.h"
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
-# 172 "/workspaces/flux-python/src/_core_clean.h"
+# 178 "/workspaces/flux-python/src/_core_clean.h"
 flux_msg_t *flux_msg_create (int type);
 void flux_msg_destroy (flux_msg_t *msg);
 
 
 
 
 int flux_msg_aux_set (const flux_msg_t *msg, const char *name,
@@ -165,15 +165,15 @@
 
 
 int flux_msg_pack (flux_msg_t *msg, const char *fmt, ...);
 int flux_msg_vpack (flux_msg_t *msg, const char *fmt, va_list ap);
 
 int flux_msg_unpack (const flux_msg_t *msg, const char *fmt, ...);
 int flux_msg_vunpack (const flux_msg_t *msg, const char *fmt, va_list ap);
-# 288 "/workspaces/flux-python/src/_core_clean.h"
+# 294 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_msg_last_error (const flux_msg_t *msg);
 
 
 
 int flux_msg_set_nodeid (flux_msg_t *msg, uint32_t nodeid);
 int flux_msg_get_nodeid (const flux_msg_t *msg, uint32_t *nodeid);
 
@@ -251,15 +251,15 @@
 void flux_msg_fprint (FILE *f, const flux_msg_t *msg);
 void flux_msg_fprint_ts (FILE *f, const flux_msg_t *msg, double timestamp);
 
 
 
 
 const char *flux_msg_typestr (int type);
-# 383 "/workspaces/flux-python/src/_core_clean.h"
+# 389 "/workspaces/flux-python/src/_core_clean.h"
 void flux_msg_route_enable (flux_msg_t *msg);
 
 
 
 
 
 void flux_msg_route_disable (flux_msg_t *msg);
@@ -310,15 +310,15 @@
 char *flux_msg_route_string (const flux_msg_t *msg);
 
 
 
 
 bool flux_msg_route_match_first (const flux_msg_t *msg1,
                                  const flux_msg_t *msg2);
-# 457 "/workspaces/flux-python/src/_core_clean.h"
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
-# 510 "/workspaces/flux-python/src/_core_clean.h"
+# 516 "/workspaces/flux-python/src/_core_clean.h"
 flux_t *flux_open (const char *uri, int flags);
 
 
 
 
 
 flux_t *flux_open_ex (const char *uri, int flags, flux_error_t *error);
@@ -387,15 +387,15 @@
 int flux_opt_set (flux_t *h, const char *option, const void *val, size_t len);
 int flux_opt_get (flux_t *h, const char *option, void *val, size_t len);
 
 
 
 
 void flux_comms_error_set (flux_t *h, flux_comms_error_f fun, void *arg);
-# 554 "/workspaces/flux-python/src/_core_clean.h"
+# 560 "/workspaces/flux-python/src/_core_clean.h"
 void *flux_aux_get (flux_t *h, const char *name);
 int flux_aux_set (flux_t *h, const char *name, void *aux, flux_free_f destroy);
 
 
 
 void flux_flags_set (flux_t *h, int flags);
 void flux_flags_unset (flux_t *h, int flags);
@@ -409,37 +409,37 @@
 uint32_t flux_matchtag_avail (flux_t *h);
 
 
 
 
 
 int flux_send (flux_t *h, const flux_msg_t *msg, int flags);
-# 583 "/workspaces/flux-python/src/_core_clean.h"
+# 589 "/workspaces/flux-python/src/_core_clean.h"
 flux_msg_t *flux_recv (flux_t *h, struct flux_match match, int flags);
 
 
 
 
 
 
 int flux_requeue (flux_t *h, const flux_msg_t *msg, int flags);
 
 
 
 
 
 int flux_pollevents (flux_t *h);
-# 607 "/workspaces/flux-python/src/_core_clean.h"
+# 613 "/workspaces/flux-python/src/_core_clean.h"
 int flux_pollfd (flux_t *h);
 
 
 
 void flux_get_msgcounters (flux_t *h, flux_msgcounters_t *mcs);
 void flux_clr_msgcounters (flux_t *h);
-# 655 "/workspaces/flux-python/src/_core_clean.h"
+# 661 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_buffer flux_buffer_t;
 
 
 
 flux_buffer_t *flux_buffer_create (int size);
 
 void flux_buffer_destroy (void *fb);
@@ -448,25 +448,25 @@
 int flux_buffer_size (flux_buffer_t *fb);
 
 
 int flux_buffer_bytes (flux_buffer_t *fb);
 
 
 int flux_buffer_space (flux_buffer_t *fb);
-# 681 "/workspaces/flux-python/src/_core_clean.h"
+# 687 "/workspaces/flux-python/src/_core_clean.h"
 int flux_buffer_readonly (flux_buffer_t *fb);
 bool flux_buffer_is_readonly (flux_buffer_t *fb);
 
 
 
 
 int flux_buffer_drop (flux_buffer_t *fb, int len);
-# 696 "/workspaces/flux-python/src/_core_clean.h"
+# 702 "/workspaces/flux-python/src/_core_clean.h"
 const void *flux_buffer_peek (flux_buffer_t *fb, int len, int *lenp);
-# 706 "/workspaces/flux-python/src/_core_clean.h"
+# 712 "/workspaces/flux-python/src/_core_clean.h"
 const void *flux_buffer_read (flux_buffer_t *fb, int len, int *lenp);
 
 
 
 
 int flux_buffer_write (flux_buffer_t *fb, const void *data, int len);
 
@@ -519,15 +519,15 @@
 int flux_buffer_read_to_fd (flux_buffer_t *fb, int fd, int len);
 
 
 
 
 
 int flux_buffer_write_from_fd (flux_buffer_t *fb, int fd, int len);
-# 782 "/workspaces/flux-python/src/_core_clean.h"
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
-# 888 "/workspaces/flux-python/src/_core_clean.h"
+# 894 "/workspaces/flux-python/src/_core_clean.h"
 int flux_buffer_write_watcher_close (flux_watcher_t *w);
 
 
 int flux_buffer_write_watcher_is_closed (flux_watcher_t *w, int *close_err);
 
 
 
@@ -694,27 +694,27 @@
 
 
 struct flux_watcher_ops {
     void (*start) (flux_watcher_t *w);
     void (*stop) (flux_watcher_t *w);
     void (*destroy) (flux_watcher_t *w);
 };
-# 973 "/workspaces/flux-python/src/_core_clean.h"
+# 979 "/workspaces/flux-python/src/_core_clean.h"
 flux_watcher_t * flux_watcher_create (flux_reactor_t *r, size_t data_size,
                                       struct flux_watcher_ops *ops,
                                       flux_watcher_f fn, void *arg);
 
 
 
 void * flux_watcher_get_data (flux_watcher_t *w);
 
 
 
 struct flux_watcher_ops * flux_watcher_get_ops (flux_watcher_t *w);
-# 1012 "/workspaces/flux-python/src/_core_clean.h"
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
-# 1083 "/workspaces/flux-python/src/_core_clean.h"
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
-# 1134 "/workspaces/flux-python/src/_core_clean.h"
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
-# 1155 "/workspaces/flux-python/src/_core_clean.h"
+# 1167 "/workspaces/flux-python/src/_core_clean.h"
 int flux_msglist_pollevents (struct flux_msglist *l);
 int flux_msglist_pollfd (struct flux_msglist *l);
-# 1191 "/workspaces/flux-python/src/_core_clean.h"
+# 1203 "/workspaces/flux-python/src/_core_clean.h"
 int flux_request_decode (const flux_msg_t *msg, const char **topic,
                          const char **s);
 
 
 
 
 
@@ -816,18 +822,18 @@
 
 
 
 
 
 flux_msg_t *flux_request_encode_raw (const char *topic,
                                      const void *data, int len);
-# 1257 "/workspaces/flux-python/src/_core_clean.h"
+# 1269 "/workspaces/flux-python/src/_core_clean.h"
 int flux_response_decode (const flux_msg_t *msg, const char **topic,
                           const char **s);
-# 1268 "/workspaces/flux-python/src/_core_clean.h"
+# 1280 "/workspaces/flux-python/src/_core_clean.h"
 int flux_response_decode_raw (const flux_msg_t *msg, const char **topic,
                               const void **data, int *len);
 
 
 
 
 
@@ -874,19 +880,19 @@
 
 
 
 
 
 int flux_respond_error (flux_t *h, const flux_msg_t *request,
                         int errnum, const char *errstr);
-# 1350 "/workspaces/flux-python/src/_core_clean.h"
+# 1362 "/workspaces/flux-python/src/_core_clean.h"
 flux_msg_t *flux_control_encode (int type, int status);
 
 int flux_control_decode (const flux_msg_t *msg, int *type, int *status);
-# 1411 "/workspaces/flux-python/src/_core_clean.h"
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
-# 1481 "/workspaces/flux-python/src/_core_clean.h"
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
-# 1559 "/workspaces/flux-python/src/_core_clean.h"
+# 1571 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_future_and_then (flux_future_t *f,
                                      flux_continuation_f cb, void *arg);
 
 
 
 
 flux_future_t *flux_future_or_then (flux_future_t *f,
@@ -1024,15 +1030,15 @@
                                  const char *errstr);
 
 
 
 int flux_future_fulfill_next (flux_future_t *prev,
                               void *result,
                               flux_free_f free_fn);
-# 1601 "/workspaces/flux-python/src/_core_clean.h"
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
-# 1670 "/workspaces/flux-python/src/_core_clean.h"
+# 1682 "/workspaces/flux-python/src/_core_clean.h"
 int flux_panic (flux_t *h, uint32_t nodeid, int flags, const char *reason);
-# 1699 "/workspaces/flux-python/src/_core_clean.h"
+# 1711 "/workspaces/flux-python/src/_core_clean.h"
 enum event_flags {
     FLUX_EVENT_PRIVATE = 1,
 };
 
 
 
 int flux_event_subscribe (flux_t *h, const char *topic);
@@ -1145,57 +1151,41 @@
                                        const char *topic, int flags,
                                        const void *data, int len);
 
 
 
 
 int flux_event_publish_get_seq (flux_future_t *f, int *seq);
-# 1814 "/workspaces/flux-python/src/_core_clean.h"
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
-# 1903 "/workspaces/flux-python/src/_core_clean.h"
+# 1895 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_attr_get (flux_t *h, const char *name);
 
 
 
 
 
 
@@ -1222,26 +1212,26 @@
 const char *flux_get_hostbyrank (flux_t *h, uint32_t rank);
 
 
 
 
 
 int flux_get_rankbyhost (flux_t *h, const char *host);
-# 1951 "/workspaces/flux-python/src/_core_clean.h"
+# 1943 "/workspaces/flux-python/src/_core_clean.h"
 char *flux_hostmap_lookup (flux_t *h,
                            const char *targets,
                            flux_error_t *errp);
 
 
 
 
 
 
 int flux_get_instance_starttime (flux_t *h, double *starttime);
-# 1989 "/workspaces/flux-python/src/_core_clean.h"
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
-# 2073 "/workspaces/flux-python/src/_core_clean.h"
+# 2065 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_barrier (flux_t *h, const char *name, int nprocs);
-# 2116 "/workspaces/flux-python/src/_core_clean.h"
+# 2108 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_service_register (flux_t *h, const char *name);
-# 2128 "/workspaces/flux-python/src/_core_clean.h"
+# 2120 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_service_unregister (flux_t *h, const char *name);
-# 2180 "/workspaces/flux-python/src/_core_clean.h"
+# 2172 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_core_version_string (void);
 
 
 
 
 
 
 int flux_core_version (int *major, int *minor, int *patch);
-# 2218 "/workspaces/flux-python/src/_core_clean.h"
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
-# 2305 "/workspaces/flux-python/src/_core_clean.h"
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
-# 2374 "/workspaces/flux-python/src/_core_clean.h"
+# 2366 "/workspaces/flux-python/src/_core_clean.h"
 int flux_plugin_call (flux_plugin_t *p, const char *name,
                       flux_plugin_arg_t *args);
-# 2384 "/workspaces/flux-python/src/_core_clean.h"
+# 2376 "/workspaces/flux-python/src/_core_clean.h"
 int flux_plugin_load_dso (flux_plugin_t *p, const char *path);
-# 2417 "/workspaces/flux-python/src/_core_clean.h"
+# 2409 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_sync_create (flux_t *h, double minimum);
-# 2449 "/workspaces/flux-python/src/_core_clean.h"
+# 2441 "/workspaces/flux-python/src/_core_clean.h"
 bool flux_disconnect_match (const flux_msg_t *msg1, const flux_msg_t *msg2);
 
 
 
 
 int flux_msglist_disconnect (struct flux_msglist *l, const flux_msg_t *msg);
 
@@ -1468,15 +1458,15 @@
 
 
 
 
 int flux_msglist_cancel (flux_t *h,
                          struct flux_msglist *l,
                          const flux_msg_t *msg);
-# 2518 "/workspaces/flux-python/src/_core_clean.h"
+# 2510 "/workspaces/flux-python/src/_core_clean.h"
 void flux_stats_count (flux_t *h, const char *name, ssize_t count);
 
 
 
 
 void flux_stats_gauge_set (flux_t *h, const char *name, ssize_t value);
 
@@ -1504,18 +1494,18 @@
 
 void flux_stats_set_prefix (flux_t *h, const char *fmt, ...);
 
 
 
 
 bool flux_stats_enabled (flux_t *h, const char *metric);
-# 2601 "/workspaces/flux-python/src/_core_clean.h"
+# 2593 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_kvsdir flux_kvsdir_t;
 typedef struct flux_kvsitr flux_kvsitr_t;
-# 2616 "/workspaces/flux-python/src/_core_clean.h"
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
-# 2689 "/workspaces/flux-python/src/_core_clean.h"
+# 2681 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_lookup (flux_t *h, const char *ns, int flags,
                                 const char *key);
 flux_future_t *flux_kvs_lookupat (flux_t *h, int flags, const char *key,
                                   const char *treeobj);
 
 int flux_kvs_lookup_get (flux_future_t *f, const char **value);
 int flux_kvs_lookup_get_unpack (flux_future_t *f, const char *fmt, ...);
@@ -1576,22 +1566,22 @@
 
 
 
 
 
 
 int flux_kvs_lookup_cancel (flux_future_t *f);
-# 2739 "/workspaces/flux-python/src/_core_clean.h"
+# 2731 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_getroot (flux_t *h, const char *ns, int flags);
-# 2748 "/workspaces/flux-python/src/_core_clean.h"
+# 2740 "/workspaces/flux-python/src/_core_clean.h"
 int flux_kvs_getroot_get_treeobj (flux_future_t *f, const char **treeobj);
 int flux_kvs_getroot_get_blobref (flux_future_t *f, const char **blobref);
 int flux_kvs_getroot_get_sequence (flux_future_t *f, int *seq);
 int flux_kvs_getroot_get_owner (flux_future_t *f, uint32_t *owner);
-# 2780 "/workspaces/flux-python/src/_core_clean.h"
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
-# 2858 "/workspaces/flux-python/src/_core_clean.h"
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
-# 2914 "/workspaces/flux-python/src/_core_clean.h"
+# 2906 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_copy (flux_t *h,
                               const char *srcns,
                               const char *srckey,
                               const char *dstns,
                               const char *dstkey,
                               int commit_flags);
-# 2931 "/workspaces/flux-python/src/_core_clean.h"
+# 2923 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_move (flux_t *h,
                               const char *srcns,
                               const char *srckey,
                               const char *dstns,
                               const char *dstkey,
                               int commit_flags);
-# 2954 "/workspaces/flux-python/src/_core_clean.h"
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
-# 2975 "/workspaces/flux-python/src/_core_clean.h"
+# 2967 "/workspaces/flux-python/src/_core_clean.h"
 flux_future_t *flux_kvs_namespace_create (flux_t *h, const char *ns,
                                           uint32_t owner, int flags);
 flux_future_t *flux_kvs_namespace_create_with (flux_t *h, const char *ns,
                                                const char *rootref,
                                                uint32_t owner, int flags);
 flux_future_t *flux_kvs_namespace_remove (flux_t *h, const char *ns);
 
@@ -1678,15 +1668,15 @@
 
 
 
 
 
 
 int flux_kvs_dropcache (flux_t *h);
-# 3023 "/workspaces/flux-python/src/_core_clean.h"
+# 3015 "/workspaces/flux-python/src/_core_clean.h"
 enum job_submit_flags {
     FLUX_JOB_PRE_SIGNED = 1,
     FLUX_JOB_DEBUG = 2,
     FLUX_JOB_WAITABLE = 4,
     FLUX_JOB_NOVALIDATE = 8,
 };
 
@@ -1740,18 +1730,18 @@
 
 typedef uint64_t flux_jobid_t;
 
 
 
 
 int flux_job_id_parse (const char *s, flux_jobid_t *id);
-# 3093 "/workspaces/flux-python/src/_core_clean.h"
+# 3085 "/workspaces/flux-python/src/_core_clean.h"
 int flux_job_id_encode (flux_jobid_t id, const char *type,
                         char *buf, size_t bufsz);
-# 3104 "/workspaces/flux-python/src/_core_clean.h"
+# 3096 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_job_statetostr (flux_job_state_t state, const char *fmt);
 
 
 
 
 int flux_job_strtostate (const char *s, flux_job_state_t *state);
 
@@ -1779,28 +1769,25 @@
 
 
 flux_future_t *flux_job_wait (flux_t *h, flux_jobid_t id);
 int flux_job_wait_get_status (flux_future_t *f,
                               bool *success,
                               const char **errstr);
 int flux_job_wait_get_id (flux_future_t *f, flux_jobid_t *id);
-# 3157 "/workspaces/flux-python/src/_core_clean.h"
-flux_future_t *flux_job_list (flux_t *h,
-                              int max_entries,
-                              const char *attrs_json_str,
-                              uint32_t userid,
-                              int states);
 
 
 
 
-flux_future_t *flux_job_list_inactive (flux_t *h,
-                                       int max_entries,
-                                       double since,
-                                       const char *attrs_json_str);
+
+                                                   ;
+
+
+
+
+                                                                     ;
 
 
 
 flux_future_t *flux_job_list_id (flux_t *h,
                                  flux_jobid_t id,
                                  const char *attrs_json_str);
 
@@ -1860,19 +1847,19 @@
 
 flux_future_t *flux_job_result (flux_t *h, flux_jobid_t id, int flags);
 
 
 
 int flux_job_result_get (flux_future_t *f,
                          const char **json_str);
-# 3255 "/workspaces/flux-python/src/_core_clean.h"
+# 3227 "/workspaces/flux-python/src/_core_clean.h"
 int flux_job_result_get_unpack (flux_future_t *f, const char *fmt, ...);
-# 3269 "/workspaces/flux-python/src/_core_clean.h"
+# 3241 "/workspaces/flux-python/src/_core_clean.h"
 int flux_job_timeleft (flux_t *h, flux_error_t *errp, double *timeleft);
-# 3294 "/workspaces/flux-python/src/_core_clean.h"
+# 3266 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_jobspec1 flux_jobspec1_t;
 typedef flux_error_t flux_jobspec1_error_t;
 
 
 
 
 
@@ -1962,37 +1949,37 @@
 
 
 
 
 
 flux_jobspec1_t *flux_jobspec1_decode (const char *s,
                                        flux_jobspec1_error_t *error);
-# 3405 "/workspaces/flux-python/src/_core_clean.h"
+# 3377 "/workspaces/flux-python/src/_core_clean.h"
 flux_jobspec1_t *flux_jobspec1_from_command (int argc,
                                              char **argv,
                                              char **env,
                                              int ntasks,
                                              int cores_per_task,
                                              int gpus_per_task,
                                              int nnodes,
                                              double duration);
 
 
 void flux_jobspec1_destroy (flux_jobspec1_t *jobspec);
-# 3447 "/workspaces/flux-python/src/_core_clean.h"
+# 3419 "/workspaces/flux-python/src/_core_clean.h"
 typedef struct flux_command flux_cmd_t;
 
 
 
 
 
 
 
 typedef struct flux_subprocess flux_subprocess_t;
-# 3467 "/workspaces/flux-python/src/_core_clean.h"
+# 3439 "/workspaces/flux-python/src/_core_clean.h"
 typedef enum {
     FLUX_SUBPROCESS_INIT,
     FLUX_SUBPROCESS_RUNNING,
     FLUX_SUBPROCESS_EXITED,
     FLUX_SUBPROCESS_FAILED,
     FLUX_SUBPROCESS_STOPPED,
 } flux_subprocess_state_t;
@@ -2045,17 +2032,29 @@
 
 typedef struct {
     flux_subprocess_hook_f pre_exec;
     void *pre_exec_arg;
     flux_subprocess_hook_f post_fork;
     void *post_fork_arg;
 } flux_subprocess_hooks_t;
-# 3538 "/workspaces/flux-python/src/_core_clean.h"
+
+
+
+
+typedef void (*subprocess_log_f) (void *arg,
+                                  const char *file,
+                                  int line,
+                                  const char *func,
+                                  const char *subsys,
+                                  int level,
+                                  const char *fmt,
+                                  va_list args);
+# 3523 "/workspaces/flux-python/src/_core_clean.h"
 void flux_standard_output (flux_subprocess_t *p, const char *stream);
-# 3547 "/workspaces/flux-python/src/_core_clean.h"
+# 3532 "/workspaces/flux-python/src/_core_clean.h"
 flux_cmd_t * flux_cmd_create (int argc, char *argv[], char **env);
 
 
 
 
 flux_cmd_t * flux_cmd_copy (const flux_cmd_t *cmd);
 
@@ -2101,15 +2100,15 @@
 char *flux_cmd_stringify (const flux_cmd_t *cmd);
 
 
 
 
 
 int flux_cmd_setenvf (flux_cmd_t *cmd, int overwrite,
-        const char *name, const char *fmt, ...)
+                      const char *name, const char *fmt, ...)
                       ;
 
 
 
 
 void flux_cmd_unsetenv (flux_cmd_t *cmd, const char *name);
 
@@ -2121,34 +2120,46 @@
 const char *flux_cmd_getenv (const flux_cmd_t *cmd, const char *name);
 
 
 
 
 int flux_cmd_setcwd (flux_cmd_t *cmd, const char *cwd);
 const char *flux_cmd_getcwd (const flux_cmd_t *cmd);
-# 3633 "/workspaces/flux-python/src/_core_clean.h"
+# 3618 "/workspaces/flux-python/src/_core_clean.h"
 int flux_cmd_add_channel (flux_cmd_t *cmd, const char *name);
-# 3683 "/workspaces/flux-python/src/_core_clean.h"
+# 3668 "/workspaces/flux-python/src/_core_clean.h"
 int flux_cmd_setopt (flux_cmd_t *cmd, const char *var, const char *val);
 const char *flux_cmd_getopt (flux_cmd_t *cmd, const char *var);
-# 3706 "/workspaces/flux-python/src/_core_clean.h"
-flux_subprocess_t *flux_exec (flux_t *h, int flags,
-                              const flux_cmd_t *cmd,
-                              const flux_subprocess_ops_t *ops,
-                              const flux_subprocess_hooks_t *hooks);
-
-flux_subprocess_t *flux_local_exec (flux_reactor_t *r, int flags,
+# 3691 "/workspaces/flux-python/src/_core_clean.h"
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
-# 3728 "/workspaces/flux-python/src/_core_clean.h"
+
+flux_subprocess_t *flux_rexec_ex (flux_t *h,
+                                  const char *service_name,
+                                  int rank,
+                                  int flags,
+                                  const flux_cmd_t *cmd,
+                                  const flux_subprocess_ops_t *ops,
+                                  subprocess_log_f log_fn,
+                                  void *log_data);
+# 3726 "/workspaces/flux-python/src/_core_clean.h"
 int flux_subprocess_stream_start (flux_subprocess_t *p, const char *stream);
 int flux_subprocess_stream_stop (flux_subprocess_t *p, const char *stream);
 int flux_subprocess_stream_status (flux_subprocess_t *p, const char *stream);
 
 
 
 
@@ -2160,33 +2171,33 @@
 
 
 
 
 
 
 int flux_subprocess_close (flux_subprocess_t *p, const char *stream);
-# 3759 "/workspaces/flux-python/src/_core_clean.h"
+# 3757 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_subprocess_read (flux_subprocess_t *p,
                                   const char *stream,
                                   int len, int *lenp);
-# 3774 "/workspaces/flux-python/src/_core_clean.h"
+# 3772 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_subprocess_read_line (flux_subprocess_t *p,
                                        const char *stream,
                                        int *lenp);
 
 
 
 
 const char *flux_subprocess_read_trimmed_line (flux_subprocess_t *p,
                                                const char *stream,
                                                int *lenp);
-# 3794 "/workspaces/flux-python/src/_core_clean.h"
+# 3792 "/workspaces/flux-python/src/_core_clean.h"
 int flux_subprocess_read_stream_closed (flux_subprocess_t *p,
                                         const char *stream);
-# 3813 "/workspaces/flux-python/src/_core_clean.h"
+# 3811 "/workspaces/flux-python/src/_core_clean.h"
 const char *flux_subprocess_getline (flux_subprocess_t *p,
                                      const char *stream,
                                      int *lenp);
 
 
 
 
@@ -2198,15 +2209,15 @@
 
 
 
 
 
 void flux_subprocess_ref (flux_subprocess_t *p);
 void flux_subprocess_unref (flux_subprocess_t *p);
-# 3840 "/workspaces/flux-python/src/_core_clean.h"
+# 3838 "/workspaces/flux-python/src/_core_clean.h"
 flux_subprocess_state_t flux_subprocess_state (flux_subprocess_t *p);
 
 
 
 const char *flux_subprocess_state_string (flux_subprocess_state_t state);
 
 int flux_subprocess_rank (flux_subprocess_t *p);
@@ -2246,30 +2257,15 @@
                              const char *name, void *ctx, flux_free_f free);
 
 
 
 
 
 void *flux_subprocess_aux_get (flux_subprocess_t *p, const char *name);
-
-typedef void (*subprocess_log_f) (void *arg,
-                                  const char *file,
-                                  int line,
-                                  const char *func,
-                                  const char *subsys,
-                                  int level,
-                                  const char *fmt,
-                                  va_list args);
-
-
-
-int flux_set_default_subprocess_log (flux_t *h,
-                                     subprocess_log_f log_fn,
-                                     void *log_data);
-# 3917 "/workspaces/flux-python/src/_core_clean.h"
+# 3899 "/workspaces/flux-python/src/_core_clean.h"
 extern "Python" void message_handler_wrapper(flux_t *, flux_msg_handler_t *, const flux_msg_t *, void *);
 
 
 extern "Python" void timeout_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void fd_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
 extern "Python" void signal_handler_wrapper(flux_reactor_t *, flux_watcher_t *, int, void *);
```

### Comparing `flux-python-0.48.0rc1/src/_hostlist_build.py` & `flux-python-0.50.0rc0/src/_hostlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_hostlist_clean.h` & `flux-python-0.50.0rc0/src/_hostlist_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_hostlist_preproc.h` & `flux-python-0.50.0rc0/src/_hostlist_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_idset_build.py` & `flux-python-0.50.0rc0/src/_idset_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_idset_clean.h` & `flux-python-0.50.0rc0/src/_idset_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_idset_preproc.h` & `flux-python-0.50.0rc0/src/_idset_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_rlist_build.py` & `flux-python-0.50.0rc0/src/_rlist_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_rlist_clean.h` & `flux-python-0.50.0rc0/src/_rlist_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_rlist_preproc.h` & `flux-python-0.50.0rc0/src/_rlist_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_security_build.py` & `flux-python-0.50.0rc0/src/_security_build.py`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_security_clean.h` & `flux-python-0.50.0rc0/src/_security_clean.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/_security_preproc.h` & `flux-python-0.50.0rc0/src/_security_preproc.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/callbacks.h` & `flux-python-0.50.0rc0/src/callbacks.h`

 * *Files identical despite different names*

### Comparing `flux-python-0.48.0rc1/src/make_clean_header.py` & `flux-python-0.50.0rc0/src/make_clean_header.py`

 * *Files identical despite different names*

